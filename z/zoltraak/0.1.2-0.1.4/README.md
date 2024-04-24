# Comparing `tmp/zoltraak-0.1.2.tar.gz` & `tmp/zoltraak-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoltraak-0.1.2.tar", last modified: Wed Apr 24 06:06:04 2024, max compression
+gzip compressed data, was "zoltraak-0.1.4.tar", last modified: Wed Apr 24 07:02:14 2024, max compression
```

## Comparing `zoltraak-0.1.2.tar` & `zoltraak-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.617213 zoltraak-0.1.2/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 06:06:04.617097 zoltraak-0.1.2/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.2/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 06:06:04.617254 zoltraak-0.1.2/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      282 2024-04-24 06:05:34.000000 zoltraak-0.1.2/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.616372 zoltraak-0.1.2/zoltraak/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.2/zoltraak/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5657 2024-04-24 06:02:47.000000 zoltraak-0.1.2/zoltraak/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.2/zoltraak/converter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    10551 2024-04-24 06:03:04.000000 zoltraak-0.1.2/zoltraak/md_generator.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 06:06:04.616967 zoltraak-0.1.2/zoltraak.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 06:06:04.000000 zoltraak-0.1.2/zoltraak.egg-info/top_level.txt
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:02:14.753098 zoltraak-0.1.4/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:02:14.752973 zoltraak-0.1.4/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.4/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 07:02:14.753134 zoltraak-0.1.4/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      435 2024-04-24 07:01:53.000000 zoltraak-0.1.4/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:02:14.752127 zoltraak-0.1.4/zoltraak/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.4/zoltraak/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5713 2024-04-24 06:17:03.000000 zoltraak-0.1.4/zoltraak/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.4/zoltraak/converter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    10617 2024-04-24 06:37:12.000000 zoltraak-0.1.4/zoltraak/md_generator.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:02:14.752808 zoltraak-0.1.4/zoltraak.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 07:02:14.000000 zoltraak-0.1.4/zoltraak.egg-info/top_level.txt
```

### Comparing `zoltraak-0.1.2/README.md` & `zoltraak-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.2/zoltraak/cli.py` & `zoltraak-0.1.4/zoltraak/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     if args.input.endswith(".md") or \
        os.path.isfile(args.input) or \
        os.path.isdir(args.input):                                          # 入力がマークダウンファイル、ファイルパス、またはディレクトリパスかどうかを判定
         print(args.input)
         md_file_path = os.path.join("requirements", os.path.basename(args.input))  # - 入力されたMarkdownファイルをrequirements/ディレクトリ内のパスに変更
         output_dir = os.path.abspath(args.output_dir)                      # - 出力ディレクトリの絶対パスを取得
         prompt = args.prompt                                               # - 追加のプロンプト情報を取得
+        print("momom")
+        print("prompt:", prompt)
         compiler_path = os.path.join("zoltraak/setting/compiler", args.compiler + ".md")    # 変更: コンパイラーのパスに.mdを追加
         formatter_path = os.path.join("zoltraak/setting/formatter", args.formatter + ".md")  # - フォーマッターのパスを設定
 
         print("compiler_path:", compiler_path)
         print("formatter_path:", formatter_path)
 
         md_file_rel_path = os.path.relpath(md_file_path, os.getcwd())      # - 現在のディレクトリからのMarkdownファイルの相対パスを取得
```

### Comparing `zoltraak-0.1.2/zoltraak/converter.py` & `zoltraak-0.1.4/zoltraak/converter.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.2/zoltraak/md_generator.py` & `zoltraak-0.1.4/zoltraak/md_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         developer (str): 使用するデベロッパー（デフォルトは "anthropic"）
         model_name (str): 使用するモデルの名前（デフォルトは "claude-3-opus-20240229"）
         compiler_path (str): コンパイラのパス（デフォルトはNone）
         formatter_path (str): フォーマッタのパス（デフォルトはNone）
         open_file (bool): ファイルを開くかどうかのフラグ（デフォルトはTrue）
     """
     prompt = create_prompt(goal_prompt, compiler_path, formatter_path)        # プロンプトを作成
+    print("goal_prompt", goal_prompt)
+    print("promtp", prompt)
     response = generate_response(                                             # developerごとの分岐を関数化して応答を生成
         developer, model_name, prompt                                         # - デベロッパー、モデル名、プロンプトを引数に渡す
     )                                                                         #
     md_content = response.strip()                                             # 生成された要件定義書の内容を取得し、前後の空白を削除
     save_md_content(md_content, target_file_path)                             # 生成された要件定義書の内容をファイルに保存
     print_generation_result(target_file_path, open_file)                      # 生成結果を出力し、open_fileフラグに応じてファイルを開く
```

