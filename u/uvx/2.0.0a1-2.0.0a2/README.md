# Comparing `tmp/uvx-2.0.0a1.tar.gz` & `tmp/uvx-2.0.0a2.tar.gz`

## Comparing `uvx-2.0.0a1.tar` & `uvx-2.0.0a2.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 uvx-2.0.0a1/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a1/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a1/.gitignore
--rw-rw-r--   0     1000     1000    85890 2024-04-15 17:25:03.000000 uvx-2.0.0a1/Cargo.lock
--rw-rw-r--   0     1000     1000      137 2024-04-15 17:26:36.000000 uvx-2.0.0a1/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a1/rustfmt.toml
--rw-rw-r--   0     1000     1000     1852 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/animate.rs
--rw-rw-r--   0     1000     1000     6162 2024-04-15 17:06:13.000000 uvx-2.0.0a1/src/cli.rs
--rw-rw-r--   0     1000     1000     2262 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000      198 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5052 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2485 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/list.rs
--rw-rw-r--   0     1000     1000      214 2024-04-11 18:39:14.000000 uvx-2.0.0a1/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2205 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000      734 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000      207 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      643 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000      211 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     2033 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000     4066 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000      211 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      970 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/helpers.rs
--rw-rw-r--   0     1000     1000      565 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/main.rs
--rw-rw-r--   0     1000     1000     7641 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/metadata.rs
--rw-rw-r--   0     1000     1000     4637 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/pip.rs
--rw-rw-r--   0     1000     1000     3724 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/symlinks.rs
--rw-rw-r--   0     1000     1000     4776 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/uv.rs
--rw-rw-r--   0     1000     1000     2320 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/venv.rs
--rw-rw-r--   0     1000     1000      526 2024-04-15 17:21:16.000000 uvx-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 uvx-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 uvx-2.0.0a2/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a2/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a2/.gitignore
+-rw-rw-r--   0     1000     1000    86391 2024-04-24 20:04:01.000000 uvx-2.0.0a2/Cargo.lock
+-rwxrwxr-x   0     1000     1000      212 2024-04-24 20:04:30.000000 uvx-2.0.0a2/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a2/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1845 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/animate.rs
+-rw-rw-r--   0     1000     1000     9735 2024-04-24 16:11:41.000000 uvx-2.0.0a2/src/cli.rs
+-rw-rw-r--   0     1000     1000     2293 2024-04-24 20:02:25.000000 uvx-2.0.0a2/src/cmd.rs
+-rw-rw-r--   0     1000     1000      626 2024-04-15 19:40:37.000000 uvx-2.0.0a2/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2262 2024-04-15 19:25:25.000000 uvx-2.0.0a2/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1628 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5066 2024-04-24 15:17:01.000000 uvx-2.0.0a2/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2580 2024-04-24 14:39:09.000000 uvx-2.0.0a2/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.0a2/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2208 2024-04-24 14:44:18.000000 uvx-2.0.0a2/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1362 2024-04-24 14:46:35.000000 uvx-2.0.0a2/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4067 2024-04-24 15:57:47.000000 uvx-2.0.0a2/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      637 2024-04-24 18:48:16.000000 uvx-2.0.0a2/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1214 2024-04-24 16:19:16.000000 uvx-2.0.0a2/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      543 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     2913 2024-04-24 20:02:25.000000 uvx-2.0.0a2/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1642 2024-04-24 14:13:20.000000 uvx-2.0.0a2/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2029 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      964 2024-04-24 14:49:47.000000 uvx-2.0.0a2/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4059 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1037 2024-04-24 14:55:02.000000 uvx-2.0.0a2/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      970 2024-04-15 17:06:47.000000 uvx-2.0.0a2/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.0a2/src/main.rs
+-rw-rw-r--   0     1000     1000     7596 2024-04-24 16:23:50.000000 uvx-2.0.0a2/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4514 2024-04-24 20:02:25.000000 uvx-2.0.0a2/src/pip.rs
+-rw-rw-r--   0     1000     1000     3724 2024-04-15 17:06:47.000000 uvx-2.0.0a2/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3828 2024-04-24 20:02:25.000000 uvx-2.0.0a2/src/uv.rs
+-rw-rw-r--   0     1000     1000     2384 2024-04-24 15:55:23.000000 uvx-2.0.0a2/src/venv.rs
+-rw-rw-r--   0     1000     1000      410 2024-04-24 20:04:06.000000 uvx-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 uvx-2.0.0a2/PKG-INFO
```

### Comparing `uvx-2.0.0a1/.gitignore` & `uvx-2.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a1/Cargo.lock` & `uvx-2.0.0a2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -461,14 +461,23 @@
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
+name = "clap_complete"
+version = "4.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd79504325bf38b10165b02e89b4347300f855f273c4cb30c4a3209e6583275e"
+dependencies = [
+ "clap",
+]
+
+[[package]]
 name = "clap_derive"
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
@@ -2367,14 +2376,24 @@
 [[package]]
 name = "strsim"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
+name = "subprocess"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2e86926081dda636c546d8c5e641661049d7562a68f5488be4a1f7f66f6086"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -3065,30 +3084,33 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.0-alpha1"
+version = "2.0.0-alpha2"
 dependencies = [
  "anstyle",
  "async_http_range_reader",
  "chrono",
  "clap",
+ "clap_complete",
  "configparser",
  "directories",
  "home",
  "install-wheel-rs",
  "itertools",
  "owo-colors",
  "pep508_rs",
+ "regex",
  "rmp-serde",
  "serde",
  "serde_json",
+ "subprocess",
  "tempfile",
  "tokio",
  "uv-cache",
  "uv-installer",
  "uv-interpreter",
 ]
```

### Comparing `uvx-2.0.0a1/src/animate.rs` & `uvx-2.0.0a2/src/animate.rs`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,20 @@
             style: AnimationStyle::Modern,
             order: AnimationOrder::Before,
         };
     }
 }
 
 fn get_spinner_chars(style: &AnimationStyle) -> Vec<char> {
-    match style {
+    return match style {
         AnimationStyle::Classic => {
-            return vec!['|', '/', '-', '\\'];
+            vec!['|', '/', '-', '\\']
         },
-        AnimationStyle::Modern => return vec!['⣷', '⣯', '⣟', '⡿', '⢿', '⣻', '⣽', '⣾'],
-    }
+        AnimationStyle::Modern => vec!['⣷', '⣯', '⣟', '⡿', '⢿', '⣻', '⣽', '⣾'],
+    };
 }
 
 pub async fn animation(
     message: String,
     style: AnimationSettings,
 ) {
     let spinner_chars = get_spinner_chars(&style.style);
```

### Comparing `uvx-2.0.0a1/src/cli.rs` & `uvx-2.0.0a2/src/cli.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use clap::{Parser, Subcommand};
+use clap_complete::Shell;
 
 pub fn get_styles() -> clap::builder::Styles {
     clap::builder::Styles::styled()
         .usage(
             anstyle::Style::new()
                 .bold()
                 .underline()
@@ -41,14 +42,17 @@
 pub trait Process {
     async fn process(self) -> Result<i32, String>;
 }
 
 #[derive(Parser, Debug)]
 #[clap(version, styles=get_styles())]
 pub struct Args {
+    #[arg(long = "generate", value_enum)]
+    pub generator: Option<Shell>,
+
     #[clap(subcommand)]
     pub cmd: Commands,
 }
 
 // impl Args {
 //     pub fn parse_from_python() -> Args {
 //         return Args::parse_from(env::args().skip(1)); // first argument is now 'python' instead of 'uvx' so skip it
@@ -100,15 +104,25 @@
 
 #[derive(Debug, Parser)]
 pub struct UninstallOptions {
     pub package_name: String,
     #[clap(
         short = 'f',
         long,
-        help = "Remove executable with the same name (in ~/.local/bin) even if related venv was not found"
+        help = "Remove executable with the same name (in ~/.local/bin) even if related venv was not found."
+    )]
+    pub force: bool,
+}
+
+#[derive(Debug, Parser)]
+pub struct UninstallAllOptions {
+    #[clap(
+        short = 'f',
+        long,
+        help = "Remove executable with the same name (in ~/.local/bin) even if related venv was not found."
     )]
     pub force: bool,
 }
 
 #[derive(Debug, Parser)]
 pub struct ReinstallOptions {
     pub package: String,
@@ -124,21 +138,55 @@
     #[clap(long, help = "Run without `uv` cache")]
     pub no_cache: bool,
     #[clap(long, short, help = "(Re)install as editable")]
     pub editable: bool,
 }
 
 #[derive(Debug, Parser)]
+pub struct ReinstallAllOptions {
+    #[clap(long, help = PYTHON_HELP_TEXT)]
+    pub python: Option<String>,
+    #[clap(short = 'f', long, help = "See `install --force`")]
+    pub force: bool,
+    #[clap(
+        long,
+        help = "Don't include previously injected libraries in reinstall"
+    )]
+    pub without_injected: bool,
+    #[clap(long, help = "Run without `uv` cache")]
+    pub no_cache: bool,
+    #[clap(long, short, help = "(Re)install as editable")]
+    pub editable: bool,
+}
+
+#[derive(Debug, Parser)]
 pub struct UpgradeAllOptions {
     #[clap(short = 'f', long, help = "Ignore previous version constraint")]
-    force: bool,
+    pub force: bool,
     #[clap(long, help = "Don't also upgrade injected packages")]
-    skip_injected: bool,
+    pub skip_injected: bool,
     #[clap(long, help = "Run without `uv` cache")]
-    no_cache: bool,
+    pub no_cache: bool,
+}
+
+#[derive(Debug, Parser)]
+pub struct RunOptions {
+    pub package_name: String,
+    #[clap(long, help = "Run without `uv` cache")]
+    pub no_cache: bool,
+    #[clap(long, help = PYTHON_HELP_TEXT)]
+    pub python: Option<String>,
+    #[clap(long, help = "Don't remove the temporary venv when done running")]
+    pub keep: bool,
+    #[clap(
+        long,
+        help = "Custom name of an executable to run (e.g. 'semantic-release' in the package 'python-semantic-release')"
+    )]
+    pub binary: Option<String>,
+    pub args: Vec<String>,
 }
 
 #[derive(Debug, Parser)]
 pub struct RunuvOptions {
     pub venv: String,
     pub uv_args: Vec<String>,
 }
@@ -159,37 +207,78 @@
 pub struct EnsurepathOptions {
     #[clap(long, short, help = "Force update")]
     pub force: bool,
 }
 
 #[derive(Debug, Parser)]
 pub struct SelfUpdateOptions {
-    #[clap(long, help = "Update with uv")]
-    with_uv: Option<bool>,
+    #[clap(long, help = "Update without also updating uv")]
+    pub without_uv: bool,
 }
 
 #[derive(Debug, Parser)]
 pub struct InjectOptions {
-    into: String,
-    package_specs: Vec<String>,
+    pub into: String,
+    pub package_specs: Vec<String>,
+
+    #[clap(long, help = "Run without `uv` cache")]
+    pub no_cache: bool,
+}
+#[derive(Debug, Parser)]
+pub struct UnInjectOptions {
+    pub outof: String,
+    pub package_specs: Vec<String>,
+}
+
+#[derive(Debug, Parser)]
+pub struct CompletionsOptions {
+    #[clap(long, short, help = "Add to ~/.bashrc")]
+    pub install: bool,
+    // todo: support others than bash
 }
 
 #[derive(Subcommand, Debug)]
 pub enum Commands {
+    #[clap(about = "Use --install to install the autocomplete script (bash).")]
+    Completions(CompletionsOptions),
+    #[clap(about = "List packages and apps installed with uvx.")]
     List(ListOptions),
+    #[clap(about = "Install a package (by pip name).")]
     Install(InstallOptions),
+    #[clap(about = "Upgrade a package.")]
     Upgrade(UpgradeOptions),
+    #[clap(about = "Upgrade all uvx-installed packages.")]
+    UpgradeAll(UpgradeAllOptions),
+    #[clap(about = "Uninstall a package (by pip name).")]
     Uninstall(UninstallOptions),
+    #[clap(about = "Uninstall all uvx-installed packages.")]
+    UninstallAll(UninstallAllOptions),
+    #[clap(
+        about = "Uninstall a package (by pip name) and re-install from the original spec (unless a new spec is supplied)."
+    )]
     Reinstall(ReinstallOptions),
+    #[clap(about = "Reinstall all uvx-installed packages.")]
+    ReinstallAll(ReinstallAllOptions),
+    #[clap(about = "Install additional packages to a virtual environment managed by uvx.")]
     Inject(InjectOptions),
-    UpgradeAll(UpgradeAllOptions),
+    #[clap(aliases = &["eject"], about="Uninstall additional packages from a virtual environment managed by uvx. (alias: `eject`)")]
+    Uninject(UnInjectOptions),
+    #[clap(about = "Run a package in a temporary virtual environment.")]
+    Run(RunOptions),
+    #[clap(about = "Run 'uv' in the right venv.")]
     Runuv(RunuvOptions),
+    #[clap(about = "Run 'pip' in the right venv.")]
     Runpip(RunpipOptions),
+    #[clap(about = "Run 'python' in the right venv.")]
     Runpython(RunpythonOptions),
+    #[clap(
+        about = "Update ~/.bashrc with a PATH that includes the local bin directory that uvx uses."
+    )]
     Ensurepath(EnsurepathOptions),
+    #[clap(about = "Update the current installation of uvx (and optionally uv).")]
     SelfUpdate(SelfUpdateOptions),
 }
 
 impl Process for Commands {
     async fn process(self) -> Result<i32, String> {
         return match self {
             Commands::List(opts) => opts.process().await,
@@ -200,10 +289,15 @@
             Commands::Inject(opts) => opts.process().await,
             Commands::UpgradeAll(opts) => opts.process().await,
             Commands::Runuv(opts) => opts.process().await,
             Commands::Runpip(opts) => opts.process().await,
             Commands::Runpython(opts) => opts.process().await,
             Commands::Ensurepath(opts) => opts.process().await,
             Commands::SelfUpdate(opts) => opts.process().await,
+            Commands::UninstallAll(opts) => opts.process().await,
+            Commands::ReinstallAll(opts) => opts.process().await,
+            Commands::Uninject(opts) => opts.process().await,
+            Commands::Completions(opts) => opts.process().await,
+            Commands::Run(opts) => opts.process().await,
         };
     }
 }
```

### Comparing `uvx-2.0.0a1/src/commands/ensurepath.rs` & `uvx-2.0.0a2/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a1/src/commands/install.rs` & `uvx-2.0.0a2/src/commands/install.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use pep508_rs::Requirement;
 use std::collections::HashMap;
 
 use std::path::{Path, PathBuf};
 
 use uv_interpreter::PythonEnvironment;
 
-async fn _install_package(
+pub async fn _install_package(
     package_name: &str,
     inject: &Vec<&str>,
     no_cache: bool,
     force: bool,
     editable: bool,
 ) -> Result<bool, String> {
     let mut args: Vec<&str> = vec!["pip", "install"];
@@ -47,29 +47,29 @@
     )
     .await;
 }
 
 async fn ensure_venv(
     maybe_venv: Option<&Path>,
     requirement: &Requirement,
-    python: Option<String>,
+    python: Option<&String>,
     force: bool,
 ) -> Result<PathBuf, String> {
     match maybe_venv {
         Some(venv) => {
             let buf = venv.to_path_buf();
             if !buf.exists() {
                 Err(String::from(
                     "Package could not be installed because supplied venv was misssing.",
                 ))
             } else {
                 Ok(buf)
             }
         },
-        None => create_venv(&requirement.name, python, force, true).await,
+        None => create_venv(&requirement.name, python, force, true, None).await,
     }
 }
 
 async fn store_metadata(
     requirement_name: &str,
     requirement: &Requirement,
     inject: &Vec<&str>,
@@ -129,15 +129,15 @@
 
     Ok(())
 }
 
 pub async fn install_package(
     install_spec: &str,
     maybe_venv: Option<&Path>,
-    python: Option<String>,
+    python: Option<&String>,
     force: bool,
     inject: Vec<&str>,
     no_cache: bool,
     editable: bool,
 ) -> Result<String, String> {
     let (requirement, resolved_install_spec) = parse_requirement(install_spec).await?;
 
@@ -168,26 +168,26 @@
         requirement_name,
         metadata.installed_version.cyan()
     )) // :package:
 }
 
 impl Process for InstallOptions {
     async fn process(self) -> Result<i32, String> {
-        match install_package(
+        return match install_package(
             &self.package_name,
             None,
-            self.python,
+            self.python.as_ref(),
             self.force,
             vec![],
             self.no_cache,
             self.editable,
         )
         .await
         {
             Ok(msg) => {
                 println!("{}", msg);
-                return Ok(0);
+                Ok(0)
             },
-            Err(msg) => return Err(msg),
-        }
+            Err(msg) => Err(msg),
+        };
     }
 }
```

### Comparing `uvx-2.0.0a1/src/commands/list.rs` & `uvx-2.0.0a2/src/commands/list.rs`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,33 @@
 
         println!("{}", json);
 
         Ok(0)
     }
 }
 
-impl Process for ListOptions {
-    async fn process(self) -> Result<i32, String> {
-        let venv_dir_path = get_venv_dir();
-        let possibly_missing = std::fs::read_dir(&venv_dir_path);
+pub async fn list_packages() -> Result<Vec<Metadata>, String> {
+    let venv_dir_path = get_venv_dir();
+    let possibly_missing = std::fs::read_dir(&venv_dir_path);
+
+    let must_exist = match possibly_missing {
+        Ok(dir) => dir,
+        Err(_) => {
+            std::fs::create_dir_all(&venv_dir_path).map_err_to_string()?;
+            std::fs::read_dir(&venv_dir_path).map_err_to_string()?
+        },
+    };
 
-        let must_exist = match possibly_missing {
-            Ok(dir) => dir,
-            Err(_) => {
-                std::fs::create_dir_all(&venv_dir_path).map_err_to_string()?;
-                std::fs::read_dir(&venv_dir_path).map_err_to_string()?
-            },
-        };
+    let result = read_from_folder(must_exist).await;
+    return Ok(result);
+}
 
-        let all_items = read_from_folder(must_exist).await;
+impl Process for ListOptions {
+    async fn process(self) -> Result<i32, String> {
+        let all_items = list_packages().await?;
 
         let filtered_items: Vec<&Metadata> = if self.venv_names.len() > 0 {
             // add filter
             all_items
                 .iter()
                 .filter(|k| self.venv_names.contains(&k.name))
                 .collect()
```

### Comparing `uvx-2.0.0a1/src/commands/reinstall.rs` & `uvx-2.0.0a2/src/commands/reinstall.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     metadata::{venv_path, Metadata},
     pip::parse_requirement,
     uv::ExtractInfo,
 };
 
 pub async fn reinstall(
     install_spec: &str,
-    python: Option<String>,
+    python: Option<&String>,
     force: bool,
     with_injected: bool,
     no_cache: bool,
     editable: bool,
 ) -> Result<String, String> {
     let (requirement, _resolved_install_spec) = parse_requirement(install_spec).await?;
     let requirement_name = requirement.name.to_string();
@@ -65,25 +65,25 @@
         editable,
     )
     .await;
 }
 
 impl Process for ReinstallOptions {
     async fn process(self) -> Result<i32, String> {
-        match reinstall(
+        return match reinstall(
             &self.package,
-            self.python,
+            self.python.as_ref(),
             self.force,
             !self.without_injected,
             self.no_cache,
             self.editable,
         )
         .await
         {
             Ok(msg) => {
                 println!("{}", msg);
-                return Ok(0);
+                Ok(0)
             },
-            Err(msg) => return Err(msg),
-        }
+            Err(msg) => Err(msg),
+        };
     }
 }
```

### Comparing `uvx-2.0.0a1/src/commands/uninstall.rs` & `uvx-2.0.0a2/src/commands/uninstall.rs`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 ) -> Result<String, String> {
     let (requirement, _) = parse_requirement(package_name).await?;
     let requirement_name = requirement.name.to_string();
 
     let venv_dir = venv_path(&requirement_name);
 
     if !venv_dir.exists() {
-        if !force {
-            return Err(format!("No virtualenv for '{}', stopping.\nUse '{}' to remove an executable with that name anyway.", 
-            &requirement_name.green(), "--force".green()));
+        return if !force {
+            Err(format!("No virtualenv for '{}', stopping.\nUse '{}' to remove an executable with that name anyway.",
+                        &requirement_name.green(), "--force".green()))
         } else {
             remove_symlink(&requirement_name).await?;
-            return Err(format!(
+            Err(format!(
                 "{}: No virtualenv for '{}'.",
                 "Warning".yellow(),
                 &requirement_name.green()
-            ));
-        }
+            ))
+        };
     }
 
     let venv = activate_venv(&venv_dir).await?;
 
     let metadata = Metadata::for_requirement(&requirement, false).await;
 
     // symlinks = find_symlinks(package_name, venv_path) or [package_name]
@@ -50,16 +50,16 @@
     let msg = format!("🗑️  {}{} removed!", package_name, version_msg);
 
     return Ok(msg);
 }
 
 impl Process for UninstallOptions {
     async fn process(self) -> Result<i32, String> {
-        match uninstall_package(&self.package_name, self.force).await {
+        return match uninstall_package(&self.package_name, self.force).await {
             Ok(msg) => {
                 println!("{}", msg);
-                return Ok(0);
+                Ok(0)
             },
-            Err(msg) => return Err(msg),
-        }
+            Err(msg) => Err(msg),
+        };
     }
 }
```

### Comparing `uvx-2.0.0a1/src/commands/upgrade.rs` & `uvx-2.0.0a2/src/commands/upgrade.rs`

 * *Files 1% similar despite different names*

```diff
@@ -133,23 +133,23 @@
         skip_injected,
     )
     .await;
 }
 
 impl Process for UpgradeOptions {
     async fn process(self) -> Result<i32, String> {
-        match upgrade_package(
+        return match upgrade_package(
             &self.package_name,
             self.force,
             self.no_cache,
             self.skip_injected,
         )
         .await
         {
             Ok(msg) => {
                 println!("{}", msg);
-                return Ok(0);
+                Ok(0)
             },
-            Err(msg) => return Err(msg),
-        }
+            Err(msg) => Err(msg),
+        };
     }
 }
```

### Comparing `uvx-2.0.0a1/src/helpers.rs` & `uvx-2.0.0a2/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a1/src/metadata.rs` & `uvx-2.0.0a2/src/metadata.rs`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         self.injected
             .iter()
             .map(|k| format!("'{}'", k.green()))
             .join(", ")
     }
 
     pub fn format_human(&self) -> String {
-        let mut result = format!("- {}", self.name); // todo: colorized extra's (+ install spec?)
+        let mut result = format!("- {}", self.name);
 
         if self.extras.len() > 0 {
             result.push_str(&format!("[{}]", self.format_extras()));
         }
 
         if self.requested_version.len() > 0 {
             result.push_str(&format!(" {}", self.requested_version.cyan()));
```

### Comparing `uvx-2.0.0a1/src/pip.rs` & `uvx-2.0.0a2/src/pip.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+use std::path::PathBuf;
 use std::str::FromStr;
 
 use pep508_rs::Requirement;
+use serde::{Deserialize, Serialize};
 use tempfile::NamedTempFile;
-use tokio::process::Command;
 
+use crate::cmd::{run, run_get_output};
 use crate::{
     animate::{show_loading_indicator, AnimationSettings},
     helpers::ResultToString,
 };
-use serde::{Deserialize, Serialize};
 
 #[derive(Debug, Serialize, Deserialize)]
 struct PipDownloadInfo {
     url: String,
     dir_info: serde_json::Value, // Since dir_info is an empty object, we can use serde_json::Value here
 }
 
@@ -58,26 +59,15 @@
     install: Vec<PipInstallItem>,
     // environment: Environment,
 }
 
 pub async fn pip(args: Vec<&str>) -> Result<bool, String> {
     let err_prefix = format!("pip {}", &args[0]);
 
-    let result = Command::new("pip").args(args).output().await;
-
-    match result {
-        Ok(result) => match result.status.code() {
-            Some(0) => Ok(true),
-            Some(_) | None => {
-                let err = String::from_utf8(result.stderr).unwrap_or_default();
-                Err(format!("{} | {}", err_prefix, err))
-            },
-        },
-        Err(result) => Err(format!("{} | {}", err_prefix, result.to_string())),
-    }
+    return run("pip", args, Some(err_prefix)).await;
 }
 
 #[derive(Debug)]
 pub struct FakeInstallResult {
     pub name: String,
     pub file_url: String,
 }
@@ -161,7 +151,12 @@
 
 pub async fn parse_requirement(install_spec: &str) -> Result<(Requirement, String), String> {
     match Requirement::from_str(install_spec) {
         Ok(requirement) => Ok((requirement, String::from(install_spec))),
         Err(_) => try_parse_local_requirement(install_spec).await,
     }
 }
+
+pub async fn pip_freeze(python: &PathBuf) -> Result<String, String> {
+    // let py = python.to_str().unwrap_or_default(); // idk why python.to_string() doesn't work
+    return run_get_output(python, vec!["-m", "pip", "freeze"]).await;
+}
```

### Comparing `uvx-2.0.0a1/src/symlinks.rs` & `uvx-2.0.0a2/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a1/src/uv.rs` & `uvx-2.0.0a2/src/uv.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,63 @@
+use std::ffi::OsStr;
+use std::{collections::HashSet, path::PathBuf};
+
+use crate::cmd::{find_sibling, run, run_print_output};
 use directories::ProjectDirs;
 use owo_colors::OwoColorize;
 use pep508_rs::{PackageName, Requirement};
-use std::env::{self};
-use std::str::FromStr;
-use std::{ffi::OsStr, process::Stdio};
-use tokio::fs::canonicalize;
-
-use std::{collections::HashSet, path::PathBuf};
-use tokio::process::Command;
-
 use uv_cache::Cache;
 use uv_installer::SitePackages;
 use uv_interpreter::PythonEnvironment;
 
-use crate::helpers::{PathToString, ResultToString};
+use crate::helpers::PathToString;
 
 pub async fn _get_uv_binary() -> Option<String> {
     // if bundled with entrypoint:
     // arg 0 = python
-    // arg 1 = .../bin/uvx (arg 0 otherwise)
-
-    let Some(binary) = env::args().nth(0) else {
-        return None;
-    };
-
-    let Ok(binary_path) = PathBuf::from_str(&binary) else {
-        return None;
-    };
-
-    let Ok(real_path) = canonicalize(&binary_path).await else {
-        return None;
-    };
+    // arg 1 = .../bin/uvx
+    // elif bundled as bin, use current_exe (because arg 0 is just 'uvx' instead of a path):
 
-    let Some(parent) = real_path.parent() else {
-        return None;
-    };
+    // let Some(binary) = env::args().nth(0) else {
+    //     return None;
+    // };
+    // let Ok(binary_path) = PathBuf::from_str(&binary) else {
+    //     return None;
+    // };
 
-    // resolve symlinks etc:
-
-    let uv_binary = parent.join("uv").to_string();
-
-    Some(uv_binary)
+    return find_sibling("uv").await.map(|buf| buf.to_string());
 }
 
 pub async fn get_uv_binary() -> String {
-    match _get_uv_binary().await {
-        Some(bin) => bin,
-        None => String::from("uv"), // fallback, hope 'uv' is available in global scope
-    }
+    _get_uv_binary().await.unwrap_or_else(
+        // fallback, hope 'uv' is available in global scope:
+        || String::from("uv"),
+    )
 }
 
 pub async fn uv<S>(args: Vec<S>) -> Result<bool, String>
 where
     S: AsRef<OsStr>,
 {
     // venv could be unavailable, use 'uv' from this library's requirement
     let script = get_uv_binary().await;
 
     let subcommand = &args[0].as_ref().to_str().unwrap_or_default(); // cursed but makes it work with both &str and String
     let err_prefix = format!("uv {}", subcommand);
 
-    let result = Command::new(script).args(args).output().await;
-
-    match result {
-        Ok(result) => match result.status.code() {
-            Some(0) => Ok(true),
-            Some(_) | None => {
-                let err = String::from_utf8(result.stderr).unwrap_or_default();
-                Err(format!("{} | {}", err_prefix, err))
-            },
-        },
-        Err(result) => Err(format!("{} | {}", err_prefix, result.to_string())),
-    }
-}
-
-pub async fn run_with_output<S1, S2>(
-    command: S1,
-    args: Vec<S2>,
-) -> Result<(), String>
-where
-    S1: AsRef<OsStr>,
-    S2: AsRef<OsStr>,
-{
-    let mut cmd = Command::new(command);
-    cmd.args(args);
-    cmd.stdout(Stdio::inherit());
-    cmd.stderr(Stdio::inherit());
-    cmd.status().await.map_err_to_string()?;
-
-    Ok(())
+    return run(&script, args, Some(err_prefix)).await;
 }
 
-pub async fn uv_with_output<S>(args: Vec<S>) -> Result<(), String>
+pub async fn uv_with_output<S>(args: Vec<S>) -> Result<i32, String>
 where
     S: AsRef<OsStr>,
 {
     let script = get_uv_binary().await;
 
-    return run_with_output(script, args).await;
+    return run_print_output(script, args).await;
 }
 
 pub fn uv_cache() -> Option<Cache> {
     if let Some(project_dirs) = ProjectDirs::from("", "", "uv") {
         Cache::from_path(project_dirs.cache_dir())
     } else {
         Cache::from_path(".uv_cache")
```

### Comparing `uvx-2.0.0a1/src/venv.rs` & `uvx-2.0.0a2/src/venv.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,37 @@
 use pep508_rs::{PackageName, Requirement};
 use std::path::PathBuf;
 
 use uv_interpreter::PythonEnvironment;
 
 pub async fn create_venv(
     package_name: &PackageName,
-    python: Option<String>,
+    python: Option<&String>,
     force: bool,
     with_pip: bool,
+    custom_prefix: Option<String>,
 ) -> Result<PathBuf, String> {
-    let venv_path = venv_path(&package_name.to_string());
+    let venv_path = match custom_prefix {
+        None => venv_path(&package_name.to_string()),
+        Some(prefix) => PathBuf::from(format!("{}{}", prefix, package_name)),
+    };
 
     if !force && venv_path.exists() {
         return Err(
             format!("'{}' is already installed.\nUse '{}' to update existing tools or pass '{}' to this command to ignore this message.", 
             &package_name.to_string().green(), "uvx upgrade".green(), "--force".green())
         );
     }
 
     let mut args: Vec<&str> = vec!["venv", venv_path.to_str().unwrap_or_default()];
 
-    // extract because 'if let Some()' has a too short lifetime.
-    let py = python.unwrap_or_default();
-
     // if let Some(py) = python {
-    if py != "" {
+    if let Some(py) = python {
         args.push("--python");
-        args.push(&py);
+        args.push(py);
     }
     if with_pip {
         args.push("--seed");
     }
 
     uv(args).await?;
```

