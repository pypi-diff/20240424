# Comparing `tmp/servicing-0.0.6.tar.gz` & `tmp/servicing-0.0.7.tar.gz`

## Comparing `servicing-0.0.6.tar` & `servicing-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.6/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-04-17 01:04:10.000000 servicing-0.0.6/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-04-17 01:04:10.000000 servicing-0.0.6/.gitignore
--rw-r--r--   0     1001      127      165 2024-04-17 01:04:10.000000 servicing-0.0.6/.vimspector.json
--rw-r--r--   0     1001      127      693 2024-04-17 01:04:10.000000 servicing-0.0.6/README.md
--rw-r--r--   0     1001      127      271 2024-04-17 01:04:10.000000 servicing-0.0.6/build.rs
--rw-r--r--   0     1001      127     3216 2024-04-17 01:04:10.000000 servicing-0.0.6/servicing.pyi
--rw-r--r--   0     1001      127    13416 2024-04-17 01:04:10.000000 servicing-0.0.6/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-04-17 01:04:10.000000 servicing-0.0.6/src/error/mod.rs
--rw-r--r--   0     1001      127     5533 2024-04-17 01:04:10.000000 servicing-0.0.6/src/helper/mod.rs
--rw-r--r--   0     1001      127      637 2024-04-17 01:04:10.000000 servicing-0.0.6/src/lib.rs
--rw-r--r--   0     1001      127     3842 2024-04-17 01:04:10.000000 servicing-0.0.6/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-04-17 01:04:10.000000 servicing-0.0.6/template/service.yaml
--rw-r--r--   0     1001      127    41832 2024-04-17 01:04:10.000000 servicing-0.0.6/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-17 01:04:10.000000 servicing-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 servicing-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-04-24 16:47:43.000000 servicing-0.0.7/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-04-24 16:47:43.000000 servicing-0.0.7/.gitignore
+-rw-r--r--   0     1001      127      165 2024-04-24 16:47:43.000000 servicing-0.0.7/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-04-24 16:47:43.000000 servicing-0.0.7/README.md
+-rw-r--r--   0     1001      127      271 2024-04-24 16:47:43.000000 servicing-0.0.7/build.rs
+-rw-r--r--   0     1001      127     3319 2024-04-24 16:47:43.000000 servicing-0.0.7/servicing.pyi
+-rw-r--r--   0     1001      127    18648 2024-04-24 16:47:43.000000 servicing-0.0.7/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-04-24 16:47:43.000000 servicing-0.0.7/src/error/mod.rs
+-rw-r--r--   0     1001      127     5892 2024-04-24 16:47:43.000000 servicing-0.0.7/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-04-24 16:47:43.000000 servicing-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      127     3883 2024-04-24 16:47:43.000000 servicing-0.0.7/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-04-24 16:47:43.000000 servicing-0.0.7/template/service.yaml
+-rw-r--r--   0     1001      127    43003 2024-04-24 16:47:43.000000 servicing-0.0.7/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-04-24 16:47:43.000000 servicing-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.7/PKG-INFO
```

### Comparing `servicing-0.0.6/Cargo.toml` & `servicing-0.0.7/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
 
@@ -18,7 +18,8 @@
 serde = { version = "1.0", features = ["derive"] }
 serde_yaml = "0.9"
 dirs = "5.0.1"
 bincode = "1.3.3"
 regex = "1.10.4"
 serde_json = "1.0.115"
 base64 = "0.22.0"
+futures = "0.3.30"
```

### Comparing `servicing-0.0.6/.github/workflows/cicd.yml` & `servicing-0.0.7/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.6/.gitignore` & `servicing-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.6/README.md` & `servicing-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `servicing-0.0.6/servicing.pyi` & `servicing-0.0.7/servicing.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     :param disk_size: the disk size of the service
     :param cpu: the CPU upper bound of the service
     :param memory: the memory upper bound of the service
     :param setup: the setup command of the service
     :param run: the run command of the service
     """
 
-    def __init__(self, port: Optional[int] = None,
+    def __init__(self,
+                 port: Optional[int] = None,
                  replicas: Optional[int] = None,
                  cloud: Optional[str] = None,
                  workdir: Optional[str] = None,
                  disk_size: Optional[int] = None,
                  cpu: Optional[str] = None,
                  memory: Optional[str] = None,
                  setup: Optional[str] = None,
@@ -54,19 +55,20 @@
     def up(self, name: str) -> None:
         """
         Start a service
 
         :param name: the name of the service to start
         """
 
-    def down(self, name: str) -> None:
+    def down(self, name: str, force: Optional[bool] = None) -> None:
         """
         Stop a service
 
         :param name: the name of the service to stop
+        :param force: whether to force stop the service
         """
 
     def status(self, name: str, pretty: Optional[bool] = None) -> str:
         """
         Get the status of a service
 
         :param name: the name of the service
```

### Comparing `servicing-0.0.6/src/dispatcher/mod.rs` & `servicing-0.0.7/src/dispatcher/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 #![allow(dead_code)] // Remove this later
 
 use std::{
     collections::HashMap,
     path::PathBuf,
     process::Command,
     sync::{Arc, Mutex, OnceLock},
-    thread::{sleep, spawn},
     time::Duration,
 };
 
 use base64::Engine;
+use futures::future::join_all;
 use log::{error, info, warn};
 use pyo3::{pyclass, pymethods, Bound, PyAny};
 use regex::Regex;
 use reqwest::Client;
 use serde::{Deserialize, Serialize};
+use tokio::{
+    runtime::{self, Runtime},
+    time::sleep,
+};
 
 use crate::{
     error::ServicingError,
     helper,
     models::{Configuration, UserProvidedConfig},
 };
 
 static CACHE_DIR: &str = ".servicing";
 static CACHE_FILE_NAME: &str = "services.bin";
 static CLUSTER_ORCHESTRATOR: &str = "skypilot";
-static SEVICE_CHECK_INTERVAL: Duration = Duration::from_secs(5);
+static SERVICE_CHECK_INTERVAL: Duration = Duration::from_secs(5);
+static REPLICA_UP_CHECK: &str = "no ready replicas";
 
 static REGEX_URL: OnceLock<Regex> = OnceLock::new();
 
 /// Dispatcher is a struct that is responsible for creating the service configuration and launching
 /// the cluster on a particular cloud provider.
 #[pyclass(subclass)]
 pub struct Dispatcher {
     client: Client,
+    rt: Runtime,
     service: Arc<Mutex<HashMap<String, Service>>>,
 }
 
 #[pyclass]
 #[derive(Debug, Deserialize, Serialize)]
 struct Service {
     data: Option<UserProvidedConfig>,
@@ -58,16 +64,27 @@
         }
 
         let re = Regex::new(r"\b(?:\d{1,3}\.){3}\d{1,3}:\d+\b")?;
         let _ = REGEX_URL.get_or_init(|| re);
 
         let service = Arc::new(Mutex::new(HashMap::new()));
 
+        // tokio runtime with one dedicated worker
+        let rt = runtime::Builder::new_multi_thread()
+            .worker_threads(1)
+            .thread_name("servicing")
+            .enable_all()
+            .build()?;
+
         Ok(Self {
-            client: Client::new(),
+            client: Client::builder()
+                .pool_max_idle_per_host(0)
+                .timeout(Duration::from_secs(10))
+                .build()?,
+            rt,
             service,
         })
     }
 
     pub fn add_service(
         &mut self,
         name: String,
@@ -189,24 +206,24 @@
                 ))?
                 .as_str();
 
             service.url = Some(url.to_string());
             let service_clone = self.service.clone();
             let client_clone = self.client.clone();
 
-            let url = url.to_string();
+            let url = url.to_string() + &service.template.service.readiness_probe;
 
-            // spawn a thread to check when service comes online, then update the service status
-            spawn(move || {
+            // spawn a green thread to check when service comes online, then update the service status
+            let fut = async move {
                 let url = format!("http://{}", url);
                 loop {
-                    match helper::fetch(&client_clone, &url) {
+                    match helper::fetch(&client_clone, &url).await {
                         Ok(resp) => {
-                            if resp.to_lowercase().contains("no ready replicas") {
-                                sleep(SEVICE_CHECK_INTERVAL);
+                            if resp.to_lowercase().contains(REPLICA_UP_CHECK) {
+                                sleep(SERVICE_CHECK_INTERVAL).await;
                                 continue;
                             }
                             match service_clone.lock() {
                                 Ok(mut service) => {
                                     if let Some(service) = service.get_mut(&name) {
                                         service.up = true;
                                     } else {
@@ -223,54 +240,93 @@
                         }
                         Err(e) => {
                             error!("Error fetching the service: {:?}", e);
                             break;
                         }
                     }
                 }
-            });
+            };
+            self.rt.spawn(fut);
 
             return Ok(());
         }
         Err(ServicingError::ServiceNotFound(name))
     }
 
-    pub fn down(&mut self, name: String) -> Result<(), ServicingError> {
+    pub fn down(&mut self, name: String, force: Option<bool>) -> Result<(), ServicingError> {
         // get the service configuration
         match self.service.lock()?.get_mut(&name) {
             Some(service) if service.up => {
-                info!("Destroying the service with the configuration: {:?}", name);
-                // launch the cluster
-                let mut child = Command::new("sky")
-                    .arg("serve")
-                    .arg("down")
-                    .arg(&name)
-                    .spawn()?;
-
-                child.wait()?;
-
                 // Update service status
                 service.url = None;
                 service.up = false;
-
-                Ok(())
             }
-            Some(_) => Err(ServicingError::ServiceNotUp(name)),
-            None => Err(ServicingError::ServiceNotFound(name)),
+            Some(_) => match force {
+                Some(true) => {}
+                Some(false) | None => {
+                    return Err(ServicingError::ServiceNotUp(name));
+                }
+            },
+            None => return Err(ServicingError::ServiceNotFound(name)),
         }
+        info!("Destroying the service with the configuration: {:?}", name);
+        // launch the cluster
+        let mut child = Command::new("sky")
+            .arg("serve")
+            .arg("down")
+            .arg(&name)
+            .spawn()?;
+
+        child.wait()?;
+
+        Ok(())
     }
 
-    pub fn status(&self, name: String, pretty: Option<bool>) -> Result<String, ServicingError> {
+    pub fn status(&mut self, name: String, pretty: Option<bool>) -> Result<String, ServicingError> {
         // Check if the service exists
-        if let Some(service) = self.service.lock()?.get(&name) {
+        if let Some(service) = self.service.lock()?.get_mut(&name) {
             info!("Checking the status of the service: {:?}", name);
+
+            // if service is up poll once to see if it's still up
+            if let (true, Some(url)) = (service.up, &service.url) {
+                let url = format!(
+                    "http://{}{}",
+                    url, &service.template.service.readiness_probe
+                );
+
+                let r = self.rt.block_on(async {
+                    let res = helper::fetch(&self.client, &url).await;
+                    match res {
+                        Ok(resp) => {
+                            if resp.to_lowercase().contains(REPLICA_UP_CHECK) {
+                                Err(ServicingError::ServiceNotUp(name.clone()))
+                            } else {
+                                // it's up
+                                Ok(())
+                            }
+                        }
+                        Err(e) => Err::<(), _>(ServicingError::General(e.to_string())),
+                    }
+                });
+
+                match r {
+                    Ok(_) => {
+                        //No-op
+                        info!("Service {} is up", name);
+                    }
+                    Err(e) => {
+                        warn!("{:?}", e);
+                        service.up = false;
+                    }
+                }
+            }
+
             return Ok(match pretty {
                 Some(true) => serde_json::to_string_pretty(service)?,
-                Some(false) => serde_json::to_string(service)?,
-                None => serde_json::to_string(service)?,
+                _ => serde_json::to_string(service)?,
             });
         }
         Err(ServicingError::ServiceNotFound(name))
     }
 
     pub fn save(&self, location: Option<PathBuf>) -> Result<(), ServicingError> {
         let bin = bincode::serialize(&*self.service.lock()?)?;
@@ -299,15 +355,19 @@
 
     pub fn save_as_b64(&self) -> Result<String, ServicingError> {
         let bin = bincode::serialize(&*self.service.lock()?)?;
         let b64 = base64::prelude::BASE64_STANDARD.encode(bin);
         Ok(b64)
     }
 
-    pub fn load(&mut self, location: Option<PathBuf>) -> Result<(), ServicingError> {
+    pub fn load(
+        &mut self,
+        location: Option<PathBuf>,
+        update_status: Option<bool>,
+    ) -> Result<(), ServicingError> {
         let location = if let Some(location) = location {
             helper::create_directory(
                 location
                     .to_str()
                     .ok_or(ServicingError::General("Location is None".to_string()))?,
                 false,
             )?
@@ -318,14 +378,95 @@
 
         let bin = helper::read_from_file_binary(&location)?;
 
         self.service
             .lock()?
             .extend(bincode::deserialize::<HashMap<String, Service>>(&bin)?);
 
+        if let Some(true) = update_status {
+            info!("Checking for services that may come up while you were away...");
+
+            // Clones to pass to threads
+            let service_clone = self.service.clone();
+            let client_clone = self.client.clone();
+            let mut service_to_check = Vec::new();
+
+            // iterate through the services and find that are down
+            self.service
+                .lock()?
+                .iter()
+                .filter(|(_, service)| !service.up && service.url.is_some())
+                .for_each(|(name, service)| {
+                    service_to_check.push((
+                        name.clone(),
+                        service
+                            .url
+                            .clone()
+                            .expect("Gettting url, this should never be None")
+                            + &service.template.service.readiness_probe,
+                    ))
+                });
+
+            if service_to_check.is_empty() {
+                info!("No services to check");
+                return Ok(());
+            }
+
+            info!("Services to check: {:?}", service_to_check);
+
+            self.rt.spawn(async move {
+                let mut handles = Vec::new();
+                for (name, url) in service_to_check {
+                    let client_clone = client_clone.clone();
+                    let url = format!("http://{}", url);
+                    let handle = tokio::spawn(async move {
+                        match helper::fetch_and_check(
+                            &client_clone,
+                            &url,
+                            REPLICA_UP_CHECK,
+                            Some(SERVICE_CHECK_INTERVAL),
+                        )
+                        .await
+                        {
+                            Ok(_) => {}
+                            Err(e) => {
+                                return Err(e);
+                            }
+                        }
+                        Ok(name)
+                    });
+                    handles.push(handle);
+                }
+                for res in join_all(handles).await {
+                    let mut service = match service_clone.lock() {
+                        Ok(s) => s,
+                        Err(e) => {
+                            error!("Poisoned lock {e}");
+                            return;
+                        }
+                    };
+
+                    match res {
+                        Ok(Ok(r)) => {
+                            if let Some(service) = service.get_mut(&r) {
+                                service.up = true;
+                                info!("Service {} is up", r);
+                            }
+                        }
+                        Ok(Err(e)) => {
+                            warn!("{e}");
+                        }
+                        Err(e) => {
+                            error!("{e}");
+                        }
+                    }
+                }
+            });
+        }
+
         Ok(())
     }
 
     pub fn load_from_b64(&mut self, b64: String) -> Result<(), ServicingError> {
         let bin = base64::prelude::BASE64_STANDARD.decode(b64.as_bytes())?;
         self.service
             .lock()?
@@ -370,33 +511,39 @@
                 Some(UserProvidedConfig {
                     port: Some(1234),
                     replicas: Some(5),
                     cloud: Some("aws".to_string()),
                     workdir: None,
                     setup: None,
                     run: None,
+                    disk_size: None,
+                    cpu: None,
+                    memory: None,
                 }),
             )
             .unwrap();
 
+            // test the runtime... should NOT panic
+            dis.rt.block_on(async { "" });
+
             dis.save(None).unwrap();
 
             // check what has been added
             {
                 let services = dis.service.lock().unwrap();
                 let service = services.get("testing").unwrap();
                 assert_eq!(service.template.resources.ports, 1234);
                 assert_eq!(service.template.service.replicas, 5);
                 assert_eq!(service.template.resources.cloud, "aws");
             }
 
             dis.remove_service("testing".to_string()).unwrap();
             assert!(dis.service.lock().unwrap().get("testing").is_none());
 
-            dis.load(None).unwrap();
+            dis.load(None, None).unwrap();
             {
                 let services = dis.service.lock().unwrap();
                 let service = services.get("testing").unwrap();
                 assert_eq!(service.template.resources.ports, 1234);
             }
         });
     }
```

### Comparing `servicing-0.0.6/src/error/mod.rs` & `servicing-0.0.7/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.6/src/helper/mod.rs` & `servicing-0.0.7/src/helper/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+//! Helper module houses all the helper functions used by the service module.
 use std::{
     fs,
     io::{self, Read},
     path::{Path, PathBuf},
     process::Command,
     sync::mpsc::Receiver,
     thread::{spawn, JoinHandle},
+    time::Duration,
 };
 
 use log::info;
 use reqwest::{header::ACCEPT, Client};
+use tokio::time::sleep;
 
 use crate::error::ServicingError;
 
 /// check_python_package_installed checks if the user has installed the required python package.
 /// True is returned if the package is installed, otherwise false.
 pub(super) fn check_python_package_installed(package: &str) -> bool {
     info!("Checking for python package: {}", package);
@@ -155,24 +158,42 @@
             }
         }
         Ok(())
     });
     (rx, handle)
 }
 
-pub fn fetch(client: &Client, url: &str) -> Result<String, ServicingError> {
-    // create tokio runtime that is single threaded
-    let result = tokio::runtime::Builder::new_current_thread()
-        .enable_all()
-        .build()?
-        .block_on(async {
-            let res = client
-                .get(url)
-                .header(ACCEPT, "application/json")
-                .send()
-                .await?;
-            let body = res.text().await?;
-            Ok::<_, ServicingError>(body)
-        })?;
+pub async fn fetch(client: &Client, url: &str) -> Result<String, reqwest::Error> {
+    let res = client
+        .get(url)
+        .header(ACCEPT, "application/json")
+        .send()
+        .await?;
+    let body = res.text().await?;
+    Ok(body)
+}
+
+pub async fn fetch_and_check(
+    client: &Client,
+    url: &str,
+    expected: &str,
+    delay: Option<Duration>,
+) -> Result<(), ServicingError> {
+    loop {
+        let res = client
+            .get(url)
+            .header(ACCEPT, "application/json")
+            .send()
+            .await?;
+        let body = res.text().await?;
+
+        if !body.to_lowercase().contains(expected) {
+            break;
+        }
+
+        if let Some(delay) = delay {
+            sleep(delay).await;
+        }
+    }
 
-    Ok(result)
+    Ok(())
 }
```

### Comparing `servicing-0.0.6/src/lib.rs` & `servicing-0.0.7/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 mod error;
 mod helper;
 mod models;
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn servicing(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    // if release mode, set log level to info
+    // if release mode, set log level to warn
     if cfg!(not(debug_assertions)) {
         Builder::new().filter_level(log::LevelFilter::Warn).init();
     } else {
         Builder::new().filter_level(log::LevelFilter::Info).init();
     }
 
     m.add_class::<Dispatcher>()?;
```

### Comparing `servicing-0.0.6/src/models/mod.rs` & `servicing-0.0.7/src/models/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     pub setup: Option<String>,
     pub run: Option<String>,
 }
 
 #[pymethods]
 impl UserProvidedConfig {
     #[new]
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         port: Option<u16>,
         replicas: Option<u16>,
         cloud: Option<String>,
         workdir: Option<String>,
         disk_size: Option<u16>,
         cpu: Option<String>,
```

### Comparing `servicing-0.0.6/Cargo.lock` & `servicing-0.0.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -270,29 +270,73 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "futures"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
 name = "futures-channel"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
+ "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
+name = "futures-executor"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
+dependencies = [
+ "futures-core",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-io"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
+
+[[package]]
+name = "futures-macro"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
@@ -302,18 +346,24 @@
 
 [[package]]
 name = "futures-util"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
+ "futures-channel",
  "futures-core",
+ "futures-io",
+ "futures-macro",
+ "futures-sink",
  "futures-task",
+ "memchr",
  "pin-project-lite",
  "pin-utils",
+ "slab",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
@@ -764,17 +814,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -894,17 +944,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -942,17 +992,17 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
@@ -965,17 +1015,17 @@
 dependencies = [
  "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -1071,36 +1121,37 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "base64",
  "bincode",
  "dirs",
  "env_logger",
+ "futures",
  "log",
  "pyo3",
  "regex",
  "reqwest",
  "serde",
  "serde_json",
  "serde_yaml",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
@@ -1124,17 +1175,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1180,26 +1231,26 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `servicing-0.0.6/PKG-INFO` & `servicing-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
```

