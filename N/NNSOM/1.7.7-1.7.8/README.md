# Comparing `tmp/nnsom-1.7.7.tar.gz` & `tmp/nnsom-1.7.8.tar.gz`

## Comparing `nnsom-1.7.7.tar` & `nnsom-1.7.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nnsom-1.7.7/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    79579 2020-02-02 00:00:00.000000 nnsom-1.7.7/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nnsom-1.7.7/src/NNSOM/som.py
--rw-r--r--   0        0        0    24827 2020-02-02 00:00:00.000000 nnsom-1.7.7/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    21590 2020-02-02 00:00:00.000000 nnsom-1.7.7/src/NNSOM/utils.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 nnsom-1.7.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.7/LICENSE
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.7/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 nnsom-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 nnsom-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77601 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.8/LICENSE
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 nnsom-1.7.8/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nnsom-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 nnsom-1.7.8/PKG-INFO
```

### Comparing `nnsom-1.7.7/src/NNSOM/som.py` & `nnsom-1.7.8/src/NNSOM/som.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,565 +1,565 @@
-from .utils import calculate_positions, distances, normalize_position, spread_positions
-
-import numpy as np
-from datetime import datetime
-from scipy.spatial.distance import cdist
-import pickle
-import warnings
-
-class SOM:
-    """
-    A class to represent a Self-Organizing Map (SOM), a type of artificial neural network
-    trained using unsupervised learning to produce a two-dimensional, discretized representation
-    of the input space of the training samples.
-
-    Attributes
-    ----------
-    dimensions : tuple, list, or array-like
-        The dimensions of the SOM grid. Determines the layout and number of neurons in the map.
-    numNeurons : int
-        The total number of neurons in the SOM, calculated as the product of the dimensions.
-    pos : array-like
-        The positions of the neurons in the SOM grid.
-    neuron_dist : array-like
-        The distances between neurons in the SOM.
-    w : array-like
-        The weight matrix of the SOM, representing the feature vectors of the neurons.
-    sim_flag : bool
-        A flag indicating whether the SOM has been simulated or not.
-
-    Methods
-    -------
-    __init__(self, dimensions):
-        Initializes the SOM with the specified dimensions.
-
-    init_w(self, x):
-        Initializes the weights of the SOM using principal components analysis on the input data x.
-
-    sim_som(self, x):
-        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
-
-    train(self, x, init_neighborhood=3, epochs=200, steps=100):
-        Trains the SOM using the batch SOM algorithm on the input data x.
-
-    quantization_error(self, dist)
-        Calculate quantization error
-
-    topological_error(self, data)
-        Calculate 1st and 1st-2nd toplogical error
-
-    distortion_error(self, data)
-        Calculate distortion error
-
-    save_pickle(self, filename, path, data_format='pkl'):
-        Saves the SOM object to a file using the pickle format.
-
-    load_pickle(self, filename, path, data_format='pkl'):
-        Loads a SOM object from a file using the pickle format.
-    """
-    def __init__(self, dimensions):
-        """
-        Initializes the SOM with the specified dimensions and calculates the positions and distances between neurons in the SOM grid.
-
-        Parameters
-        ----------
-        dimensions : tuple, list, or np.ndarray
-                    The dimensions (shape) of the SOM grid.
-        """
-
-        self.dimensions = dimensions
-        self.numNeurons = np.prod(dimensions)
-        # Calculate positions of neurons
-        self.pos = calculate_positions(dimensions)
-        # Calculate distances between neurons
-        self.neuron_dist = distances(self.pos)
-        # Initialize the weight matrix with empty list
-        self.w = []
-        # Set simulation flag to True,  needs to do simulation
-        self.sim_flag = True
-        # Initialize the output of simulation
-        self.outputs = None
-        # Initialize a normalize() function
-        self.norm_func = None
-
-        # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
-        self.sub_som = {}
-
-    def init_w(self, x, norm_func=None):
-        """
-        Initializes the weights of the SOM using principal components analysis (PCA) on the input data x.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data used for weight initialization.
-        """
-        # Initialize SOM weights using principal components
-
-        # Print Beginning time for initialization
-        print('Beginning Initialization')
-        now = datetime.now()
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-        # Normalize the input data
-        x = self.normalize(x, norm_func)
-
-        sz = x.shape
-
-        posMean = np.mean(x, axis=1)
-        posMean = np.expand_dims(posMean, axis=1)
-
-        xc = x - posMean
-
-        components, gains, encodedInputsT = np.linalg.svd(xc)
-
-        encodedInputsT = np.transpose(encodedInputsT)
-
-        basis = components * gains
-        stdev = np.std(encodedInputsT, axis=0)
-        stdev = stdev[:len(basis)]
-        posBasis = 2.5 * basis * stdev
-
-        numNeurons = self.numNeurons
-        numDimensions = len(self.dimensions)
-        sampleSize = sz[1]
-        inputSize = sz[0]
-        dimOrder = np.argsort(self.dimensions)
-
-        restoreOrder = np.concatenate((np.sort(dimOrder), np.arange(numDimensions, np.minimum(inputSize, sampleSize))))
-
-        if numDimensions > inputSize:
-            posBasis = np.concatenate((posBasis, np.random.rand(inputSize, inputSize) * 0.001))
-
-        posBasis = posBasis[restoreOrder]
-
-        pos1 = self.pos
-
-        if sampleSize < inputSize:
-            posBasis = np.concatenate((posBasis, np.zeros((inputSize, inputSize - sampleSize))))
-
-        if inputSize > numDimensions:
-            pos1 = np.concatenate((pos1, np.zeros((inputSize - numDimensions, numNeurons))), axis=0)
-
-        pos2 = normalize_position(pos1)
-
-        pos3 = spread_positions(pos2, posMean, posBasis)
-
-        self.w = np.transpose(pos3)
-
-        # Print Ending time for initialization
-        print('Ending Initialization')
-        now = datetime.now()
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-    def sim_som(self, x):
-        """
-        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data to simulate the SOM with.
-
-        Returns
-        -------
-        np.ndarray
-            The simulated output of the SOM.
-        """
-
-        # Simulate the SOM, with x as the input
-        shapx = x.shape   # shapes of the input x
-        shapw = self.w.shape # weights of the SOM
-
-        # Compute the negative distance from the inputs to each center
-        n = -cdist(self.w, np.transpose(x), 'euclidean')
-        # n = np.empty((shapw[0], shapx[1]))
-        # for jj in range(shapw[0]):
-        #     wj = self.w[jj]
-        #     wj = np.expand_dims(wj, axis=1)
-        #     n[jj] = np.sum((x - wj)**2, axis=0)
-
-        # n = -np.sqrt(n)
-        #print(n)
-
-        # Find out which center was closest to the input
-        maxRows = np.argmax(n, axis=0)
-        a = self._to_categorical(maxRows, num_classes=n.shape[0])   # made correction-added number of class
-        # a = tf.constant(a, shape=[np.transpose(n).shape[0],np.transpose(n).shape[1]])  # made change
-        return np.transpose(a)
-
-    def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
-        """
-        Trains the SOM using the batch SOM algorithm on the input data x.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data to train the SOM with.
-        init_neighborhood : int, optional
-            The initial neighborhood size.
-        epochs : int, optional
-            The number of epochs to train for.
-        steps : int, optional
-            The number of steps for training.
-
-        Returns
-        -------
-        None
-        """
-        # Normalize the input data
-        x = self.normalize(x, norm_func)
-
-        # Train the SOM using the batch SOM algorithm
-
-        w = self.w
-        shapw = w.shape
-        S = shapw[0]
-        shapx = x.shape
-        Q = shapx[1]
-
-        step = 0
-
-        now = datetime.now()
-
-        print('Beginning Training')
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-        # Train the network
-        for i in range(epochs):
-
-            # network output
-            a = self.sim_som(x)
-
-            # neighborhood distance
-            nd = 1 + (init_neighborhood-1) * (1 - step/steps)
-            neighborhood = self.neuron_dist <= nd
-            #print(nd)
-            # remove some outputs at random
-            a = a * (np.random.rand(S, Q) < 0.90)
-            a2 = np.matmul(neighborhood,a) + a
-
-            # find how many times each neuron won
-            # (The winning neuron is the one that exhibits the smallest distance or similarity to the input data)
-            suma2 = np.sum(a2, axis=1)
-            loserIndex = np.squeeze(np.asarray(suma2 == 0))
-            suma2[loserIndex] = 1
-            suma2 = np.expand_dims(suma2,axis = 1)
-            a3 = a2 / np.repeat(suma2, Q, axis=1)
-
-            neww = np.matmul(a3, np.transpose(x))
-
-            dw = neww - w
-
-            dw[loserIndex] = 0
-
-            w = w + np.array(dw)
-
-            step = step + 1
-
-            if step % 50 == 0:
-                print(step)
-                now = datetime.now()
-                current_time = now.strftime("%H:%M:%S")
-                print("Current Time =", current_time)
-
-        self.w = w
-        self.outputs = self.sim_som(x)
-        self.sim_flag = False
-
-        print('Ending Training')
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-    def cluster_data(self, x):
-        """
-        Cluster the input data based on the trained SOM reference vectors.
-
-        Parameters
-        ----------
-        x : ndarray (normalized)
-            The input data to be clustered.
-
-        Returns
-        -------
-        clusters : list of lists
-            A list containing sub-lists, where each sublist represents a cluster.
-            The indices of the input data points belonging to the same cluster
-            are stored in the corresponding sublist, sorted by their proximity
-            to the cluster center.
-
-        cluster_distances : list of lists
-            A list containing sub-lists, where each sublist represents the distances
-            of the input data points to the corresponding cluster center, sorted in
-            the same order as the indices in the `clusters` list.
-
-        max_cluster_distances : ndarray
-            A list containing the maximum distance between each cluster center
-            and the data points belonging to that cluster.
-
-        cluster_sizes : ndarray
-            A list containing the number of data points in each cluster.
-
-        Raises
-        -------
-        ValueError
-            If the SOM has not been trained.
-
-        ValueError
-            If the number of features in the input data and the SOM weights do not match.
-        """
-
-        if self.sim_flag:
-            raise ValueError("SOM has not been trained.")
-
-        if x.shape[1] != self.w.shape[1]:
-            raise ValueError('The number of features in the input data and the SOM weights do not match.')
-
-        # Normalize the input data
-        x = self.normalize(x, self.norm_func)
-
-        w = self.w
-        shapw = w.shape
-        S = shapw[0]
-
-        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
-        ind1 = np.argmin(x_w_dist, axis=0)
-
-        clusters = []  # a cluster array of indices sorted by distances
-        cluster_distances = []  # a cluster array of distances sorted by distances
-        max_cluster_distances = np.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
-        cluster_sizes = []  # cluster array sizes
-
-        for i in range(S):
-            # Find which inputs are closest to each weight (in cluster i)
-            tempclust = np.where(ind1 == i)[0]
-
-            # Save distance of each input in the cluster to cluster center (weight)
-            tempdist = x_w_dist[i, tempclust]
-            indsort = np.argsort(tempdist)
-            tempclust = tempclust[indsort]  # Sort indices
-            tempdist = tempdist[indsort]
-
-            # Add to distance array sorted distances
-            cluster_distances.append(tempdist)
-
-            # Add to Cluster array sorted indices
-            clusters.append(tempclust)
-
-            # Cluster size
-            num = len(tempclust)
-            cluster_sizes.append(num)
-
-            # Save the maximum distance to any input in the cluster from cluster center
-            if num > 0:
-                max_cluster_distances[i] = tempdist[-1]
-
-        return clusters, cluster_distances, max_cluster_distances, cluster_sizes
-
-    def normalize(self, x, norm_func=None):
-        """
-        Normalize the input data using a custom function.
-
-        Parameters
-        ----------
-        x: array-like
-            The input data to be normalized.
-        norm_func: callable, optional
-            A custom normalization or standardization function to be applied to the input data.
-            If provided, it should take the input data as its argument and return the preprocessed data.
-            Default is None, in which case the input data is returned as-is.
-
-        Returns
-        -------
-        x_preprocessed: array-like
-            The preprocessed input data.
-
-        Raises
-        ------
-        Warning
-            If `norm_func` is None, a warning is raised to indicate the potential inefficiency in SOM training.
-
-        Examples
-        --------
-        >>> import numpy as np
-        >>> from sklearn.datasets import load_iris
-        >>> from sklearn.feature_extraction.text import TfidfVectorizer
-        >>> from sklearn.preprocessing import StandardScaler
-
-        >>> # Case 1: Tabular data (without normalization)
-        >>> iris = load_iris()
-        >>> X = iris.data
-        >>> som = SOM(dimensions=(5, 5))
-        >>> X_norm = som.normalize(X)
-        >>> print(np.allclose(np.transpose(X_norm), X))
-        True
-
-        >>> # Case 2: Image data (using custom normalization)
-        >>> image_data = np.random.randint(0, 256, size=(28, 28))
-        >>> som = SOM(dimensions=(10, 10))
-        >>> custom_norm_func = lambda x: x / 255  # Custom normalization function
-        >>> image_data_norm = som.normalize(image_data, norm_func=custom_norm_func)
-        >>> print(image_data_norm.min(), image_data_norm.max())
-        0.0 1.0
-
-        >>> # Case 3: Text data (without normalization)
-        >>> text_data = ["This is a sample text.", "Another example sentence."]
-        >>> vectorizer = TfidfVectorizer()
-        >>> tfidf_matrix = vectorizer.fit_transform(text_data)
-        >>> som = SOM(dimensions=(8, 8))
-        >>> text_data_norm = som.normalize(tfidf_matrix.toarray())
-        >>> print(np.allclose(np.transpose(text_data_norm), tfidf_matrix.toarray()))
-        True
-        """
-
-        if norm_func is not None:
-            x_norm = norm_func(x)  # Use the provided custom normalization function
-            self.norm_func = norm_func
-        else:
-            warnings.warn(
-                "Without normalization function: SOM training may be inefficient if you are not normalized.",
-                UserWarning, stacklevel=2)
-            x_norm = x  # Return the input data as-is
-
-        return np.transpose(x_norm)
-
-    def quantization_error(self, dist):
-        """
-        Calculate quantization error
-        """
-        quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
-
-        return quant_err
-
-    def topological_error(self, x):
-        """
-        Calculate topological error
-        """
-        w = self.w
-        ndist = self.neuron_dist
-
-        # Normalize Input
-        x = self.normalize(x, self.norm_func)
-
-        # Calculate the distance between item vs. cluster center
-        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
-
-        sort_dist = np.argsort(x_w_dist, axis=0)
-        top_dist = [ndist[sort_dist[0, ii], sort_dist[1, ii]] for ii in range(sort_dist.shape[1])]
-        neighbors = np.where(np.array(top_dist) > 1.1)
-        top_error_1st = 100 * len(neighbors[0]) / x_w_dist.shape[1]
-        neighbors = np.where(np.array(top_dist) > 2.1)
-        top_error_1st_and_2nd = 100 * len(neighbors[0]) / x_w_dist.shape[1]
-
-        return top_error_1st, top_error_1st_and_2nd
-
-    def distortion_error(self, x):
-        """
-        Calculate distortion
-        """
-        # Normalize input data
-        x = self.normalize(x, self.norm_func)
-
-        shapx = x.shape
-        Q = shapx[1]  # Number of samples
-
-        ww = self.w
-        ndist = self.neuron_dist
-        x_w_dist = cdist(ww, np.transpose(x), 'euclidean')
-        ind1 = np.argmin(x_w_dist, axis=0)
-
-        dd = [1, 2, 3]  # neighborhood distances
-        wwdist = cdist(ww, ww, 'euclidean')
-        sst = ndist[:, ind1]
-
-        for d in dd:
-            factor1 = 2 * d * d
-            factor2 = Q * d * np.sqrt(2 * np.pi)
-            temp = np.exp(-np.multiply(sst, sst) / factor1)
-            distortion = np.sum(np.multiply(temp, x_w_dist)) / factor2
-            print('Distortion (d=' + str(d) + ') = ' + str(distortion))
-
-    def save_pickle(self, filename, path, data_format='pkl'):
-        """ Save the SOM object to a file using pickle.
-        
-        Parameters
-        ----------
-        filename : str
-            The name of the file to save the SOM object to.
-
-        path : str
-            The path to the file to save the SOM object to.
-
-        data_format : str
-            The format to save the SOM object in. Must be one of: pkl
-
-        Returns
-        -------
-        None
-        """
-        if data_format not in ['pkl']:
-            raise ValueError('data_format must be one of: pkl')
-
-        if data_format == 'pkl':
-            with open(path + filename, 'wb') as f:
-                pickle.dump(self, f)
-
-    def load_pickle(self, filename, path, data_format='pkl'):
-        """ Load the SOM object from a file using pickle.
-
-        Parameters
-        ----------
-        filename : str
-            The name of the file to load the SOM object from.
-
-        path : str
-            The path to the file to load the SOM object from.
-
-        data_format : str
-            The format to load the SOM object from. Must be one of: pkl
-
-        Returns
-        -------
-        None
-        """
-        if data_format not in ['pkl']:
-            raise ValueError('data_format must be one of: pkl')
-
-        if data_format == 'pkl':
-            with open(path + filename, 'rb') as f:
-                som = pickle.load(f)
-
-        return som
-
-    def _to_categorical(self, x, num_classes=None):
-        """ Converts a class vector (integers) to binary class matrix.
-
-        Args:
-        x: Array-like with class values to be converted into a matrix
-            (integers from 0 to `num_classes - 1`).
-        num_classes: Total number of classes. If `None`, this would be inferred
-            as `max(x) + 1`. Defaults to `None`.
-
-        Returns:
-        A binary matrix representation of the input as a NumPy or Cupy array. The class
-        axis is placed last.
-
-        """
-        x = np.array(x, dtype="int64")
-        input_shape = x.shape
-
-        # Shrink the last dimension if the shape is (..., 1).
-        if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-            input_shape = tuple(input_shape[:-1])
-
-        x = x.reshape(-1)
-        if not num_classes:
-            num_classes = np.max(x) + 1
-        batch_size = x.shape[0]
-        categorical = np.zeros((batch_size, num_classes))
-        categorical[np.arange(batch_size), x] = 1
-        output_shape = input_shape + (num_classes,)
-        categorical = np.reshape(categorical, output_shape)
-
+from .utils import calculate_positions, distances, normalize_position, spread_positions
+
+import numpy as np
+from datetime import datetime
+from scipy.spatial.distance import cdist
+import pickle
+import warnings
+
+class SOM:
+    """
+    A class to represent a Self-Organizing Map (SOM), a type of artificial neural network
+    trained using unsupervised learning to produce a two-dimensional, discretized representation
+    of the input space of the training samples.
+
+    Attributes
+    ----------
+    dimensions : tuple, list, or array-like
+        The dimensions of the SOM grid. Determines the layout and number of neurons in the map.
+    numNeurons : int
+        The total number of neurons in the SOM, calculated as the product of the dimensions.
+    pos : array-like
+        The positions of the neurons in the SOM grid.
+    neuron_dist : array-like
+        The distances between neurons in the SOM.
+    w : array-like
+        The weight matrix of the SOM, representing the feature vectors of the neurons.
+    sim_flag : bool
+        A flag indicating whether the SOM has been simulated or not.
+
+    Methods
+    -------
+    __init__(self, dimensions):
+        Initializes the SOM with the specified dimensions.
+
+    init_w(self, x):
+        Initializes the weights of the SOM using principal components analysis on the input data x.
+
+    sim_som(self, x):
+        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
+
+    train(self, x, init_neighborhood=3, epochs=200, steps=100):
+        Trains the SOM using the batch SOM algorithm on the input data x.
+
+    quantization_error(self, dist)
+        Calculate quantization error
+
+    topological_error(self, data)
+        Calculate 1st and 1st-2nd toplogical error
+
+    distortion_error(self, data)
+        Calculate distortion error
+
+    save_pickle(self, filename, path, data_format='pkl'):
+        Saves the SOM object to a file using the pickle format.
+
+    load_pickle(self, filename, path, data_format='pkl'):
+        Loads a SOM object from a file using the pickle format.
+    """
+    def __init__(self, dimensions):
+        """
+        Initializes the SOM with the specified dimensions and calculates the positions and distances between neurons in the SOM grid.
+
+        Parameters
+        ----------
+        dimensions : tuple, list, or np.ndarray
+                    The dimensions (shape) of the SOM grid.
+        """
+
+        self.dimensions = dimensions
+        self.numNeurons = np.prod(dimensions)
+        # Calculate positions of neurons
+        self.pos = calculate_positions(dimensions)
+        # Calculate distances between neurons
+        self.neuron_dist = distances(self.pos)
+        # Initialize the weight matrix with empty list
+        self.w = []
+        # Set simulation flag to True,  needs to do simulation
+        self.sim_flag = True
+        # Initialize the output of simulation
+        self.outputs = None
+        # Initialize a normalize() function
+        self.norm_func = None
+
+        # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
+        self.sub_som = {}
+
+    def init_w(self, x, norm_func=None):
+        """
+        Initializes the weights of the SOM using principal components analysis (PCA) on the input data x.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data used for weight initialization.
+        """
+        # Initialize SOM weights using principal components
+
+        # Print Beginning time for initialization
+        print('Beginning Initialization')
+        now = datetime.now()
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+
+        sz = x.shape
+
+        posMean = np.mean(x, axis=1)
+        posMean = np.expand_dims(posMean, axis=1)
+
+        xc = x - posMean
+
+        components, gains, encodedInputsT = np.linalg.svd(xc)
+
+        encodedInputsT = np.transpose(encodedInputsT)
+
+        basis = components * gains
+        stdev = np.std(encodedInputsT, axis=0)
+        stdev = stdev[:len(basis)]
+        posBasis = 2.5 * basis * stdev
+
+        numNeurons = self.numNeurons
+        numDimensions = len(self.dimensions)
+        sampleSize = sz[1]
+        inputSize = sz[0]
+        dimOrder = np.argsort(self.dimensions)
+
+        restoreOrder = np.concatenate((np.sort(dimOrder), np.arange(numDimensions, np.minimum(inputSize, sampleSize))))
+
+        if numDimensions > inputSize:
+            posBasis = np.concatenate((posBasis, np.random.rand(inputSize, inputSize) * 0.001))
+
+        posBasis = posBasis[restoreOrder]
+
+        pos1 = self.pos
+
+        if sampleSize < inputSize:
+            posBasis = np.concatenate((posBasis, np.zeros((inputSize, inputSize - sampleSize))))
+
+        if inputSize > numDimensions:
+            pos1 = np.concatenate((pos1, np.zeros((inputSize - numDimensions, numNeurons))), axis=0)
+
+        pos2 = normalize_position(pos1)
+
+        pos3 = spread_positions(pos2, posMean, posBasis)
+
+        self.w = np.transpose(pos3)
+
+        # Print Ending time for initialization
+        print('Ending Initialization')
+        now = datetime.now()
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+    def sim_som(self, x):
+        """
+        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to simulate the SOM with.
+
+        Returns
+        -------
+        np.ndarray
+            The simulated output of the SOM.
+        """
+
+        # Simulate the SOM, with x as the input
+        shapx = x.shape   # shapes of the input x
+        shapw = self.w.shape # weights of the SOM
+
+        # Compute the negative distance from the inputs to each center
+        n = -cdist(self.w, np.transpose(x), 'euclidean')
+        # n = np.empty((shapw[0], shapx[1]))
+        # for jj in range(shapw[0]):
+        #     wj = self.w[jj]
+        #     wj = np.expand_dims(wj, axis=1)
+        #     n[jj] = np.sum((x - wj)**2, axis=0)
+
+        # n = -np.sqrt(n)
+        #print(n)
+
+        # Find out which center was closest to the input
+        maxRows = np.argmax(n, axis=0)
+        a = self._to_categorical(maxRows, num_classes=n.shape[0])   # made correction-added number of class
+        # a = tf.constant(a, shape=[np.transpose(n).shape[0],np.transpose(n).shape[1]])  # made change
+        return np.transpose(a)
+
+    def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
+        """
+        Trains the SOM using the batch SOM algorithm on the input data x.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to train the SOM with.
+        init_neighborhood : int, optional
+            The initial neighborhood size.
+        epochs : int, optional
+            The number of epochs to train for.
+        steps : int, optional
+            The number of steps for training.
+
+        Returns
+        -------
+        None
+        """
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+
+        # Train the SOM using the batch SOM algorithm
+
+        w = self.w
+        shapw = w.shape
+        S = shapw[0]
+        shapx = x.shape
+        Q = shapx[1]
+
+        step = 0
+
+        now = datetime.now()
+
+        print('Beginning Training')
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+        # Train the network
+        for i in range(epochs):
+
+            # network output
+            a = self.sim_som(x)
+
+            # neighborhood distance
+            nd = 1 + (init_neighborhood-1) * (1 - step/steps)
+            neighborhood = self.neuron_dist <= nd
+            #print(nd)
+            # remove some outputs at random
+            a = a * (np.random.rand(S, Q) < 0.90)
+            a2 = np.matmul(neighborhood,a) + a
+
+            # find how many times each neuron won
+            # (The winning neuron is the one that exhibits the smallest distance or similarity to the input data)
+            suma2 = np.sum(a2, axis=1)
+            loserIndex = np.squeeze(np.asarray(suma2 == 0))
+            suma2[loserIndex] = 1
+            suma2 = np.expand_dims(suma2,axis = 1)
+            a3 = a2 / np.repeat(suma2, Q, axis=1)
+
+            neww = np.matmul(a3, np.transpose(x))
+
+            dw = neww - w
+
+            dw[loserIndex] = 0
+
+            w = w + np.array(dw)
+
+            step = step + 1
+
+            if step % 50 == 0:
+                print(step)
+                now = datetime.now()
+                current_time = now.strftime("%H:%M:%S")
+                print("Current Time =", current_time)
+
+        self.w = w
+        self.outputs = self.sim_som(x)
+        self.sim_flag = False
+
+        print('Ending Training')
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+    def cluster_data(self, x):
+        """
+        Cluster the input data based on the trained SOM reference vectors.
+
+        Parameters
+        ----------
+        x : ndarray (normalized)
+            The input data to be clustered.
+
+        Returns
+        -------
+        clusters : list of lists
+            A list containing sub-lists, where each sublist represents a cluster.
+            The indices of the input data points belonging to the same cluster
+            are stored in the corresponding sublist, sorted by their proximity
+            to the cluster center.
+
+        cluster_distances : list of lists
+            A list containing sub-lists, where each sublist represents the distances
+            of the input data points to the corresponding cluster center, sorted in
+            the same order as the indices in the `clusters` list.
+
+        max_cluster_distances : ndarray
+            A list containing the maximum distance between each cluster center
+            and the data points belonging to that cluster.
+
+        cluster_sizes : ndarray
+            A list containing the number of data points in each cluster.
+
+        Raises
+        -------
+        ValueError
+            If the SOM has not been trained.
+
+        ValueError
+            If the number of features in the input data and the SOM weights do not match.
+        """
+
+        if self.sim_flag:
+            raise ValueError("SOM has not been trained.")
+
+        if x.shape[1] != self.w.shape[1]:
+            raise ValueError('The number of features in the input data and the SOM weights do not match.')
+
+        # Normalize the input data
+        x = self.normalize(x, self.norm_func)
+
+        w = self.w
+        shapw = w.shape
+        S = shapw[0]
+
+        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
+        ind1 = np.argmin(x_w_dist, axis=0)
+
+        clusters = []  # a cluster array of indices sorted by distances
+        cluster_distances = []  # a cluster array of distances sorted by distances
+        max_cluster_distances = np.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
+        cluster_sizes = []  # cluster array sizes
+
+        for i in range(S):
+            # Find which inputs are closest to each weight (in cluster i)
+            tempclust = np.where(ind1 == i)[0]
+
+            # Save distance of each input in the cluster to cluster center (weight)
+            tempdist = x_w_dist[i, tempclust]
+            indsort = np.argsort(tempdist)
+            tempclust = tempclust[indsort]  # Sort indices
+            tempdist = tempdist[indsort]
+
+            # Add to distance array sorted distances
+            cluster_distances.append(tempdist)
+
+            # Add to Cluster array sorted indices
+            clusters.append(tempclust)
+
+            # Cluster size
+            num = len(tempclust)
+            cluster_sizes.append(num)
+
+            # Save the maximum distance to any input in the cluster from cluster center
+            if num > 0:
+                max_cluster_distances[i] = tempdist[-1]
+
+        return clusters, cluster_distances, max_cluster_distances, cluster_sizes
+
+    def normalize(self, x, norm_func=None):
+        """
+        Normalize the input data using a custom function.
+
+        Parameters
+        ----------
+        x: array-like
+            The input data to be normalized.
+        norm_func: callable, optional
+            A custom normalization or standardization function to be applied to the input data.
+            If provided, it should take the input data as its argument and return the preprocessed data.
+            Default is None, in which case the input data is returned as-is.
+
+        Returns
+        -------
+        x_preprocessed: array-like
+            The preprocessed input data.
+
+        Raises
+        ------
+        Warning
+            If `norm_func` is None, a warning is raised to indicate the potential inefficiency in SOM training.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> from sklearn.datasets import load_iris
+        >>> from sklearn.feature_extraction.text import TfidfVectorizer
+        >>> from sklearn.preprocessing import StandardScaler
+
+        >>> # Case 1: Tabular data (without normalization)
+        >>> iris = load_iris()
+        >>> X = iris.data
+        >>> som = SOM(dimensions=(5, 5))
+        >>> X_norm = som.normalize(X)
+        >>> print(np.allclose(np.transpose(X_norm), X))
+        True
+
+        >>> # Case 2: Image data (using custom normalization)
+        >>> image_data = np.random.randint(0, 256, size=(28, 28))
+        >>> som = SOM(dimensions=(10, 10))
+        >>> custom_norm_func = lambda x: x / 255  # Custom normalization function
+        >>> image_data_norm = som.normalize(image_data, norm_func=custom_norm_func)
+        >>> print(image_data_norm.min(), image_data_norm.max())
+        0.0 1.0
+
+        >>> # Case 3: Text data (without normalization)
+        >>> text_data = ["This is a sample text.", "Another example sentence."]
+        >>> vectorizer = TfidfVectorizer()
+        >>> tfidf_matrix = vectorizer.fit_transform(text_data)
+        >>> som = SOM(dimensions=(8, 8))
+        >>> text_data_norm = som.normalize(tfidf_matrix.toarray())
+        >>> print(np.allclose(np.transpose(text_data_norm), tfidf_matrix.toarray()))
+        True
+        """
+
+        if norm_func is not None:
+            x_norm = norm_func(x)  # Use the provided custom normalization function
+            self.norm_func = norm_func
+        else:
+            warnings.warn(
+                "Without normalization function: SOM training may be inefficient if you are not normalized.",
+                UserWarning, stacklevel=2)
+            x_norm = x  # Return the input data as-is
+
+        return np.transpose(x_norm)
+
+    def quantization_error(self, dist):
+        """
+        Calculate quantization error
+        """
+        quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
+
+        return quant_err
+
+    def topological_error(self, x):
+        """
+        Calculate topological error
+        """
+        w = self.w
+        ndist = self.neuron_dist
+
+        # Normalize Input
+        x = self.normalize(x, self.norm_func)
+
+        # Calculate the distance between item vs. cluster center
+        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
+
+        sort_dist = np.argsort(x_w_dist, axis=0)
+        top_dist = [ndist[sort_dist[0, ii], sort_dist[1, ii]] for ii in range(sort_dist.shape[1])]
+        neighbors = np.where(np.array(top_dist) > 1.1)
+        top_error_1st = 100 * len(neighbors[0]) / x_w_dist.shape[1]
+        neighbors = np.where(np.array(top_dist) > 2.1)
+        top_error_1st_and_2nd = 100 * len(neighbors[0]) / x_w_dist.shape[1]
+
+        return top_error_1st, top_error_1st_and_2nd
+
+    def distortion_error(self, x):
+        """
+        Calculate distortion
+        """
+        # Normalize input data
+        x = self.normalize(x, self.norm_func)
+
+        shapx = x.shape
+        Q = shapx[1]  # Number of samples
+
+        ww = self.w
+        ndist = self.neuron_dist
+        x_w_dist = cdist(ww, np.transpose(x), 'euclidean')
+        ind1 = np.argmin(x_w_dist, axis=0)
+
+        dd = [1, 2, 3]  # neighborhood distances
+        wwdist = cdist(ww, ww, 'euclidean')
+        sst = ndist[:, ind1]
+
+        for d in dd:
+            factor1 = 2 * d * d
+            factor2 = Q * d * np.sqrt(2 * np.pi)
+            temp = np.exp(-np.multiply(sst, sst) / factor1)
+            distortion = np.sum(np.multiply(temp, x_w_dist)) / factor2
+            print('Distortion (d=' + str(d) + ') = ' + str(distortion))
+
+    def save_pickle(self, filename, path, data_format='pkl'):
+        """ Save the SOM object to a file using pickle.
+        
+        Parameters
+        ----------
+        filename : str
+            The name of the file to save the SOM object to.
+
+        path : str
+            The path to the file to save the SOM object to.
+
+        data_format : str
+            The format to save the SOM object in. Must be one of: pkl
+
+        Returns
+        -------
+        None
+        """
+        if data_format not in ['pkl']:
+            raise ValueError('data_format must be one of: pkl')
+
+        if data_format == 'pkl':
+            with open(path + filename, 'wb') as f:
+                pickle.dump(self, f)
+
+    def load_pickle(self, filename, path, data_format='pkl'):
+        """ Load the SOM object from a file using pickle.
+
+        Parameters
+        ----------
+        filename : str
+            The name of the file to load the SOM object from.
+
+        path : str
+            The path to the file to load the SOM object from.
+
+        data_format : str
+            The format to load the SOM object from. Must be one of: pkl
+
+        Returns
+        -------
+        None
+        """
+        if data_format not in ['pkl']:
+            raise ValueError('data_format must be one of: pkl')
+
+        if data_format == 'pkl':
+            with open(path + filename, 'rb') as f:
+                som = pickle.load(f)
+
+        return som
+
+    def _to_categorical(self, x, num_classes=None):
+        """ Converts a class vector (integers) to binary class matrix.
+
+        Args:
+        x: Array-like with class values to be converted into a matrix
+            (integers from 0 to `num_classes - 1`).
+        num_classes: Total number of classes. If `None`, this would be inferred
+            as `max(x) + 1`. Defaults to `None`.
+
+        Returns:
+        A binary matrix representation of the input as a NumPy or Cupy array. The class
+        axis is placed last.
+
+        """
+        x = np.array(x, dtype="int64")
+        input_shape = x.shape
+
+        # Shrink the last dimension if the shape is (..., 1).
+        if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
+            input_shape = tuple(input_shape[:-1])
+
+        x = x.reshape(-1)
+        if not num_classes:
+            num_classes = np.max(x) + 1
+        batch_size = x.shape[0]
+        categorical = np.zeros((batch_size, num_classes))
+        categorical[np.arange(batch_size), x] = 1
+        output_shape = input_shape + (num_classes,)
+        categorical = np.reshape(categorical, output_shape)
+
         return categorical
```

### Comparing `nnsom-1.7.7/src/NNSOM/som_gpu.py` & `nnsom-1.7.8/src/NNSOM/som_gpu.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,662 +1,662 @@
-try:
-    import cupy as cp
-    print("You are using GPU acceleration with Cupy")
-except ImportError:
-    print("CuPy is not available. For CPU-based operations, you can use the NumPy version of this SOM.")
-    print("Please consider installing the 'NNSOM' package, and use 'from NNSOM.som import SOM' for a NumPy-based SOM implementation.")
-    raise SystemExit
-
-from .utils import calculate_positions, distances
-
-import numpy as np
-from datetime import datetime
-import pickle
-import warnings
-
-
-class SOMGpu:
-    """
-    Represents a Self-Organizing Map (SOM) using GPU acceleration with CuPy.
-
-    A Self-Organizing Map (SOM) is an artificial neural network used for unsupervised learning,
-    which projects high-dimensional data into a lower-dimensional (typically two-dimensional) space.
-    It is trained using a competitive learning approach to produce a discretized representation
-    of the input space of training samples.
-
-    Attributes:
-        dimensions (tuple, list, np.ndarray): Dimensions of the SOM grid, defining the layout and number of neurons.
-        numNeurons (int): Total number of neurons, computed as the product of the grid dimensions.
-        pos (np.ndarray): Positions of neurons within the grid.
-        neuron_dist (np.ndarray): Precomputed Euclidean distances between neurons in the grid.
-        w (np.ndarray): Weight matrix representing the feature vectors of the neurons.
-        sim_flag (bool): Indicates if the SOM has been simulated/trained.
-        output (np.ndarray): Output from the latest simulation.
-        norm_func (callable): Function used to normalize input data.
-        sub_som (dict): Optional sub-clustering using additional SOMs at neuron positions.
-
-    Methods:
-        __init__(self, dimensions): Initializes the SOM with the specified dimensions.
-        init_w(self, x, norm_func=None): Initializes the weights using PCA on input data `x`.
-        sim_som(self, x): Simulates SOM processing for input `x`, identifying activated neurons.
-        train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
-            Trains the SOM using batch SOM algorithm on input data `x`.
-        quantization_error(self, dist): Calculates the quantization error of the model.
-        topological_error(self, data): Calculates the topological error of the model.
-        distortion_error(self, data): Calculates the distortion error of the model.
-        save_pickle(self, filename, path, data_format='pkl'): Saves the SOM object to a file in pickle format.
-        load_pickle(self, filename, path, data_format='pkl'): Loads the SOM object from a file in pickle format.
-        _normalize_position(self, position): Helper method to normalize neuron positions.
-        _spread_positions(self, position, positionMean, positionBasis): Helper method to adjust neuron positions.
-        _euclidean_distance(self, XA, XB): Computes Euclidean distances between two sets of vectors.
-        _to_categorical(self, x, num_classes=None): Converts class vector to binary class matrix.
-
-    Raises:
-        ImportError: If CuPy is not available, suggests using the NNSOM package for a NumPy-based implementation.
-
-    Example:
-        >>> dimensions = (10, 10)
-        >>> som = SOMGpu(dimensions)
-        >>> data = np.random.rand(100, 10)
-        >>> som.init_w(data, norm_func=None)
-        >>> som.train(data, norm_func=None)
-        >>> output = som.sim_som(data)
-    """
-    def __init__(self, dimensions):
-        """
-        Initializes the SOM with the specified dimensions and calculates the positions and distances between neurons in the SOM grid.
-
-        Parameters
-        ----------
-        dimensions : tuple, list, or np.ndarray
-                    The dimensions (shape) of the SOM grid.
-        """
-
-        self.dimensions = dimensions  # Processing as numpy
-        self.numNeurons = np.prod(dimensions) # Processing as numpy
-        # Calculate positions of neurons
-        self.pos = calculate_positions(dimensions)
-        # Calculate distances between neurons
-        self.neuron_dist = distances(self.pos)
-        # Initialize the weight matrix with empty list
-        self.w = []
-        # Set simulation flag to True,  needs to do simulation
-        self.sim_flag = True
-        # Initialize the output of simulation
-        self.output = None
-        # Initialize a normalize() function
-        self.norm_func = None
-
-        # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
-        self.sub_som = {}
-
-    def init_w(self, x, norm_func=None):
-        """
-        Initializes the weights of the SOM using principal components analysis (PCA) on the input data x.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data used for weight initialization.
-        """
-        # Initialize SOM weights using principal components
-
-        # Print Beginning time for initialization
-        print('Beginning Initialization')
-        now = datetime.now()
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-        # Normalize the input data
-        x = self.normalize(x, norm_func)
-        x = cp.asarray(x)
-
-        sz = x.shape
-
-        posMean = cp.mean(x, axis=1)
-        posMean = cp.expand_dims(posMean, axis=1)
-
-        xc = x - posMean
-
-        components, gains, encodedInputsT = cp.linalg.svd(xc)
-
-        encodedInputsT = cp.transpose(encodedInputsT)
-
-        basis = components * gains
-        stdev = cp.std(encodedInputsT, axis=0)
-        stdev = stdev[:len(basis)]
-        posBasis = 2.5 * basis * stdev
-
-        numNeurons = self.numNeurons
-        numDimensions = len(self.dimensions)
-        dimensions = self.dimensions
-        sampleSize = sz[1]
-        inputSize = sz[0]
-        dimOrder = cp.argsort(cp.asarray(dimensions))
-
-        restoreOrder = cp.concatenate((cp.sort(dimOrder), cp.arange(numDimensions, cp.minimum(inputSize, sampleSize))))
-
-        if numDimensions > inputSize:
-            posBasis = cp.concatenate((posBasis, cp.random.rand(inputSize, inputSize) * 0.001))
-
-        posBasis = posBasis[restoreOrder]
-
-        pos1 = self.pos
-        pos1 = cp.asarray(pos1)
-
-        if sampleSize < inputSize:
-            posBasis = cp.concatenate((posBasis, cp.zeros((inputSize, inputSize - sampleSize))))
-
-        if inputSize > numDimensions:
-            pos1 = cp.concatenate((pos1, cp.zeros((inputSize - numDimensions, numNeurons))), axis=0)
-
-        pos2 = self._normalize_position(pos1)
-
-        pos3 = self._spread_positions(pos2, posMean, posBasis)
-
-        self.w = cp.asnumpy(cp.transpose(pos3))
-
-        # Print Ending time for initialization
-        print('Ending Initialization')
-        now = datetime.now()
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-    def sim_som(self, x):
-        """
-        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data to simulate the SOM with.
-
-        Returns
-        -------
-        np.ndarray
-            The simulated output of the SOM.
-        """
-        # Simulate the SOM, with x as the input
-        # Transform np.ndarray into cp.ndarray
-        w = cp.asarray(self.w)
-        x = cp.asarray(x)
-
-        # Compute the negative distance from the inputs to each center
-        n = -self._euclidean_distance(w, cp.transpose(x))
-
-        # Find out which center was closest to the input
-        maxRows = cp.argmax(n, axis=0)
-        a = self._to_categorical(maxRows, num_classes=n.shape[0]) #made correction-added number of class
-        a = cp.asnumpy(a)
-
-        return np.transpose(a)
-
-    def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
-        """
-        Trains the SOM using the batch SOM algorithm on the input data x.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The input data to train the SOM with.
-        init_neighborhood : int, optional
-            The initial neighborhood size.
-        epochs : int, optional
-            The number of epochs to train for.
-        steps : int, optional
-            The number of steps for training.
-
-        Returns
-        -------
-        None
-        """
-        # Normalize the input data
-        x = self.normalize(x, norm_func)
-        x = cp.asarray(x)
-
-        # Train the SOM using the batch SOM algorithm
-
-        w = self.w
-        w = cp.asarray(w)
-        shapw = w.shape
-        S = shapw[0]
-        shapx = x.shape
-        Q = shapx[1]
-
-        step = 0
-
-        print('Beginning Training')
-        now = datetime.now()
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-        # Train the network
-        for i in range(epochs):
-
-            # network output
-            a = self.sim_som(x)
-            a = cp.asarray(a)
-
-            # neighborhood distance
-            nd = 1 + (init_neighborhood-1) * (1 - step/steps)
-            neighborhood = self.neuron_dist <= nd
-            neighborhood = cp.asarray(neighborhood)
-            #print(nd)
-            # remove some outputs at random
-            a = a * (cp.random.rand(S, Q) < 0.90)
-            a2 = cp.matmul(neighborhood, a) + a
-
-            # find how many times each neuron won
-            # (The winning neuron is the one that exhibits the smallest distance or similarity to the input data)
-            suma2 = cp.sum(a2, axis=1)
-            loserIndex = cp.squeeze(cp.asarray(suma2 == 0))
-            suma2[loserIndex] = 1
-            suma2 = cp.expand_dims(suma2,axis = 1)
-            a3 = a2 / cp.repeat(suma2, Q, axis=1)
-
-            neww = cp.matmul(a3, cp.transpose(x))
-
-            dw = neww - w
-
-            dw[loserIndex] = 0
-
-            w = w + cp.array(dw)
-
-            step = step + 1
-
-            if step % 50 == 0:
-                print(step)
-                now = datetime.now()
-                current_time = now.strftime("%H:%M:%S")
-                print("Current Time =", current_time)
-
-        self.w = cp.asnumpy(w)
-        self.outputs = self.sim_som(x)
-        self.sim_flag = False
-
-        print('Ending Training')
-        current_time = now.strftime("%H:%M:%S")
-        print("Current Time =", current_time)
-
-    def cluster_data(self, x):
-        """
-        Cluster the input data based on the trained SOM reference vectors.
-
-        Parameters
-        ----------
-        x : ndarray (normalized)
-            The input data to be clustered.
-
-        Returns
-        -------
-        clusters : list of lists
-            A list containing sub-lists, where each sublist represents a cluster.
-            The indices of the input data points belonging to the same cluster
-            are stored in the corresponding sublist, sorted by their proximity
-            to the cluster center.
-
-        cluster_distances : list of lists
-            A list containing sub-lists, where each sublist represents the distances
-            of the input data points to the corresponding cluster center, sorted in
-            the same order as the indices in the `clusters` list.
-
-        max_cluster_distances : ndarray
-            A list containing the maximum distance between each cluster center
-            and the data points belonging to that cluster.
-
-        cluster_sizes : ndarray
-            A list containing the number of data points in each cluster.
-
-        Raises
-        -------
-        ValueError
-            If the SOM has not been trained.
-
-        ValueError
-            If the number of features in the input data and the SOM weights do not match.
-        """
-
-        if self.sim_flag:
-            raise ValueError("SOM has not been trained.")
-
-        if x.shape[1] != self.w.shape[1]:
-            raise ValueError('The number of features in the input data and the SOM weights do not match.')
-
-        # Normalize the input data
-        x = self.normalize(x, self.norm_func)
-        x = cp.asarray(x)
-
-        w = self.w
-        w = cp.asarray(w)
-        shapw = w.shape
-        S = shapw[0]
-
-        x_w_dist = self._euclidean_distance(w, cp.transpose(x))
-        ind1 = cp.argmin(x_w_dist, axis=0)
-
-        clusters = []  # a cluster array of indices sorted by distances
-        cluster_distances = []  # a cluster array of distances sorted by distances
-        max_cluster_distances = cp.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
-        cluster_sizes = []  # cluster array sizes
-
-        for i in range(S):
-            # Find which inputs are closest to each weight (in cluster i)
-            tempclust = cp.where(ind1 == i)[0]
-
-            # Save distance of each input in the cluster to cluster center (weight)
-            tempdist = x_w_dist[i, tempclust]
-            indsort = cp.argsort(tempdist)
-            tempclust = tempclust[indsort]  # Sort indices
-            tempdist = tempdist[indsort]
-
-            # Add to distance array sorted distances
-            cluster_distances.append(tempdist)
-
-            # Add to Cluster array sorted indices
-            clusters.append(tempclust)
-
-            # Cluster size
-            num = len(tempclust)
-            cluster_sizes.append(num)
-
-            # Save the maximum distance to any input in the cluster from cluster center
-            if num > 0:
-                max_cluster_distances[i] = tempdist[-1]
-
-        # Convert clusters to a list of lists
-        clusters = [clust.get().tolist() for clust in clusters]
-        # Convert cluster_distances to a list of lists
-        cluster_distances = [dist.get().tolist() for dist in cluster_distances]
-        # Convert max_cluster_distances to a NumPy array
-        max_cluster_distances = max_cluster_distances.get()
-        # Convert cluster_sizes to a NumPy array
-        cluster_sizes = np.array(cluster_sizes)
-
-        return clusters, cluster_distances, max_cluster_distances, cluster_sizes
-
-    def normalize(self, x, norm_func=None):
-        """
-        Normalize the input data using a custom function.
-
-        Parameters
-        ----------
-        x: array-like
-            The input data to be normalized.
-        norm_func: callable, optional
-            A custom normalization or standardization function to be applied to the input data.
-            If provided, it should take the input data as its argument and return the preprocessed data.
-            Default is None, in which case the input data is returned as-is.
-
-        Returns
-        -------
-        x_preprocessed: array-like
-            The preprocessed input data.
-
-        Raises
-        ------
-        Warning
-            If `norm_func` is None, a warning is raised to indicate the potential inefficiency in SOM training.
-
-        Examples
-        --------
-        >>> import numpy as np
-        >>> from sklearn.datasets import load_iris
-        >>> from sklearn.feature_extraction.text import TfidfVectorizer
-        >>> from sklearn.preprocessing import StandardScaler
-
-        >>> # Case 1: Tabular data (without normalization)
-        >>> iris = load_iris()
-        >>> X = iris.data
-        >>> som = SOM(dimensions=(5, 5))
-        >>> X_norm = som.normalize(X)
-        >>> print(np.allclose(np.transpose(X_norm), X))
-        True
-
-        >>> # Case 2: Image data (using custom normalization)
-        >>> image_data = np.random.randint(0, 256, size=(28, 28))
-        >>> som = SOM(dimensions=(10, 10))
-        >>> custom_norm_func = lambda x: x / 255  # Custom normalization function
-        >>> image_data_norm = som.normalize(image_data, norm_func=custom_norm_func)
-        >>> print(image_data_norm.min(), image_data_norm.max())
-        0.0 1.0
-
-        >>> # Case 3: Text data (without normalization)
-        >>> text_data = ["This is a sample text.", "Another example sentence."]
-        >>> vectorizer = TfidfVectorizer()
-        >>> tfidf_matrix = vectorizer.fit_transform(text_data)
-        >>> som = SOM(dimensions=(8, 8))
-        >>> text_data_norm = som.normalize(tfidf_matrix.toarray())
-        >>> print(np.allclose(np.transpose(text_data_norm), tfidf_matrix.toarray()))
-        True
-        """
-
-        if norm_func is not None:
-            x_norm = norm_func(x)  # Use the provided custom normalization function
-            self.norm_func = norm_func
-        else:
-            warnings.warn(
-                "Without normalization function: SOM training may be inefficient if you are not normalized.",
-                UserWarning, stacklevel=2)
-            x_norm = x  # Return the input data as-is
-
-        return np.transpose(x_norm)
-
-    def quantization_error(self, dist):
-        """
-        Calculate quantization error
-        """
-        quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
-
-        return quant_err
-
-    def topological_error(self, x):
-        """
-        Calculate topological error
-        """
-        w = self.w
-        ndist = self.neuron_dist
-
-        # Normalize Input
-        x = self.normalize(x, self.norm_func)
-
-        # Calculate the distance between item vs. cluster center
-        x_w_dist = self._euclidean_distance(w, np.transpose(x))
-
-        sort_dist = np.argsort(x_w_dist, axis=0)
-        top_dist = [ndist[sort_dist[0, ii], sort_dist[1, ii]] for ii in range(sort_dist.shape[1])]
-        neighbors = np.where(np.array(top_dist) > 1.1)
-        top_error_1st = 100 * len(neighbors[0]) / x_w_dist.shape[1]
-        neighbors = np.where(np.array(top_dist) > 2.1)
-        top_error_1st_and_2nd = 100 * len(neighbors[0]) / x_w_dist.shape[1]
-
-        return top_error_1st, top_error_1st_and_2nd
-
-    def distortion_error(self, x):
-        """
-        Calculate distortion
-        """
-        # Normalize input data
-        x = self.normalize(x, self.norm_func)
-
-        shapx = x.shape
-        Q = shapx[1]  # Number of samples
-
-        ww = self.w
-        ndist = self.neuron_dist
-        x_w_dist = self._euclidean_distance(ww, np.transpose(x))
-        ind1 = np.argmin(x_w_dist, axis=0)
-
-        dd = [1, 2, 3]  # neighborhood distances
-        wwdist = self._euclidean_distance(ww, ww)
-        sst = ndist[:, ind1]
-
-        for d in dd:
-            factor1 = 2 * d * d
-            factor2 = Q * d * np.sqrt(2 * np.pi)
-            temp = np.exp(-np.multiply(sst, sst) / factor1)
-            distortion = np.sum(np.multiply(temp, x_w_dist)) / factor2
-            print('Distortion (d=' + str(d) + ') = ' + str(distortion))
-
-    def save_pickle(self, filename, path, data_format='pkl'):
-        """ Save the SOM object to a file using pickle.
-
-        Parameters
-        ----------
-        filename : str
-            The name of the file to save the SOM object to.
-
-        path : str
-            The path to the file to save the SOM object to.
-
-        data_format : str
-            The format to save the SOM object in. Must be one of: pkl
-
-        Returns
-        -------
-        None
-        """
-        if data_format not in ['pkl']:
-            raise ValueError('data_format must be one of: pkl')
-
-        if data_format == 'pkl':
-            with open(path + filename, 'wb') as f:
-                pickle.dump(self, f)
-
-    def load_pickle(self, filename, path, data_format='pkl'):
-        """ Load the SOM object from a file using pickle.
-
-        Parameters
-        ----------
-        filename : str
-            The name of the file to load the SOM object from.
-
-        path : str
-            The path to the file to load the SOM object from.
-
-        data_format : str
-            The format to load the SOM object from. Must be one of: pkl
-
-        Returns
-        -------
-        None
-        """
-        if data_format not in ['pkl']:
-            raise ValueError('data_format must be one of: pkl')
-
-        if data_format == 'pkl':
-            with open(path + filename, 'rb') as f:
-                som = pickle.load(f)
-
-        return som
-
-    def _normalize_position(self, position):  # Implement from utils
-        # Normalize the positions of the neurons to be in the range [-1, 1]
-        shap = position.shape
-        numPos = shap[1]
-        minPos = cp.ndarray.min(position,axis=1)
-        maxPos = cp.ndarray.max(position,axis=1)
-        difPos = maxPos - minPos
-        equal = cp.equal(minPos, maxPos)
-        difPos[equal] = 1
-        minPos = cp.expand_dims(minPos, axis=1)
-        minPos = cp.repeat(minPos, numPos, axis=1)
-        difPos = cp.expand_dims(difPos, axis=1)
-        difPos = cp.repeat(difPos, numPos, axis=1)
-        posit = 2 * ((position - minPos)/difPos) - 1
-        return posit
-
-    def _spread_positions(self, position, positionMean, positionBasis): # Implement from utils
-        # Spread the positions of the neurons
-        shappos = position.shape
-        numPos = shappos[1]
-        position1 = cp.repeat(positionMean, numPos, axis=1) + cp.matmul(positionBasis, position)
-        return position1
-
-    def _euclidean_distance(self, XA, XB):
-        """ Compute distance between each pair of the two collections of inputs.
-
-        Parameters
-        ----------
-        XA : array_like
-            An :math:`m_A` by :math:`n` array of :math:`m_A`
-            original observations in an :math:`n`-dimensional space.
-            Inputs are converted to float type.
-        XB : array_like
-            An :math:`m_B` by :math:`n` array of :math:`m_B`
-            original observations in an :math:`n`-dimensional space.
-            Inputs are converted to float type.
-
-        Returns
-        -------
-        Y : ndarray
-            A :math:`m_A` by :math:`m_B` distance matrix is returned.
-            For each :math:`i` and :math:`j`, the metric
-            ``dist(u=XA[i], v=XB[j])`` is computed and stored in the
-            :math:`ij` th entry.
-
-        Raises
-        ------
-        ValueError
-            An exception is thrown if `XA` and `XB` do not have
-            the same number of columns.
-
-
-        """
-        XA = cp.asarray(XA)
-        XB = cp.asarray(XB)
-
-        s = XA.shape
-        sB = XB.shape
-
-        if len(s) != 2:
-            raise ValueError('XA must be a 2-dimensional array.')
-        if len(sB) != 2:
-            raise ValueError('XB must be a 2-dimensional array.')
-        if s[1] != sB[1]:
-            raise ValueError('XA and XB must have the same number of columns '
-                            '(i.e. feature dimension.)')
-
-        XA2 = cp.sum(XA**2, axis=1).reshape(-1, 1)  # Squares of norms of x, reshaped to column vector
-        XB2 = cp.sum(XB**2, axis=1).reshape(1, -1)  # Squares of norms of y, reshaped to row vector
-        xy = cp.dot(XA, XB.T)  # Matrix product of x and transpose of y
-        distances = cp.sqrt(cp.maximum(0, XA2 + XB2 - 2 * xy))  # Ensure non-negative for sqrt
-
-        return distances
-
-    def _to_categorical(self, x, num_classes=None):
-        """ Converts a class vector (integers) to binary class matrix.
-
-        Args:
-        x: Array-like with class values to be converted into a matrix
-            (integers from 0 to `num_classes - 1`).
-        num_classes: Total number of classes. If `None`, this would be inferred
-            as `max(x) + 1`. Defaults to `None`.
-
-        Returns:
-        A binary matrix representation of the input as a NumPy or Cupy array. The class
-        axis is placed last.
-
-        Examples:
-
-        >>> a = self._to_categorical([0, 1, 2, 3], num_classes=4)
-        >>> a
-        array([[1., 0., 0., 0.],
-               [0., 1., 0., 0.],
-               [0., 0., 1., 0.],
-               [0., 0., 0., 1.]])
-        """
-        x = cp.array(x, dtype="int64")
-        input_shape = x.shape
-
-        # Shrink the last dimension if the shape is (..., 1).
-        if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-            input_shape = tuple(input_shape[:-1])
-
-        x = x.reshape(-1)
-        if not num_classes:
-            num_classes = cp.max(x) + 1
-        batch_size = x.shape[0]
-        categorical = cp.zeros((batch_size, num_classes))
-        categorical[cp.arange(batch_size), x] = 1
-        output_shape = input_shape + (num_classes,)
-        categorical = cp.reshape(categorical, output_shape)
-
-        return categorical
+try:
+    import cupy as cp
+    print("You are using GPU acceleration with Cupy")
+except ImportError:
+    print("CuPy is not available. For CPU-based operations, you can use the NumPy version of this SOM.")
+    print("Please consider installing the 'NNSOM' package, and use 'from NNSOM.som import SOM' for a NumPy-based SOM implementation.")
+    raise SystemExit
+
+from .utils import calculate_positions, distances
+
+import numpy as np
+from datetime import datetime
+import pickle
+import warnings
+
+
+class SOMGpu:
+    """
+    Represents a Self-Organizing Map (SOM) using GPU acceleration with CuPy.
+
+    A Self-Organizing Map (SOM) is an artificial neural network used for unsupervised learning,
+    which projects high-dimensional data into a lower-dimensional (typically two-dimensional) space.
+    It is trained using a competitive learning approach to produce a discretized representation
+    of the input space of training samples.
+
+    Attributes:
+        dimensions (tuple, list, np.ndarray): Dimensions of the SOM grid, defining the layout and number of neurons.
+        numNeurons (int): Total number of neurons, computed as the product of the grid dimensions.
+        pos (np.ndarray): Positions of neurons within the grid.
+        neuron_dist (np.ndarray): Precomputed Euclidean distances between neurons in the grid.
+        w (np.ndarray): Weight matrix representing the feature vectors of the neurons.
+        sim_flag (bool): Indicates if the SOM has been simulated/trained.
+        output (np.ndarray): Output from the latest simulation.
+        norm_func (callable): Function used to normalize input data.
+        sub_som (dict): Optional sub-clustering using additional SOMs at neuron positions.
+
+    Methods:
+        __init__(self, dimensions): Initializes the SOM with the specified dimensions.
+        init_w(self, x, norm_func=None): Initializes the weights using PCA on input data `x`.
+        sim_som(self, x): Simulates SOM processing for input `x`, identifying activated neurons.
+        train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
+            Trains the SOM using batch SOM algorithm on input data `x`.
+        quantization_error(self, dist): Calculates the quantization error of the model.
+        topological_error(self, data): Calculates the topological error of the model.
+        distortion_error(self, data): Calculates the distortion error of the model.
+        save_pickle(self, filename, path, data_format='pkl'): Saves the SOM object to a file in pickle format.
+        load_pickle(self, filename, path, data_format='pkl'): Loads the SOM object from a file in pickle format.
+        _normalize_position(self, position): Helper method to normalize neuron positions.
+        _spread_positions(self, position, positionMean, positionBasis): Helper method to adjust neuron positions.
+        _euclidean_distance(self, XA, XB): Computes Euclidean distances between two sets of vectors.
+        _to_categorical(self, x, num_classes=None): Converts class vector to binary class matrix.
+
+    Raises:
+        ImportError: If CuPy is not available, suggests using the NNSOM package for a NumPy-based implementation.
+
+    Example:
+        >>> dimensions = (10, 10)
+        >>> som = SOMGpu(dimensions)
+        >>> data = np.random.rand(100, 10)
+        >>> som.init_w(data, norm_func=None)
+        >>> som.train(data, norm_func=None)
+        >>> output = som.sim_som(data)
+    """
+    def __init__(self, dimensions):
+        """
+        Initializes the SOM with the specified dimensions and calculates the positions and distances between neurons in the SOM grid.
+
+        Parameters
+        ----------
+        dimensions : tuple, list, or np.ndarray
+                    The dimensions (shape) of the SOM grid.
+        """
+
+        self.dimensions = dimensions  # Processing as numpy
+        self.numNeurons = np.prod(dimensions) # Processing as numpy
+        # Calculate positions of neurons
+        self.pos = calculate_positions(dimensions)
+        # Calculate distances between neurons
+        self.neuron_dist = distances(self.pos)
+        # Initialize the weight matrix with empty list
+        self.w = []
+        # Set simulation flag to True,  needs to do simulation
+        self.sim_flag = True
+        # Initialize the output of simulation
+        self.output = None
+        # Initialize a normalize() function
+        self.norm_func = None
+
+        # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
+        self.sub_som = {}
+
+    def init_w(self, x, norm_func=None):
+        """
+        Initializes the weights of the SOM using principal components analysis (PCA) on the input data x.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data used for weight initialization.
+        """
+        # Initialize SOM weights using principal components
+
+        # Print Beginning time for initialization
+        print('Beginning Initialization')
+        now = datetime.now()
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+        x = cp.asarray(x)
+
+        sz = x.shape
+
+        posMean = cp.mean(x, axis=1)
+        posMean = cp.expand_dims(posMean, axis=1)
+
+        xc = x - posMean
+
+        components, gains, encodedInputsT = cp.linalg.svd(xc)
+
+        encodedInputsT = cp.transpose(encodedInputsT)
+
+        basis = components * gains
+        stdev = cp.std(encodedInputsT, axis=0)
+        stdev = stdev[:len(basis)]
+        posBasis = 2.5 * basis * stdev
+
+        numNeurons = self.numNeurons
+        numDimensions = len(self.dimensions)
+        dimensions = self.dimensions
+        sampleSize = sz[1]
+        inputSize = sz[0]
+        dimOrder = cp.argsort(cp.asarray(dimensions))
+
+        restoreOrder = cp.concatenate((cp.sort(dimOrder), cp.arange(numDimensions, cp.minimum(inputSize, sampleSize))))
+
+        if numDimensions > inputSize:
+            posBasis = cp.concatenate((posBasis, cp.random.rand(inputSize, inputSize) * 0.001))
+
+        posBasis = posBasis[restoreOrder]
+
+        pos1 = self.pos
+        pos1 = cp.asarray(pos1)
+
+        if sampleSize < inputSize:
+            posBasis = cp.concatenate((posBasis, cp.zeros((inputSize, inputSize - sampleSize))))
+
+        if inputSize > numDimensions:
+            pos1 = cp.concatenate((pos1, cp.zeros((inputSize - numDimensions, numNeurons))), axis=0)
+
+        pos2 = self._normalize_position(pos1)
+
+        pos3 = self._spread_positions(pos2, posMean, posBasis)
+
+        self.w = cp.asnumpy(cp.transpose(pos3))
+
+        # Print Ending time for initialization
+        print('Ending Initialization')
+        now = datetime.now()
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+    def sim_som(self, x):
+        """
+        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to simulate the SOM with.
+
+        Returns
+        -------
+        np.ndarray
+            The simulated output of the SOM.
+        """
+        # Simulate the SOM, with x as the input
+        # Transform np.ndarray into cp.ndarray
+        w = cp.asarray(self.w)
+        x = cp.asarray(x)
+
+        # Compute the negative distance from the inputs to each center
+        n = -self._euclidean_distance(w, cp.transpose(x))
+
+        # Find out which center was closest to the input
+        maxRows = cp.argmax(n, axis=0)
+        a = self._to_categorical(maxRows, num_classes=n.shape[0]) #made correction-added number of class
+        a = cp.asnumpy(a)
+
+        return np.transpose(a)
+
+    def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
+        """
+        Trains the SOM using the batch SOM algorithm on the input data x.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to train the SOM with.
+        init_neighborhood : int, optional
+            The initial neighborhood size.
+        epochs : int, optional
+            The number of epochs to train for.
+        steps : int, optional
+            The number of steps for training.
+
+        Returns
+        -------
+        None
+        """
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+        x = cp.asarray(x)
+
+        # Train the SOM using the batch SOM algorithm
+
+        w = self.w
+        w = cp.asarray(w)
+        shapw = w.shape
+        S = shapw[0]
+        shapx = x.shape
+        Q = shapx[1]
+
+        step = 0
+
+        print('Beginning Training')
+        now = datetime.now()
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+        # Train the network
+        for i in range(epochs):
+
+            # network output
+            a = self.sim_som(x)
+            a = cp.asarray(a)
+
+            # neighborhood distance
+            nd = 1 + (init_neighborhood-1) * (1 - step/steps)
+            neighborhood = self.neuron_dist <= nd
+            neighborhood = cp.asarray(neighborhood)
+            #print(nd)
+            # remove some outputs at random
+            a = a * (cp.random.rand(S, Q) < 0.90)
+            a2 = cp.matmul(neighborhood, a) + a
+
+            # find how many times each neuron won
+            # (The winning neuron is the one that exhibits the smallest distance or similarity to the input data)
+            suma2 = cp.sum(a2, axis=1)
+            loserIndex = cp.squeeze(cp.asarray(suma2 == 0))
+            suma2[loserIndex] = 1
+            suma2 = cp.expand_dims(suma2,axis = 1)
+            a3 = a2 / cp.repeat(suma2, Q, axis=1)
+
+            neww = cp.matmul(a3, cp.transpose(x))
+
+            dw = neww - w
+
+            dw[loserIndex] = 0
+
+            w = w + cp.array(dw)
+
+            step = step + 1
+
+            if step % 50 == 0:
+                print(step)
+                now = datetime.now()
+                current_time = now.strftime("%H:%M:%S")
+                print("Current Time =", current_time)
+
+        self.w = cp.asnumpy(w)
+        self.outputs = self.sim_som(x)
+        self.sim_flag = False
+
+        print('Ending Training')
+        current_time = now.strftime("%H:%M:%S")
+        print("Current Time =", current_time)
+
+    def cluster_data(self, x):
+        """
+        Cluster the input data based on the trained SOM reference vectors.
+
+        Parameters
+        ----------
+        x : ndarray (normalized)
+            The input data to be clustered.
+
+        Returns
+        -------
+        clusters : list of lists
+            A list containing sub-lists, where each sublist represents a cluster.
+            The indices of the input data points belonging to the same cluster
+            are stored in the corresponding sublist, sorted by their proximity
+            to the cluster center.
+
+        cluster_distances : list of lists
+            A list containing sub-lists, where each sublist represents the distances
+            of the input data points to the corresponding cluster center, sorted in
+            the same order as the indices in the `clusters` list.
+
+        max_cluster_distances : ndarray
+            A list containing the maximum distance between each cluster center
+            and the data points belonging to that cluster.
+
+        cluster_sizes : ndarray
+            A list containing the number of data points in each cluster.
+
+        Raises
+        -------
+        ValueError
+            If the SOM has not been trained.
+
+        ValueError
+            If the number of features in the input data and the SOM weights do not match.
+        """
+
+        if self.sim_flag:
+            raise ValueError("SOM has not been trained.")
+
+        if x.shape[1] != self.w.shape[1]:
+            raise ValueError('The number of features in the input data and the SOM weights do not match.')
+
+        # Normalize the input data
+        x = self.normalize(x, self.norm_func)
+        x = cp.asarray(x)
+
+        w = self.w
+        w = cp.asarray(w)
+        shapw = w.shape
+        S = shapw[0]
+
+        x_w_dist = self._euclidean_distance(w, cp.transpose(x))
+        ind1 = cp.argmin(x_w_dist, axis=0)
+
+        clusters = []  # a cluster array of indices sorted by distances
+        cluster_distances = []  # a cluster array of distances sorted by distances
+        max_cluster_distances = cp.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
+        cluster_sizes = []  # cluster array sizes
+
+        for i in range(S):
+            # Find which inputs are closest to each weight (in cluster i)
+            tempclust = cp.where(ind1 == i)[0]
+
+            # Save distance of each input in the cluster to cluster center (weight)
+            tempdist = x_w_dist[i, tempclust]
+            indsort = cp.argsort(tempdist)
+            tempclust = tempclust[indsort]  # Sort indices
+            tempdist = tempdist[indsort]
+
+            # Add to distance array sorted distances
+            cluster_distances.append(tempdist)
+
+            # Add to Cluster array sorted indices
+            clusters.append(tempclust)
+
+            # Cluster size
+            num = len(tempclust)
+            cluster_sizes.append(num)
+
+            # Save the maximum distance to any input in the cluster from cluster center
+            if num > 0:
+                max_cluster_distances[i] = tempdist[-1]
+
+        # Convert clusters to a list of lists
+        clusters = [clust.get().tolist() for clust in clusters]
+        # Convert cluster_distances to a list of lists
+        cluster_distances = [dist.get().tolist() for dist in cluster_distances]
+        # Convert max_cluster_distances to a NumPy array
+        max_cluster_distances = max_cluster_distances.get()
+        # Convert cluster_sizes to a NumPy array
+        cluster_sizes = np.array(cluster_sizes)
+
+        return clusters, cluster_distances, max_cluster_distances, cluster_sizes
+
+    def normalize(self, x, norm_func=None):
+        """
+        Normalize the input data using a custom function.
+
+        Parameters
+        ----------
+        x: array-like
+            The input data to be normalized.
+        norm_func: callable, optional
+            A custom normalization or standardization function to be applied to the input data.
+            If provided, it should take the input data as its argument and return the preprocessed data.
+            Default is None, in which case the input data is returned as-is.
+
+        Returns
+        -------
+        x_preprocessed: array-like
+            The preprocessed input data.
+
+        Raises
+        ------
+        Warning
+            If `norm_func` is None, a warning is raised to indicate the potential inefficiency in SOM training.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> from sklearn.datasets import load_iris
+        >>> from sklearn.feature_extraction.text import TfidfVectorizer
+        >>> from sklearn.preprocessing import StandardScaler
+
+        >>> # Case 1: Tabular data (without normalization)
+        >>> iris = load_iris()
+        >>> X = iris.data
+        >>> som = SOM(dimensions=(5, 5))
+        >>> X_norm = som.normalize(X)
+        >>> print(np.allclose(np.transpose(X_norm), X))
+        True
+
+        >>> # Case 2: Image data (using custom normalization)
+        >>> image_data = np.random.randint(0, 256, size=(28, 28))
+        >>> som = SOM(dimensions=(10, 10))
+        >>> custom_norm_func = lambda x: x / 255  # Custom normalization function
+        >>> image_data_norm = som.normalize(image_data, norm_func=custom_norm_func)
+        >>> print(image_data_norm.min(), image_data_norm.max())
+        0.0 1.0
+
+        >>> # Case 3: Text data (without normalization)
+        >>> text_data = ["This is a sample text.", "Another example sentence."]
+        >>> vectorizer = TfidfVectorizer()
+        >>> tfidf_matrix = vectorizer.fit_transform(text_data)
+        >>> som = SOM(dimensions=(8, 8))
+        >>> text_data_norm = som.normalize(tfidf_matrix.toarray())
+        >>> print(np.allclose(np.transpose(text_data_norm), tfidf_matrix.toarray()))
+        True
+        """
+
+        if norm_func is not None:
+            x_norm = norm_func(x)  # Use the provided custom normalization function
+            self.norm_func = norm_func
+        else:
+            warnings.warn(
+                "Without normalization function: SOM training may be inefficient if you are not normalized.",
+                UserWarning, stacklevel=2)
+            x_norm = x  # Return the input data as-is
+
+        return np.transpose(x_norm)
+
+    def quantization_error(self, dist):
+        """
+        Calculate quantization error
+        """
+        quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
+
+        return quant_err
+
+    def topological_error(self, x):
+        """
+        Calculate topological error
+        """
+        w = self.w
+        ndist = self.neuron_dist
+
+        # Normalize Input
+        x = self.normalize(x, self.norm_func)
+
+        # Calculate the distance between item vs. cluster center
+        x_w_dist = self._euclidean_distance(w, np.transpose(x))
+
+        sort_dist = np.argsort(x_w_dist, axis=0)
+        top_dist = [ndist[sort_dist[0, ii], sort_dist[1, ii]] for ii in range(sort_dist.shape[1])]
+        neighbors = np.where(np.array(top_dist) > 1.1)
+        top_error_1st = 100 * len(neighbors[0]) / x_w_dist.shape[1]
+        neighbors = np.where(np.array(top_dist) > 2.1)
+        top_error_1st_and_2nd = 100 * len(neighbors[0]) / x_w_dist.shape[1]
+
+        return top_error_1st, top_error_1st_and_2nd
+
+    def distortion_error(self, x):
+        """
+        Calculate distortion
+        """
+        # Normalize input data
+        x = self.normalize(x, self.norm_func)
+
+        shapx = x.shape
+        Q = shapx[1]  # Number of samples
+
+        ww = self.w
+        ndist = self.neuron_dist
+        x_w_dist = self._euclidean_distance(ww, np.transpose(x))
+        ind1 = np.argmin(x_w_dist, axis=0)
+
+        dd = [1, 2, 3]  # neighborhood distances
+        wwdist = self._euclidean_distance(ww, ww)
+        sst = ndist[:, ind1]
+
+        for d in dd:
+            factor1 = 2 * d * d
+            factor2 = Q * d * np.sqrt(2 * np.pi)
+            temp = np.exp(-np.multiply(sst, sst) / factor1)
+            distortion = np.sum(np.multiply(temp, x_w_dist)) / factor2
+            print('Distortion (d=' + str(d) + ') = ' + str(distortion))
+
+    def save_pickle(self, filename, path, data_format='pkl'):
+        """ Save the SOM object to a file using pickle.
+
+        Parameters
+        ----------
+        filename : str
+            The name of the file to save the SOM object to.
+
+        path : str
+            The path to the file to save the SOM object to.
+
+        data_format : str
+            The format to save the SOM object in. Must be one of: pkl
+
+        Returns
+        -------
+        None
+        """
+        if data_format not in ['pkl']:
+            raise ValueError('data_format must be one of: pkl')
+
+        if data_format == 'pkl':
+            with open(path + filename, 'wb') as f:
+                pickle.dump(self, f)
+
+    def load_pickle(self, filename, path, data_format='pkl'):
+        """ Load the SOM object from a file using pickle.
+
+        Parameters
+        ----------
+        filename : str
+            The name of the file to load the SOM object from.
+
+        path : str
+            The path to the file to load the SOM object from.
+
+        data_format : str
+            The format to load the SOM object from. Must be one of: pkl
+
+        Returns
+        -------
+        None
+        """
+        if data_format not in ['pkl']:
+            raise ValueError('data_format must be one of: pkl')
+
+        if data_format == 'pkl':
+            with open(path + filename, 'rb') as f:
+                som = pickle.load(f)
+
+        return som
+
+    def _normalize_position(self, position):  # Implement from utils
+        # Normalize the positions of the neurons to be in the range [-1, 1]
+        shap = position.shape
+        numPos = shap[1]
+        minPos = cp.ndarray.min(position,axis=1)
+        maxPos = cp.ndarray.max(position,axis=1)
+        difPos = maxPos - minPos
+        equal = cp.equal(minPos, maxPos)
+        difPos[equal] = 1
+        minPos = cp.expand_dims(minPos, axis=1)
+        minPos = cp.repeat(minPos, numPos, axis=1)
+        difPos = cp.expand_dims(difPos, axis=1)
+        difPos = cp.repeat(difPos, numPos, axis=1)
+        posit = 2 * ((position - minPos)/difPos) - 1
+        return posit
+
+    def _spread_positions(self, position, positionMean, positionBasis): # Implement from utils
+        # Spread the positions of the neurons
+        shappos = position.shape
+        numPos = shappos[1]
+        position1 = cp.repeat(positionMean, numPos, axis=1) + cp.matmul(positionBasis, position)
+        return position1
+
+    def _euclidean_distance(self, XA, XB):
+        """ Compute distance between each pair of the two collections of inputs.
+
+        Parameters
+        ----------
+        XA : array_like
+            An :math:`m_A` by :math:`n` array of :math:`m_A`
+            original observations in an :math:`n`-dimensional space.
+            Inputs are converted to float type.
+        XB : array_like
+            An :math:`m_B` by :math:`n` array of :math:`m_B`
+            original observations in an :math:`n`-dimensional space.
+            Inputs are converted to float type.
+
+        Returns
+        -------
+        Y : ndarray
+            A :math:`m_A` by :math:`m_B` distance matrix is returned.
+            For each :math:`i` and :math:`j`, the metric
+            ``dist(u=XA[i], v=XB[j])`` is computed and stored in the
+            :math:`ij` th entry.
+
+        Raises
+        ------
+        ValueError
+            An exception is thrown if `XA` and `XB` do not have
+            the same number of columns.
+
+
+        """
+        XA = cp.asarray(XA)
+        XB = cp.asarray(XB)
+
+        s = XA.shape
+        sB = XB.shape
+
+        if len(s) != 2:
+            raise ValueError('XA must be a 2-dimensional array.')
+        if len(sB) != 2:
+            raise ValueError('XB must be a 2-dimensional array.')
+        if s[1] != sB[1]:
+            raise ValueError('XA and XB must have the same number of columns '
+                            '(i.e. feature dimension.)')
+
+        XA2 = cp.sum(XA**2, axis=1).reshape(-1, 1)  # Squares of norms of x, reshaped to column vector
+        XB2 = cp.sum(XB**2, axis=1).reshape(1, -1)  # Squares of norms of y, reshaped to row vector
+        xy = cp.dot(XA, XB.T)  # Matrix product of x and transpose of y
+        distances = cp.sqrt(cp.maximum(0, XA2 + XB2 - 2 * xy))  # Ensure non-negative for sqrt
+
+        return distances
+
+    def _to_categorical(self, x, num_classes=None):
+        """ Converts a class vector (integers) to binary class matrix.
+
+        Args:
+        x: Array-like with class values to be converted into a matrix
+            (integers from 0 to `num_classes - 1`).
+        num_classes: Total number of classes. If `None`, this would be inferred
+            as `max(x) + 1`. Defaults to `None`.
+
+        Returns:
+        A binary matrix representation of the input as a NumPy or Cupy array. The class
+        axis is placed last.
+
+        Examples:
+
+        >>> a = self._to_categorical([0, 1, 2, 3], num_classes=4)
+        >>> a
+        array([[1., 0., 0., 0.],
+               [0., 1., 0., 0.],
+               [0., 0., 1., 0.],
+               [0., 0., 0., 1.]])
+        """
+        x = cp.array(x, dtype="int64")
+        input_shape = x.shape
+
+        # Shrink the last dimension if the shape is (..., 1).
+        if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
+            input_shape = tuple(input_shape[:-1])
+
+        x = x.reshape(-1)
+        if not num_classes:
+            num_classes = cp.max(x) + 1
+        batch_size = x.shape[0]
+        categorical = cp.zeros((batch_size, num_classes))
+        categorical[cp.arange(batch_size), x] = 1
+        output_shape = input_shape + (num_classes,)
+        categorical = cp.reshape(categorical, output_shape)
+
+        return categorical
```

### Comparing `nnsom-1.7.7/src/NNSOM/utils.py` & `nnsom-1.7.8/src/NNSOM/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,653 +1,653 @@
-from scipy.spatial.distance import cdist
-from scipy import sparse
-import numpy as np
-import networkx as nx
-from matplotlib.widgets import Button
-
-
-def preminmax(p):
-    # Normalize the inputs to be in the range [-1, 1]
-    minp = np.amin(p, 1)
-    maxp = np.amax(p, 1)
-
-    equal = np.equal(minp, maxp)
-    nequal = np.logical_not(equal)
-
-    if sum(equal) != 0:
-        print('Some maximums and minimums are equal. Those inputs won''t be transformed.')
-        minp0 = minp*nequal - 1*equal
-        maxp0 = maxp*nequal + 1*equal
-    else:
-        minp0 = minp
-        maxp0 = maxp
-
-    minp0 = np.expand_dims(minp0, axis=1)
-    maxp0 = np.expand_dims(maxp0, axis=1)
-    pn = 2*(p-minp0)/(maxp0-minp0) - 1
-    return pn, minp, maxp
-
-
-def calculate_positions(dim):
-    # Calculate the positions of the neurons in the SOM
-    dims = len(dim)
-    position = np.zeros((dims, np.prod(dim)))
-    len1 = 1
-
-    center = 0
-
-    for i in range(2):
-        dimi = dim[i]
-        newlen = len1 * dimi
-        offset = np.sqrt(1 - center*center)
-
-        if i == 1:
-            for j in range(1, dimi):
-                ishift = [center * (j % 2)]
-                doshift = np.array(ishift*len1)
-                position[0, np.arange(len1)+len1*j] = position[0, np.arange(len1)] + doshift
-
-        posi = np.array(range(dimi)) * offset
-        ind2 = np.floor(np.arange(newlen) / len1)
-        ind2 = ind2.astype(int)
-        position[i, np.arange(newlen)] = posi[ind2]
-
-        len1 = newlen
-        center = 0.5
-
-    return position
-
-
-def cart2pol(x, y):
-    # Convert cartesian coordinates to polar coordinates
-    theta = np.arctan2(y, x)
-    rho = np.hypot(x, y)
-    return theta, rho
-
-
-def pol2cart(theta, rho):
-    # Convert polar coordinates to cartesian coordinates
-    x = rho * np.cos(theta)
-    y = rho * np.sin(theta)
-    return x, y
-
-
-def rotate_xy(x1, y1, angle):
-    # Rotate the coordinates x1, y1 by angle
-    [a, r] = cart2pol(x1, y1)
-    a = a + angle
-    x2, y2 = pol2cart(a, r)
-    return x2, y2
-
-
-def normalize_position(position):
-    # Normalize the positions of the neurons to be in the range [-1, 1]
-    shap = position.shape
-    numPos = shap[1]
-    minPos = np.ndarray.min(position,axis=1)
-    maxPos = np.ndarray.max(position,axis=1)
-    difPos = maxPos - minPos
-    equal = np.equal(minPos, maxPos)
-    difPos[equal] = 1
-    minPos = np.expand_dims(minPos, axis=1)
-    minPos = np.repeat(minPos, numPos, axis=1)
-    difPos = np.expand_dims(difPos, axis=1)
-    difPos = np.repeat(difPos, numPos, axis=1)
-    posit = 2 * ((position - minPos)/difPos) - 1
-    return posit
-
-
-def spread_positions(position, positionMean, positionBasis):
-    # Spread the positions of the neurons
-    shappos = position.shape
-    numPos = shappos[1]
-    position1 = np.repeat(positionMean, numPos, axis=1) + np.matmul(positionBasis, position)
-    return position1
-
-
-def distances(pos):
-    # Compute the distances between the neurons in the SOM topology
-    posT = np.transpose(pos)
-    dist = cdist(posT, posT, 'euclidean')
-
-    link = dist <= 1.00001
-    link = sparse.csr_matrix(1.0*link)
-
-    g = nx.DiGraph(link)
-    dist = nx.floyd_warshall_numpy(g)
-
-    return dist
-
-
-def get_hexagon_shape():
-    # Determine the shape of the hexagon to represent each cluster
-    shapex = np.array([-1, 0, 1, 1, 0, -1]) * 0.5
-    shapey = np.array([1, 2, 1, -1, -2, -1]) * np.sqrt(0.75) / 3
-    return shapex, shapey
-
-
-def get_edge_shape():
-    # Determine the shape of the elongated hexagon to represent edge between each cluster
-    edgex = np.array([-1, 0, 1, 0]) * 0.5
-    edgey = np.array([0, 1, 0, - 1]) * np.sqrt(0.75) / 3
-
-    return edgex, edgey
-
-
-# Helper Functions to extract information from the input data for passing to the plot
-def get_cluster_data(data, clust):
-    """
-    For each cluster, extract the corresponding data points and return them in a list.
-
-    Parameters
-    ----------
-    data : numpy array
-        The dataset from which to extract the clusters' data.
-    clust : list of arrays
-        A list where each element is an array of indices for data points in the corresponding cluster.
-
-    Returns
-    -------
-    cluster_data_list : list of numpy arrays
-        A list where each element is a numpy array containing the data points of a cluster.
-    """
-    cluster_data_list = []
-    for cluster_indices in clust:
-        if len(cluster_indices) > 0:
-            # Ensure cluster_indices are integers and within the range of data
-            cluster_indices = np.array(cluster_indices, dtype=int)
-            cluster_data = data[cluster_indices]
-            cluster_data_list.append(cluster_data)
-        else:
-            cluster_data_list.append(np.array([]))  # Use an empty array for empty clusters
-
-    return cluster_data_list
-
-
-def get_cluster_array(feature, clust):
-    """
-    Returns a NumPy array of objects, each containing the feature values for each cluster.
-
-    Parameters
-    ----------
-    feature : array-like
-        Feature array.
-    clust : list
-        A list of cluster arrays, each containing indices sorted by distances.
-
-    Returns
-    -------
-    cluster_array : numpy.ndarray
-        A NumPy array where each element is an array of feature values for that cluster.
-    """
-    cluster_array = np.empty(len(clust), dtype=object)
-
-    for i, cluster_indices in enumerate(clust):
-        if len(cluster_indices) > 0:
-            cluster_array[i] = feature[cluster_indices]
-        else:
-            cluster_array[i] = np.array([])  # Store an empty array if the cluster is empty
-
-    return cluster_array
-
-
-def get_cluster_avg(feature, clust):
-    """
-    Returns the average value of a feature for each cluster.
-
-    Parameters
-    ----------
-    feature : array-like
-        Feature array.
-    clust : list
-        A list of cluster arrays, each containing indices sorted by distances.
-
-    Returns
-    -------
-    cluster_avg : numpy array
-        A cluster array with the average value of the feature for each cluster.
-    """
-    cluster_array = get_cluster_array(feature, clust)
-    cluster_avg = np.zeros(len(cluster_array))
-    for i in range(len(cluster_array)):
-        if len(cluster_array[i]) > 0:
-            cluster_avg[i] = np.mean(cluster_array[i])
-
-    return cluster_avg
-
-
-def closest_class_cluster(cat_feature, clust):
-    """
-    Returns the cluster array with the closest class for each cluster.
-
-    Paramters
-    ----------
-    cat_feature : array-like
-        Categorical feature array.
-    clust : list
-        A cluster array of indices sorted by distances.
-
-    Returns
-    -------
-    closest_class : numpy array
-        A cluster array with the closest class for each cluster.
-    """
-    closest_class = np.zeros(len(clust))
-    for i in range(len(clust)):
-        cluster_indices = clust[i]
-        if len(cluster_indices) > 0:
-            closest_class[i] = cat_feature[cluster_indices[0]]
-        else:
-            closest_class[i] = None  # Avoid division by zero if the cluster is empty
-
-    return closest_class
-
-
-def majority_class_cluster(cat_feature, clust):
-    """
-    Returns the cluster array with the majority class for each cluster.
-
-    Paramters
-    ----------
-    cat_feature : array-like
-        Categorical feature array.
-    clust : list
-        A cluster array of indices sorted by distances.
-
-    Returns
-    -------
-    majority_class : numpy array
-        A cluster array with the majority class
-    """
-    majority_class = np.zeros(len(clust))
-    for i in range(len(clust)):
-        cluster_indices = clust[i]
-        if len(cluster_indices) > 0:
-            majority_class[i] = np.argmax(np.bincount(cat_feature[cluster_indices]))
-        else:
-            majority_class[i] = None  # Avoid division by zero if the cluster is empty
-
-    return majority_class
-
-
-def get_perc_cluster(cat_feature, target, clust):
-    """
-    Return cluster array with the percentage of a specific target class in each cluster.
-
-    Parameters
-    ----------
-    cat_feature : array-like
-        Categorical feature array.
-    target : int or str
-        Target class to calculate the percentage.
-    clust : list
-        A cluster array of indices sorted by distances.
-
-    Returns
-    -------
-    cluster_array : numpy array
-        A cluster array with the percentage of target class.
-    """
-    # Create Cluster Array with the percentage of target class
-    cluster_array = np.zeros(len(clust))
-    for i in range(len(clust)):
-        cluster_indices = clust[i]
-        if len(cluster_indices) > 0:
-            cluster_array[i] = np.sum(cat_feature[cluster_indices] == target) / len(cluster_indices)
-        else:
-            cluster_array[i] = 0  # Avoid division by zero if the cluster is empty
-
-    return cluster_array * 100
-
-
-def count_classes_in_cluster(cat_feature, clust):
-    """
-    Count the occurrences of each class in each cluster using vectorized operations
-    for efficiency.
-
-    Parameters
-    ----------
-    cat_feature : array-like
-        Categorical feature array.
-    clust : list
-        A list of arrays, each containing the indices of elements in a cluster.
-
-    Returns
-    -------
-    cluster_counts : numpy array
-        A 2D array with counts of each class in each cluster.
-    """
-    unique_classes, _ = np.unique(cat_feature, return_counts=True)
-    num_classes = len(unique_classes)
-
-    # Initialize the array to hold class counts for each cluster
-    cluster_counts = np.zeros((len(clust), num_classes), dtype=int)
-
-    # Loop over clusters to count class occurrences
-    for i, indices in enumerate(clust):
-        if len(indices) > 0:
-            # Count occurrences of each class in the cluster
-            cluster_counts[i] = [np.sum(cat_feature[indices] == cls) for cls in unique_classes]
-        else:
-            cluster_counts[i] = np.zeros(num_classes, dtype=int)
-
-    return cluster_counts
-
-
-def cal_class_cluster_intersect(clust, *args):
-    """
-    Calculate the intersection sizes of each class with each neuron cluster.
-
-    This function computes the size of the intersection between each given class
-    (represented by arrays of indices) and each neuron cluster (represented by
-    a list of lists of indices). The result is a 2D array where each row corresponds
-    to a neuron cluster, and each column corresponds to one of the classes.
-
-    Parameters
-    ----------
-    clust : list of lists
-        A collection of neuron clusters, where each neuron cluster is a list of indices.
-    *args : sequence of array-like
-        A variable number of arrays, each representing a class with indices.
-
-    Returns
-    -------
-    numpy.ndarray
-        A 2D array where the entry at position (i, j) represents the number of indices
-        in the j-th class that are also in the i-th neuron cluster.
-
-    Examples
-    --------
-    >>> clust = [[4, 5, 9], [1, 7], [2, 10, 11], [3, 6, 8]]
-    >>> ind1 = np.array([1, 2, 3])
-    >>> ind2 = np.array([4, 5, 6])
-    >>> ind3 = np.array([7, 8, 9])
-    >>> ind4 = np.array([10, 11, 12])
-    >>> get_sizes_clust(clust, ind1, ind2, ind3, ind4)
-    array([[0, 2, 1, 0],
-           [1, 0, 1, 0],
-           [1, 0, 0, 2],
-           [1, 1, 1, 0]])
-    """
-    numst = list(args)
-
-    cluster_sizes_matrix = np.zeros((len(numst), len(clust)))
-
-    for i, ind in enumerate(numst):
-        for j, cluster in enumerate(clust):
-            cluster_sizes_matrix[i][j] = np.sum(np.isin(cluster, ind))
-
-    return cluster_sizes_matrix.T
-
-
-# Helper function  to extract information from the post-training model for passing to the plot
-def get_ind_misclassified(target, prediction):
-    """
-    Get the indices of misclassified items.
-
-    Parameters
-    ----------
-    target : array-like
-        The true target values.
-    prediction : array-like
-        The predicted values.
-
-    Returns
-    -------
-    misclassified_indices : list
-        List of indices of misclassified items.
-    """
-    misclassified_indices = np.where(target != prediction)[0]
-
-    return misclassified_indices
-
-
-def get_perc_misclassified(target, prediction, clust):
-    """
-    Calculate the percentage of misclassified items in each cluster and return as a numpy array.
-
-    Parameters
-    ----------
-    target : array-like
-        The true target values.
-    prediction : array-like
-        The predicted values.
-    clust : array-like
-        List of arrays, each containing the indices of elements in a cluster.
-
-    Returns
-    -------
-    proportion_misclassified : numpy array
-        Percentage of misclassified items in each cluster.
-    """
-    # Get the indices of misclassified items.
-    misclassified_indices = get_ind_misclassified(target, prediction)
-
-    # Initialize array to store proportion of misclassified items
-    proportion_misclassified = np.zeros(len(clust))
-
-    for i, cluster_indices in enumerate(clust):
-        if len(cluster_indices) > 0:
-            # Compute intersection of cluster indices and misclassified indices
-            misclassified_count = np.intersect1d(cluster_indices, misclassified_indices).size
-            proportion_misclassified[i] = (misclassified_count / len(cluster_indices)) * 100
-
-    return proportion_misclassified
-
-
-def get_conf_indices(target, results, target_class):
-    """
-    Get the indices of True Positive, True Negative, False Positive, and False Negative for a specific target class.
-
-    Parameters
-    ----------
-    target : array-like
-        The true target values.
-    results : array-like
-        The predicted values.
-    target_class : int
-        The target class for which to get the confusion indices.
-
-    Returns
-    -------
-    tp_index : numpy array
-        Indices of True Positives.
-    tn_index : numpy array
-        Indices of True Negatives.
-    fp_index : numpy array
-        Indices of False Positives.
-    fn_index : numpy array
-        Indices of False Negatives.
-    """
-    tp_index = np.where((target == target_class) & (results == target_class))[0]
-    tn_index = np.where((target != target_class) & (results != target_class))[0]
-    fp_index = np.where((target != target_class) & (results == target_class))[0]
-    fn_index = np.where((target == target_class) & (results != target_class))[0]
-
-    return tp_index, tn_index, fp_index, fn_index
-
-
-def get_dominant_class_error_types(dominant_classes, error_types):
-    """
-    Map dominant class to the corresponding majority error type for each cluster,
-    dynamically applying the correct error type based on the dominant class.
-
-    Parameters:
-    ---------------
-    dominant_classes: array-like (som.numNeurons, )
-        List of dominant class labels for each cluster. May contain NaN values.
-    error_types: list of array-like (numClasses, som.numNeurons)
-        Variable number of arrays, each representing majority error types for each class.
-
-    Returns:
-    ---------------
-    array-like (som.numNeurons, )
-        List of majority error type for each cluster corresponding to the dominant class.
-    """
-    if len(error_types) < np.max([dc for dc in dominant_classes if not np.isnan(dc)]) + 1:
-        raise ValueError("Not enough error type arrays provided for all classes.")
-
-    # Initialize the output array with NaNs to handle possible missing classes
-    output_error_types = np.full(len(dominant_classes), np.nan)
-
-    # Map the correct error type based on the dominant class
-    for idx, dominant_class in enumerate(dominant_classes):
-        if not np.isnan(dominant_class):  # Check if the dominant class is not NaN
-            if dominant_class < len(error_types):
-                output_error_types[idx] = error_types[int(dominant_class)][idx]
-            else:
-                raise ValueError(f"Class {dominant_class} is out of the provided error type array bounds.")
-        else:
-            output_error_types[idx] = np.nan  # Explicitly setting NaN if no dominant class
-
-    return output_error_types
-
-
-def flatten(data):
-    """
-    Recursively flattens a nested list structure of numbers into a single list.
-
-    Args:
-        data: A number (int or float) or a nested list of numbers. The data to be flattened.
-
-    Returns:
-        A list of numbers, where all nested structures in the input have been
-        flattened into a single list.
-    """
-    if isinstance(data, (int, float, np.float64)):  # base case for numbers
-        return [data]
-    else:
-        flat_list = []
-        for item in data:
-            flat_list.extend(flatten(item))  # recursive call to flatten
-        return flat_list
-
-
-def get_global_min_max(data):
-    """
-    Finds the global minimum and maximum values in a nested list structure.
-
-    This function flattens the input data into a single list and then
-    determines the minimum and maximum values.
-
-    Args:
-        data: A nested list of integers. The structure can be of any depth.
-
-    Returns:
-        A tuple (min_value, max_value) where min_value is the minimum value
-        in the data, and max_value is the maximum value.
-    """
-    flat_list = flatten(data)
-    return min(flat_list), max(flat_list)
-
-
-def get_edge_widths(indices, clust):
-    """ Calculate edge width for each cluster based on the number of indices in the cluster.
-
-    Args:
-        indices: 1-d array
-            Array of indices for the specific class.
-        clust: sequence of vectors
-            A sequence of vectors, each containing the indices of elements in a cluster.
-
-    Returns:
-        lwidth: 1-d array
-            Array of edge widths for each cluster.
-    """
-    lwidth = np.zeros(len(clust))
-
-    for i in range(len(clust)):
-        if len(clust[i]) != 0:
-            if len(np.intersect1d(clust[i], indices)) > 0:
-                lwidth[i] = 20. * len(np.intersect1d(clust[i], indices)) / len(clust[i])
-            else:
-                lwidth[i] = None
-        else:
-            lwidth[i] = None
-
-    return lwidth
-
-
-def get_color_labels(clust, *listOfIndices):
-    """ Generates color label for each cluster based on indices of classes.
-
-    Args:
-        clust: sequence of vectors
-            A sequence of vectors, each containing the indices of elements in a cluster.
-
-        *args: 1-d array
-            A list of indices where the specific class is present.
-    """
-    # Validate if the user have provided at least one class indices
-    if len(listOfIndices) == 0:
-        raise ValueError('At least one class indices must be provided.')
-
-    # Validate if the arg is a list or numpy array and unpack them
-    numst = []
-    for arg in listOfIndices:
-        if not isinstance(arg, (list, np.ndarray)):
-            raise ValueError('The arguments must be a list or numpy array.')
-        else:
-            numst.append(arg)
-
-            # Initialize the color label array
-    color_labels = np.zeros(len(clust))
-
-    # When there is only one list provides,
-    # check if the cluster contains the indices of the class.
-    # If that class is majority in the cluster, assign 1, otherwise 0.
-    if len(numst) == 1:
-        indices = numst[0]
-        for i in range(len(clust)):
-            if len(clust[i]) != 0:
-                num_class = len(np.intersect1d(clust[i], indices))
-                if num_class > len(clust[i]) / 2:
-                    color_labels[i] = 1
-                else:
-                    color_labels[i] = 0
-            else:
-                color_labels[i] = None
-
-    else:
-        # Detect the intersection of the cluster and each list of indices (class),
-        # and get the majority class in the cluster.
-        # Append the majority class to the edge color array.
-        for i in range(len(clust)):
-            if len(clust[i]) != 0:
-                intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
-                color_labels[i] = np.argmax(intersection)
-            else:
-                color_labels[i] = None
-
-    return color_labels
-
-
-# Helper functions to create button objects in the interactive plot
-def create_buttons(fig, button_types):
-    sidebar_width = 0.2
-    button_config = calculate_button_positions(len(button_types), sidebar_width)
-
-    buttons = {}
-    for i, button_type in enumerate(button_types):
-        button_ax = fig.add_axes(button_config[i])
-        buttons[button_type] = Button(button_ax, button_type.capitalize(), hovercolor='0.975')
-
-    return buttons
-
-
-def calculate_button_positions(num_buttons, sidebar_width):
-    # Calculate button positions and sizes
-    button_ratio = 16 / 9
-    single_button_width = sidebar_width * 0.8
-    single_button_height = single_button_width / button_ratio
-    margin = 0.05
-    total_buttons_height = num_buttons * single_button_height + (num_buttons - 1) * margin
-
-    button_config = []
-    for i in range(num_buttons):
-        y_pos = (1 - total_buttons_height) / 2 + (num_buttons - 1 - i) * (single_button_height + margin)
-        x_centered = 0.8 + (0.2 - single_button_width) / 2
-        button_config.append([x_centered, y_pos, single_button_width, single_button_height])
-
-    return button_config
-
-
+from scipy.spatial.distance import cdist
+from scipy import sparse
+import numpy as np
+import networkx as nx
+from matplotlib.widgets import Button
+
+
+def preminmax(p):
+    # Normalize the inputs to be in the range [-1, 1]
+    minp = np.amin(p, 1)
+    maxp = np.amax(p, 1)
+
+    equal = np.equal(minp, maxp)
+    nequal = np.logical_not(equal)
+
+    if sum(equal) != 0:
+        print('Some maximums and minimums are equal. Those inputs won''t be transformed.')
+        minp0 = minp*nequal - 1*equal
+        maxp0 = maxp*nequal + 1*equal
+    else:
+        minp0 = minp
+        maxp0 = maxp
+
+    minp0 = np.expand_dims(minp0, axis=1)
+    maxp0 = np.expand_dims(maxp0, axis=1)
+    pn = 2*(p-minp0)/(maxp0-minp0) - 1
+    return pn, minp, maxp
+
+
+def calculate_positions(dim):
+    # Calculate the positions of the neurons in the SOM
+    dims = len(dim)
+    position = np.zeros((dims, np.prod(dim)))
+    len1 = 1
+
+    center = 0
+
+    for i in range(2):
+        dimi = dim[i]
+        newlen = len1 * dimi
+        offset = np.sqrt(1 - center*center)
+
+        if i == 1:
+            for j in range(1, dimi):
+                ishift = [center * (j % 2)]
+                doshift = np.array(ishift*len1)
+                position[0, np.arange(len1)+len1*j] = position[0, np.arange(len1)] + doshift
+
+        posi = np.array(range(dimi)) * offset
+        ind2 = np.floor(np.arange(newlen) / len1)
+        ind2 = ind2.astype(int)
+        position[i, np.arange(newlen)] = posi[ind2]
+
+        len1 = newlen
+        center = 0.5
+
+    return position
+
+
+def cart2pol(x, y):
+    # Convert cartesian coordinates to polar coordinates
+    theta = np.arctan2(y, x)
+    rho = np.hypot(x, y)
+    return theta, rho
+
+
+def pol2cart(theta, rho):
+    # Convert polar coordinates to cartesian coordinates
+    x = rho * np.cos(theta)
+    y = rho * np.sin(theta)
+    return x, y
+
+
+def rotate_xy(x1, y1, angle):
+    # Rotate the coordinates x1, y1 by angle
+    [a, r] = cart2pol(x1, y1)
+    a = a + angle
+    x2, y2 = pol2cart(a, r)
+    return x2, y2
+
+
+def normalize_position(position):
+    # Normalize the positions of the neurons to be in the range [-1, 1]
+    shap = position.shape
+    numPos = shap[1]
+    minPos = np.ndarray.min(position,axis=1)
+    maxPos = np.ndarray.max(position,axis=1)
+    difPos = maxPos - minPos
+    equal = np.equal(minPos, maxPos)
+    difPos[equal] = 1
+    minPos = np.expand_dims(minPos, axis=1)
+    minPos = np.repeat(minPos, numPos, axis=1)
+    difPos = np.expand_dims(difPos, axis=1)
+    difPos = np.repeat(difPos, numPos, axis=1)
+    posit = 2 * ((position - minPos)/difPos) - 1
+    return posit
+
+
+def spread_positions(position, positionMean, positionBasis):
+    # Spread the positions of the neurons
+    shappos = position.shape
+    numPos = shappos[1]
+    position1 = np.repeat(positionMean, numPos, axis=1) + np.matmul(positionBasis, position)
+    return position1
+
+
+def distances(pos):
+    # Compute the distances between the neurons in the SOM topology
+    posT = np.transpose(pos)
+    dist = cdist(posT, posT, 'euclidean')
+
+    link = dist <= 1.00001
+    link = sparse.csr_matrix(1.0*link)
+
+    g = nx.DiGraph(link)
+    dist = nx.floyd_warshall_numpy(g)
+
+    return dist
+
+
+def get_hexagon_shape():
+    # Determine the shape of the hexagon to represent each cluster
+    shapex = np.array([-1, 0, 1, 1, 0, -1]) * 0.5
+    shapey = np.array([1, 2, 1, -1, -2, -1]) * np.sqrt(0.75) / 3
+    return shapex, shapey
+
+
+def get_edge_shape():
+    # Determine the shape of the elongated hexagon to represent edge between each cluster
+    edgex = np.array([-1, 0, 1, 0]) * 0.5
+    edgey = np.array([0, 1, 0, - 1]) * np.sqrt(0.75) / 3
+
+    return edgex, edgey
+
+
+# Helper Functions to extract information from the input data for passing to the plot
+def get_cluster_data(data, clust):
+    """
+    For each cluster, extract the corresponding data points and return them in a list.
+
+    Parameters
+    ----------
+    data : numpy array
+        The dataset from which to extract the clusters' data.
+    clust : list of arrays
+        A list where each element is an array of indices for data points in the corresponding cluster.
+
+    Returns
+    -------
+    cluster_data_list : list of numpy arrays
+        A list where each element is a numpy array containing the data points of a cluster.
+    """
+    cluster_data_list = []
+    for cluster_indices in clust:
+        if len(cluster_indices) > 0:
+            # Ensure cluster_indices are integers and within the range of data
+            cluster_indices = np.array(cluster_indices, dtype=int)
+            cluster_data = data[cluster_indices]
+            cluster_data_list.append(cluster_data)
+        else:
+            cluster_data_list.append(np.array([]))  # Use an empty array for empty clusters
+
+    return cluster_data_list
+
+
+def get_cluster_array(feature, clust):
+    """
+    Returns a NumPy array of objects, each containing the feature values for each cluster.
+
+    Parameters
+    ----------
+    feature : array-like
+        Feature array.
+    clust : list
+        A list of cluster arrays, each containing indices sorted by distances.
+
+    Returns
+    -------
+    cluster_array : numpy.ndarray
+        A NumPy array where each element is an array of feature values for that cluster.
+    """
+    cluster_array = np.empty(len(clust), dtype=object)
+
+    for i, cluster_indices in enumerate(clust):
+        if len(cluster_indices) > 0:
+            cluster_array[i] = feature[cluster_indices]
+        else:
+            cluster_array[i] = np.array([])  # Store an empty array if the cluster is empty
+
+    return cluster_array
+
+
+def get_cluster_avg(feature, clust):
+    """
+    Returns the average value of a feature for each cluster.
+
+    Parameters
+    ----------
+    feature : array-like
+        Feature array.
+    clust : list
+        A list of cluster arrays, each containing indices sorted by distances.
+
+    Returns
+    -------
+    cluster_avg : numpy array
+        A cluster array with the average value of the feature for each cluster.
+    """
+    cluster_array = get_cluster_array(feature, clust)
+    cluster_avg = np.zeros(len(cluster_array))
+    for i in range(len(cluster_array)):
+        if len(cluster_array[i]) > 0:
+            cluster_avg[i] = np.mean(cluster_array[i])
+
+    return cluster_avg
+
+
+def closest_class_cluster(cat_feature, clust):
+    """
+    Returns the cluster array with the closest class for each cluster.
+
+    Paramters
+    ----------
+    cat_feature : array-like
+        Categorical feature array.
+    clust : list
+        A cluster array of indices sorted by distances.
+
+    Returns
+    -------
+    closest_class : numpy array
+        A cluster array with the closest class for each cluster.
+    """
+    closest_class = np.zeros(len(clust))
+    for i in range(len(clust)):
+        cluster_indices = clust[i]
+        if len(cluster_indices) > 0:
+            closest_class[i] = cat_feature[cluster_indices[0]]
+        else:
+            closest_class[i] = None  # Avoid division by zero if the cluster is empty
+
+    return closest_class
+
+
+def majority_class_cluster(cat_feature, clust):
+    """
+    Returns the cluster array with the majority class for each cluster.
+
+    Paramters
+    ----------
+    cat_feature : array-like
+        Categorical feature array.
+    clust : list
+        A cluster array of indices sorted by distances.
+
+    Returns
+    -------
+    majority_class : numpy array
+        A cluster array with the majority class
+    """
+    majority_class = np.zeros(len(clust))
+    for i in range(len(clust)):
+        cluster_indices = clust[i]
+        if len(cluster_indices) > 0:
+            majority_class[i] = np.argmax(np.bincount(cat_feature[cluster_indices]))
+        else:
+            majority_class[i] = None  # Avoid division by zero if the cluster is empty
+
+    return majority_class
+
+
+def get_perc_cluster(cat_feature, target, clust):
+    """
+    Return cluster array with the percentage of a specific target class in each cluster.
+
+    Parameters
+    ----------
+    cat_feature : array-like
+        Categorical feature array.
+    target : int or str
+        Target class to calculate the percentage.
+    clust : list
+        A cluster array of indices sorted by distances.
+
+    Returns
+    -------
+    cluster_array : numpy array
+        A cluster array with the percentage of target class.
+    """
+    # Create Cluster Array with the percentage of target class
+    cluster_array = np.zeros(len(clust))
+    for i in range(len(clust)):
+        cluster_indices = clust[i]
+        if len(cluster_indices) > 0:
+            cluster_array[i] = np.sum(cat_feature[cluster_indices] == target) / len(cluster_indices)
+        else:
+            cluster_array[i] = 0  # Avoid division by zero if the cluster is empty
+
+    return cluster_array * 100
+
+
+def count_classes_in_cluster(cat_feature, clust):
+    """
+    Count the occurrences of each class in each cluster using vectorized operations
+    for efficiency.
+
+    Parameters
+    ----------
+    cat_feature : array-like
+        Categorical feature array.
+    clust : list
+        A list of arrays, each containing the indices of elements in a cluster.
+
+    Returns
+    -------
+    cluster_counts : numpy array
+        A 2D array with counts of each class in each cluster.
+    """
+    unique_classes, _ = np.unique(cat_feature, return_counts=True)
+    num_classes = len(unique_classes)
+
+    # Initialize the array to hold class counts for each cluster
+    cluster_counts = np.zeros((len(clust), num_classes), dtype=int)
+
+    # Loop over clusters to count class occurrences
+    for i, indices in enumerate(clust):
+        if len(indices) > 0:
+            # Count occurrences of each class in the cluster
+            cluster_counts[i] = [np.sum(cat_feature[indices] == cls) for cls in unique_classes]
+        else:
+            cluster_counts[i] = np.zeros(num_classes, dtype=int)
+
+    return cluster_counts
+
+
+def cal_class_cluster_intersect(clust, *args):
+    """
+    Calculate the intersection sizes of each class with each neuron cluster.
+
+    This function computes the size of the intersection between each given class
+    (represented by arrays of indices) and each neuron cluster (represented by
+    a list of lists of indices). The result is a 2D array where each row corresponds
+    to a neuron cluster, and each column corresponds to one of the classes.
+
+    Parameters
+    ----------
+    clust : list of lists
+        A collection of neuron clusters, where each neuron cluster is a list of indices.
+    *args : sequence of array-like
+        A variable number of arrays, each representing a class with indices.
+
+    Returns
+    -------
+    numpy.ndarray
+        A 2D array where the entry at position (i, j) represents the number of indices
+        in the j-th class that are also in the i-th neuron cluster.
+
+    Examples
+    --------
+    >>> clust = [[4, 5, 9], [1, 7], [2, 10, 11], [3, 6, 8]]
+    >>> ind1 = np.array([1, 2, 3])
+    >>> ind2 = np.array([4, 5, 6])
+    >>> ind3 = np.array([7, 8, 9])
+    >>> ind4 = np.array([10, 11, 12])
+    >>> get_sizes_clust(clust, ind1, ind2, ind3, ind4)
+    array([[0, 2, 1, 0],
+           [1, 0, 1, 0],
+           [1, 0, 0, 2],
+           [1, 1, 1, 0]])
+    """
+    numst = list(args)
+
+    cluster_sizes_matrix = np.zeros((len(numst), len(clust)))
+
+    for i, ind in enumerate(numst):
+        for j, cluster in enumerate(clust):
+            cluster_sizes_matrix[i][j] = np.sum(np.isin(cluster, ind))
+
+    return cluster_sizes_matrix.T
+
+
+# Helper function  to extract information from the post-training model for passing to the plot
+def get_ind_misclassified(target, prediction):
+    """
+    Get the indices of misclassified items.
+
+    Parameters
+    ----------
+    target : array-like
+        The true target values.
+    prediction : array-like
+        The predicted values.
+
+    Returns
+    -------
+    misclassified_indices : list
+        List of indices of misclassified items.
+    """
+    misclassified_indices = np.where(target != prediction)[0]
+
+    return misclassified_indices
+
+
+def get_perc_misclassified(target, prediction, clust):
+    """
+    Calculate the percentage of misclassified items in each cluster and return as a numpy array.
+
+    Parameters
+    ----------
+    target : array-like
+        The true target values.
+    prediction : array-like
+        The predicted values.
+    clust : array-like
+        List of arrays, each containing the indices of elements in a cluster.
+
+    Returns
+    -------
+    proportion_misclassified : numpy array
+        Percentage of misclassified items in each cluster.
+    """
+    # Get the indices of misclassified items.
+    misclassified_indices = get_ind_misclassified(target, prediction)
+
+    # Initialize array to store proportion of misclassified items
+    proportion_misclassified = np.zeros(len(clust))
+
+    for i, cluster_indices in enumerate(clust):
+        if len(cluster_indices) > 0:
+            # Compute intersection of cluster indices and misclassified indices
+            misclassified_count = np.intersect1d(cluster_indices, misclassified_indices).size
+            proportion_misclassified[i] = (misclassified_count / len(cluster_indices)) * 100
+
+    return proportion_misclassified
+
+
+def get_conf_indices(target, results, target_class):
+    """
+    Get the indices of True Positive, True Negative, False Positive, and False Negative for a specific target class.
+
+    Parameters
+    ----------
+    target : array-like
+        The true target values.
+    results : array-like
+        The predicted values.
+    target_class : int
+        The target class for which to get the confusion indices.
+
+    Returns
+    -------
+    tp_index : numpy array
+        Indices of True Positives.
+    tn_index : numpy array
+        Indices of True Negatives.
+    fp_index : numpy array
+        Indices of False Positives.
+    fn_index : numpy array
+        Indices of False Negatives.
+    """
+    tp_index = np.where((target == target_class) & (results == target_class))[0]
+    tn_index = np.where((target != target_class) & (results != target_class))[0]
+    fp_index = np.where((target != target_class) & (results == target_class))[0]
+    fn_index = np.where((target == target_class) & (results != target_class))[0]
+
+    return tp_index, tn_index, fp_index, fn_index
+
+
+def get_dominant_class_error_types(dominant_classes, error_types):
+    """
+    Map dominant class to the corresponding majority error type for each cluster,
+    dynamically applying the correct error type based on the dominant class.
+
+    Parameters:
+    ---------------
+    dominant_classes: array-like (som.numNeurons, )
+        List of dominant class labels for each cluster. May contain NaN values.
+    error_types: list of array-like (numClasses, som.numNeurons)
+        Variable number of arrays, each representing majority error types for each class.
+
+    Returns:
+    ---------------
+    array-like (som.numNeurons, )
+        List of majority error type for each cluster corresponding to the dominant class.
+    """
+    if len(error_types) < np.max([dc for dc in dominant_classes if not np.isnan(dc)]) + 1:
+        raise ValueError("Not enough error type arrays provided for all classes.")
+
+    # Initialize the output array with NaNs to handle possible missing classes
+    output_error_types = np.full(len(dominant_classes), np.nan)
+
+    # Map the correct error type based on the dominant class
+    for idx, dominant_class in enumerate(dominant_classes):
+        if not np.isnan(dominant_class):  # Check if the dominant class is not NaN
+            if dominant_class < len(error_types):
+                output_error_types[idx] = error_types[int(dominant_class)][idx]
+            else:
+                raise ValueError(f"Class {dominant_class} is out of the provided error type array bounds.")
+        else:
+            output_error_types[idx] = np.nan  # Explicitly setting NaN if no dominant class
+
+    return output_error_types
+
+
+def flatten(data):
+    """
+    Recursively flattens a nested list structure of numbers into a single list.
+
+    Args:
+        data: A number (int or float) or a nested list of numbers. The data to be flattened.
+
+    Returns:
+        A list of numbers, where all nested structures in the input have been
+        flattened into a single list.
+    """
+    if isinstance(data, (int, float, np.float64)):  # base case for numbers
+        return [data]
+    else:
+        flat_list = []
+        for item in data:
+            flat_list.extend(flatten(item))  # recursive call to flatten
+        return flat_list
+
+
+def get_global_min_max(data):
+    """
+    Finds the global minimum and maximum values in a nested list structure.
+
+    This function flattens the input data into a single list and then
+    determines the minimum and maximum values.
+
+    Args:
+        data: A nested list of integers. The structure can be of any depth.
+
+    Returns:
+        A tuple (min_value, max_value) where min_value is the minimum value
+        in the data, and max_value is the maximum value.
+    """
+    flat_list = flatten(data)
+    return min(flat_list), max(flat_list)
+
+
+def get_edge_widths(indices, clust):
+    """ Calculate edge width for each cluster based on the number of indices in the cluster.
+
+    Args:
+        indices: 1-d array
+            Array of indices for the specific class.
+        clust: sequence of vectors
+            A sequence of vectors, each containing the indices of elements in a cluster.
+
+    Returns:
+        lwidth: 1-d array
+            Array of edge widths for each cluster.
+    """
+    lwidth = np.zeros(len(clust))
+
+    for i in range(len(clust)):
+        if len(clust[i]) != 0:
+            if len(np.intersect1d(clust[i], indices)) > 0:
+                lwidth[i] = 20. * len(np.intersect1d(clust[i], indices)) / len(clust[i])
+            else:
+                lwidth[i] = None
+        else:
+            lwidth[i] = None
+
+    return lwidth
+
+
+def get_color_labels(clust, *listOfIndices):
+    """ Generates color label for each cluster based on indices of classes.
+
+    Args:
+        clust: sequence of vectors
+            A sequence of vectors, each containing the indices of elements in a cluster.
+
+        *args: 1-d array
+            A list of indices where the specific class is present.
+    """
+    # Validate if the user have provided at least one class indices
+    if len(listOfIndices) == 0:
+        raise ValueError('At least one class indices must be provided.')
+
+    # Validate if the arg is a list or numpy array and unpack them
+    numst = []
+    for arg in listOfIndices:
+        if not isinstance(arg, (list, np.ndarray)):
+            raise ValueError('The arguments must be a list or numpy array.')
+        else:
+            numst.append(arg)
+
+            # Initialize the color label array
+    color_labels = np.zeros(len(clust))
+
+    # When there is only one list provides,
+    # check if the cluster contains the indices of the class.
+    # If that class is majority in the cluster, assign 1, otherwise 0.
+    if len(numst) == 1:
+        indices = numst[0]
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                num_class = len(np.intersect1d(clust[i], indices))
+                if num_class > len(clust[i]) / 2:
+                    color_labels[i] = 1
+                else:
+                    color_labels[i] = 0
+            else:
+                color_labels[i] = None
+
+    else:
+        # Detect the intersection of the cluster and each list of indices (class),
+        # and get the majority class in the cluster.
+        # Append the majority class to the edge color array.
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
+                color_labels[i] = np.argmax(intersection)
+            else:
+                color_labels[i] = None
+
+    return color_labels
+
+
+# Helper functions to create button objects in the interactive plot
+def create_buttons(fig, button_types):
+    sidebar_width = 0.2
+    button_config = calculate_button_positions(len(button_types), sidebar_width)
+
+    buttons = {}
+    for i, button_type in enumerate(button_types):
+        button_ax = fig.add_axes(button_config[i])
+        buttons[button_type] = Button(button_ax, button_type.capitalize(), hovercolor='0.975')
+
+    return buttons
+
+
+def calculate_button_positions(num_buttons, sidebar_width):
+    # Calculate button positions and sizes
+    button_ratio = 16 / 9
+    single_button_width = sidebar_width * 0.8
+    single_button_height = single_button_width / button_ratio
+    margin = 0.05
+    total_buttons_height = num_buttons * single_button_height + (num_buttons - 1) * margin
+
+    button_config = []
+    for i in range(num_buttons):
+        y_pos = (1 - total_buttons_height) / 2 + (num_buttons - 1 - i) * (single_button_height + margin)
+        x_centered = 0.8 + (0.2 - single_button_width) / 2
+        button_config.append([x_centered, y_pos, single_button_width, single_button_height])
+
+    return button_config
+
+
```

### Comparing `nnsom-1.7.7/.gitignore` & `nnsom-1.7.8/.gitignore`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1080 +1,1080 @@
-### Diff template
-*.patch
-*.diff
-
-### Tags template
-# Ignore tags created by etags, ctags, gtags (GNU global) and cscope
-TAGS
-.TAGS
-!TAGS/
-tags
-.tags
-!tags/
-gtags.files
-GTAGS
-GRTAGS
-GPATH
-GSYMS
-cscope.files
-cscope.out
-cscope.in.out
-cscope.po.out
-
-
-### Images template
-# JPEG
-*.jpg
-*.jpeg
-*.jpe
-*.jif
-*.jfif
-*.jfi
-
-# JPEG 2000
-*.jp2
-*.j2k
-*.jpf
-*.jpx
-*.jpm
-*.mj2
-
-# JPEG XR
-*.jxr
-*.hdp
-*.wdp
-
-# Graphics Interchange Format
-*.gif
-
-# RAW
-*.raw
-
-# Web P
-*.webp
-
-# Portable Network Graphics
-#*.png
-
-# Animated Portable Network Graphics
-*.apng
-
-# Multiple-image Network Graphics
-*.mng
-
-# Tagged Image File Format
-*.tiff
-*.tif
-
-# Scalable Vector Graphics
-*.svg
-*.svgz
-
-# Portable Document Format
-*.pdf
-
-# X BitMap
-*.xbm
-
-# BMP
-*.bmp
-*.dib
-
-# ICO
-*.ico
-
-# 3D Images
-*.3dm
-*.max
-
-### AL template
-.vscode/*
-!.vscode/settings.json
-!.vscode/tasks.json
-!.vscode/launch.json
-!.vscode/extensions.json
-*.code-workspace
-
-# Local History for Visual Studio Code
-.history/
-*.app
-.snapshots/*
-
-### LyX template
-# Ignore LyX backup and autosave files
-# http://www.lyx.org/
-*.lyx~
-*.lyx#
-
-### Bazaar template
-.bzr/
-.bzrignore
-
-### PSoCCreator template
-# Project Settings
-*.cywrk.*
-*.cyprj.*
-
-# Generated Assets and Resources
-Debug/
-Release/
-Export/
-*/codegentemp
-*/Generated_Source
-*_datasheet.pdf
-*_timing.html
-*.cycdx
-*.cyfit
-*.rpt
-*.svd
-*.log
-*.zip
-
-### JEnv template
-# JEnv local Java version configuration file
-.java-version
-
-# Used by previous versions of JEnv
-.jenv-version
-
-### Redcar template
-.redcar
-
-### NetBeans template
-**/nbproject/private/
-**/nbproject/Makefile-*.mk
-**/nbproject/Package-*.bash
-nbbuild/
-nbdist/
-.nb-gradle/
-
-### GPG template
-secring.*
-
-
-### Stata template
-# .gitignore file for git projects containing Stata files
-# Commercial statistical software: http://www.stata.com
-
-# Stata dataset and output files
-*.dta
-*.gph
-*.log
-*.smcl
-*.stpr
-*.stsem
-
-# Graphic export files from Stata
-# Stata command graph export: http://www.stata.com/manuals14/g-2graphexport.pdf
-#
-# You may add graphic export files to your .gitignore. However you should be
-# aware that this will exclude all image files from this main directory
-# and subdirectories.
-# *.ps
-# *.eps
-# *.wmf
-# *.emf
-# *.pdf
-# *.png
-# *.tif
-
-### Linux template
-*~
-
-# temporary files which can be created if a process still has a handle open of a deleted file
-.fuse_hidden*
-
-# KDE directory preferences
-.directory
-
-# Linux trash folder which might appear on any partition or disk
-.Trash-*
-
-# .nfs files are created when an open file is removed but is still being accessed
-.nfs*
-
-### Patch template
-*.orig
-*.rej
-
-### Cloud9 template
-# Cloud9 IDE - http://c9.io
-.c9revisions
-.c9
-
-### Mercurial template
-.hg/
-.hgignore
-.hgsigs
-.hgsub
-.hgsubstate
-.hgtags
-
-### MonoDevelop template
-#User Specific
-*.userprefs
-*.usertasks
-
-#Mono Project Files
-*.pidb
-*.resources
-test-results/
-
-### VisualStudioCode template
-.vscode/*
-!.vscode/settings.json
-!.vscode/tasks.json
-!.vscode/launch.json
-!.vscode/extensions.json
-!.vscode/*.code-snippets
-
-# Local History for Visual Studio Code
-.history/
-
-# Built Visual Studio Code Extensions
-*.vsix
-
-### PuTTY template
-# Private key
-*.ppk
-
-### Syncthing template
-# Syncthing caches
-.stversions
-
-### TortoiseGit template
-# Project-level settings
-/.tgitconfig
-
-### SlickEdit template
-# SlickEdit workspace and project files are ignored by default because
-# typically they are considered to be developer-specific and not part of a
-# project.
-*.vpw
-*.vpj
-
-# SlickEdit workspace history and tag files always contain user-specific
-# data so they should not be stored in a repository.
-*.vpwhistu
-*.vpwhist
-*.vtg
-
-### Emacs template
-# -*- mode: gitignore; -*-
-*~
-\#*\#
-/.emacs.desktop
-/.emacs.desktop.lock
-*.elc
-auto-save-list
-tramp
-.\#*
-
-# Org-mode
-.org-id-locations
-*_archive
-
-# flymake-mode
-*_flymake.*
-
-# eshell files
-/eshell/history
-/eshell/lastdir
-
-# elpa packages
-/elpa/
-
-# reftex files
-*.rel
-
-# AUCTeX auto folder
-/auto/
-
-# cask packages
-.cask/
-
-# Flycheck
-flycheck_*.el
-
-# server auth directory
-/server/
-
-# projectiles files
-.projectile
-
-# directory configuration
-.dir-locals.el
-
-# network security
-/network-security.data
-
-
-### Lazarus template
-# Lazarus compiler-generated binaries (safe to delete)
-*.exe
-*.dll
-*.so
-*.dylib
-*.lrs
-*.res
-*.compiled
-*.dbg
-*.ppu
-*.o
-*.or
-*.a
-
-# Lazarus autogenerated files (duplicated info)
-#*.rst
-*.rsj
-*.lrt
-
-# Lazarus local files (user-specific info)
-*.lps
-
-# Lazarus backups and unit output folders.
-# These can be changed by user in Lazarus/project options.
-backup/
-*.bak
-lib/
-
-# Application bundle for Mac OS
-*.app/
-
-### macOS template
-# General
-.DS_Store
-.AppleDouble
-.LSOverride
-
-# Icon must end with two \r
-Icon
-
-# Thumbnails
-._*
-
-# Files that might appear in the root of a volume
-.DocumentRevisions-V100
-.fseventsd
-.Spotlight-V100
-.TemporaryItems
-.Trashes
-.VolumeIcon.icns
-.com.apple.timemachine.donotpresent
-
-# Directories potentially created on remote AFP share
-.AppleDB
-.AppleDesktop
-Network Trash Folder
-Temporary Items
-.apdisk
-
-### JDeveloper template
-# default application storage directory used by the IDE Performance Cache feature
-.data/
-
-# used for ADF styles caching
-temp/
-
-# default output directories
-classes/
-deploy/
-javadoc/
-
-# lock file, a part of Oracle Credential Store Framework
-cwallet.sso.lck
-### Virtuoso template
-# Gitignore for Cadence Virtuoso
-################################################################
-
-# Log files
-*.log
-panic*.log.*
-
-# OpenAccess database lock files
-*.cdslck*
-
-# Run directories for layout vs. schematic and design rule check
-lvsRunDir/*
-drcRunDir/*
-
-# Abstract generation tool
-abstract.log*
-abstract.record*
-
-
-### WebMethods template
-**/IntegrationServer/datastore/
-**/IntegrationServer/db/
-**/IntegrationServer/DocumentStore/
-**/IntegrationServer/lib/
-**/IntegrationServer/logs/
-**/IntegrationServer/replicate/
-**/IntegrationServer/sdk/
-**/IntegrationServer/support/
-**/IntegrationServer/update/
-**/IntegrationServer/userFtpRoot/
-**/IntegrationServer/web/
-**/IntegrationServer/WmRepository4/
-**/IntegrationServer/XAStore/
-**/IntegrationServer/packages/Wm*/
-
-### Vagrant template
-# General
-.vagrant/
-
-# Log files (if you are creating logs in debug mode, uncomment this)
-# *.log
-
-### Archives template
-# It's better to unpack these files and commit the raw source because
-# git has its own built in compression methods.
-*.7z
-*.jar
-*.rar
-*.zip
-*.gzip
-*.tgz
-*.bzip
-*.bzip2
-*.bz2
-*.xz
-*.lzma
-*.cab
-*.xar
-
-# Packing-only formats
-*.iso
-
-# Package management formats
-*.dmg
-*.xpi
-*.gem
-*.egg
-*.deb
-*.rpm
-*.msi
-*.msm
-*.msp
-*.txz
-
-### SynopsysVCS template
-# Waveform formats
-*.vcd
-*.vpd
-*.evcd
-*.fsdb
-
-# Default name of the simulation executable.  A different name can be
-# specified with this switch (the associated daidir database name is
-# also taken from here):  -o <path>/<filename>
-simv
-
-# Generated for Verilog and VHDL top configs
-simv.daidir/
-simv.db.dir/
-
-# Infrastructure necessary to co-simulate SystemC models with
-# Verilog/VHDL models.  An alternate directory may be specified with this
-# switch:  -Mdir=<directory_path>
-csrc/
-
-# Log file - the following switch allows to specify the file that will be
-# used to write all messages from simulation:  -l <filename>
-*.log
-
-# Coverage results (generated with urg) and database location.  The
-# following switch can also be used:  urg -dir <coverage_directory>.vdb
-simv.vdb/
-urgReport/
-
-# DVE and UCLI related files.
-DVEfiles/
-ucli.key
-
-# When the design is elaborated for DirectC, the following file is created
-# with declarations for C/C++ functions.
-vc_hdrs.h
-
-### Octave template
-# Windows default autosave extension
-*.asv
-
-# OSX / *nix default autosave extension
-*.m~
-
-# Compiled MEX binaries (all platforms)
-*.mex*
-
-# Packaged app and toolbox files
-*.mlappinstall
-*.mltbx
-
-# Generated helpsearch folders
-helpsearch*/
-
-# Simulink code generation folders
-slprj/
-sccprj/
-
-# Matlab code generation folders
-codegen/
-
-# Simulink autosave extension
-*.autosave
-
-# Simulink cache files
-*.slxc
-
-# Octave session info
-octave-workspace
-
-### Windows template
-# Windows thumbnail cache files
-Thumbs.db
-Thumbs.db:encryptable
-ehthumbs.db
-ehthumbs_vista.db
-
-# Dump file
-*.stackdump
-
-# Folder config file
-[Dd]esktop.ini
-
-# Recycle Bin used on file shares
-$RECYCLE.BIN/
-
-# Windows Installer files
-*.cab
-*.msi
-*.msix
-*.msm
-*.msp
-
-# Windows shortcuts
-*.lnk
-
-### LibreOffice template
-# LibreOffice locks
-.~lock.*#
-
-### Redis template
-# Ignore redis binary dump (dump.rdb) files
-
-*.rdb
-
-### TextMate template
-*.tmproj
-*.tmproject
-tmtags
-
-### MicrosoftOffice template
-*.tmp
-
-# Word temporary
-~$*.doc*
-
-# Word Auto Backup File
-Backup of *.doc*
-
-# Excel temporary
-~$*.xls*
-
-# Excel Backup File
-*.xlk
-
-# PowerPoint temporary
-~$*.ppt*
-
-# Visio autosave temporary files
-*.~vsd*
-
-### Ninja template
-.ninja_deps
-.ninja_log
-
-### CVS template
-/CVS/*
-**/CVS/*
-.cvsignore
-*/.cvsignore
-
-### Kate template
-# Swap Files #
-.*.kate-swp
-.swp.*
-
-### SVN template
-.svn/
-
-### FlexBuilder template
-bin/
-bin-debug/
-bin-release/
-
-### Dropbox template
-# Dropbox settings and caches
-.dropbox
-.dropbox.attr
-.dropbox.cache
-
-### Espresso template
-*.esproj
-
-### VirtualEnv template
-# Virtualenv
-# http://iamzed.com/2009/05/07/a-primer-on-virtualenv/
-.Python
-[Bb]in
-[Ii]nclude
-[Ll]ib
-[Ll]ib64
-[Ll]ocal
-[Ss]cripts
-pyvenv.cfg
-.venv
-pip-selfcheck.json
-
-### Dreamweaver template
-# DW Dreamweaver added files
-_notes
-_compareTemp
-configs/
-dwsync.xml
-dw_php_codehinting.config
-*.mno
-
-### DartEditor template
-.project
-.buildlog
-
-### Ensime template
-# Ensime specific
-.ensime
-.ensime_cache/
-.ensime_lucene/
-
-### CodeKit template
-# General CodeKit files to ignore
-config.codekit
-config.codekit3
-/min
-
-### BricxCC template
-# Bricx Command Center IDE
-# http://bricxcc.sourceforge.net
-*.bak
-*.sym
-
-### Eclipse template
-.metadata
-bin/
-tmp/
-*.tmp
-*.bak
-*.swp
-*~.nib
-local.properties
-.settings/
-.loadpath
-.recommenders
-
-# External tool builders
-.externalToolBuilders/
-
-# Locally stored "Eclipse launch configurations"
-*.launch
-
-# PyDev specific (Python IDE for Eclipse)
-*.pydevproject
-
-# CDT-specific (C/C++ Development Tooling)
-.cproject
-
-# CDT- autotools
-.autotools
-
-# Java annotation processor (APT)
-.factorypath
-
-# PDT-specific (PHP Development Tools)
-.buildpath
-
-# sbteclipse plugin
-.target
-
-# Tern plugin
-.tern-project
-
-# TeXlipse plugin
-.texlipse
-
-# STS (Spring Tool Suite)
-.springBeans
-
-# Code Recommenders
-.recommenders/
-
-# Annotation Processing
-.apt_generated/
-.apt_generated_test/
-
-# Scala IDE specific (Scala & Java development for Eclipse)
-.cache-main
-.scala_dependencies
-.worksheet
-
-# Uncomment this line if you wish to ignore the project description file.
-# Typically, this file would be tracked if it contains build/dependency configurations:
-#.project
-
-### MATLAB template
-# Windows default autosave extension
-*.asv
-
-# OSX / *nix default autosave extension
-*.m~
-
-# Compiled MEX binaries (all platforms)
-*.mex*
-
-# Packaged app and toolbox files
-*.mlappinstall
-*.mltbx
-
-# Generated helpsearch folders
-helpsearch*/
-
-# Simulink code generation folders
-slprj/
-sccprj/
-
-# Matlab code generation folders
-codegen/
-
-# Simulink autosave extension
-*.autosave
-
-# Simulink cache files
-*.slxc
-
-# Octave session info
-octave-workspace
-
-### JetBrains template
-# Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
-# Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
-*.ini
-# User-specific stuff
-.idea/**/workspace.xml
-.idea/**/tasks.xml
-.idea/**/usage.statistics.xml
-.idea/**/dictionaries
-.idea/**/shelf
-.DS_Store
-# AWS User-specific
-.idea/**/aws.xml
-
-# Generated files
-.idea/**/contentModel.xml
-
-# Sensitive or high-churn files
-.idea/**/dataSources/
-.idea/**/dataSources.ids
-.idea/**/dataSources.local.xml
-.idea/**/sqlDataSources.xml
-.idea/**/dynamic.xml
-.idea/**/uiDesigner.xml
-.idea/**/dbnavigator.xml
-
-# Gradle
-.idea/**/gradle.xml
-.idea/**/libraries
-
-# Gradle and Maven with auto-import
-# When using Gradle or Maven with auto-import, you should exclude module files,
-# since they will be recreated, and may cause churn.  Uncomment if using
-# auto-import.
-# .idea/artifacts
-# .idea/compiler.xml
-# .idea/jarRepositories.xml
-# .idea/modules.xml
-# .idea/*.iml
-# .idea/modules
-# *.iml
-# *.ipr
-
-# CMake
-cmake-build-*/
-
-# Mongo Explorer plugin
-.idea/**/mongoSettings.xml
-
-# File-based project format
-*.iws
-
-# IntelliJ
-out/
-
-# mpeltonen/sbt-idea plugin
-.idea_modules/
-
-# JIRA plugin
-atlassian-ide-plugin.xml
-
-# Cursive Clojure plugin
-.idea/replstate.xml
-
-# SonarLint plugin
-.idea/sonarlint/
-
-# Crashlytics plugin (for Android Studio and IntelliJ)
-com_crashlytics_export_strings.xml
-crashlytics.properties
-crashlytics-build.properties
-fabric.properties
-
-# Editor-based Rest Client
-.idea/httpRequests
-
-# Android studio 3.1+ serialized cache file
-.idea/caches/build_file_checksums.ser
-
-### KDevelop4 template
-*.kdev4
-.kdev4/
-
-### Calabash template
-# Calabash / Cucumber
-rerun/
-reports/
-screenshots/
-screenshot*.png
-test-servers/
-
-# bundler
-.bundle
-vendor
-
-### Xcode template
-## User settings
-xcuserdata/
-
-## Xcode 8 and earlier
-*.xcscmblueprint
-*.xccheckout
-
-### Metals template
- # Generated Metals (Scala Language Server) files
- # Reference: https://scalameta.org/metals/
-.metals/
-.bloop/
-project/metals.sbt
-
-### Otto template
-.otto/
-
-### NotepadPP template
-# Notepad++ backups #
-*.bak
-
-### EiffelStudio template
-# The compilation directory
-EIFGENs
-
-### Example user template template
-### Example user template
-
-# IntelliJ project files
-.idea
-*.iml
-out
-gen
-### Momentics template
-# Built files
-x86/
-arm/
-arm-p/
-translations/*.qm
-
-# IDE settings
-.settings/
-
-### XilinxISE template
-# intermediate build files
-*.bgn
-*.bit
-*.bld
-*.cmd_log
-*.drc
-*.ll
-*.lso
-*.msd
-*.msk
-*.ncd
-*.ngc
-*.ngd
-*.ngr
-*.pad
-*.par
-*.pcf
-*.prj
-*.ptwx
-*.rbb
-*.rbd
-*.stx
-*.syr
-*.twr
-*.twx
-*.unroutes
-*.ut
-*.xpi
-*.xst
-*_bitgen.xwbt
-*_envsettings.html
-*_map.map
-*_map.mrp
-*_map.ngm
-*_map.xrpt
-*_ngdbuild.xrpt
-*_pad.csv
-*_pad.txt
-*_par.xrpt
-*_summary.html
-*_summary.xml
-*_usage.xml
-*_xst.xrpt
-
-# iMPACT generated files
-_impactbatch.log
-impact.xsl
-impact_impact.xwbt
-ise_impact.cmd
-webtalk_impact.xml
-
-# Core Generator generated files
-xaw2verilog.log
-
-# project-wide generated files
-*.gise
-par_usage_statistics.html
-usage_statistics_webtalk.html
-webtalk.log
-webtalk_pn.xml
-
-# generated folders
-iseconfig/
-xlnx_auto_0_xdb/
-xst/
-_ngo/
-_xmsgs/
-
-### Ansible template
-*.retry
-
-### Backup template
-*.bak
-*.gho
-*.ori
-*.orig
-*.tmp
-
-### SublimeText template
-# Cache files for Sublime Text
-*.tmlanguage.cache
-*.tmPreferences.cache
-*.stTheme.cache
-
-# Workspace files are user-specific
-*.sublime-workspace
-
-# Project files should be checked into the repository, unless a significant
-# proportion of contributors will probably not be using Sublime Text
-# *.sublime-project
-
-# SFTP configuration file
-sftp-config.json
-sftp-config-alt*.json
-
-# Package control specific files
-Package Control.last-run
-Package Control.ca-list
-Package Control.ca-bundle
-Package Control.system-ca-bundle
-Package Control.cache/
-Package Control.ca-certs/
-Package Control.merged-ca-bundle
-Package Control.user-ca-bundle
-oscrypto-ca-bundle.crt
-bh_unicode_properties.cache
-
-# Sublime-github package stores a github token in this file
-# https://packagecontrol.io/packages/sublime-github
-GitHub.sublime-settings
-
-### SBT template
-# Simple Build Tool
-# http://www.scala-sbt.org/release/docs/Getting-Started/Directories.html#configuring-version-control
-
-target/
-lib_managed/
-src_managed/
-project/boot/
-project/plugins/project/
-.history
-.cache
-.lib/
-
-### Anjuta template
-# Local configuration folder and symbol database
-/.anjuta/
-/.anjuta_sym_db.db
-
-### ModelSim template
-# ignore ModelSim generated files and directories (temp files and so on)
-#[_@]*
-
-# ignore compilation output of ModelSim
-*.mti
-*.dat
-*.dbs
-*.psm
-*.bak
-*.cmp
-*.jpg
-#*.html
-*.bsf
-
-# ignore simulation output of ModelSim
-wlf*
-*.wlf
-*.vstf
-*.ucdb
-cov*/
-transcript*
-sc_dpiheader.h
-vsim.dbg
-
-### Vim template
-# Swap
-[._]*.s[a-v][a-z]
-!*.svg  # comment out if you don't need vector files
-[._]*.sw[a-p]
-[._]s[a-rt-v][a-z]
-[._]ss[a-gi-z]
-[._]sw[a-p]
-
-# Session
-Session.vim
-Sessionx.vim
-
-# Temporary
-.netrwhist
-*~
-# Auto-generated tag files
-tags
-# Persistent undo
-[._]*.un~
-
-!/token.ini
-/token.ini
+### Diff template
+*.patch
+*.diff
+
+### Tags template
+# Ignore tags created by etags, ctags, gtags (GNU global) and cscope
+TAGS
+.TAGS
+!TAGS/
+tags
+.tags
+!tags/
+gtags.files
+GTAGS
+GRTAGS
+GPATH
+GSYMS
+cscope.files
+cscope.out
+cscope.in.out
+cscope.po.out
+
+
+### Images template
+# JPEG
+*.jpg
+*.jpeg
+*.jpe
+*.jif
+*.jfif
+*.jfi
+
+# JPEG 2000
+*.jp2
+*.j2k
+*.jpf
+*.jpx
+*.jpm
+*.mj2
+
+# JPEG XR
+*.jxr
+*.hdp
+*.wdp
+
+# Graphics Interchange Format
+*.gif
+
+# RAW
+*.raw
+
+# Web P
+*.webp
+
+# Portable Network Graphics
+#*.png
+
+# Animated Portable Network Graphics
+*.apng
+
+# Multiple-image Network Graphics
+*.mng
+
+# Tagged Image File Format
+*.tiff
+*.tif
+
+# Scalable Vector Graphics
+*.svg
+*.svgz
+
+# Portable Document Format
+*.pdf
+
+# X BitMap
+*.xbm
+
+# BMP
+*.bmp
+*.dib
+
+# ICO
+*.ico
+
+# 3D Images
+*.3dm
+*.max
+
+### AL template
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+*.code-workspace
+
+# Local History for Visual Studio Code
+.history/
+*.app
+.snapshots/*
+
+### LyX template
+# Ignore LyX backup and autosave files
+# http://www.lyx.org/
+*.lyx~
+*.lyx#
+
+### Bazaar template
+.bzr/
+.bzrignore
+
+### PSoCCreator template
+# Project Settings
+*.cywrk.*
+*.cyprj.*
+
+# Generated Assets and Resources
+Debug/
+Release/
+Export/
+*/codegentemp
+*/Generated_Source
+*_datasheet.pdf
+*_timing.html
+*.cycdx
+*.cyfit
+*.rpt
+*.svd
+*.log
+*.zip
+
+### JEnv template
+# JEnv local Java version configuration file
+.java-version
+
+# Used by previous versions of JEnv
+.jenv-version
+
+### Redcar template
+.redcar
+
+### NetBeans template
+**/nbproject/private/
+**/nbproject/Makefile-*.mk
+**/nbproject/Package-*.bash
+nbbuild/
+nbdist/
+.nb-gradle/
+
+### GPG template
+secring.*
+
+
+### Stata template
+# .gitignore file for git projects containing Stata files
+# Commercial statistical software: http://www.stata.com
+
+# Stata dataset and output files
+*.dta
+*.gph
+*.log
+*.smcl
+*.stpr
+*.stsem
+
+# Graphic export files from Stata
+# Stata command graph export: http://www.stata.com/manuals14/g-2graphexport.pdf
+#
+# You may add graphic export files to your .gitignore. However you should be
+# aware that this will exclude all image files from this main directory
+# and subdirectories.
+# *.ps
+# *.eps
+# *.wmf
+# *.emf
+# *.pdf
+# *.png
+# *.tif
+
+### Linux template
+*~
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
+
+### Patch template
+*.orig
+*.rej
+
+### Cloud9 template
+# Cloud9 IDE - http://c9.io
+.c9revisions
+.c9
+
+### Mercurial template
+.hg/
+.hgignore
+.hgsigs
+.hgsub
+.hgsubstate
+.hgtags
+
+### MonoDevelop template
+#User Specific
+*.userprefs
+*.usertasks
+
+#Mono Project Files
+*.pidb
+*.resources
+test-results/
+
+### VisualStudioCode template
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+!.vscode/*.code-snippets
+
+# Local History for Visual Studio Code
+.history/
+
+# Built Visual Studio Code Extensions
+*.vsix
+
+### PuTTY template
+# Private key
+*.ppk
+
+### Syncthing template
+# Syncthing caches
+.stversions
+
+### TortoiseGit template
+# Project-level settings
+/.tgitconfig
+
+### SlickEdit template
+# SlickEdit workspace and project files are ignored by default because
+# typically they are considered to be developer-specific and not part of a
+# project.
+*.vpw
+*.vpj
+
+# SlickEdit workspace history and tag files always contain user-specific
+# data so they should not be stored in a repository.
+*.vpwhistu
+*.vpwhist
+*.vtg
+
+### Emacs template
+# -*- mode: gitignore; -*-
+*~
+\#*\#
+/.emacs.desktop
+/.emacs.desktop.lock
+*.elc
+auto-save-list
+tramp
+.\#*
+
+# Org-mode
+.org-id-locations
+*_archive
+
+# flymake-mode
+*_flymake.*
+
+# eshell files
+/eshell/history
+/eshell/lastdir
+
+# elpa packages
+/elpa/
+
+# reftex files
+*.rel
+
+# AUCTeX auto folder
+/auto/
+
+# cask packages
+.cask/
+
+# Flycheck
+flycheck_*.el
+
+# server auth directory
+/server/
+
+# projectiles files
+.projectile
+
+# directory configuration
+.dir-locals.el
+
+# network security
+/network-security.data
+
+
+### Lazarus template
+# Lazarus compiler-generated binaries (safe to delete)
+*.exe
+*.dll
+*.so
+*.dylib
+*.lrs
+*.res
+*.compiled
+*.dbg
+*.ppu
+*.o
+*.or
+*.a
+
+# Lazarus autogenerated files (duplicated info)
+#*.rst
+*.rsj
+*.lrt
+
+# Lazarus local files (user-specific info)
+*.lps
+
+# Lazarus backups and unit output folders.
+# These can be changed by user in Lazarus/project options.
+backup/
+*.bak
+lib/
+
+# Application bundle for Mac OS
+*.app/
+
+### macOS template
+# General
+.DS_Store
+.AppleDouble
+.LSOverride
+
+# Icon must end with two \r
+Icon
+
+# Thumbnails
+._*
+
+# Files that might appear in the root of a volume
+.DocumentRevisions-V100
+.fseventsd
+.Spotlight-V100
+.TemporaryItems
+.Trashes
+.VolumeIcon.icns
+.com.apple.timemachine.donotpresent
+
+# Directories potentially created on remote AFP share
+.AppleDB
+.AppleDesktop
+Network Trash Folder
+Temporary Items
+.apdisk
+
+### JDeveloper template
+# default application storage directory used by the IDE Performance Cache feature
+.data/
+
+# used for ADF styles caching
+temp/
+
+# default output directories
+classes/
+deploy/
+javadoc/
+
+# lock file, a part of Oracle Credential Store Framework
+cwallet.sso.lck
+### Virtuoso template
+# Gitignore for Cadence Virtuoso
+################################################################
+
+# Log files
+*.log
+panic*.log.*
+
+# OpenAccess database lock files
+*.cdslck*
+
+# Run directories for layout vs. schematic and design rule check
+lvsRunDir/*
+drcRunDir/*
+
+# Abstract generation tool
+abstract.log*
+abstract.record*
+
+
+### WebMethods template
+**/IntegrationServer/datastore/
+**/IntegrationServer/db/
+**/IntegrationServer/DocumentStore/
+**/IntegrationServer/lib/
+**/IntegrationServer/logs/
+**/IntegrationServer/replicate/
+**/IntegrationServer/sdk/
+**/IntegrationServer/support/
+**/IntegrationServer/update/
+**/IntegrationServer/userFtpRoot/
+**/IntegrationServer/web/
+**/IntegrationServer/WmRepository4/
+**/IntegrationServer/XAStore/
+**/IntegrationServer/packages/Wm*/
+
+### Vagrant template
+# General
+.vagrant/
+
+# Log files (if you are creating logs in debug mode, uncomment this)
+# *.log
+
+### Archives template
+# It's better to unpack these files and commit the raw source because
+# git has its own built in compression methods.
+*.7z
+*.jar
+*.rar
+*.zip
+*.gzip
+*.tgz
+*.bzip
+*.bzip2
+*.bz2
+*.xz
+*.lzma
+*.cab
+*.xar
+
+# Packing-only formats
+*.iso
+
+# Package management formats
+*.dmg
+*.xpi
+*.gem
+*.egg
+*.deb
+*.rpm
+*.msi
+*.msm
+*.msp
+*.txz
+
+### SynopsysVCS template
+# Waveform formats
+*.vcd
+*.vpd
+*.evcd
+*.fsdb
+
+# Default name of the simulation executable.  A different name can be
+# specified with this switch (the associated daidir database name is
+# also taken from here):  -o <path>/<filename>
+simv
+
+# Generated for Verilog and VHDL top configs
+simv.daidir/
+simv.db.dir/
+
+# Infrastructure necessary to co-simulate SystemC models with
+# Verilog/VHDL models.  An alternate directory may be specified with this
+# switch:  -Mdir=<directory_path>
+csrc/
+
+# Log file - the following switch allows to specify the file that will be
+# used to write all messages from simulation:  -l <filename>
+*.log
+
+# Coverage results (generated with urg) and database location.  The
+# following switch can also be used:  urg -dir <coverage_directory>.vdb
+simv.vdb/
+urgReport/
+
+# DVE and UCLI related files.
+DVEfiles/
+ucli.key
+
+# When the design is elaborated for DirectC, the following file is created
+# with declarations for C/C++ functions.
+vc_hdrs.h
+
+### Octave template
+# Windows default autosave extension
+*.asv
+
+# OSX / *nix default autosave extension
+*.m~
+
+# Compiled MEX binaries (all platforms)
+*.mex*
+
+# Packaged app and toolbox files
+*.mlappinstall
+*.mltbx
+
+# Generated helpsearch folders
+helpsearch*/
+
+# Simulink code generation folders
+slprj/
+sccprj/
+
+# Matlab code generation folders
+codegen/
+
+# Simulink autosave extension
+*.autosave
+
+# Simulink cache files
+*.slxc
+
+# Octave session info
+octave-workspace
+
+### Windows template
+# Windows thumbnail cache files
+Thumbs.db
+Thumbs.db:encryptable
+ehthumbs.db
+ehthumbs_vista.db
+
+# Dump file
+*.stackdump
+
+# Folder config file
+[Dd]esktop.ini
+
+# Recycle Bin used on file shares
+$RECYCLE.BIN/
+
+# Windows Installer files
+*.cab
+*.msi
+*.msix
+*.msm
+*.msp
+
+# Windows shortcuts
+*.lnk
+
+### LibreOffice template
+# LibreOffice locks
+.~lock.*#
+
+### Redis template
+# Ignore redis binary dump (dump.rdb) files
+
+*.rdb
+
+### TextMate template
+*.tmproj
+*.tmproject
+tmtags
+
+### MicrosoftOffice template
+*.tmp
+
+# Word temporary
+~$*.doc*
+
+# Word Auto Backup File
+Backup of *.doc*
+
+# Excel temporary
+~$*.xls*
+
+# Excel Backup File
+*.xlk
+
+# PowerPoint temporary
+~$*.ppt*
+
+# Visio autosave temporary files
+*.~vsd*
+
+### Ninja template
+.ninja_deps
+.ninja_log
+
+### CVS template
+/CVS/*
+**/CVS/*
+.cvsignore
+*/.cvsignore
+
+### Kate template
+# Swap Files #
+.*.kate-swp
+.swp.*
+
+### SVN template
+.svn/
+
+### FlexBuilder template
+bin/
+bin-debug/
+bin-release/
+
+### Dropbox template
+# Dropbox settings and caches
+.dropbox
+.dropbox.attr
+.dropbox.cache
+
+### Espresso template
+*.esproj
+
+### VirtualEnv template
+# Virtualenv
+# http://iamzed.com/2009/05/07/a-primer-on-virtualenv/
+.Python
+[Bb]in
+[Ii]nclude
+[Ll]ib
+[Ll]ib64
+[Ll]ocal
+[Ss]cripts
+pyvenv.cfg
+.venv
+pip-selfcheck.json
+
+### Dreamweaver template
+# DW Dreamweaver added files
+_notes
+_compareTemp
+configs/
+dwsync.xml
+dw_php_codehinting.config
+*.mno
+
+### DartEditor template
+.project
+.buildlog
+
+### Ensime template
+# Ensime specific
+.ensime
+.ensime_cache/
+.ensime_lucene/
+
+### CodeKit template
+# General CodeKit files to ignore
+config.codekit
+config.codekit3
+/min
+
+### BricxCC template
+# Bricx Command Center IDE
+# http://bricxcc.sourceforge.net
+*.bak
+*.sym
+
+### Eclipse template
+.metadata
+bin/
+tmp/
+*.tmp
+*.bak
+*.swp
+*~.nib
+local.properties
+.settings/
+.loadpath
+.recommenders
+
+# External tool builders
+.externalToolBuilders/
+
+# Locally stored "Eclipse launch configurations"
+*.launch
+
+# PyDev specific (Python IDE for Eclipse)
+*.pydevproject
+
+# CDT-specific (C/C++ Development Tooling)
+.cproject
+
+# CDT- autotools
+.autotools
+
+# Java annotation processor (APT)
+.factorypath
+
+# PDT-specific (PHP Development Tools)
+.buildpath
+
+# sbteclipse plugin
+.target
+
+# Tern plugin
+.tern-project
+
+# TeXlipse plugin
+.texlipse
+
+# STS (Spring Tool Suite)
+.springBeans
+
+# Code Recommenders
+.recommenders/
+
+# Annotation Processing
+.apt_generated/
+.apt_generated_test/
+
+# Scala IDE specific (Scala & Java development for Eclipse)
+.cache-main
+.scala_dependencies
+.worksheet
+
+# Uncomment this line if you wish to ignore the project description file.
+# Typically, this file would be tracked if it contains build/dependency configurations:
+#.project
+
+### MATLAB template
+# Windows default autosave extension
+*.asv
+
+# OSX / *nix default autosave extension
+*.m~
+
+# Compiled MEX binaries (all platforms)
+*.mex*
+
+# Packaged app and toolbox files
+*.mlappinstall
+*.mltbx
+
+# Generated helpsearch folders
+helpsearch*/
+
+# Simulink code generation folders
+slprj/
+sccprj/
+
+# Matlab code generation folders
+codegen/
+
+# Simulink autosave extension
+*.autosave
+
+# Simulink cache files
+*.slxc
+
+# Octave session info
+octave-workspace
+
+### JetBrains template
+# Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
+# Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
+*.ini
+# User-specific stuff
+.idea/**/workspace.xml
+.idea/**/tasks.xml
+.idea/**/usage.statistics.xml
+.idea/**/dictionaries
+.idea/**/shelf
+.DS_Store
+# AWS User-specific
+.idea/**/aws.xml
+
+# Generated files
+.idea/**/contentModel.xml
+
+# Sensitive or high-churn files
+.idea/**/dataSources/
+.idea/**/dataSources.ids
+.idea/**/dataSources.local.xml
+.idea/**/sqlDataSources.xml
+.idea/**/dynamic.xml
+.idea/**/uiDesigner.xml
+.idea/**/dbnavigator.xml
+
+# Gradle
+.idea/**/gradle.xml
+.idea/**/libraries
+
+# Gradle and Maven with auto-import
+# When using Gradle or Maven with auto-import, you should exclude module files,
+# since they will be recreated, and may cause churn.  Uncomment if using
+# auto-import.
+# .idea/artifacts
+# .idea/compiler.xml
+# .idea/jarRepositories.xml
+# .idea/modules.xml
+# .idea/*.iml
+# .idea/modules
+# *.iml
+# *.ipr
+
+# CMake
+cmake-build-*/
+
+# Mongo Explorer plugin
+.idea/**/mongoSettings.xml
+
+# File-based project format
+*.iws
+
+# IntelliJ
+out/
+
+# mpeltonen/sbt-idea plugin
+.idea_modules/
+
+# JIRA plugin
+atlassian-ide-plugin.xml
+
+# Cursive Clojure plugin
+.idea/replstate.xml
+
+# SonarLint plugin
+.idea/sonarlint/
+
+# Crashlytics plugin (for Android Studio and IntelliJ)
+com_crashlytics_export_strings.xml
+crashlytics.properties
+crashlytics-build.properties
+fabric.properties
+
+# Editor-based Rest Client
+.idea/httpRequests
+
+# Android studio 3.1+ serialized cache file
+.idea/caches/build_file_checksums.ser
+
+### KDevelop4 template
+*.kdev4
+.kdev4/
+
+### Calabash template
+# Calabash / Cucumber
+rerun/
+reports/
+screenshots/
+screenshot*.png
+test-servers/
+
+# bundler
+.bundle
+vendor
+
+### Xcode template
+## User settings
+xcuserdata/
+
+## Xcode 8 and earlier
+*.xcscmblueprint
+*.xccheckout
+
+### Metals template
+ # Generated Metals (Scala Language Server) files
+ # Reference: https://scalameta.org/metals/
+.metals/
+.bloop/
+project/metals.sbt
+
+### Otto template
+.otto/
+
+### NotepadPP template
+# Notepad++ backups #
+*.bak
+
+### EiffelStudio template
+# The compilation directory
+EIFGENs
+
+### Example user template template
+### Example user template
+
+# IntelliJ project files
+.idea
+*.iml
+out
+gen
+### Momentics template
+# Built files
+x86/
+arm/
+arm-p/
+translations/*.qm
+
+# IDE settings
+.settings/
+
+### XilinxISE template
+# intermediate build files
+*.bgn
+*.bit
+*.bld
+*.cmd_log
+*.drc
+*.ll
+*.lso
+*.msd
+*.msk
+*.ncd
+*.ngc
+*.ngd
+*.ngr
+*.pad
+*.par
+*.pcf
+*.prj
+*.ptwx
+*.rbb
+*.rbd
+*.stx
+*.syr
+*.twr
+*.twx
+*.unroutes
+*.ut
+*.xpi
+*.xst
+*_bitgen.xwbt
+*_envsettings.html
+*_map.map
+*_map.mrp
+*_map.ngm
+*_map.xrpt
+*_ngdbuild.xrpt
+*_pad.csv
+*_pad.txt
+*_par.xrpt
+*_summary.html
+*_summary.xml
+*_usage.xml
+*_xst.xrpt
+
+# iMPACT generated files
+_impactbatch.log
+impact.xsl
+impact_impact.xwbt
+ise_impact.cmd
+webtalk_impact.xml
+
+# Core Generator generated files
+xaw2verilog.log
+
+# project-wide generated files
+*.gise
+par_usage_statistics.html
+usage_statistics_webtalk.html
+webtalk.log
+webtalk_pn.xml
+
+# generated folders
+iseconfig/
+xlnx_auto_0_xdb/
+xst/
+_ngo/
+_xmsgs/
+
+### Ansible template
+*.retry
+
+### Backup template
+*.bak
+*.gho
+*.ori
+*.orig
+*.tmp
+
+### SublimeText template
+# Cache files for Sublime Text
+*.tmlanguage.cache
+*.tmPreferences.cache
+*.stTheme.cache
+
+# Workspace files are user-specific
+*.sublime-workspace
+
+# Project files should be checked into the repository, unless a significant
+# proportion of contributors will probably not be using Sublime Text
+# *.sublime-project
+
+# SFTP configuration file
+sftp-config.json
+sftp-config-alt*.json
+
+# Package control specific files
+Package Control.last-run
+Package Control.ca-list
+Package Control.ca-bundle
+Package Control.system-ca-bundle
+Package Control.cache/
+Package Control.ca-certs/
+Package Control.merged-ca-bundle
+Package Control.user-ca-bundle
+oscrypto-ca-bundle.crt
+bh_unicode_properties.cache
+
+# Sublime-github package stores a github token in this file
+# https://packagecontrol.io/packages/sublime-github
+GitHub.sublime-settings
+
+### SBT template
+# Simple Build Tool
+# http://www.scala-sbt.org/release/docs/Getting-Started/Directories.html#configuring-version-control
+
+target/
+lib_managed/
+src_managed/
+project/boot/
+project/plugins/project/
+.history
+.cache
+.lib/
+
+### Anjuta template
+# Local configuration folder and symbol database
+/.anjuta/
+/.anjuta_sym_db.db
+
+### ModelSim template
+# ignore ModelSim generated files and directories (temp files and so on)
+#[_@]*
+
+# ignore compilation output of ModelSim
+*.mti
+*.dat
+*.dbs
+*.psm
+*.bak
+*.cmp
+*.jpg
+#*.html
+*.bsf
+
+# ignore simulation output of ModelSim
+wlf*
+*.wlf
+*.vstf
+*.ucdb
+cov*/
+transcript*
+sc_dpiheader.h
+vsim.dbg
+
+### Vim template
+# Swap
+[._]*.s[a-v][a-z]
+!*.svg  # comment out if you don't need vector files
+[._]*.sw[a-p]
+[._]s[a-rt-v][a-z]
+[._]ss[a-gi-z]
+[._]sw[a-p]
+
+# Session
+Session.vim
+Sessionx.vim
+
+# Temporary
+.netrwhist
+*~
+# Auto-generated tag files
+tags
+# Persistent undo
+[._]*.un~
+
+!/token.ini
+/token.ini
```

### Comparing `nnsom-1.7.7/README.md` & `nnsom-1.7.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-# NNSOM
-
-## Self-Organizing Maps
-
-NNSOM is a Python library that provides an implementation of Self-Organizing Maps (SOM) using NumPy and CuPy.
-SOM is a type of Artificial Neural Network that can transform complex, nonlinear statistical relationships between high-dimensional data into simple topological relationships on a low-dimensional display (typically 2-dimensional).
-
-The library is designed with two main goals in mind:
-
-- Extensibility: NNSOM aims to provide a solid foundation for researchers to build upon and extend its functionality according to their specific requirements.
-- Educational Value: The implementation is structured in a way that allows students to quickly understand the inner workings of SOM, fostering a better grasp of the algorithm's details.
-
-With NNSOM, researchers and students alike can leverage the power of SOM for various applications, such as data visualization, clustering, and dimensionality reduction, while benefiting from the flexibility and educational value offered by this library.
-
-## Installation
-
-You can install the NNSOM by just using pip:
-
-```angular2html
-pip install NNSOM
-```
-
-## How to use it
-
-You can see the example file with Iris dataset on Jupyter Notebook [here](https://github.com/amir-jafari/SOM/blob/main/examples/Tabular/Iris/notebook/Iris_training.ipynb).
-
-### Data Preparation
-To use the NNSOM library effectively, format your data as a NumPy matrix where each row is an observation. 
-```bash
-import numpy as np
-np.random.seed(42)
-data = np.random.rand(3000, 10)
-```
-
-Alternatively, you can provide the data as a list of lists, following this structure:
-```bash
-data = [
-  [value1, value2, value3, ..., valueN], # Observation 1
-  [value1, value2, value3, ..., valueN], # Observation 2
-  ...,
-  [value1, value2, value3, ..., valueN], # Observation M
-]
-```
-
-### Customize Your Normalization
-Depending on your data's specific characteristics, you may opt to define a custom normalization function. 
-Here's how to normalize your data using sklearn's MinMaxScaler:
-```bash 
-from sklearn.preprocessing import MinMaxScaler
-scaler = MinMaxScaler(feature_range=(-1, 1))
-norm_func = scaler.fit_transform
-```
-
-### Configurate the SOM Grid Parameters
-Then, you can configurate the SOM Grid Parameters as follows:
-```bash
-SOM_Row_Num = 4  # The number of rows in the SOM grid
-SOM_Col_Num = 4  # The number of columns in the SOM grid
-Dimensions = (SOM_Row_Num, SOM_Col_Num) # The two-dimensional layout of the SOM grid 
-```
-
-### Configurate the Training Parameters 
-Next, you can configurate the Training Parameters as follows:
-```bash
-Epochs = 200  # The total number of training epochs 
-Steps = 100  #  The granularity of the weight update process within each epoch.
-Init_neighborhood = 3 # Initial size of the neighborhood radius   
-```
-
-### Train the SOM
-Then, you can train NNSOM just as follows:
-```bash
-from NNSOM.plots import SOMPlots
-som = SOMPlots(Dimensions)  # Initialization of 4x4 SOM
-som.init_w(data, norm_func=norm_func) # Initialize the weight
-som.train(data, Init_neighborhood, Epochs, Steps)
-```
-
-### Export a SOM and load it again
-A model can be saved using pickle as follows:
-```bash
-file_name = "..."
-model_path = ".../"
-
-som.save_pickle(file_name, model_path)
-```
-and can be loaded as follows:
-```bash
-from NNSOM.plots import SOMPlots
-som = SOMPlots(Dimensions)  # Use the same dimension with the stored model.
-som = som.load_pickle(file_name, model_path)
-```
-
-### Post-Training Data Clustering with NNSOM
-After training SOM with NNSOM, you can leverage the trained model to cluster new or existing data. 
-```bash
-clust, dist, mdist, clusterSizes = som.cluster_data(data)
-```
-- clust: This is a list where each sublist contains the indices of data points that are assigned to the same cluster.
-- dist: This list mirrors the structure of the "clust" list, with each sublist containing the distances of the corresponding data points. in "clust" from their Best Matching Unit.
-- mdist: An array where each element represents the maximum distance between the SOM neuron.
-- clusterSizes: An array listing the number of data points in each cluster.
-
-### Error Analysis
-NNSOM offers comprehensive tools to assess the quality and reliability of the trained SOM through various error metrics. 
-Understanding these errors can help refine the SOM's configuration and interpret its performance effectively. 
-Below are the three types of error measures provided by NNSOM:
-
-#### 1. Quantization Error
-Quantization error measures the average distance between each data point and its Best Matching Unit (BMU). This error provides insight into the SOM's ability to accurately represent the data space. A lower quantization error generally indicates a better representation.
-
-Examples:
-```bash
-# Find quantization error
-clust, dist, mdist, clusterSizes = som.cluster_data(data)
-quant_err = som.quantization_error(dist)
-print('Quantization error: ' + str(quant_err))
-```
-
-#### 2. Topological Error
-Topological error evaluates the SOM's preservation of the data's topological structure. It is calculated by checking if adjacent data points in the input space are mapped to adjacent neurons in the SOM. This metric is split into two:
-
-- Topological Error (1st neighbor): Measures the proportion of data points whose first nearest neighbor in the input space is not their neighbor on the map.
-- Topological Error (1st and 2nd neighbor): Extends this to the first and second nearest neighbors.
-
-Examples:
-```bash
-# Find topological error
-top_error_1, top_error_1_2 =  som.topological_error(data)
-print('Topological Error (1st neighbor) = ' + str(top_error_1) + '%')
-print('Topological Error (1st and 2nd neighbor) = ' + str(top_error_1_2) + '%')
-```
-
-#### 3. Distortion Error
-Distortion error calculates the total distance between each data point and its corresponding BMU, scaled by the data density around each BMU. This error helps to understand how well the SOM covers the distribution of the dataset and identifies areas where the map might be over or under-fitting.
-
-Examples:
-```bash
-# Find Distortion Error
-som.distortion_error(data)
-```
-
-### Visualize the SOM
-
-To effectively understand and interpret the results of your SOM training, visualizing the SOM grid is crucial.
-The NNSOM library offers a variety of plotting functions that allow you to visualize different aspects of the SOM and the training process.
-
-#### The Generic Plot Function [[source]](https://github.com/amir-jafari/SOM/blob/main/src/NNSOM/plots.py#L1391)
-This generic plot function can be used to generate multiple types of visualizations depending on the specified plot type.
-
-Usage of the Plot Function:
-```bash
-som.plot('plot_type', data_dict=None, ind=None, target_class=None, use_add_array=False)
-```
-
-Parameters:
-- plot_type: A string indicating the type of plot to generate. Options include 'top', 'neuron_dist', 'hit_hist', etc.
-- data_dict: Optional dictionary containing data needed for specific plots.
-- ind: Optional index for targeted plotting.
-- target_class: Optional parameter to specify a target class for the plot.
-- use_add_array: Boolean flag to indicate whether additional arrays in data_dict should be used.
-
-Structure of data_dict:
-
-The data_dict parameter should be structured as follows to provide necessary data for the plots:
-```bash
-data_dict = {
-  "data": data,          # Main dataset used in SOM training or the new inputs data
-  "target": y,           # Target variable, if applicable
-  "clust": clust,        # Clustering results from SOM
-  "add_1d_array": [],    # Additional 1D arrays for enhanced plotting
-  "add_2d_array": [],    # Additional 2D arrays for enhanced plotting
-}
-```
-
-The source code for the plot function can be found [here](https://github.com/amir-jafari/SOM/blob/main/src/NNSOM/plots.py#L1391).
-
-#### Examples of Common Visualizations
-
-1. Topological Grid
-    
-    Visualize the topological grid of the SOM to understand the layout and structure of the neurons.
-```bash
-import matplotlib.pyplot as plt
-fig, ax, patches = som.plot('top')
-plt.show()
-```
-
-2. Neuron Distance Map (U-Map)
-    
-    Display a distance map (U-Map) to see the distances between neighboring neurons, highlighting potential clusters.
-```bash
-fig, ax, pathces = som.plot('neuron_dist')
-plt.show()
-```
-
-3. Hit Histogram
-
-    Generate a hit histogram to visualize the frequency of each neuron being the best matching unit.
-```bash
-fig, ax, patches, text = som.plot('hit_hist', data_dict)
-plt.show()
-```
+# NNSOM
+
+## Self-Organizing Maps
+
+NNSOM is a Python library that provides an implementation of Self-Organizing Maps (SOM) using NumPy and CuPy.
+SOM is a type of Artificial Neural Network that can transform complex, nonlinear statistical relationships between high-dimensional data into simple topological relationships on a low-dimensional display (typically 2-dimensional).
+
+The library is designed with two main goals in mind:
+
+- Extensibility: NNSOM aims to provide a solid foundation for researchers to build upon and extend its functionality according to their specific requirements.
+- Educational Value: The implementation is structured in a way that allows students to quickly understand the inner workings of SOM, fostering a better grasp of the algorithm's details.
+
+With NNSOM, researchers and students alike can leverage the power of SOM for various applications, such as data visualization, clustering, and dimensionality reduction, while benefiting from the flexibility and educational value offered by this library.
+
+## Installation
+
+You can install the NNSOM by just using pip:
+
+```angular2html
+pip install NNSOM
+```
+
+## How to use it
+
+You can see the example file with Iris dataset on Jupyter Notebook [here](https://github.com/amir-jafari/SOM/blob/main/examples/Tabular/Iris/notebook/iris_training.ipynb).
+
+### Data Preparation
+To use the NNSOM library effectively, format your data as a NumPy matrix where each row is an observation. 
+```bash
+import numpy as np
+np.random.seed(42)
+data = np.random.rand(3000, 10)
+```
+
+Alternatively, you can provide the data as a list of lists, following this structure:
+```bash
+data = [
+  [value1, value2, value3, ..., valueN], # Observation 1
+  [value1, value2, value3, ..., valueN], # Observation 2
+  ...,
+  [value1, value2, value3, ..., valueN], # Observation M
+]
+```
+
+### Customize Your Normalization
+Depending on your data's specific characteristics, you may opt to define a custom normalization function. 
+Here's how to normalize your data using sklearn's MinMaxScaler:
+```bash 
+from sklearn.preprocessing import MinMaxScaler
+scaler = MinMaxScaler(feature_range=(-1, 1))
+norm_func = scaler.fit_transform
+```
+
+### Configurate the SOM Grid Parameters
+Then, you can configurate the SOM Grid Parameters as follows:
+```bash
+SOM_Row_Num = 4  # The number of rows in the SOM grid
+SOM_Col_Num = 4  # The number of columns in the SOM grid
+Dimensions = (SOM_Row_Num, SOM_Col_Num) # The two-dimensional layout of the SOM grid 
+```
+
+### Configurate the Training Parameters 
+Next, you can configurate the Training Parameters as follows:
+```bash
+Epochs = 200  # The total number of training epochs 
+Steps = 100  #  The granularity of the weight update process within each epoch.
+Init_neighborhood = 3 # Initial size of the neighborhood radius   
+```
+
+### Train the SOM
+Then, you can train NNSOM just as follows:
+```bash
+from NNSOM.plots import SOMPlots
+som = SOMPlots(Dimensions)  # Initialization of 4x4 SOM
+som.init_w(data, norm_func=norm_func) # Initialize the weight
+som.train(data, Init_neighborhood, Epochs, Steps)
+```
+
+### Export a SOM and load it again
+A model can be saved using pickle as follows:
+```bash
+file_name = "..."
+model_path = ".../"
+
+som.save_pickle(file_name, model_path)
+```
+and can be loaded as follows:
+```bash
+from NNSOM.plots import SOMPlots
+som = SOMPlots(Dimensions)  # Use the same dimension with the stored model.
+som = som.load_pickle(file_name, model_path)
+```
+
+### Post-Training Data Clustering with NNSOM
+After training SOM with NNSOM, you can leverage the trained model to cluster new or existing data. 
+```bash
+clust, dist, mdist, clusterSizes = som.cluster_data(data)
+```
+- clust: This is a list where each sublist contains the indices of data points that are assigned to the same cluster.
+- dist: This list mirrors the structure of the "clust" list, with each sublist containing the distances of the corresponding data points. in "clust" from their Best Matching Unit.
+- mdist: An array where each element represents the maximum distance between the SOM neuron.
+- clusterSizes: An array listing the number of data points in each cluster.
+
+### Error Analysis
+NNSOM offers comprehensive tools to assess the quality and reliability of the trained SOM through various error metrics. 
+Understanding these errors can help refine the SOM's configuration and interpret its performance effectively. 
+Below are the three types of error measures provided by NNSOM:
+
+#### 1. Quantization Error
+Quantization error measures the average distance between each data point and its Best Matching Unit (BMU). This error provides insight into the SOM's ability to accurately represent the data space. A lower quantization error generally indicates a better representation.
+
+Examples:
+```bash
+# Find quantization error
+clust, dist, mdist, clusterSizes = som.cluster_data(data)
+quant_err = som.quantization_error(dist)
+print('Quantization error: ' + str(quant_err))
+```
+
+#### 2. Topological Error
+Topological error evaluates the SOM's preservation of the data's topological structure. It is calculated by checking if adjacent data points in the input space are mapped to adjacent neurons in the SOM. This metric is split into two:
+
+- Topological Error (1st neighbor): Measures the proportion of data points whose first nearest neighbor in the input space is not their neighbor on the map.
+- Topological Error (1st and 2nd neighbor): Extends this to the first and second nearest neighbors.
+
+Examples:
+```bash
+# Find topological error
+top_error_1, top_error_1_2 =  som.topological_error(data)
+print('Topological Error (1st neighbor) = ' + str(top_error_1) + '%')
+print('Topological Error (1st and 2nd neighbor) = ' + str(top_error_1_2) + '%')
+```
+
+#### 3. Distortion Error
+Distortion error calculates the total distance between each data point and its corresponding BMU, scaled by the data density around each BMU. This error helps to understand how well the SOM covers the distribution of the dataset and identifies areas where the map might be over or under-fitting.
+
+Examples:
+```bash
+# Find Distortion Error
+som.distortion_error(data)
+```
+
+### Visualize the SOM
+
+To effectively understand and interpret the results of your SOM training, visualizing the SOM grid is crucial.
+The NNSOM library offers a variety of plotting functions that allow you to visualize different aspects of the SOM and the training process.
+
+#### The Generic Plot Function [[source]](https://github.com/amir-jafari/SOM/blob/main/src/NNSOM/plots.py#L1391)
+This generic plot function can be used to generate multiple types of visualizations depending on the specified plot type.
+
+Usage of the Plot Function:
+```bash
+som.plot('plot_type', data_dict=None, ind=None, target_class=None, use_add_array=False)
+```
+
+Parameters:
+- plot_type: A string indicating the type of plot to generate. Options include 'top', 'neuron_dist', 'hit_hist', etc.
+- data_dict: Optional dictionary containing data needed for specific plots.
+- ind: Optional index for targeted plotting.
+- target_class: Optional parameter to specify a target class for the plot.
+- use_add_array: Boolean flag to indicate whether additional arrays in data_dict should be used.
+
+Structure of data_dict:
+
+The data_dict parameter should be structured as follows to provide necessary data for the plots:
+```bash
+data_dict = {
+  "data": data,          # Main dataset used in SOM training or the new inputs data
+  "target": y,           # Target variable, if applicable
+  "clust": clust,        # Clustering results from SOM
+  "add_1d_array": [],    # Additional 1D arrays for enhanced plotting
+  "add_2d_array": [],    # Additional 2D arrays for enhanced plotting
+}
+```
+
+The source code for the plot function can be found [here](https://github.com/amir-jafari/SOM/blob/main/src/NNSOM/plots.py#L1391).
+
+#### Examples of Common Visualizations
+
+1. Topological Grid
+    
+    Visualize the topological grid of the SOM to understand the layout and structure of the neurons.
+```bash
+import matplotlib.pyplot as plt
+fig, ax, patches = som.plot('top')
+plt.show()
+```
+
+2. Neuron Distance Map (U-Map)
+    
+    Display a distance map (U-Map) to see the distances between neighboring neurons, highlighting potential clusters.
+```bash
+fig, ax, pathces = som.plot('neuron_dist')
+plt.show()
+```
+
+3. Hit Histogram
+
+    Generate a hit histogram to visualize the frequency of each neuron being the best matching unit.
+```bash
+fig, ax, patches, text = som.plot('hit_hist', data_dict)
+plt.show()
+```
```

### Comparing `nnsom-1.7.7/PKG-INFO` & `nnsom-1.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.7.7
+Version: 1.7.8
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Project-URL: Documenation, https://amir-jafari.github.io/SOM/
 Author: Dr. Martin Hagan, Dr. Amir Jafari, Lakshmi Sravya Chalapati, Ei Tanaka
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
 Keywords: Clustering,Machine Learning,Neural Network,SOM,Unsupervised Learning
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # NNSOM
 
 ## Self-Organizing Maps
@@ -47,15 +44,15 @@
 
 ```angular2html
 pip install NNSOM
 ```
 
 ## How to use it
 
-You can see the example file with Iris dataset on Jupyter Notebook [here](https://github.com/amir-jafari/SOM/blob/main/examples/Tabular/Iris/notebook/Iris_training.ipynb).
+You can see the example file with Iris dataset on Jupyter Notebook [here](https://github.com/amir-jafari/SOM/blob/main/examples/Tabular/Iris/notebook/iris_training.ipynb).
 
 ### Data Preparation
 To use the NNSOM library effectively, format your data as a NumPy matrix where each row is an observation. 
 ```bash
 import numpy as np
 np.random.seed(42)
 data = np.random.rand(3000, 10)
```

