# Comparing `tmp/receipt_enhancer-0.1.2.tar.gz` & `tmp/receipt_enhancer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receipt_enhancer-0.1.2.tar", max compression
+gzip compressed data, was "receipt_enhancer-0.1.4.tar", max compression
```

## Comparing `receipt_enhancer-0.1.2.tar` & `receipt_enhancer-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-03-06 17:46:27.092848 receipt_enhancer-0.1.2/LICENSE
--rw-r--r--   0        0        0     2381 2024-03-06 18:00:03.264872 receipt_enhancer-0.1.2/README.md
--rw-r--r--   0        0        0      500 2024-03-18 15:37:31.152944 receipt_enhancer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       93 2024-03-06 17:48:19.540852 receipt_enhancer-0.1.2/receipt_enhancer/__init__.py
--rw-r--r--   0        0        0    17658 2024-03-18 15:36:17.548942 receipt_enhancer-0.1.2/receipt_enhancer/receipt_enhancer.py
--rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-06 17:46:27.092848 receipt_enhancer-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2381 2024-03-06 18:00:03.264872 receipt_enhancer-0.1.4/README.md
+-rw-r--r--   0        0        0      500 2024-04-24 04:37:03.946422 receipt_enhancer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-03-06 17:48:19.540852 receipt_enhancer-0.1.4/receipt_enhancer/__init__.py
+-rw-r--r--   0        0        0    15106 2024-04-24 04:30:27.650411 receipt_enhancer-0.1.4/receipt_enhancer/receipt_enhancer.py
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.4/PKG-INFO
```

### Comparing `receipt_enhancer-0.1.2/LICENSE` & `receipt_enhancer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.2/README.md` & `receipt_enhancer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.2/receipt_enhancer/receipt_enhancer.py` & `receipt_enhancer-0.1.4/receipt_enhancer/receipt_enhancer.py`

 * *Files 25% similar despite different names*

```diff
@@ -40,120 +40,95 @@
 
         lines = cv2.HoughLinesP(edges, 1, np.pi / 180, threshold=hough_threshold,
                                 minLineLength=int(length[0]), maxLineGap=max_gap)
 
         if lines is None:
             return []
 
-        # Calcular distâncias entre todas as linhas
         line_distances = np.zeros((len(lines), len(lines)))
         for i in range(len(lines)):
             for j in range(i + 1, len(lines)):
                 dist = np.linalg.norm(np.array(lines[i][0][:2]) - np.array(lines[j][0][:2]))
                 line_distances[i][j] = dist
 
-        # Encontrar grupos de linhas que não atendem aos critérios de distância mínima e máxima
         lines_to_remove = set()
         for i in range(len(lines)):
             if i in lines_to_remove:
                 continue
             for j in range(i + 1, len(lines)):
                 if j in lines_to_remove:
                     continue
                 if min_distance[0] <= line_distances[i][j] <= min_distance[1]:
                     lines_to_remove.add(i)
                     lines_to_remove.add(j)
 
-        # Remover grupos de linhas que não atendem aos critérios
         filtered_lines = [lines[i] for i in range(len(lines)) if i not in lines_to_remove]
 
         return filtered_lines
 
     def calculate_roi_size_fraction(self, image: np.ndarray) -> float:
-        # Convert image to grayscale
         grey = self.convert_to_greyscale(image)
 
-        # Calcula os contornos na imagem
         contours, _ = cv2.findContours(grey, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
-        # Encontra o maior contorno (maior área)
         max_contour = max(contours, key=cv2.contourArea)
-
-        # Calcula o retângulo delimitador do maior contorno
         x, y, w, h = cv2.boundingRect(max_contour)
-
-        # Calcula a área do maior contorno
         object_area = w * h
 
-        # Calcula a fração de tamanho da ROI em relação à resolução da imagem
         resolution = min(image.shape[0], image.shape[1])
-        roi_size_fraction = object_area / (resolution * resolution)  # Normalizado pela resolução ao quadrado
+        roi_size_fraction = object_area / (resolution * resolution)
 
         return roi_size_fraction
 
     def remove_overlapping_lines(self, lines: List) -> List:
-        # Lista para armazenar índices das linhas a serem removidas
         lines_to_remove = set()
 
-        # Itera sobre todas as combinações possíveis de pares de linhas
         for i in range(len(lines)):
             if i in lines_to_remove:
                 continue
             for j in range(i + 1, len(lines)):
                 if j in lines_to_remove:
                     continue
-                # Coordenadas da primeira linha
+
                 x1, y1, x2, y2 = lines[i][0]
-                # Coordenadas da segunda linha
                 x3, y3, x4, y4 = lines[j][0]
 
-                # Calcula a interseção entre as duas linhas
                 intersection = self.line_intersection((x1, y1), (x2, y2), (x3, y3), (x4, y4))
 
-                # Verifica se há interseção
                 if intersection is not None:
-                    # Se houver interseção, marca ambas as linhas para remoção
+
                     lines_to_remove.add(i)
                     lines_to_remove.add(j)
 
-        # Remove as linhas marcadas para remoção
         filtered_lines = [lines[i] for i in range(len(lines)) if i not in lines_to_remove]
 
         return filtered_lines
 
     def line_intersection(self, p1: Tuple[float, float], p2: Tuple[float, float],
-                        p3: Tuple[float, float], p4: Tuple[float, float]) -> Optional[Tuple[float, float]]:
-        """
-        Calcula a interseção entre duas linhas definidas pelos pontos p1-p2 e p3-p4.
-        Retorna None se as linhas forem paralelas ou se a interseção estiver fora dos limites das linhas.
-        Retorna as coordenadas (x, y) da interseção se existir dentro dos limites das linhas.
-        """
+                          p3: Tuple[float, float], p4: Tuple[float, float]) -> Optional[Tuple[float, float]]:
+
         x1, y1 = p1
         x2, y2 = p2
         x3, y3 = p3
         x4, y4 = p4
 
         denominator = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4)
 
-        # Verifica se as linhas são paralelas
         if denominator == 0:
             return None
 
-        # Calcula as coordenadas da interseção
         px = ((x1 * y2 - y1 * x2) * (x3 - x4) - (x1 - x2) * (x3 * y4 - y3 * x4)) / denominator
         py = ((x1 * y2 - y1 * x2) * (y3 - y4) - (y1 - y2) * (x3 * y4 - y3 * x4)) / denominator
 
-        # Verifica se a interseção está dentro dos limites das linhas
         if min(x1, x2) <= px <= max(x1, x2) and min(y1, y2) <= py <= max(y1, y2) \
                 and min(x3, x4) <= px <= max(x3, x4) and min(y3, y4) <= py <= max(y3, y4):
             return px, py
         else:
             return None
 
-
     def find_densest_region(self, image: ndarray, lines, proximity_threshold=50):
         max_density = 0
         best_x, best_y = 0, 0
 
         for line1 in lines:
             x1_1, y1_1, x2_1, y2_1 = line1[0]
             density = 0
@@ -295,102 +270,96 @@
         blocks_resized = [cv2.resize(block, (max_block_width, max_block_height)) for block in blocks]
 
         cols_per_row = int(np.sqrt(len(blocks_resized)))
         blocks_per_row = [blocks_resized[i:i + cols_per_row] for i in range(0, len(blocks_resized), cols_per_row)]
 
         return np.vstack([np.hstack(row_blocks) for row_blocks in blocks_per_row])
 
-    def adaptive_local_contrast(self, image: np.ndarray) -> np.ndarray:
-        image = self.convert_to_greyscale(image)
-        blocks = self.__segment_image_into_blocks(image)
+    def get_clip_limit(self, block: np.ndarray, grid_size: Tuple[int, int]):
+        hist_before = np.histogram(block, bins=256, range=(0, 255))[0]
 
-        adaptive_blocks_final = []
+        best_clip_limit = 0
+        best_score = float('-inf')
 
-        for block in blocks:
-            mean_block_intensity = np.mean(block)
-            std_block_intensity = np.std(block)
-            max_block_intensity = np.max(block)
-            min_block_intensity = np.min(block)
+        clip_limits = np.linspace(0.1, 2.0, num=20)
 
-            resolution = min(block.shape[0], block.shape[1])
+        for clip_limit in clip_limits:
+            clahe = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=grid_size)
+            block_clahe = clahe.apply(block.astype(np.uint8))
 
-            clip_limit = min(max(3.0, 2.0 * std_block_intensity / (mean_block_intensity - min_block_intensity + 1e-6)), 50.0)
-            tile_grid_size = max(3, int(resolution / 150))
+            hist_after = np.histogram(block_clahe, bins=256, range=(0, 255))[0]
+            hist_score = -np.sum(np.abs(hist_before - hist_after))
+            score = hist_score
+            if score > best_score:
+                best_score = score
+                best_clip_limit = clip_limit
 
-            clahe = cv2.createCLAHE(clipLimit=clip_limit,
-                                    tileGridSize=(tile_grid_size, tile_grid_size))
+        return max(0, min(5, best_clip_limit))
 
-            block_clahe = clahe.apply(block.astype(np.uint8))
-            alpha, beta, gamma = self.__get_adaptive_alpha_beta_gamma(image)
+    def __reduce_noise_and_texture(self, block):
 
-            gamma_corrected = np.clip(255.0 * (block_clahe / 255.0) ** gamma, 0, 255).astype(np.uint8)
+        f_transform = np.fft.fft2(block)
+        f_transform_shifted = np.fft.fftshift(f_transform)
+        magnitude_spectrum = 20 * np.log(np.abs(f_transform_shifted))
+        _, thresholded_spectrum = cv2.threshold(magnitude_spectrum, np.mean(magnitude_spectrum), 255, cv2.THRESH_BINARY)
 
-            block_clahe = gamma_corrected.astype(np.uint8)
+        high_frequency_mask = np.fft.ifftshift(thresholded_spectrum)
+        high_frequency_mask = np.fft.ifft2(high_frequency_mask)
+        high_frequency_mask = np.abs(high_frequency_mask)
 
-            mean_clahe_intensity = np.mean(block_clahe)
-            max_clahe_intensity = np.max(block_clahe)
-            min_clahe_intensity = np.min(block_clahe)
+        high_frequency_mask = cv2.normalize(high_frequency_mask, None, alpha=0, beta=1, norm_type=cv2.NORM_MINMAX)
+        high_frequency_mask = (high_frequency_mask * 255).astype(np.uint8)
 
-            adapt_factor_min_clahe = min(1.0, (mean_clahe_intensity - min_clahe_intensity) / 255)
-            adapt_factor_max_clahe = min(1.0, (max_clahe_intensity - mean_clahe_intensity) / 255)
+        equalized_block = cv2.equalizeHist(block)
+        _, text_mask = cv2.threshold(equalized_block, 0, 255, cv2.THRESH_BINARY_INV | cv2.THRESH_OTSU)
 
-            min_threshold_clahe = mean_block_intensity * adapt_factor_min_clahe
-            max_threshold_clahe = mean_block_intensity * adapt_factor_max_clahe
+        smoothed_block = np.where(text_mask == 0, cv2.medianBlur(block, 5), block)
 
-            _, dark_regions = cv2.threshold(block_clahe, min_threshold_clahe, 255, cv2.THRESH_BINARY)
-            _, bright_regions = cv2.threshold(block_clahe, max_threshold_clahe, 255, cv2.THRESH_BINARY_INV)
+        return smoothed_block
 
-            dark_mask = cv2.bitwise_not(dark_regions)
-            bright_mask = cv2.bitwise_not(bright_regions)
+    def adaptive_local_contrast(self, image: np.ndarray) -> np.ndarray:
+        image = self.convert_to_greyscale(image)
+        blocks = self.__segment_image_into_blocks(image)
 
-            texture_smoothed_block = cv2.bilateralFilter(block_clahe,
-                                                         d=max(10, int(0.1 * tile_grid_size)),
-                                                         sigmaColor=int(0.1 * mean_block_intensity),
-                                                         sigmaSpace=int(0.1 * tile_grid_size))
+        adaptive_blocks_final = []
 
-            black_adjustment = min(1.0, max(0.6, (min_block_intensity - 10) / 255))
-            black_adaptive = cv2.convertScaleAbs(texture_smoothed_block, alpha=black_adjustment, beta=0)
+        global_mean_intensity = np.mean(image)
 
-            white_adjustment = min(1.0, (255 - max_block_intensity) / 255)
-            white_adaptive = cv2.convertScaleAbs(texture_smoothed_block, alpha=white_adjustment, beta=0)
+        for block in blocks:
+            block = self.__reduce_noise_and_texture(block)
+            mean_block_intensity = np.mean(block)
+            max_block_intensity = np.max(block)
 
-            black_adaptive = cv2.bitwise_and(black_adaptive, black_adaptive, mask=bright_mask)
-            white_adaptive = cv2.bitwise_and(white_adaptive, white_adaptive, mask=dark_mask)
+            resolution = min(block.shape[0], block.shape[1])
+            tile_grid_size = max(3, int(resolution / 150))
 
-            local_std_dev = np.std(block_clahe)
-            beta = max(0.1, min(1.0, (local_std_dev / 255) * 2))
+            clip_limit = self.get_clip_limit(block, (tile_grid_size, tile_grid_size))
 
-            adaptive_block = cv2.addWeighted(block_clahe, 1, white_adaptive, beta, 0)
-            adaptive_block = cv2.addWeighted(adaptive_block, 1, black_adaptive, beta, 0)
+            clahe = cv2.createCLAHE(clipLimit=clip_limit,
+                                    tileGridSize=(tile_grid_size, tile_grid_size))
 
-            adaptive_block = cv2.bilateralFilter(adaptive_block,
-                                                 d=max(10, int(0.1 * tile_grid_size)),
-                                                 sigmaColor=int(0.1 * mean_block_intensity),
-                                                 sigmaSpace=int(0.1 * tile_grid_size))
+            block_clahe = clahe.apply(block.astype(np.uint8))
 
-            local_std_dev = np.std(adaptive_block)
-            local_variance = np.var(adaptive_block)
-            adjusted_variance = max(10, local_variance)
+            mean_clahe_intensity = np.mean(block_clahe)
+            adapt_factor_min_clahe = mean_clahe_intensity / 255.0
+            adapt_factor_max_clahe = (255 - mean_clahe_intensity) / 255.0
+
+            black_adjustment = min(1.0, (global_mean_intensity - mean_block_intensity) / 255)
+            black_adaptive = cv2.convertScaleAbs(block_clahe, alpha=black_adjustment, beta=0)
 
-            sharpness_block_color = cv2.detailEnhance(cv2.cvtColor(adaptive_block, cv2.COLOR_GRAY2BGR),
-                                                      sigma_s=max(0.2, min(1.0, local_std_dev / 100)),
-                                                      sigma_r=max(0.1, min(2.0, np.sqrt(adjusted_variance))))
+            white_adjustment = min(1.0, (255 - max_block_intensity) / 255)
+            white_adaptive = cv2.convertScaleAbs(block_clahe, alpha=white_adjustment, beta=0)
 
-            sharpness_block = cv2.cvtColor(sharpness_block_color, cv2.COLOR_BGR2GRAY)
+            adaptive_block = cv2.addWeighted(block_clahe, 1, white_adaptive, adapt_factor_max_clahe, 0)
+            adaptive_block = cv2.addWeighted(adaptive_block, 1, black_adaptive, adapt_factor_min_clahe, 0)
 
-            adaptive_blocks_final.append(sharpness_block)
+            adaptive_blocks_final.append(adaptive_block)
 
         adaptive_image = self.__build_image_from_blocks(adaptive_blocks_final)
 
-        std_dev = np.std(adaptive_image)
-        adaptive_image = cv2.bilateralFilter(adaptive_image,
-                                             d=max(10, int(0.1 * std_dev)),
-                                             sigmaColor=int(0.1 * std_dev),
-                                             sigmaSpace=int(0.1 * std_dev))
-
         return adaptive_image
 
     def adaptative_weight(self, image: ndarray) -> ndarray:
         image = self.convert_to_greyscale(image)
 
         blocks = self.__segment_image_into_blocks(image)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `receipt_enhancer-0.1.2/PKG-INFO` & `receipt_enhancer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receipt-enhancer
-Version: 0.1.2
+Version: 0.1.4
 Summary: This module is essential for preprocessing receipt images to improve visual quality and facilitate automatic analysis.
 License: MIT
 Keywords: document,nfe,invoice,receipt
 Author: Ricardo Castro
 Author-email: srrenks@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

