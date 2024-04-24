# Comparing `tmp/PyPyNum-1.8.0.tar.gz` & `tmp/PyPyNum-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPyNum-1.8.0.tar", last modified: Fri Apr 12 14:50:36 2024, max compression
+gzip compressed data, was "PyPyNum-1.8.1.tar", last modified: Wed Apr 24 12:33:16 2024, max compression
```

## Comparing `PyPyNum-1.8.0.tar` & `PyPyNum-1.8.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:50:36.375800 PyPyNum-1.8.0/
--rw-rw-rw-   0        0        0    85418 2024-04-12 14:50:36.374800 PyPyNum-1.8.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 14:50:35.904800 PyPyNum-1.8.0/PyPyNum.egg-info/
--rw-rw-rw-   0        0        0    85418 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 14:50:36.355800 PyPyNum-1.8.0/pypynum/
--rw-rw-rw-   0        0        0     6632 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Array.py
--rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.0/pypynum/FourierT.py
--rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.0/pypynum/Geometry.py
--rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.0/pypynum/Graph.py
--rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.0/pypynum/Group.py
--rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.0/pypynum/Logic.py
--rw-rw-rw-   0        0        0    11024 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Matrix.py
--rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.0/pypynum/NeuralN.py
--rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.0/pypynum/PyPyNum.png
--rw-rw-rw-   0        0        0     8007 2024-01-25 08:45:23.000000 PyPyNum-1.8.0/pypynum/Quaternion.py
--rw-rw-rw-   0        0        0    43971 2024-04-12 12:58:03.000000 PyPyNum-1.8.0/pypynum/README.md
--rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.0/pypynum/Symbolics.py
--rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Tensor.py
--rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.0/pypynum/Tree.py
--rw-rw-rw-   0        0        0     3552 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Vector.py
--rw-rw-rw-   0        0        0     1831 2024-04-12 12:05:55.000000 PyPyNum-1.8.0/pypynum/__init__.py
--rw-rw-rw-   0        0        0     5860 2024-01-22 12:57:34.000000 PyPyNum-1.8.0/pypynum/__temporary.py
--rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.0/pypynum/chars.py
--rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.0/pypynum/cipher.py
--rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.0/pypynum/constants.py
--rw-rw-rw-   0        0        0      744 2024-01-22 13:17:32.000000 PyPyNum-1.8.0/pypynum/equations.py
--rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.0/pypynum/errors.py
--rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.0/pypynum/file.py
--rw-rw-rw-   0        0        0    26518 2024-03-28 08:22:55.000000 PyPyNum-1.8.0/pypynum/maths.py
--rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.0/pypynum/numbers.py
--rw-rw-rw-   0        0        0     8326 2024-02-01 12:22:16.000000 PyPyNum-1.8.0/pypynum/plotting.py
--rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.0/pypynum/polynomial.py
--rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.0/pypynum/probability.py
--rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.0/pypynum/random.py
--rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.0/pypynum/regression.py
--rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.0/pypynum/sequence.py
--rw-rw-rw-   0        0        0     8428 2024-01-24 05:43:19.000000 PyPyNum-1.8.0/pypynum/test.py
--rw-rw-rw-   0        0        0     2129 2024-02-27 12:58:01.000000 PyPyNum-1.8.0/pypynum/this.py
--rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.0/pypynum/tools.py
--rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.0/pypynum/types.py
--rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.0/pypynum/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-12 14:50:36.377800 PyPyNum-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0    36764 2024-04-12 14:50:12.000000 PyPyNum-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.688000 PyPyNum-1.8.1/
+-rw-rw-rw-   0        0        0    84338 2024-04-24 12:33:16.686999 PyPyNum-1.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.577000 PyPyNum-1.8.1/PyPyNum.egg-info/
+-rw-rw-rw-   0        0        0    84338 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.682000 PyPyNum-1.8.1/pypynum/
+-rw-rw-rw-   0        0        0     6632 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Array.py
+-rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.1/pypynum/FourierT.py
+-rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.1/pypynum/Geometry.py
+-rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.1/pypynum/Graph.py
+-rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.1/pypynum/Group.py
+-rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.1/pypynum/Logic.py
+-rw-rw-rw-   0        0        0    18050 2024-04-24 11:35:12.000000 PyPyNum-1.8.1/pypynum/Matrix.py
+-rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.1/pypynum/NeuralN.py
+-rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.1/pypynum/PyPyNum.png
+-rw-rw-rw-   0        0        0     8007 2024-01-25 08:45:23.000000 PyPyNum-1.8.1/pypynum/Quaternion.py
+-rw-rw-rw-   0        0        0    42891 2024-04-24 12:12:47.000000 PyPyNum-1.8.1/pypynum/README.md
+-rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.1/pypynum/Symbolics.py
+-rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Tensor.py
+-rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.1/pypynum/Tree.py
+-rw-rw-rw-   0        0        0     3552 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Vector.py
+-rw-rw-rw-   0        0        0     1843 2024-04-22 14:16:33.000000 PyPyNum-1.8.1/pypynum/__init__.py
+-rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.1/pypynum/chars.py
+-rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.1/pypynum/cipher.py
+-rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.1/pypynum/constants.py
+-rw-rw-rw-   0        0        0      713 2024-04-24 11:23:59.000000 PyPyNum-1.8.1/pypynum/equations.py
+-rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.1/pypynum/errors.py
+-rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.1/pypynum/file.py
+-rw-rw-rw-   0        0        0    26637 2024-04-21 23:30:31.000000 PyPyNum-1.8.1/pypynum/maths.py
+-rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.1/pypynum/numbers.py
+-rw-rw-rw-   0        0        0     8463 2024-04-24 12:20:39.000000 PyPyNum-1.8.1/pypynum/plotting.py
+-rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.1/pypynum/polynomial.py
+-rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.1/pypynum/probability.py
+-rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.1/pypynum/random.py
+-rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.1/pypynum/regression.py
+-rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.1/pypynum/sequence.py
+-rw-rw-rw-   0        0        0     8428 2024-01-24 05:43:19.000000 PyPyNum-1.8.1/pypynum/test.py
+-rw-rw-rw-   0        0        0     2129 2024-02-27 12:58:01.000000 PyPyNum-1.8.1/pypynum/this.py
+-rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.1/pypynum/tools.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.1/pypynum/types.py
+-rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.1/pypynum/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 12:33:16.689000 PyPyNum-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0    36724 2024-04-24 12:31:55.000000 PyPyNum-1.8.1/setup.py
```

### Comparing `PyPyNum-1.8.0/PKG-INFO` & `PyPyNum-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.8.0
+Version: 1.8.1
 Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
 Home-page: https://www.gitee.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -688,15 +688,15 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
@@ -737,98 +737,34 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增代码行数为603行
+eig函数修复了计算错误并改名为eigen
 
-Add 603 new lines of code
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增函数“magic_square”的功能简介：可
-以生成任意大于等于三的整数阶幻方。
-
-Introduction to the newly added
-function "magic square": It can
-generate any integer order magic
-square greater than or equal to
-three.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“Graph”的功能简介：具有有向图
-、无向图、带权有向图、带权无向图这四个对
-象，支持添加或删除顶点和边，以及深度优先
-搜索与广度优先搜索这两种图的遍历方式，还
-有计算最短路径等功能。
-
-Introduction to the functions of
-the newly added module "Graph":
-it has four objects: directed
-graph, undirected graph,
-weighted directed graph, and
-weighted undirected graph. It
-supports adding or removing
-vertices and edges, as well as
-depth first search and breadth
-first search for graph
-traversal. It also has functions
-such as calculating the shortest
-path.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“polynomial”的功能简介：有一
-个多项式对象，可以通过传入包含“(次数,
-系数)”的二元组组成的序列创建多项式对象
-，可以随时设置某一项的数值，并且支持多
-项式形式的四则运算，还有取商式、取余式
-、求幂、求模幂的功能。
-
-Introduction to the newly added
-module "polynomial": There is a
-polynomial object that can be
-created by passing in a sequence
-of binary tuples containing
-"degree, coefficient". The value
-of a certain term can be set at
-any time, and it supports
-polynomial form arithmetic
-operations. It also has
-functions such as quotient,
-remainder, exponentiation, and
-modular exponentiation.
+The eig function fixed
+calculation errors and changed
+its name to eigen
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
 <<<以下结构中的省略号表示原有的部分>>>
 
 <<<The ellipsis in the following structure represents the original part>>>
 
 PyPyNum
-    ★ Graph [Graph theory]
-        CLASSES
-            BaseGraph
-                BaseWeGraph
-                    WeDiGraph
-                    WeUnGraph
-                DiGraph
-                UnGraph
-    ★ polynomial [Polynomial object]
-        CLASSES
-            Polynomial
-        FUNCTIONS
-            poly(terms=None)
-    ★ tools [Other useful tools]
+    ★ Matrix [Matrix calculation]
         FUNCTIONS
             ...
-            magic_square(n)
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            ...
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -935,22 +871,24 @@
                     DFF
                     NOT
                     TFF
     ★ Matrix [Matrix calculation]
         CLASSES
             Matrix
         FUNCTIONS
-            eig(matrix)
-            identity(n)
-            lu(matrix)
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            identity(n: int) -> pypynum.Matrix.Matrix
+            lu(matrix: pypynum.Matrix.Matrix) -> tuple
             mat(data)
-            qr(matrix)
+            qr(matrix: pypynum.Matrix.Matrix) -> tuple
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
             same(rows, cols, value=0)
-            svd(matrix)
-            tril_indices(n, k=0, m=None)
+            svd(matrix: pypynum.Matrix.Matrix) -> tuple
+            tril_indices(n: int, k: int = 0, m: int = None) -> tuple
             zeros(_dimensions)
             zeros_like(_nested_list)
     ★ NeuralN [A simple neural network model]
         CLASSES
             NeuralNetwork
         FUNCTIONS
             neuraln(_input, _hidden, _output)
@@ -1126,14 +1064,17 @@
             totient(n: int) -> int
             mod_order(a: int, n: int, b: int) -> int
             primitive_root(a: int, single: bool = False) -> Union[int, list]
             normalize(data: arr, target: num = 1) -> arr
             average(data, weights, expected=False)
             exgcd(a: int, b: int) -> tuple
             crt(n: arr, a: arr) -> int
+            isqrt(x: int) -> int
+            is_possibly_square(n: int) -> bool
+            is_square(n: int) -> bool
     ★ numbers [Conversion of various numbers]
         FUNCTIONS
             float2fraction(number: float, mixed: bool = False, error: float = 1e-15) -> tuple
             int2roman(integer: int, overline: bool = True) -> str
             roman2int(roman_num: str) -> int
             str2int(string: str) -> int
         DATA
@@ -1355,29 +1296,31 @@
 >>> print(constants.tera)
 
 1099511627776
 2.718281828459045
 6.62607015e-34
 1.618033988749895
 3.141592653589793
-1000000000000.0
+1000000000000
 
 >>> p = [1, -2, -3, 4]
 >>> m = [
     [
         [1, 2, 3],
         [6, 10, 12],
         [7, 16, 9]
     ],
     [-1, -2, -3]
 ]
 >>> print(equations.polynomial_equation(p))
 >>> print(equations.linear_equation(*m))
 
-[(-1.5615528128088307-6.5209667308287455e-24j)   (2.5615528128088294+4.456233626665941e-24j)   (1.0000000000000007+3.241554513744382e-25j)]
+[[(-1.5615528128088307-6.5209667308287455e-24j)                                             0                                             0]
+ [                                            0   (2.5615528128088294+4.456233626665941e-24j)                                             0]
+ [                                            0                                             0   (1.0000000000000007+3.241554513744382e-25j)]]
 [ 1.6666666666666667 -0.6666666666666666 -0.4444444444444444]
 
 >>> print(maths.cot(constants.pi / 3))
 >>> print(maths.gamma(1.5))
 >>> print(maths.pi(1, 10, lambda x: x ** 2))
 >>> print(maths.product([2, 3, 5, 7, 11, 13, 17, 19, 23, 29]))
 >>> print(maths.sigma(1, 10, lambda x: x ** 2))
@@ -1464,18 +1407,18 @@
            -2.00e+00                            0.00e+00                            2.00e+00
 
 >>> print(random.gauss(0, 1, [2, 3, 4]))
 >>> print(random.rand([2, 3, 4]))
 >>> print(random.randint(0, 9, [2, 3, 4]))
 >>> print(random.uniform(0, 9, [2, 3, 4]))
 
-[[[0.4334341920363395, 0.055711784711422116, -1.0235500373980284, 0.30031229336738374], [-0.2650367914670356, 0.5513398538865067, -0.9735921328831166, 0.41345578602104827], [-0.11598957920080871, -0.9044539791933183, 1.6448227575237069, -0.26304156924843813]], [[0.27363898507271256, -0.5897181011789576, 1.5120937498473583, 2.1302709742844694], [1.9743293887616236, 0.4117207260898469, 0.5809554193110543, -1.8456249006764007], [1.274481044612177, -0.30645083457981553, -1.3285606156236818, 0.33473439037886943]]]
-[[[0.5269441534226782, 0.36498666932667356, 0.7363066388832684, 0.5878544826035406], [0.5684721009896431, 0.9009577979323332, 0.036288112799501615, 0.18351641818419884], [0.24258369409385339, 0.09354340906140202, 0.4856203412285762, 0.783031677244552]], [[0.8777465681935882, 0.6406910705155251, 0.10275292827025073, 0.01295823682977526], [0.3898500974345528, 0.6216248983423127, 0.3179425906177036, 0.012870877167621808], [0.2660481991211192, 0.09872041627158801, 0.3681944568198672, 0.494087114885137]]]
-[[[5, 9, 5, 6], [6, 7, 6, 1], [1, 3, 2, 4]], [[5, 8, 8, 3], [3, 2, 3, 9], [3, 0, 7, 1]]]
-[[[8.610851610963957, 1.3747433091161905, 1.3831050577679438, 4.715182178697273], [0.8765517657148284, 4.809554825684029, 2.7557819856736137, 5.938765584746821], [6.088739464744903, 4.627722536295625, 0.6116370455995369, 5.875683438664389]], [[7.7228845997304845, 5.428461366109726, 8.02712172516869, 5.9319006090345425], [5.726626482636939, 7.978329508380601, 1.114307478513796, 6.236721706167868], [1.4123245528031072, 5.327811122183013, 7.324213082306745, 1.5016363011868927]]]
+[[[1.524086835643172, -0.20868457467847845, 0.5240261503975477, -0.6439838767682032], [-1.091904210196648, -0.20567633973733265, 1.374424576574523, 0.6563097903476932], [0.2171635934136032, 1.0821030876490199, -0.8410496800310051, -0.8321549344577578]], [[0.5306996954571072, -0.4441704154154241, 1.0481960055260355, 0.39805451821848287], [-0.4006858882593715, -0.06238294764009237, -1.1536673264483728, -0.8063185246185602], [0.3029117113345387, -0.32570360518676644, 0.6608320231980702, 1.7415150171137153]]]
+[[[0.3736243541521843, 0.8599079983285199, 0.4260061864869946, 0.8441437619796597], [0.8955986631978392, 0.7570336992646656, 0.6706841989644684, 0.328634366074538], [0.4371430562585502, 0.9576395263025738, 0.2380278778546957, 0.806813631306664]], [[0.18549375381453237, 0.5749941389233029, 0.7009767023241946, 0.30017399397762223], [0.6661914823434657, 0.7802291606608635, 0.6847755352217044, 0.2661053533652564], [0.07937643994416943, 0.5452043474222034, 0.8026792060861194, 0.07776400257578953]]]
+[[[9, 0, 9, 0], [2, 6, 3, 4], [5, 8, 4, 7]], [[7, 7, 6, 3], [5, 5, 5, 8], [3, 4, 6, 6]]]
+[[[5.049093842782947, 1.3880585421884204, 8.533634113864629, 3.550264239771317], [3.3311351975225176, 5.131771033264564, 0.9570872044431911, 5.165536082759862], [1.2035779060925538, 8.292998518472567, 8.014641974770818, 6.251632912237915]], [[6.411677800595937, 5.365937405245105, 8.70943859614565, 4.348757668525482], [7.827612569569748, 1.3718742546020972, 0.5252489627763138, 2.065015517785291], [4.620664668451086, 2.604569735623819, 5.548107842615733, 7.60342292447815]]]
 
 >>> print(regression.linear_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.parabolic_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.polynomial_regression(list(range(5)), [2, 4, 6, 7, 8], 4))
 
 [1.5, 2.4000000000000004]
 [-0.21428571428571183, 2.3571428571428474, 1.9714285714285764]
```

### Comparing `PyPyNum-1.8.0/PyPyNum.egg-info/PKG-INFO` & `PyPyNum-1.8.1/PyPyNum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.8.0
+Version: 1.8.1
 Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
 Home-page: https://www.gitee.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -688,15 +688,15 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
@@ -737,98 +737,34 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增代码行数为603行
+eig函数修复了计算错误并改名为eigen
 
-Add 603 new lines of code
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增函数“magic_square”的功能简介：可
-以生成任意大于等于三的整数阶幻方。
-
-Introduction to the newly added
-function "magic square": It can
-generate any integer order magic
-square greater than or equal to
-three.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“Graph”的功能简介：具有有向图
-、无向图、带权有向图、带权无向图这四个对
-象，支持添加或删除顶点和边，以及深度优先
-搜索与广度优先搜索这两种图的遍历方式，还
-有计算最短路径等功能。
-
-Introduction to the functions of
-the newly added module "Graph":
-it has four objects: directed
-graph, undirected graph,
-weighted directed graph, and
-weighted undirected graph. It
-supports adding or removing
-vertices and edges, as well as
-depth first search and breadth
-first search for graph
-traversal. It also has functions
-such as calculating the shortest
-path.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“polynomial”的功能简介：有一
-个多项式对象，可以通过传入包含“(次数,
-系数)”的二元组组成的序列创建多项式对象
-，可以随时设置某一项的数值，并且支持多
-项式形式的四则运算，还有取商式、取余式
-、求幂、求模幂的功能。
-
-Introduction to the newly added
-module "polynomial": There is a
-polynomial object that can be
-created by passing in a sequence
-of binary tuples containing
-"degree, coefficient". The value
-of a certain term can be set at
-any time, and it supports
-polynomial form arithmetic
-operations. It also has
-functions such as quotient,
-remainder, exponentiation, and
-modular exponentiation.
+The eig function fixed
+calculation errors and changed
+its name to eigen
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
 <<<以下结构中的省略号表示原有的部分>>>
 
 <<<The ellipsis in the following structure represents the original part>>>
 
 PyPyNum
-    ★ Graph [Graph theory]
-        CLASSES
-            BaseGraph
-                BaseWeGraph
-                    WeDiGraph
-                    WeUnGraph
-                DiGraph
-                UnGraph
-    ★ polynomial [Polynomial object]
-        CLASSES
-            Polynomial
-        FUNCTIONS
-            poly(terms=None)
-    ★ tools [Other useful tools]
+    ★ Matrix [Matrix calculation]
         FUNCTIONS
             ...
-            magic_square(n)
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            ...
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -935,22 +871,24 @@
                     DFF
                     NOT
                     TFF
     ★ Matrix [Matrix calculation]
         CLASSES
             Matrix
         FUNCTIONS
-            eig(matrix)
-            identity(n)
-            lu(matrix)
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            identity(n: int) -> pypynum.Matrix.Matrix
+            lu(matrix: pypynum.Matrix.Matrix) -> tuple
             mat(data)
-            qr(matrix)
+            qr(matrix: pypynum.Matrix.Matrix) -> tuple
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
             same(rows, cols, value=0)
-            svd(matrix)
-            tril_indices(n, k=0, m=None)
+            svd(matrix: pypynum.Matrix.Matrix) -> tuple
+            tril_indices(n: int, k: int = 0, m: int = None) -> tuple
             zeros(_dimensions)
             zeros_like(_nested_list)
     ★ NeuralN [A simple neural network model]
         CLASSES
             NeuralNetwork
         FUNCTIONS
             neuraln(_input, _hidden, _output)
@@ -1126,14 +1064,17 @@
             totient(n: int) -> int
             mod_order(a: int, n: int, b: int) -> int
             primitive_root(a: int, single: bool = False) -> Union[int, list]
             normalize(data: arr, target: num = 1) -> arr
             average(data, weights, expected=False)
             exgcd(a: int, b: int) -> tuple
             crt(n: arr, a: arr) -> int
+            isqrt(x: int) -> int
+            is_possibly_square(n: int) -> bool
+            is_square(n: int) -> bool
     ★ numbers [Conversion of various numbers]
         FUNCTIONS
             float2fraction(number: float, mixed: bool = False, error: float = 1e-15) -> tuple
             int2roman(integer: int, overline: bool = True) -> str
             roman2int(roman_num: str) -> int
             str2int(string: str) -> int
         DATA
@@ -1355,29 +1296,31 @@
 >>> print(constants.tera)
 
 1099511627776
 2.718281828459045
 6.62607015e-34
 1.618033988749895
 3.141592653589793
-1000000000000.0
+1000000000000
 
 >>> p = [1, -2, -3, 4]
 >>> m = [
     [
         [1, 2, 3],
         [6, 10, 12],
         [7, 16, 9]
     ],
     [-1, -2, -3]
 ]
 >>> print(equations.polynomial_equation(p))
 >>> print(equations.linear_equation(*m))
 
-[(-1.5615528128088307-6.5209667308287455e-24j)   (2.5615528128088294+4.456233626665941e-24j)   (1.0000000000000007+3.241554513744382e-25j)]
+[[(-1.5615528128088307-6.5209667308287455e-24j)                                             0                                             0]
+ [                                            0   (2.5615528128088294+4.456233626665941e-24j)                                             0]
+ [                                            0                                             0   (1.0000000000000007+3.241554513744382e-25j)]]
 [ 1.6666666666666667 -0.6666666666666666 -0.4444444444444444]
 
 >>> print(maths.cot(constants.pi / 3))
 >>> print(maths.gamma(1.5))
 >>> print(maths.pi(1, 10, lambda x: x ** 2))
 >>> print(maths.product([2, 3, 5, 7, 11, 13, 17, 19, 23, 29]))
 >>> print(maths.sigma(1, 10, lambda x: x ** 2))
@@ -1464,18 +1407,18 @@
            -2.00e+00                            0.00e+00                            2.00e+00
 
 >>> print(random.gauss(0, 1, [2, 3, 4]))
 >>> print(random.rand([2, 3, 4]))
 >>> print(random.randint(0, 9, [2, 3, 4]))
 >>> print(random.uniform(0, 9, [2, 3, 4]))
 
-[[[0.4334341920363395, 0.055711784711422116, -1.0235500373980284, 0.30031229336738374], [-0.2650367914670356, 0.5513398538865067, -0.9735921328831166, 0.41345578602104827], [-0.11598957920080871, -0.9044539791933183, 1.6448227575237069, -0.26304156924843813]], [[0.27363898507271256, -0.5897181011789576, 1.5120937498473583, 2.1302709742844694], [1.9743293887616236, 0.4117207260898469, 0.5809554193110543, -1.8456249006764007], [1.274481044612177, -0.30645083457981553, -1.3285606156236818, 0.33473439037886943]]]
-[[[0.5269441534226782, 0.36498666932667356, 0.7363066388832684, 0.5878544826035406], [0.5684721009896431, 0.9009577979323332, 0.036288112799501615, 0.18351641818419884], [0.24258369409385339, 0.09354340906140202, 0.4856203412285762, 0.783031677244552]], [[0.8777465681935882, 0.6406910705155251, 0.10275292827025073, 0.01295823682977526], [0.3898500974345528, 0.6216248983423127, 0.3179425906177036, 0.012870877167621808], [0.2660481991211192, 0.09872041627158801, 0.3681944568198672, 0.494087114885137]]]
-[[[5, 9, 5, 6], [6, 7, 6, 1], [1, 3, 2, 4]], [[5, 8, 8, 3], [3, 2, 3, 9], [3, 0, 7, 1]]]
-[[[8.610851610963957, 1.3747433091161905, 1.3831050577679438, 4.715182178697273], [0.8765517657148284, 4.809554825684029, 2.7557819856736137, 5.938765584746821], [6.088739464744903, 4.627722536295625, 0.6116370455995369, 5.875683438664389]], [[7.7228845997304845, 5.428461366109726, 8.02712172516869, 5.9319006090345425], [5.726626482636939, 7.978329508380601, 1.114307478513796, 6.236721706167868], [1.4123245528031072, 5.327811122183013, 7.324213082306745, 1.5016363011868927]]]
+[[[1.524086835643172, -0.20868457467847845, 0.5240261503975477, -0.6439838767682032], [-1.091904210196648, -0.20567633973733265, 1.374424576574523, 0.6563097903476932], [0.2171635934136032, 1.0821030876490199, -0.8410496800310051, -0.8321549344577578]], [[0.5306996954571072, -0.4441704154154241, 1.0481960055260355, 0.39805451821848287], [-0.4006858882593715, -0.06238294764009237, -1.1536673264483728, -0.8063185246185602], [0.3029117113345387, -0.32570360518676644, 0.6608320231980702, 1.7415150171137153]]]
+[[[0.3736243541521843, 0.8599079983285199, 0.4260061864869946, 0.8441437619796597], [0.8955986631978392, 0.7570336992646656, 0.6706841989644684, 0.328634366074538], [0.4371430562585502, 0.9576395263025738, 0.2380278778546957, 0.806813631306664]], [[0.18549375381453237, 0.5749941389233029, 0.7009767023241946, 0.30017399397762223], [0.6661914823434657, 0.7802291606608635, 0.6847755352217044, 0.2661053533652564], [0.07937643994416943, 0.5452043474222034, 0.8026792060861194, 0.07776400257578953]]]
+[[[9, 0, 9, 0], [2, 6, 3, 4], [5, 8, 4, 7]], [[7, 7, 6, 3], [5, 5, 5, 8], [3, 4, 6, 6]]]
+[[[5.049093842782947, 1.3880585421884204, 8.533634113864629, 3.550264239771317], [3.3311351975225176, 5.131771033264564, 0.9570872044431911, 5.165536082759862], [1.2035779060925538, 8.292998518472567, 8.014641974770818, 6.251632912237915]], [[6.411677800595937, 5.365937405245105, 8.70943859614565, 4.348757668525482], [7.827612569569748, 1.3718742546020972, 0.5252489627763138, 2.065015517785291], [4.620664668451086, 2.604569735623819, 5.548107842615733, 7.60342292447815]]]
 
 >>> print(regression.linear_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.parabolic_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.polynomial_regression(list(range(5)), [2, 4, 6, 7, 8], 4))
 
 [1.5, 2.4000000000000004]
 [-0.21428571428571183, 2.3571428571428474, 1.9714285714285764]
```

### Comparing `PyPyNum-1.8.0/PyPyNum.egg-info/SOURCES.txt` & `PyPyNum-1.8.1/PyPyNum.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 pypynum/Quaternion.py
 pypynum/README.md
 pypynum/Symbolics.py
 pypynum/Tensor.py
 pypynum/Tree.py
 pypynum/Vector.py
 pypynum/__init__.py
-pypynum/__temporary.py
 pypynum/chars.py
 pypynum/cipher.py
 pypynum/constants.py
 pypynum/equations.py
 pypynum/errors.py
 pypynum/file.py
 pypynum/maths.py
```

### Comparing `PyPyNum-1.8.0/pypynum/Array.py` & `PyPyNum-1.8.1/pypynum/Array.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/FourierT.py` & `PyPyNum-1.8.1/pypynum/FourierT.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Geometry.py` & `PyPyNum-1.8.1/pypynum/Geometry.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Graph.py` & `PyPyNum-1.8.1/pypynum/Graph.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Group.py` & `PyPyNum-1.8.1/pypynum/Group.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Logic.py` & `PyPyNum-1.8.1/pypynum/Logic.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Matrix.py` & `PyPyNum-1.8.1/pypynum/Matrix.py`

 * *Files 26% similar despite different names*

```diff
@@ -213,46 +213,58 @@
     return Matrix(data)
 
 
 def same(rows, cols, value=0):
     return Matrix([[value] * cols for _ in range(rows)])
 
 
-def lu(matrix):
+def rotate90(matrix: Matrix, times: int) -> Matrix:
+    matrix = matrix.copy()
+    if times % 4 == 0:
+        return matrix
+    elif times % 4 == 1:
+        return Matrix([list(col)[::-1] for col in zip(*matrix)])
+    elif times % 4 == 2:
+        return Matrix([row[::-1] for row in matrix[::-1]])
+    else:
+        return Matrix([list(col)[::-1] for col in zip(*matrix[::-1])][::-1])
+
+
+def lu(matrix: Matrix) -> tuple:
     rows = matrix.rows
     cols = matrix.cols
     if rows != cols:
         raise SquareError
     L = [[1.0 if a == b else 0.0 for a in range(cols)] for b in range(rows)]
-    U = [[float(matrix.data[b][a]) for a in range(cols)] for b in range(rows)]
+    U = [[float(matrix[b][a]) for a in range(cols)] for b in range(rows)]
     for i in range(rows - 1):
         for j in range(i + 1, rows):
             L[j][i] = U[j][i] / U[i][i]
         for j in range(i + 1, rows):
             for k in range(i + 1, rows):
                 U[j][k] = U[j][k] - L[j][i] * U[i][k]
         for j in range(i + 1, rows):
             U[j][i] = 0
     return Matrix(L), Matrix(U)
 
 
-def tril_indices(n, k=0, m=None):
+def tril_indices(n: int, k: int = 0, m: int = None) -> tuple:
     if m is None:
         m = n
     if n < 1 or k <= -n or m < 1:
         return [], []
     _indices = [[x, y] for y in range(n) for x in range(y + k + 1) if x < m]
     return [y[1] for y in _indices], [x[0] for x in _indices]
 
 
-def identity(n):
+def identity(n: int) -> Matrix:
     return Matrix([[1.0 if a == b else 0.0 for a in range(n)] for b in range(n)])
 
 
-def qr(matrix):
+def qr(matrix: Matrix) -> tuple:
     from math import hypot
     r = matrix.rows
     c = matrix.cols
     Q = identity(r).data
     R = [[float(item) for item in line] for line in matrix.data]
     rows, cols = tril_indices(r, -1, c)
     for row, col in zip(rows, cols):
@@ -269,37 +281,229 @@
             Q = Matrix(Q)
             R = Matrix(R)
             Q = Q.inner(G).data
             R = (G @ R).data
     return Matrix([[item for item in line] for line in Q]), Matrix([[item for item in line] for line in R])
 
 
-def eig(matrix):
-    try:
-        from numpy.linalg import eig as eigen
-        e, Q = eigen(matrix.data)
-        e, Q = Matrix([e.tolist()]), Matrix(Q.tolist())
-        return e, Q
-    except ImportError:
-        eigen = "\n\033[91m提示：Matrix模块的eig函数可能存在计算错误\n\nTip: The eig function of the Matrix module may have calculation errors\033[m\n"
-        print(eigen)
-    _qr = []
-    n = matrix.rows
-    Q = identity(n)
-    for i in range(100):
-        _qr = qr(matrix)
-        Q = Q @ _qr[0]
-        matrix = _qr[1] @ _qr[0]
-    AK = (_qr[0] @ _qr[1]).data
-    e = Matrix([[AK[i][i] for i in range(n)]])
-    return e, Q
-
-
-def svd(matrix):
-    e0, U = eig(matrix @ matrix.t())
-    e1, V = eig(matrix.t() @ matrix)
-    sigma = Matrix([[((e0.data[0][a] + e1.data[0][a]) / 2) ** 0.5 if a == b else 0 for a in range(matrix.cols)]
-                    for b in range(matrix.rows)])
-    return U, sigma, V.t()
+def hessenberg(matrix: Matrix) -> tuple:
+    from math import sqrt
+    a = matrix.copy()
+    n = a.rows
+    t = [0.0] * n
+    a[-1, -1] = float(a[-1, -1])
+    if n > 2:
+        inf = float("inf")
+        for i in range(n - 1, 1, -1):
+            scale = 0.0
+            for k in range(0, i):
+                scale += abs(a[i, k].real) + abs(a[i, k].imag)
+            scale_inv = 0.0
+            if scale != 0:
+                scale_inv = 1 / scale
+            if scale == 0 or scale_inv == inf:
+                t[i] = 0.0
+                a[i, i - 1] = 0.0
+                continue
+            h = 0.0
+            for k in range(0, i):
+                a[i, k] = a[i, k] * scale_inv
+                rr, ii = a[i, k].real, a[i, k].imag
+                h += rr * rr + ii * ii
+            f = a[i, i - 1]
+            f0 = abs(f)
+            g = sqrt(h)
+            a[i, i - 1] = - g * scale
+            if f0 == 0:
+                t[i] = g
+            else:
+                ff = f / f0
+                t[i] = f + g * ff
+                a[i, i - 1] = a[i, i - 1] * ff
+            h += g * f0
+            h = 1 / sqrt(h)
+            t[i] *= h
+            for k in range(0, i - 1):
+                a[i, k] = a[i, k] * h
+            for j in range(0, i):
+                g = t[i].conjugate() * a[j, i - 1]
+                for k in range(0, i - 1):
+                    g += a[i, k].conjugate() * a[j, k]
+                a[j, i - 1] = a[j, i - 1] - g * t[i]
+                for k in range(0, i - 1):
+                    a[j, k] = a[j, k] - g * a[i, k]
+            for j in range(0, n):
+                g = t[i] * a[i - 1, j]
+                for k in range(0, i - 1):
+                    g += a[i, k] * a[k, j]
+                a[i - 1, j] = a[i - 1, j] - g * t[i].conjugate()
+                for k in range(0, i - 1):
+                    a[k, j] = a[k, j] - g * a[i, k].conjugate()
+    q = a.copy()
+    if n == 1:
+        q[0, 0] = 1.0
+        return q, a
+    q[0, 0] = q[1, 1] = 1.0
+    q[0, 1] = q[1, 0] = 0.0
+    for i in range(2, n):
+        if t[i] != 0:
+            for j in range(0, i):
+                g = t[i] * q[i - 1, j]
+                for k in range(0, i - 1):
+                    g += q[i, k] * q[k, j]
+                q[i - 1, j] -= g * t[i].conjugate()
+                for k in range(0, i - 1):
+                    q[k, j] -= g * a[i, k].conjugate()
+        q[i, i] = 1.0
+        for j in range(0, i):
+            q[j, i] = q[i, j] = 0.0
+    for x in range(n):
+        for y in range(x + 2, n):
+            a[y, x] = 0.0
+    return q, a
+
+
+def eigen(matrix: Matrix) -> tuple:
+    from math import hypot
+    from cmath import sqrt
+    a = matrix.copy()
+    n = a.rows
+    if n == 1:
+        return Matrix([[float(a[0, 0])]]), Matrix([[1.0]])
+    q, a = hessenberg(a)
+    norm = 0
+    for x in range(n):
+        for y in range(min(x + 2, n)):
+            norm += abs(a[y, x])
+    norm = norm ** 0.5 / n
+    if norm == 0:
+        return None, None
+    n0 = 0
+    n1 = n
+    its = 0
+    while True:
+        k = n0
+        while k + 1 < n1:
+            if abs(a[k + 1, k]) <= 1e-100:
+                break
+            k += 1
+        if k + 1 < n1:
+            a[k + 1, k] = 0.0
+            n0 = k + 1
+            its = 0
+            if n0 + 1 >= n1:
+                n0 = 0
+                n1 = k + 1
+                if n1 < 2:
+                    break
+        else:
+            if its % 30 == 10:
+                shift = a[n1 - 1, n1 - 2]
+            elif its % 30 == 20:
+                shift = abs(a[n1 - 1, n1 - 2])
+            elif its % 30 == 29:
+                shift = norm
+            else:
+                t = a[n1 - 2, n1 - 2] + a[n1 - 1, n1 - 1]
+                s = (a[n1 - 1, n1 - 1] - a[n1 - 2, n1 - 2]) ** 2 + 4 * a[n1 - 1, n1 - 2] * a[n1 - 2, n1 - 1]
+                if s.real > 0:
+                    s = sqrt(s)
+                else:
+                    s = sqrt(-s) * 1j
+                if s.imag == 0:
+                    s = s.real
+                a0 = (t + s) / 2
+                b0 = (t - s) / 2
+                if abs(a[n1 - 1, n1 - 1] - a0) > abs(a[n1 - 1, n1 - 1] - b0):
+                    shift = b0
+                else:
+                    shift = a0
+            its += 1
+            c = a[n0, n0] - shift
+            s = a[n0 + 1, n0]
+            v = hypot(abs(c), abs(s))
+            if v == 0:
+                c = 1
+                s = 0
+            else:
+                c /= v
+                s /= v
+            cc = c.conjugate()
+            cs = s.conjugate()
+            for k in range(n0, n):
+                x = a[n0, k]
+                y = a[n0 + 1, k]
+                a[n0, k] = cc * x + cs * y
+                a[n0 + 1, k] = c * y - s * x
+            for k in range(min(n1, n0 + 3)):
+                x = a[k, n0]
+                y = a[k, n0 + 1]
+                a[k, n0] = c * x + s * y
+                a[k, n0 + 1] = cc * y - cs * x
+            if not isinstance(q, bool):
+                for k in range(n):
+                    x = q[k, n0]
+                    y = q[k, n0 + 1]
+                    q[k, n0] = c * x + s * y
+                    q[k, n0 + 1] = cc * y - cs * x
+            for j in range(n0, n1 - 2):
+                c = a[j + 1, j]
+                s = a[j + 2, j]
+                v = hypot(abs(c), abs(s))
+                if v == 0:
+                    a[j + 1, j] = 0.0
+                    c = 1
+                    s = 0
+                else:
+                    a[j + 1, j] = v
+                    c /= v
+                    s /= v
+                a[j + 2, j] = 0.0
+                cc = c.conjugate()
+                cs = s.conjugate()
+                for k in range(j + 1, n):
+                    x = a[j + 1, k]
+                    y = a[j + 2, k]
+                    a[j + 1, k] = cc * x + cs * y
+                    a[j + 2, k] = c * y - s * x
+                for k in range(0, min(n1, j + 4)):
+                    x = a[k, j + 1]
+                    y = a[k, j + 2]
+                    a[k, j + 1] = c * x + s * y
+                    a[k, j + 2] = cc * y - cs * x
+                if not isinstance(q, bool):
+                    for k in range(0, n):
+                        x = q[k, j + 1]
+                        y = q[k, j + 2]
+                        q[k, j + 1] = c * x + s * y
+                        q[k, j + 2] = cc * y - cs * x
+    e = Matrix([[a[i, i] if j == i else 0 for j in range(n)] for i in range(n)])
+    er = identity(n)
+    m = 1
+    for i in range(1, n):
+        s = a[i, i]
+        for j in range(i - 1, -1, -1):
+            r = 0
+            for k in range(j + 1, i + 1):
+                r += a[j, k] * er[k, i]
+            t = a[j, j] - s
+            r = -r / t
+            er[j, i] = r
+            m = max(m, abs(r))
+        if m != 1:
+            for k in range(0, i + 1):
+                er[k, i] /= m
+    q = q @ er
+    return e, q
+
+
+def svd(matrix: Matrix) -> tuple:
+    print("\n警告：SVD函数可能存在计算错误\n\nWarning: The SVD function may have calculation errors\n")
+    e0, u = eigen(matrix @ matrix.t())
+    u = Matrix([_[::-1] for _ in u])
+    e1, v = eigen(matrix.t() @ matrix)
+    sigma = Matrix([[((e0[i, i] + e1[i, i]) / 2) ** 0.5 if j == i else 0 for j in range(matrix.cols - 1, -1, -1)]
+                    for i in range(matrix.rows - 1, -1, -1)])
+    return u, sigma, v.t()
 
 
 del Array
```

### Comparing `PyPyNum-1.8.0/pypynum/NeuralN.py` & `PyPyNum-1.8.1/pypynum/NeuralN.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/PyPyNum.png` & `PyPyNum-1.8.1/pypynum/PyPyNum.png`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Quaternion.py` & `PyPyNum-1.8.1/pypynum/Quaternion.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/README.md` & `PyPyNum-1.8.1/pypynum/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
@@ -63,98 +63,34 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增代码行数为603行
+eig函数修复了计算错误并改名为eigen
 
-Add 603 new lines of code
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增函数“magic_square”的功能简介：可
-以生成任意大于等于三的整数阶幻方。
-
-Introduction to the newly added
-function "magic square": It can
-generate any integer order magic
-square greater than or equal to
-three.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“Graph”的功能简介：具有有向图
-、无向图、带权有向图、带权无向图这四个对
-象，支持添加或删除顶点和边，以及深度优先
-搜索与广度优先搜索这两种图的遍历方式，还
-有计算最短路径等功能。
-
-Introduction to the functions of
-the newly added module "Graph":
-it has four objects: directed
-graph, undirected graph,
-weighted directed graph, and
-weighted undirected graph. It
-supports adding or removing
-vertices and edges, as well as
-depth first search and breadth
-first search for graph
-traversal. It also has functions
-such as calculating the shortest
-path.
-
-!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
-
-新增模块“polynomial”的功能简介：有一
-个多项式对象，可以通过传入包含“(次数,
-系数)”的二元组组成的序列创建多项式对象
-，可以随时设置某一项的数值，并且支持多
-项式形式的四则运算，还有取商式、取余式
-、求幂、求模幂的功能。
-
-Introduction to the newly added
-module "polynomial": There is a
-polynomial object that can be
-created by passing in a sequence
-of binary tuples containing
-"degree, coefficient". The value
-of a certain term can be set at
-any time, and it supports
-polynomial form arithmetic
-operations. It also has
-functions such as quotient,
-remainder, exponentiation, and
-modular exponentiation.
+The eig function fixed
+calculation errors and changed
+its name to eigen
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
 <<<以下结构中的省略号表示原有的部分>>>
 
 <<<The ellipsis in the following structure represents the original part>>>
 
 PyPyNum
-    ★ Graph [Graph theory]
-        CLASSES
-            BaseGraph
-                BaseWeGraph
-                    WeDiGraph
-                    WeUnGraph
-                DiGraph
-                UnGraph
-    ★ polynomial [Polynomial object]
-        CLASSES
-            Polynomial
-        FUNCTIONS
-            poly(terms=None)
-    ★ tools [Other useful tools]
+    ★ Matrix [Matrix calculation]
         FUNCTIONS
             ...
-            magic_square(n)
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            ...
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -261,22 +197,24 @@
                     DFF
                     NOT
                     TFF
     ★ Matrix [Matrix calculation]
         CLASSES
             Matrix
         FUNCTIONS
-            eig(matrix)
-            identity(n)
-            lu(matrix)
+            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
+            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
+            identity(n: int) -> pypynum.Matrix.Matrix
+            lu(matrix: pypynum.Matrix.Matrix) -> tuple
             mat(data)
-            qr(matrix)
+            qr(matrix: pypynum.Matrix.Matrix) -> tuple
+            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
             same(rows, cols, value=0)
-            svd(matrix)
-            tril_indices(n, k=0, m=None)
+            svd(matrix: pypynum.Matrix.Matrix) -> tuple
+            tril_indices(n: int, k: int = 0, m: int = None) -> tuple
             zeros(_dimensions)
             zeros_like(_nested_list)
     ★ NeuralN [A simple neural network model]
         CLASSES
             NeuralNetwork
         FUNCTIONS
             neuraln(_input, _hidden, _output)
@@ -452,14 +390,17 @@
             totient(n: int) -> int
             mod_order(a: int, n: int, b: int) -> int
             primitive_root(a: int, single: bool = False) -> Union[int, list]
             normalize(data: arr, target: num = 1) -> arr
             average(data, weights, expected=False)
             exgcd(a: int, b: int) -> tuple
             crt(n: arr, a: arr) -> int
+            isqrt(x: int) -> int
+            is_possibly_square(n: int) -> bool
+            is_square(n: int) -> bool
     ★ numbers [Conversion of various numbers]
         FUNCTIONS
             float2fraction(number: float, mixed: bool = False, error: float = 1e-15) -> tuple
             int2roman(integer: int, overline: bool = True) -> str
             roman2int(roman_num: str) -> int
             str2int(string: str) -> int
         DATA
@@ -681,29 +622,31 @@
 >>> print(constants.tera)
 
 1099511627776
 2.718281828459045
 6.62607015e-34
 1.618033988749895
 3.141592653589793
-1000000000000.0
+1000000000000
 
 >>> p = [1, -2, -3, 4]
 >>> m = [
     [
         [1, 2, 3],
         [6, 10, 12],
         [7, 16, 9]
     ],
     [-1, -2, -3]
 ]
 >>> print(equations.polynomial_equation(p))
 >>> print(equations.linear_equation(*m))
 
-[(-1.5615528128088307-6.5209667308287455e-24j)   (2.5615528128088294+4.456233626665941e-24j)   (1.0000000000000007+3.241554513744382e-25j)]
+[[(-1.5615528128088307-6.5209667308287455e-24j)                                             0                                             0]
+ [                                            0   (2.5615528128088294+4.456233626665941e-24j)                                             0]
+ [                                            0                                             0   (1.0000000000000007+3.241554513744382e-25j)]]
 [ 1.6666666666666667 -0.6666666666666666 -0.4444444444444444]
 
 >>> print(maths.cot(constants.pi / 3))
 >>> print(maths.gamma(1.5))
 >>> print(maths.pi(1, 10, lambda x: x ** 2))
 >>> print(maths.product([2, 3, 5, 7, 11, 13, 17, 19, 23, 29]))
 >>> print(maths.sigma(1, 10, lambda x: x ** 2))
@@ -790,18 +733,18 @@
            -2.00e+00                            0.00e+00                            2.00e+00
 
 >>> print(random.gauss(0, 1, [2, 3, 4]))
 >>> print(random.rand([2, 3, 4]))
 >>> print(random.randint(0, 9, [2, 3, 4]))
 >>> print(random.uniform(0, 9, [2, 3, 4]))
 
-[[[0.4334341920363395, 0.055711784711422116, -1.0235500373980284, 0.30031229336738374], [-0.2650367914670356, 0.5513398538865067, -0.9735921328831166, 0.41345578602104827], [-0.11598957920080871, -0.9044539791933183, 1.6448227575237069, -0.26304156924843813]], [[0.27363898507271256, -0.5897181011789576, 1.5120937498473583, 2.1302709742844694], [1.9743293887616236, 0.4117207260898469, 0.5809554193110543, -1.8456249006764007], [1.274481044612177, -0.30645083457981553, -1.3285606156236818, 0.33473439037886943]]]
-[[[0.5269441534226782, 0.36498666932667356, 0.7363066388832684, 0.5878544826035406], [0.5684721009896431, 0.9009577979323332, 0.036288112799501615, 0.18351641818419884], [0.24258369409385339, 0.09354340906140202, 0.4856203412285762, 0.783031677244552]], [[0.8777465681935882, 0.6406910705155251, 0.10275292827025073, 0.01295823682977526], [0.3898500974345528, 0.6216248983423127, 0.3179425906177036, 0.012870877167621808], [0.2660481991211192, 0.09872041627158801, 0.3681944568198672, 0.494087114885137]]]
-[[[5, 9, 5, 6], [6, 7, 6, 1], [1, 3, 2, 4]], [[5, 8, 8, 3], [3, 2, 3, 9], [3, 0, 7, 1]]]
-[[[8.610851610963957, 1.3747433091161905, 1.3831050577679438, 4.715182178697273], [0.8765517657148284, 4.809554825684029, 2.7557819856736137, 5.938765584746821], [6.088739464744903, 4.627722536295625, 0.6116370455995369, 5.875683438664389]], [[7.7228845997304845, 5.428461366109726, 8.02712172516869, 5.9319006090345425], [5.726626482636939, 7.978329508380601, 1.114307478513796, 6.236721706167868], [1.4123245528031072, 5.327811122183013, 7.324213082306745, 1.5016363011868927]]]
+[[[1.524086835643172, -0.20868457467847845, 0.5240261503975477, -0.6439838767682032], [-1.091904210196648, -0.20567633973733265, 1.374424576574523, 0.6563097903476932], [0.2171635934136032, 1.0821030876490199, -0.8410496800310051, -0.8321549344577578]], [[0.5306996954571072, -0.4441704154154241, 1.0481960055260355, 0.39805451821848287], [-0.4006858882593715, -0.06238294764009237, -1.1536673264483728, -0.8063185246185602], [0.3029117113345387, -0.32570360518676644, 0.6608320231980702, 1.7415150171137153]]]
+[[[0.3736243541521843, 0.8599079983285199, 0.4260061864869946, 0.8441437619796597], [0.8955986631978392, 0.7570336992646656, 0.6706841989644684, 0.328634366074538], [0.4371430562585502, 0.9576395263025738, 0.2380278778546957, 0.806813631306664]], [[0.18549375381453237, 0.5749941389233029, 0.7009767023241946, 0.30017399397762223], [0.6661914823434657, 0.7802291606608635, 0.6847755352217044, 0.2661053533652564], [0.07937643994416943, 0.5452043474222034, 0.8026792060861194, 0.07776400257578953]]]
+[[[9, 0, 9, 0], [2, 6, 3, 4], [5, 8, 4, 7]], [[7, 7, 6, 3], [5, 5, 5, 8], [3, 4, 6, 6]]]
+[[[5.049093842782947, 1.3880585421884204, 8.533634113864629, 3.550264239771317], [3.3311351975225176, 5.131771033264564, 0.9570872044431911, 5.165536082759862], [1.2035779060925538, 8.292998518472567, 8.014641974770818, 6.251632912237915]], [[6.411677800595937, 5.365937405245105, 8.70943859614565, 4.348757668525482], [7.827612569569748, 1.3718742546020972, 0.5252489627763138, 2.065015517785291], [4.620664668451086, 2.604569735623819, 5.548107842615733, 7.60342292447815]]]
 
 >>> print(regression.linear_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.parabolic_regression(list(range(5)), [2, 4, 6, 7, 8]))
 >>> print(regression.polynomial_regression(list(range(5)), [2, 4, 6, 7, 8], 4))
 
 [1.5, 2.4000000000000004]
 [-0.21428571428571183, 2.3571428571428474, 1.9714285714285764]
```

### Comparing `PyPyNum-1.8.0/pypynum/Symbolics.py` & `PyPyNum-1.8.1/pypynum/Symbolics.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Tensor.py` & `PyPyNum-1.8.1/pypynum/Tensor.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Tree.py` & `PyPyNum-1.8.1/pypynum/Tree.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/Vector.py` & `PyPyNum-1.8.1/pypynum/Vector.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/__init__.py` & `PyPyNum-1.8.1/pypynum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .file import read, write
 from .FourierT import *
 from .Geometry import *
 from .Graph import *
 from .Group import group
 from .Logic import *
 from .maths import *
-from .Matrix import mat, identity, lu, qr, eig, svd
+from .Matrix import mat, identity, rotate90, lu, qr, eigen, svd
 from .NeuralN import *
 from .numbers import *
 from .plotting import unary, binary, c_unary, color
 from .polynomial import *
 from .probability import *
 from .Quaternion import quat, euler
 from .random import *
@@ -35,11 +35,11 @@
 from .Tensor import ten, tensorproduct
 from .tools import *
 from .Tree import *
 from . import types
 from .utils import OrderedSet, InfIterator
 from .Vector import vec
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 print("PyPyNum", "Version -> " + __version__, "PyPI -> https://pypi.org/project/PyPyNum/",
       "Gitee -> https://www.gitee.com/PythonSJL/PyPyNum", sep=" | ")
 del math, arr, ite, num, real, geom, ContentError, RandomError, LogicError, InputError, FullError, Union
```

### Comparing `PyPyNum-1.8.0/pypynum/chars.py` & `PyPyNum-1.8.1/pypynum/chars.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/cipher.py` & `PyPyNum-1.8.1/pypynum/cipher.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/constants.py` & `PyPyNum-1.8.1/pypynum/constants.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/equations.py` & `PyPyNum-1.8.1/pypynum/equations.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,12 +6,11 @@
         return array([mat([left[_][:item] + [right[_]] + left[_][item + 1:] for _ in range(len(left))]).det() / d
                       for item in range(len(left))])
     return array([float("inf")] * len(right))
 
 
 def polynomial_equation(coefficients: list) -> list:
     from .Array import array
-    from .Matrix import mat
-    from .__temporary import eigenvalue as eig
+    from .Matrix import eigen, mat
     p = [_ / coefficients[0] for _ in coefficients[1:]]
-    return array(eig(mat([[-p[i] if j == 0 else 1 if i + 1 == j else 0
-                           for j in range(len(p))] for i in range(len(p))])))
+    return array(eigen(mat([[-p[i] if j == 0 else 1 if i + 1 == j else 0
+                           for j in range(len(p))] for i in range(len(p))]))[0].data)
```

### Comparing `PyPyNum-1.8.0/pypynum/file.py` & `PyPyNum-1.8.1/pypynum/file.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/maths.py` & `PyPyNum-1.8.1/pypynum/maths.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,22 @@
     72
     >>>
     :param args: integer
     :return:
     """
     if not args:
         return 0
+    try:
+        f = math.lcm
+    except AttributeError:
+        def f(a, b):
+            return a * b // math.gcd(a, b)
     lcm_value = args[0]
     for n in args[1:]:
-        lcm_value = math.lcm(lcm_value, n)
+        lcm_value = f(lcm_value, n)
     return lcm_value
 
 
 def sin(x: real) -> real:
     """
     Sine
     :param x: integer | float
```

### Comparing `PyPyNum-1.8.0/pypynum/numbers.py` & `PyPyNum-1.8.1/pypynum/numbers.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/plotting.py` & `PyPyNum-1.8.1/pypynum/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,15 @@
     :param string: bool.
     :param basic: list
     :param character: string
     :param data: bool.
     :param coloration: bool.
     :return:
     """
+    print("\n注意：自变量目前只支持实数范围\n\nNote: The independent variable currently only supports the real range\n")
     if abs(interval) != interval:
         raise ValueError("The interval cannot be less than zero")
     if not isinstance(character, str) or (len(character) != 1 and not coloration):
         raise ValueError("The parameter character must be one character")
     if projection == "ri":
         x = linspace(start, end, round((end - start) * interval + 1))
     else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyPyNum-1.8.0/pypynum/polynomial.py` & `PyPyNum-1.8.1/pypynum/polynomial.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/probability.py` & `PyPyNum-1.8.1/pypynum/probability.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/random.py` & `PyPyNum-1.8.1/pypynum/random.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/regression.py` & `PyPyNum-1.8.1/pypynum/regression.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/sequence.py` & `PyPyNum-1.8.1/pypynum/sequence.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/test.py` & `PyPyNum-1.8.1/pypynum/test.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/this.py` & `PyPyNum-1.8.1/pypynum/this.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/tools.py` & `PyPyNum-1.8.1/pypynum/tools.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/pypynum/utils.py` & `PyPyNum-1.8.1/pypynum/utils.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.0/setup.py` & `PyPyNum-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 ﻿from setuptools import setup, find_packages
 
 with open("pypynum/README.md", "r", encoding="UTF-8") as r:
     md = r.read()
 
 keywords = [
-    "math", "数学", "mathematics", "数学计算",
-    "numerical", "数值", "computation", "计算",
-    "scientific", "科学", "algebra", "代数",
-    "calculus", "微积分", "statistics", "统计",
-    "linear-algebra", "线性代数", "optimization", "优化",
-    "numerical-analysis", "数值分析", "matrix", "矩阵",
-    "vector", "向量", "tensor", "张量",
-    "numerics", "数值计算", "library", "库",
-    "tools", "工具", "utils", "实用程序",
-    "algorithms", "算法", "software", "软件",
-    "package", "包", "methods", "方法",
-    "data-science", "数据科学", "machine-learning", "机器学习",
-    "computational", "计算的", "operations", "操作",
-    "functions", "函数", "processing", "处理",
-    "programming", "编程", "simulation", "仿真",
-    "visualization", "可视化", "physics", "物理"
+    "math", "数学", "mathematics", "数学计算", "numerical", "数值", "computation", "计算",
+    "scientific", "科学", "algebra", "代数", "calculus", "微积分", "statistics", "统计",
+    "linear-algebra", "线性代数", "optimization", "优化", "numerical-analysis", "数值分析", "matrix", "矩阵",
+    "vector", "向量", "tensor", "张量", "numerics", "数值计算", "library", "库",
+    "tools", "工具", "utils", "实用程序", "algorithms", "算法", "software", "软件",
+    "package", "包", "methods", "方法", "data-science", "数据科学", "machine-learning", "机器学习",
+    "computational", "计算的", "operations", "操作", "functions", "函数", "processing", "处理",
+    "programming", "编程", "simulation", "仿真", "visualization", "可视化", "physics", "物理"
 ]
 
 LICENSE = """
                     GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -684,15 +676,15 @@
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <http://www.gnu.org/licenses/>.
 """
 
 setup(
     name="PyPyNum",
-    version="1.8.0",
+    version="1.8.1",
     packages=find_packages(),
     url="https://www.gitee.com/PythonSJL/PyPyNum",
     license=LICENSE,
     author="Shen Jiayi",
     author_email="2261748025@qq.com",
     description="""
     A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
```

