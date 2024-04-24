# Comparing `tmp/zoltraak-0.1.1.tar.gz` & `tmp/zoltraak-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoltraak-0.1.1.tar", last modified: Wed Apr 24 04:14:54 2024, max compression
+gzip compressed data, was "zoltraak-0.1.2.tar", last modified: Wed Apr 24 06:06:04 2024, max compression
```

## Comparing `zoltraak-0.1.1.tar` & `zoltraak-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.449837 zoltraak-0.1.1/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 04:14:54.449591 zoltraak-0.1.1/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.1/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 04:14:54.449884 zoltraak-0.1.1/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      282 2024-04-24 04:14:52.000000 zoltraak-0.1.1/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.448659 zoltraak-0.1.1/zoltraak/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.1/zoltraak/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5639 2024-04-24 03:06:10.000000 zoltraak-0.1.1/zoltraak/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.1/zoltraak/converter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    10542 2024-04-23 23:25:04.000000 zoltraak-0.1.1/zoltraak/md_generator.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.449383 zoltraak-0.1.1/zoltraak.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/top_level.txt
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.617213 zoltraak-0.1.2/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 06:06:04.617097 zoltraak-0.1.2/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.2/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 06:06:04.617254 zoltraak-0.1.2/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      282 2024-04-24 06:05:34.000000 zoltraak-0.1.2/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.616372 zoltraak-0.1.2/zoltraak/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.2/zoltraak/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5657 2024-04-24 06:02:47.000000 zoltraak-0.1.2/zoltraak/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.2/zoltraak/converter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    10551 2024-04-24 06:03:04.000000 zoltraak-0.1.2/zoltraak/md_generator.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.616967 zoltraak-0.1.2/zoltraak.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/top_level.txt
```

### Comparing `zoltraak-0.1.1/README.md` & `zoltraak-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.1/zoltraak/cli.py` & `zoltraak-0.1.2/zoltraak/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     if args.input.endswith(".md") or \
        os.path.isfile(args.input) or \
        os.path.isdir(args.input):                                          # 入力がマークダウンファイル、ファイルパス、またはディレクトリパスかどうかを判定
         print(args.input)
         md_file_path = os.path.join("requirements", os.path.basename(args.input))  # - 入力されたMarkdownファイルをrequirements/ディレクトリ内のパスに変更
         output_dir = os.path.abspath(args.output_dir)                      # - 出力ディレクトリの絶対パスを取得
         prompt = args.prompt                                               # - 追加のプロンプト情報を取得
-        compiler_path = os.path.join("setting/compiler", args.compiler + ".md")    # 変更: コンパイラーのパスに.mdを追加
-        formatter_path = os.path.join("setting/formatter", args.formatter + ".md")  # - フォーマッターのパスを設定
+        compiler_path = os.path.join("zoltraak/setting/compiler", args.compiler + ".md")    # 変更: コンパイラーのパスに.mdを追加
+        formatter_path = os.path.join("zoltraak/setting/formatter", args.formatter + ".md")  # - フォーマッターのパスを設定
 
         print("compiler_path:", compiler_path)
         print("formatter_path:", formatter_path)
 
         md_file_rel_path = os.path.relpath(md_file_path, os.getcwd())      # - 現在のディレクトリからのMarkdownファイルの相対パスを取得
         py_file_rel_path = os.path.splitext(md_file_rel_path)[0] + ".py"   # - Markdownファイルの拡張子を.pyに変更して、Pythonファイルの相対パスを作成
         py_file_path = os.path.join(output_dir, py_file_rel_path)          # - 出力ディレクトリとPythonファイルの相対パスを結合して、Pythonファイルの絶対パスを作成
```

### Comparing `zoltraak-0.1.1/zoltraak/converter.py` & `zoltraak-0.1.2/zoltraak/converter.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.1/zoltraak/md_generator.py` & `zoltraak-0.1.2/zoltraak/md_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 "content": prompt,
             }
         ],
         model=model,
     )
     return chat_completion.choices[0].message.content.strip()
 
-def create_prompt(goal_prompt, compiler_path="setting/compiler/dev_obj.md", formatter_path=None):
+def create_prompt(goal_prompt, compiler_path="zoltraak/setting/compiler/dev_obj.md", formatter_path=None):
     """
     LLMへのプロンプトを作成する関数
 
     Args:
         goal_prompt (str): 要件定義書の生成に使用するプロンプト
         compiler_path (str): コンパイラのパス
         formatter_path (str): フォーマッタのパス
```

