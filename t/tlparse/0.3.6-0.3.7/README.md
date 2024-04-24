# Comparing `tmp/tlparse-0.3.6.tar.gz` & `tmp/tlparse-0.3.7.tar.gz`

## Comparing `tlparse-0.3.6.tar` & `tlparse-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 tlparse-0.3.6/Cargo.toml
--rw-r--r--   0     1001      127     2431 2024-03-06 19:22:29.000000 tlparse-0.3.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      127       27 2024-03-06 19:22:29.000000 tlparse-0.3.6/.gitignore
--rw-r--r--   0     1001      127    15933 2024-03-06 19:22:29.000000 tlparse-0.3.6/Cargo.lock
--rw-r--r--   0     1001      127     6734 2024-03-06 19:22:29.000000 tlparse-0.3.6/plan.txt
--rw-r--r--   0     1001      127    21001 2024-03-06 19:22:29.000000 tlparse-0.3.6/src/main.rs
--rw-r--r--   0     1001      127      284 2024-03-06 19:22:29.000000 tlparse-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 tlparse-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 tlparse-0.3.7/Cargo.toml
+-rw-r--r--   0     1001      127     2576 2024-03-12 23:40:26.000000 tlparse-0.3.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127       27 2024-03-12 23:40:26.000000 tlparse-0.3.7/.gitignore
+-rw-r--r--   0     1001      127    15933 2024-03-12 23:40:26.000000 tlparse-0.3.7/Cargo.lock
+-rw-r--r--   0     1001      127     6734 2024-03-12 23:40:26.000000 tlparse-0.3.7/plan.txt
+-rw-r--r--   0     1001      127    21087 2024-03-12 23:40:26.000000 tlparse-0.3.7/src/main.rs
+-rw-r--r--   0     1001      127      284 2024-03-12 23:40:26.000000 tlparse-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 tlparse-0.3.7/PKG-INFO
```

### Comparing `tlparse-0.3.6/Cargo.toml` & `tlparse-0.3.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "tlparse"
-version = "0.3.6"
+version = "0.3.7"
 edition = "2021"
 authors = ["Edward Z. Yang <ezyang@mit.edu>"]
 description = "Parse TORCH_LOG logs produced by PyTorch torch.compile"
 license = "BSD-3-Clause"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `tlparse-0.3.6/.github/workflows/CI.yml` & `tlparse-0.3.7/.github/workflows/CI.yml`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 permissions:
   contents: read
   id-token: write
 
 jobs:
   linux:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
@@ -37,14 +40,17 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
+    strategy:
+      matrix:
+        target: [x64, x86]
     steps:
       - uses: actions/checkout@v3
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
```

### Comparing `tlparse-0.3.6/Cargo.lock` & `tlparse-0.3.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 dependencies = [
  "anstyle",
  "windows-sys",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "base16ct"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
@@ -336,17 +336,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
@@ -447,15 +447,15 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tlparse"
-version = "0.3.6"
+version = "0.3.7"
 dependencies = [
  "anyhow",
  "base16ct",
  "clap",
  "fxhash",
  "html-escape",
  "indexmap",
```

### Comparing `tlparse-0.3.6/plan.txt` & `tlparse-0.3.7/plan.txt`

 * *Files identical despite different names*

### Comparing `tlparse-0.3.6/src/main.rs` & `tlparse-0.3.7/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         bytes_read += line.len() as u64;
         pb.set_position(bytes_read);
         spinner.set_message(format!("{:?}", stats));
         //spinner.set_message(format!("{:?} {:?}", slowest_time, fastest_time));
         let start = Instant::now();
 
         let Some(caps) = re_glog.captures(&line) else {
-            eprintln!("fail_glog {}", lineno);
+            eprintln!("Failed to parse glog prefix on line {}", lineno);
             stats.fail_glog += 1;
             continue;
         };
 
         let end = start.elapsed();
         if end < fastest_time {
             fastest_time = end;
@@ -424,15 +424,15 @@
         }
         let payload = &line[caps.name("payload").unwrap().start()..];
 
         let e = match serde_json::from_str::<Envelope>(payload) {
             Ok(r) => r,
             Err(err) => {
                 multi.suspend(|| {
-                    eprintln!("{}\n{:?}", payload, err);
+                    eprintln!("Failed to parse metadata JSON: {}\n{:?}", payload, err);
                 });
                 stats.fail_json += 1;
                 continue;
             }
         };
 
         if let Some((s, i)) = e.str {
@@ -546,15 +546,15 @@
             match serde_json::from_str::<Vec<DynamoGuard>>(payload.as_str()) {
                 Ok(guards) => {
                     let guards_context = DynamoGuardsContext { guards: guards };
                     fs::write(&f, tt.render("dynamo_guards.html", &guards_context)?)?;
                     compile_directory.push(compile_id_dir.join(filename));
                 }
                 Err(err) => {
-                    eprintln!("{}", err);
+                    eprintln!("Failed to parse guards json: {}", err);
                     stats.fail_dynamo_guards_json += 1;
                 }
             }
         }
 
         if let Some(metadata) = e.inductor_output_code {
             let filename = metadata
```

#### html2text {}

```diff
@@ -167,22 +167,23 @@
 they're never valid (a blank line in payload will still be \t) let mut iter =
 reader .lines() .enumerate() .filter_map(|(i, l)| match l { // 1-indexed line
 numbers please Ok(l) if !l.is_empty() => Some((i + 1, l)), _ => None, })
 .peekable(); while let Some((lineno, line)) = iter.next() { bytes_read +=
 line.len() as u64; pb.set_position(bytes_read); spinner.set_message(format!("{:
 ?}", stats)); //spinner.set_message(format!("{:?} {:?}", slowest_time,
 fastest_time)); let start = Instant::now(); let Some(caps) = re_glog.captures
-(&line) else { eprintln!("fail_glog {}", lineno); stats.fail_glog += 1;
-continue; }; let end = start.elapsed(); if end < fastest_time { fastest_time =
-end; } if end > slowest_time { slowest_time = end; //println!("{}", line); }
-let payload = &line[caps.name("payload").unwrap().start()..]; let e = match
-serde_json::from_str::(payload) { Ok(r) => r, Err(err) => { multi.suspend(||
-{ eprintln!("{}\n{:?}", payload, err); }); stats.fail_json += 1; continue; } };
-if let Some((s, i)) = e.str { let mut intern_table = INTERN_TABLE.lock().unwrap
-(); intern_table.insert(i, s); continue; }; match expected_rank { Some(rank) =>
+(&line) else { eprintln!("Failed to parse glog prefix on line {}", lineno);
+stats.fail_glog += 1; continue; }; let end = start.elapsed(); if end <
+fastest_time { fastest_time = end; } if end > slowest_time { slowest_time =
+end; //println!("{}", line); } let payload = &line[caps.name("payload").unwrap
+().start()..]; let e = match serde_json::from_str::(payload) { Ok(r) => r, Err
+(err) => { multi.suspend(|| { eprintln!("Failed to parse metadata JSON: {}\n{:
+?}", payload, err); }); stats.fail_json += 1; continue; } }; if let Some((s,
+i)) = e.str { let mut intern_table = INTERN_TABLE.lock().unwrap();
+intern_table.insert(i, s); continue; }; match expected_rank { Some(rank) =>
 { if rank != e.rank { stats.other_rank += 1; continue; } } None =>
 { multi.suspend(|| { eprintln!("Detected rank: {:?}", e.rank); });
 expected_rank = Some(e.rank); } }; let compile_id_dir: PathBuf = e .compile_id
 .as_ref() .map_or( format!("unknown_{lineno}"), |CompileId { frame_id,
 frame_compile_id, attempt, }| { format!("{frame_id}_{frame_compile_id}_
 {attempt}") }, ) .into(); let subdir = out_path.join(&compile_id_dir); fs::
 create_dir_all(&subdir)?; let mut payload = String::new(); if let Some(expect)
@@ -211,18 +212,18 @@
 "dynamo_output_graph.txt"; let f = subdir.join(&filename); fs::write(&f,
 &payload)?; compile_directory.push(compile_id_dir.join(filename)); } if
 e.dynamo_guards.is_some() { let filename = "dynamo_guards.html"; let f =
 subdir.join(&filename); match serde_json::from_str::
 DynamoGuard>>(payload.as_str()) { Ok(guards) => { let guards_context =
 DynamoGuardsContext { guards: guards }; fs::write(&f, tt.render
 ("dynamo_guards.html", &guards_context)?)?; compile_directory.push
-(compile_id_dir.join(filename)); } Err(err) => { eprintln!("{}", err);
-stats.fail_dynamo_guards_json += 1; } } } if let Some(metadata) =
-e.inductor_output_code { let filename = metadata .filename .as_ref() .and_then
-(|p| Path::file_stem(p)) .map_or_else( || PathBuf::from
+(compile_id_dir.join(filename)); } Err(err) => { eprintln!("Failed to parse
+guards json: {}", err); stats.fail_dynamo_guards_json += 1; } } } if let Some
+(metadata) = e.inductor_output_code { let filename = metadata .filename .as_ref
+() .and_then(|p| Path::file_stem(p)) .map_or_else( || PathBuf::from
 ("inductor_output_code.txt"), |stem| { let mut r = OsString::from
 ("inductor_output_code_"); r.push(stem); r.push(OsStr::new(".txt")); r.into()
 }, ); let f = subdir.join(&filename); fs::write(&f, &payload)?;
 compile_directory.push(compile_id_dir.join(filename)); } if let Some(metadata)
 = e.optimize_ddp_split_child { let filename = format!
 ("optimize_ddp_split_child_{}.txt", metadata.name); let f = subdir.join
 (&filename); fs::write(&f, &payload)?; compile_directory.push
```

