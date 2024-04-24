# Comparing `tmp/zoltraak-0.1.0.tar.gz` & `tmp/zoltraak-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoltraak-0.1.0.tar", last modified: Tue Apr 23 23:44:00 2024, max compression
+gzip compressed data, was "zoltraak-0.1.1.tar", last modified: Wed Apr 24 04:14:54 2024, max compression
```

## Comparing `zoltraak-0.1.0.tar` & `zoltraak-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-23 23:44:00.931647 zoltraak-0.1.0/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-23 23:44:00.931519 zoltraak-0.1.0/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    37231 2024-04-23 23:34:17.000000 zoltraak-0.1.0/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-23 23:44:00.931682 zoltraak-0.1.0/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      282 2024-04-21 17:03:12.000000 zoltraak-0.1.0/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-23 23:44:00.930542 zoltraak-0.1.0/zoltraak/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.0/zoltraak/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5631 2024-04-23 23:27:31.000000 zoltraak-0.1.0/zoltraak/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    17086 2024-04-23 23:07:24.000000 zoltraak-0.1.0/zoltraak/converter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    10542 2024-04-23 23:25:04.000000 zoltraak-0.1.0/zoltraak/md_generator.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-23 23:44:00.931361 zoltraak-0.1.0/zoltraak.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-23 23:44:00.000000 zoltraak-0.1.0/zoltraak.egg-info/top_level.txt
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.449837 zoltraak-0.1.1/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 04:14:54.449591 zoltraak-0.1.1/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.1/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 04:14:54.449884 zoltraak-0.1.1/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      282 2024-04-24 04:14:52.000000 zoltraak-0.1.1/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.448659 zoltraak-0.1.1/zoltraak/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.1/zoltraak/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5639 2024-04-24 03:06:10.000000 zoltraak-0.1.1/zoltraak/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.1/zoltraak/converter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    10542 2024-04-23 23:25:04.000000 zoltraak-0.1.1/zoltraak/md_generator.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 04:14:54.449383 zoltraak-0.1.1/zoltraak.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      296 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 04:14:54.000000 zoltraak-0.1.1/zoltraak.egg-info/top_level.txt
```

### Comparing `zoltraak-0.1.0/README.md` & `zoltraak-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -376,14 +376,32 @@
 
 
 
 
 
 ## TODO
 
+### 急ぎ
+
+- [ ] https://x.com/ai_syacho/status/1782956863912649114
+
+```
+ModuleNotFoundError系は
+pip install ~~~~
+で解決されます。
+
+今回は
+pip install anthropic
+を行うことで解決されます。
+
+↓
+pip install zoltraak
+一発で依存関係全て入る様に調整します。
+```
+
 ### CLIコマンド関連
 - [ ] zoltraak -p "manim動画を作りたい"  これで要件定義書とプログラムが生成
 
   - 
 
 ### ドキュメント生成
 - [ ] 出力されたPythonファイルと詳細設計書のドキュメントを欲しい。
@@ -416,14 +434,16 @@
 - [ ] 全て１から作り直す。mdファイルから
 ![image](assets/images//graph.png)
 
 
 
 
 
+
+
 ## プロンプトの分類
 
 プロンプトは以下の4つの分類に分けることができます。
 
 |       | 抽象的 | 具体的 |
 |-------|-------|--------|
 | 曖昧 | ① 初期プロンプト<br>例）ほにゃらしたい | ③ 試行錯誤段階<br>対話型（インタプリタ）|
@@ -763,7 +783,244 @@
 - `setup.py`ファイルには、適切なメタデータと依存関係を記述してください。
 - `README.md`ファイルには、パッケージの説明や使用方法を明確に記載してください。
 
 以上が、PyPIへのパッケージのアップロード手順です。問題がある場合は、PyPIのドキュメンテーションを参照するか、コミュニティに質問してください。
 
 
 
+
+## 仮想環境を用いて実行
+
+`pyenv` はPythonのバージョン管理ツールですが、直接的に仮想環境を作成する機能は持っていません。仮想環境を作成するためには、`pyenv-virtualenv` というプラグインを使用する必要があります。
+
+以下は `pyenv-virtualenv` を使用して仮想環境を作成する手順です。
+
+1. **pyenv-virtualenv のインストール**
+
+   まずは `pyenv-virtualenv` プラグインをインストールします。これは `pyenv` が既にインストールされていることを前提としています。
+
+   ```bash
+   git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
+   ```
+
+   インストール後、シェルの設定ファイル (例えば `.bashrc` や `.zshrc`) に以下を追加して、シェルを再起動します。
+
+   ```bash
+   eval "$(pyenv init --path)"
+   eval "$(pyenv virtualenv-init -)"
+   ```
+
+2. **Python のインストール**
+
+   `pyenv` を使用して、仮想環境用の Python バージョンをインストールします。
+
+   ```bash
+   pyenv install 3.8.5  # 例として Python 3.8.5 をインストール
+   ```
+
+3. **仮想環境の作成**
+
+   次に、指定した Python バージョンで仮想環境を作成します。
+
+   ```bash
+   pyenv virtualenv 3.8.5 my-virtual-env-3.8.5
+   ```
+
+   ここで `my-virtual-env-3.8.5` は仮想環境の名前です。
+
+4. **仮想環境のアクティベーション**
+
+   作成した仮想環境をアクティブにします。
+
+   ```bash
+   pyenv activate my-virtual-env-3.8.5
+   ```
+
+   これで、指定した仮想環境がアクティブになります。
+
+5. **仮想環境のデアクティベーション**
+
+   仮想環境をデアクティブにするには、以下のコマンドを使用します。
+
+   ```bash
+   pyenv deactivate
+   ```
+
+これで `pyenv` と `pyenv-virtualenv` を使用して Python の仮想環境を作成し、管理する方法を説明しました。
+
+
+### howto
+
+使い方
+1 .env ファイルにANTHROPIC_API_KEY={Anthropicのキー}
+2. pip install zoltraak
+3. zoltraak "最新の大規模言語モデルが学べるポケモンゲームの様なシステムを作りたい"
+
+これで、以下の様な要件定義書が出来ます。
+叩き台なので、適宜修正してください。
+
+-c 以降は用途に応じて変更できるプロンプトコンパイラになります。
+コンパイラ名: dev_func
+説明: 関数型プログラミングを用いた開発タスクに関する要件定義書を生成するコンパイラ
+
+コンパイラ名: dev_obj
+説明: オブジェクト指向設計を用いた開発タスクに関する要件定義書を生成するコンパイラ
+
+コンパイラ名: biz_consult
+説明: ビジネスコンサルティングに関するドキュメントを生成するコンパイラ
+
+コンパイラ名: general_def
+説明: 一般的な開発タスクに関する要件定義書を生成するコンパイラ
+
+コンパイラ名: general_reqdef
+説明: 一般的な要求事項に関する要件定義書を生成するコンパイラ
+
+具体例
+zoltraak "Manimを用いて、MoE（専門家の混合）モデルを視覚化するプログラムを開発する" -c dev_func
+zoltraak "今月中にオブジェクト指向設計を用いて、多機能在庫管理システムを開発する" -c dev_obj
+zoltraak "今月中に中小企業向けのビジネスコンサルティングドキュメントを作成する。具体的には、マーケティング戦略、財務管理、人材育成に関するアドバイスを含む" -c biz_consult
+zoltraak "今月中に教育用の拡張現実（AR）アプリケーションを開発する" -c general_def
+zoltraak "今月中に政府向けの少子化対策として、具体的な施策と予算案を含む提言書を執筆する" -c general_reqdef
+
+dev_func
+dev_obj
+biz_consult
+general_def
+general_reqdef
+
+
+
+
+## アーキ
+
+- compiler: 抽象文書を具体文書に変換するコンパイラ
+- archtecture: 
+  - 文書を構造体として骨組みを作る実行体
+  - 
+- execute: 
+
+
+
+```
+アーキテクチャ (Architecture) とデザイン (Design) という言葉の原義から、その意図を読み解いてみましょう。
+
+アーキテクチャ (Architecture):
+- 語源はギリシャ語の "arkhitekton" で、"chief builder" (主要な建設者) を意味します。
+- 建築の文脈では、建物の全体的な構造や様式を指します。
+- ITの文脈では、システムの全体的な構造や設計原則を意味します。
+- つまり、アーキテクチャは「全体を見渡し、大局的な設計を行う」という意図を持っています。
+
+デザイン (Design):
+- 語源はラテン語の "designare" で、"to mark out, devise, choose, designate, appoint" (印をつける、考案する、選ぶ、指定する、任命する) を意味します。
+- 一般的に、機能性と美的感覚を兼ね備えた設計を指します。
+- ITの文脈では、システムの詳細な設計や実装方法を意味します。
+- つまり、デザインは「具体的な設計を行い、機能性と美的感覚を追求する」という意図を持っています。
+
+これらの言葉の原義から、アーキテクチャは「大局的な視点」を、デザインは「詳細な視点」を重視していることがわかります。アーキテクチャは、システム全体の構造や設計原則を定義し、デザインはその原則に基づいて具体的な設計を行うという役割分担があると言えます。
+
+また、アーキテクチャが "chief builder" を意味することから、アーキテクトは技術的なリーダーシップを発揮し、プロジェクトの方向性を示す役割を担っていることがわかります。一方、デザインは "to mark out, devise" を意味することから、デザイナーは創造性を発揮し、機能性と美的感覚を兼ね備えた設計を行う役割を担っていると言えます。
+
+```
+
+
+
+
+
+
+# サードパーティ定義書
+- `Python開発者`= `{developer.dev_python}`
+- `JavaScript開発者` = `{developer.dev_javascript}`
+- `保険システムアーキテクト` = `{insurance_system_architect.architecture}`
+- `デザイナー` = `{designer.design}`
+- `保険ドメインエキスパート` = `{insurance_domain_expert.domain_knowledge}`
+- `アクチュアリー` = `{actuary.risk_analysis}`
+- `プロジェクトマネージャー` = `{project_manager.management}`
+- `品質保証エンジニア` = `{qa_engineer.quality_assurance}`
+- `セキュリティスペシャリスト` = `{security_specialist.security}`
+- `電話応対ロボット` = `{phone_robot.customer_service}`
+- `窓口応対ロボット` = `{counter_robot.customer_service}`
+
+# 自作定義書
+- `システム全体図` = `{insurance_system_architect.system_overview_diagram}`
+- `ユースケース図` = `{insurance_domain_expert.usecase_diagram}` 
+- `シーケンス図` = `{insurance_system_architect.sequence_diagram}`
+- `ER図` = `{insurance_domain_expert.er_diagram}`
+## 保険システム開発の仕様書
+
+### 目的
+本仕様書は、保険関係のシステム開発を行うにあたり、開発者、アーキテクト、デザイナー、ドメインエキスパート、アクチュアリー、プロジェクトマネージャー、品質保証エンジニア、セキュリティスペシャリスト、そしてカスタマーサービスロボットの役割と連携方法を明確にすることを目的とします。
+
+### 成果物
+- 業務要件定義書 (`保険ドメインエキスパート`・`アクチュアリー`)
+- システム設計書 (`保険システムアーキテクト`) 
+- ユーザーインターフェース設計書 (`デザイナー`)
+- ソースコード (開発者)
+  - `Python開発者`によるバックエンドシステム
+  - `JavaScript開発者`によるフロントエンドシステム
+- テスト仕様書・テスト結果報告書 (`品質保証エンジニア`) 
+- 脆弱性診断報告書・セキュリティテスト結果報告書 (`セキュリティスペシャリスト`)
+- プロジェクト計画書・進捗報告書 (`プロジェクトマネージャー`)
+- カスタマーサービスロボット仕様書 (`電話応対ロボット`・`窓口応対ロボット`)
+- ユーザーマニュアル (`デザイナー`・開発者)
+- `システム全体図`
+- `ユースケース図`
+- `シーケンス図`
+- `ER図`
+
+### 開発体制
+- 開発者 (Developer)
+  - Pythonによる開発を担当: `Python開発者`
+  - JavaScriptによる開発を担当: `JavaScript開発者` 
+- アーキテクト (Architect): `保険システムアーキテクト`
+  - システム全体のアーキテクチャ設計を担当
+  - 技術的なリーダーシップを発揮し、プロジェクトの方向性を示す
+- デザイナー (Designer): `デザイナー`
+  - ユーザーインターフェースのデザインを担当 
+  - 機能性と美的感覚を兼ね備えたデザインを追求する
+- 保険ドメインエキスパート: `保険ドメインエキスパート`
+  - 保険業務に関する専門知識を提供
+  - 業務要件の定義と確認を行う
+- アクチュアリー: `アクチュアリー`  
+  - 保険商品の設計と料率計算を担当
+  - リスク分析とモデリングを行う
+- プロジェクトマネージャー: `プロジェクトマネージャー`
+  - プロジェクト全体の管理と調整を行う
+  - スケジュール、コスト、品質、リスクを管理する
+- 品質保証エンジニア: `品質保証エンジニア` 
+  - テスト計画の作成とテストの実施を担当
+  - 品質基準の設定と品質管理を行う  
+- セキュリティスペシャリスト: `セキュリティスペシャリスト`
+  - セキュリティ要件の定義とセキュリティ設計を担当
+  - 脆弱性診断とセキュリティテストを実施する
+- カスタマーサービスロボット:
+  - 電話応対: `電話応対ロボット`
+  - 窓口応対: `窓口応対ロボット`
+
+### 開発プロセス 
+1. `保険ドメインエキスパート`と`アクチュアリー`が業務要件を定義する
+   - 保険商品の仕様と料率体系を決定する
+2. `保険システムアーキテクト`がシステム全体のアーキテクチャを設計する
+   - 設計原則を定義し、全体的な構造を決定する 
+   - `セキュリティスペシャリスト`と協力し、セキュリティ要件を組み込む
+3. `デザイナー`がユーザーインターフェースのデザインを行う
+   - `保険システムアーキテクト`の設計原則に基づき、具体的なデザインを作成する
+4. 開発者が`保険システムアーキテクト`の設計と`デザイナー`のデザインに基づいて開発を行う
+   - `Python開発者`は主にバックエンドの開発を担当
+   - `JavaScript開発者`はフロントエンドの開発を担当
+5. `品質保証エンジニア`がテスト計画を作成し、テストを実施する
+   - 単体テスト、結合テスト、システムテストを網羅的に行う
+6. `セキュリティスペシャリスト`が脆弱性診断とセキュリティテストを実施する
+   - 潜在的なセキュリティリスクを特定し、対策を講じる
+7. `プロジェクトマネージャー`が各工程の進捗を管理し、問題があれば適宜調整する
+   - スケジュール、コスト、品質、リスクを常にモニタリングする
+8. `電話応対ロボット`と`窓口応対ロボット`の動作を確認する
+   - カスタマーサービスの自動化部分をテストし、チューニングする
+9. 各工程で密な連携を取り、フィードバックを行う 
+   - 定期的なミーティングを開催し、進捗状況の共有と課題の解決を図る
+
+
+### 留意事項
+- 各工程でのコミュニケーションを密に取り、認識齟齬がないようにする
+- `保険ドメインエキスパート`と`アクチュアリー`の知見を活かし、業務要件を正しく理解する
+- `セキュリティスペシャリスト`の助言を得て、セキュリティとパフォーマンスに十分配慮し、堅牢で効率的なシステムを構築する
+- 変化する要件に柔軟に対応できるよう、保守性の高いコードを書く
+- `電話応対ロボット`と`窓口応対ロボット`の自然な対話を実現し、顧客満足度を高める
```

### Comparing `zoltraak-0.1.0/zoltraak/cli.py` & `zoltraak-0.1.1/zoltraak/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     parser = argparse.ArgumentParser(description="MarkdownファイルをPythonファイルに変換します")
     parser.add_argument("input", help="変換対象のMarkdownファイルのパスまたはテキスト", nargs='?')
     parser.add_argument("--output-dir", help="生成されたPythonファイルの出力ディレクトリ", default="generated")
     parser.add_argument("-p", "--prompt", help="追加のプロンプト情報", default=None)
     parser.add_argument("-c", "--compiler", help="コンパイラー（要件定義書のテンプレート）", default="dev_obj")
     # parser.add_argument("-i", "--interpreter", help="インタプリタータイプ定義書ののパス", default="general_def") TODO
 
-    parser.add_argument("-f", "--formatter", help="コードフォーマッター", default=None)
+    parser.add_argument("-f", "--formatter", help="コードフォーマッター", default="md_comment")
     args = parser.parse_args()
 
     if args.input is None:
         print("エラー: 入力ファイルまたはテキストが指定されていません。")
         print("使用方法: zoltraak <mdファイルのパス または テキスト> [オプション]")
         print("例1: zoltraak calc.md -p \"計算機を作りたい\" -c lisp")  # 変更: -c オプションの値から.mdを削除
         print("例2: zoltraak \"本書きたい\"  -c lisp")  # 変更: -c オプションの値から.mdを削除
```

### Comparing `zoltraak-0.1.0/zoltraak/converter.py` & `zoltraak-0.1.1/zoltraak/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,21 +293,21 @@
     # 現在のソースファイルを過去のソースファイルとして保存
     if past_source_file_path is not None:
         shutil.copy(source_file_path, past_source_file_path)
     
     # ソースファイルとLLMの説明文を読み込む
     with open(source_file_path, "r") as source_file:
         source_content = source_file.read()
-    with open("llms/claude.txt", "r") as f:
-        claude_code = f.read()
+    # with open("zoltraak/llms/claude.txt", "r") as f:
+    #     claude_code = f.read()
 
     # LLMへのプロンプトを作成
+    # 利用LLM: {claude_code}
     prompt = f'''
     pythonに変換すること
-    利用LLM: {claude_code}
     読み込みファイル: {source_content}
     要件書からターゲットファイルのコードのみ出力（コードブロックは記載しないこと）
     関数の1行説明はprintで
     実行するプログラムコードのみ記載
     説明等はコメントアウト
 
     if __name__ == "__main__":以降の
```

### Comparing `zoltraak-0.1.0/zoltraak/md_generator.py` & `zoltraak-0.1.1/zoltraak/md_generator.py`

 * *Files identical despite different names*

