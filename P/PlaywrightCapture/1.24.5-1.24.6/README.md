# Comparing `tmp/playwrightcapture-1.24.5.tar.gz` & `tmp/playwrightcapture-1.24.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.5.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.6.tar", max compression
```

## Comparing `playwrightcapture-1.24.5.tar` & `playwrightcapture-1.24.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/LICENSE
--rw-r--r--   0        0        0     1441 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/README.md
--rw-r--r--   0        0        0      511 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    63307 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1487 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.5/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/LICENSE
+-rw-r--r--   0        0        0     1441 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/README.md
+-rw-r--r--   0        0        0      511 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    64094 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1488 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.6/PKG-INFO
```

### Comparing `playwrightcapture-1.24.5/LICENSE` & `playwrightcapture-1.24.6/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.5/README.md` & `playwrightcapture-1.24.6/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.5/playwrightcapture/capture.py` & `playwrightcapture-1.24.6/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 if sys.version_info < (3, 9):
     from pytz import all_timezones_set
 else:
     from zoneinfo import available_timezones
     all_timezones_set = available_timezones()
 
+if sys.version_info < (3, 11):
+    from async_timeout import timeout
+else:
+    from asyncio import timeout
+
 if TYPE_CHECKING:
     from playwright._impl._api_structures import (SetCookieParam, Geolocation,
                                                   HttpCredentials, Headers,
                                                   ViewportSize, Cookie,
                                                   ProxySettings)
     BROWSER = Literal['chromium', 'firefox', 'webkit']
 
@@ -465,44 +470,41 @@
     async def __dialog_didomi_clickthrough(self, page: Page) -> None:
         # Setup the handler.
         async def handler() -> None:
             self.logger.debug('Didomi dialog found, clicking through.')
             if await page.locator("#didomi-notice-agree-button").is_visible():
                 await page.locator("#didomi-notice-agree-button").click(timeout=2000)
 
-        await page.add_locator_handler(page.locator(".didomi-popup-view"), handler)
+        await page.add_locator_handler(page.locator(".didomi-popup-view").last, handler)
         self.logger.info('Didomi handler added')
 
     async def __dialog_onetrust_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## OT Dialog found, clicking through.')
             if await page.locator("#onetrust-accept-btn-handler").is_visible():
                 await page.locator("#onetrust-accept-btn-handler").click(timeout=2000)
 
         await page.add_locator_handler(
-            page.locator('#onetrust-banner-sdk'),
+            page.locator('#onetrust-banner-sdk').last,
             handler
         )
         self.logger.info('OT handler added')
 
     async def __dialog_hubspot_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## HS Dialog found, clicking through.')
             if await page.locator("#hs-eu-confirmation-button").is_visible():
                 await page.locator("#hs-eu-confirmation-button").click(timeout=2000)
 
         await page.add_locator_handler(
-            page.locator('#hs-eu-cookie-confirmation'),
+            page.locator('#hs-eu-cookie-confirmation').last,
             handler
         )
         self.logger.info('HS handler added')
 
     async def __dialog_cookiebot_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## Cookiebot Dialog found, clicking through.')
             if await page.locator("#CybotCookiebotDialogBodyLevelButtonLevelOptinAllowAll").is_visible():
                 await page.locator("#CybotCookiebotDialogBodyLevelButtonLevelOptinAllowAll").click(timeout=2000)
 
         await page.add_locator_handler(
             page.locator('#CybotCookiebotDialogBody'),
             handler
         )
@@ -515,15 +517,15 @@
                 await page.frame_locator("iframe[title=\"Consent window\"]").locator("button.button__acceptAll").click(timeout=2000)
             elif await page.locator('#onetrust-button-group').locator("#onetrust-accept-btn-handler").is_visible():
                 await page.locator('#onetrust-button-group').locator("#onetrust-accept-btn-handler").click(timeout=1000)
             else:
                 self.logger.info('Consent window found, but no button to click through.')
 
         await page.add_locator_handler(
-            page.get_by_role("alertdialog"),
+            page.get_by_role("alertdialog").last,
             handler
         )
         self.logger.info('alert dialog handler added')
 
     async def __dialog_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
             if await page.locator(".qc-cmp2-summary-buttons").locator("button").first.is_visible():
@@ -541,39 +543,36 @@
             page.get_by_role("dialog").last,
             handler
         )
         self.logger.info('dialog handler added')
 
     async def __dialog_complianz_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## Complianz found, clicking through.')
             if await page.locator('.cmplz-show').locator("button.cmplz-accept").is_visible():
                 await page.locator('.cmplz-show').locator("button.cmplz-accept").click(timeout=2000)
 
         await page.add_locator_handler(
             page.locator('.cmplz-show'),
             handler
         )
         self.logger.info('Complianz handler added')
 
     async def __dialog_yahoo_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## Yahoo found, clicking through.')
             if await page.locator('.con-wizard').locator("button.accept-all").is_visible():
                 await page.locator('.con-wizard').locator("button.accept-all").click(timeout=2000)
 
         await page.add_locator_handler(
             page.locator('.con-wizard'),
             handler
         )
         self.logger.info('Yahoo handler added')
 
     async def __dialog_ppms_clickthrough(self, page: Page) -> None:
         async def handler() -> None:
-            self.logger.info('######## piwik found, clicking through.')
             if await page.locator('.ppms_cm_popup_overlay').locator("button.ppms_cm_agree-to-all").is_visible():
                 await page.locator('.ppms_cm_popup_overlay').locator("button.ppms_cm_agree-to-all").click(timeout=2000)
 
         await page.add_locator_handler(
             page.locator('#ppms_cm_popup_overlay'),
             handler
         )
@@ -606,15 +605,19 @@
                     await download.save_as(tmp_f.name)
                     filename = download.suggested_filename
                     with open(tmp_f.name, "rb") as f:
                         file_content = f.read()
                     multiple_downloads.append((filename, file_content))
                     self.logger.info('Done with download.')
             except Exception as e:
-                self.logger.warning(f'Unable to finish download triggered from JS: {e}')
+                if download.page.is_closed():
+                    # Page is closed, skip logging.
+                    pass
+                else:
+                    self.logger.warning(f'Unable to finish download triggered from JS: {e}')
             finally:
                 self.wait_for_download -= 1
 
         async def store_request(request: Request) -> None:
             # This method is called on each request, to store the body (if it is an image) in a dict indexed by URL
             if got_favicons or request.resource_type != 'image':
                 return
@@ -828,22 +831,25 @@
                                 child_urls = child_urls[:1]
                             else:
                                 child_urls = child_urls[:max_captures]
                         self.logger.info(f'Capturing children, {max_captures} URLs')
                         for index, url in enumerate(child_urls):
                             self.logger.info(f'Capture child {url} - Timeout: {max_capture_time}s')
                             start_time = time.time()
+                            if page.is_closed():
+                                self.logger.info('Page is closed, unable to capture children.')
+                                break
                             try:
-                                child_capture = await asyncio.wait_for(
-                                    self.capture_page(url=url, referer=page.url,
-                                                      page=page, depth=depth,
-                                                      rendered_hostname_only=rendered_hostname_only,
-                                                      max_depth_capture_time=max_capture_time),
-                                    timeout=max_capture_time + 1)  # just adding a bit of padding so playwright has the chance to raise the exception first
-                                to_return['children'].append(child_capture)  # type: ignore[union-attr]
+                                async with timeout(max_capture_time + 1):  # just adding a bit of padding so playwright has the chance to raise the exception first
+                                    child_capture = await self.capture_page(
+                                        url=url, referer=page.url,
+                                        page=page, depth=depth,
+                                        rendered_hostname_only=rendered_hostname_only,
+                                        max_depth_capture_time=max_capture_time)
+                                    to_return['children'].append(child_capture)  # type: ignore[union-attr]
                             except (TimeoutError, asyncio.exceptions.TimeoutError):
                                 self.logger.info(f'Timeout error, took more than {max_capture_time}s. Unable to capture {url}.')
                             except Exception as e:
                                 self.logger.warning(f'Error while capturing child "{url}": {e}. {len(child_urls) - index - 1} more to go.')
                             else:
                                 runtime = int(time.time() - start_time)
                                 self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {len(child_urls) - index - 1} to go.')
@@ -876,33 +882,43 @@
                             'NS_ERROR_PARSED_DATA_CACHED',
                             'NS_ERROR_DOCUMENT_NOT_CACHED']:
                 # this one sounds like something we can retry...
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
+                            'Connection terminated unexpectedly',
                             'Navigation interrupted by another one',
                             'Navigation failed because page was closed!',
+                            'Target page, context or browser has been closed',
                             'Protocol error (Page.bringToFront): Not attached to an active page',
                             'Peer failed to perform TLS handshake: The TLS connection was non-properly terminated.',
                             'Peer failed to perform TLS handshake: Error sending data: Connection reset by peer',
+                            'Peer failed to perform TLS handshake: Error receiving data: Connection reset by peer',
                             'Peer sent fatal TLS alert: The server name sent was not recognized',
+                            'Peer sent fatal TLS alert: Internal error',
                             'Load cannot follow more than 20 redirections',
                             'Page crashed',
                             'Error receiving data: Connection reset by peer']:
                 # Other errors, let's give it another shot
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Target page, context or browser has been closed']:
                 # The browser barfed, let's try again
                 self.logger.info(f'Browser barfed on {url} (retrying): {e.message}')
                 self.should_retry = True
-            elif e.name in ['net::ERR_INVALID_AUTH_CREDENTIALS']:
+            elif e.name in ['net::ERR_INVALID_AUTH_CREDENTIALS',
+                            'net::ERR_BAD_SSL_CLIENT_AUTH_CERT',
+                            'net::ERR_UNEXPECTED_PROXY_AUTH']:
                 # No need to retry, the credentials are wrong/missing.
                 pass
+            elif e.name and any([msg in e.name for msg in ['is interrupted by another navigation to']]):
+                self.should_retry = True
+            elif e.name and any([msg in e.name for msg in ['Error resolving', 'Could not connect to']]):
+                pass
             else:
                 # Unexpected ones
                 self.logger.exception(f'Something went poorly with {url}: {e.message}')
         except Exception as e:
             # we may get a non-playwright exception to.
             # The ones we try to handle here should be treated as if they were.
             to_return['error'] = str(e)
@@ -945,15 +961,15 @@
             return await page.screenshot(full_page=True, scale="css", timeout=5000)
         except Error as e:
             self.logger.info(f"Capturing a screenshot of the full page failed, trying to get the current viewport only: {e}")
 
         try:
             return await page.screenshot(scale="css", animations='disabled', caret='initial', timeout=5000)
         except Error as e:
-            self.logger.warning(f"Unable to get any screenshot: {e}")
+            self.logger.info(f"Unable to get any screenshot: {e}")
             raise e
 
     async def _safe_wait(self, page: Page, force_max_wait_in_sec: int | None=None) -> None:
         max_wait: float
         try:
             if force_max_wait_in_sec is not None:
                 max_wait = force_max_wait_in_sec
@@ -1133,19 +1149,21 @@
                 'net::ERR_CONNECTION_TIMED_OUT',
                 'net::ERR_EMPTY_RESPONSE',
                 'net::ERR_HTTP_RESPONSE_CODE_FAILURE',
                 'net::ERR_HTTP2_PROTOCOL_ERROR',
                 'net::ERR_INVALID_RESPONSE',
                 'net::ERR_NAME_NOT_RESOLVED',
                 'net::ERR_SOCKS_CONNECTION_FAILED',
+                'net::ERR_SSL_KEY_USAGE_INCOMPATIBLE',
+                'net::ERR_SSL_PROTOCOL_ERROR',
                 'net::ERR_SSL_UNRECOGNIZED_NAME_ALERT',
                 'net::ERR_SSL_VERSION_OR_CIPHER_MISMATCH',
-                'net::ERR_SSL_PROTOCOL_ERROR',
                 'net::ERR_TIMED_OUT',
                 'net::ERR_TOO_MANY_REDIRECTS',
+                'SSL_ERROR_UNKNOWN',
         ]:
             return True
         return False
 
     async def _wait_for_random_timeout(self, page: Page, timeout: int) -> None:
         '''Instead of waiting for the exact same time, we wait +-500ms around the given time. The time is fiven in seconds for simplicity's sake.'''
         if timeout > 1000:
```

### Comparing `playwrightcapture-1.24.5/playwrightcapture/helpers.py` & `playwrightcapture-1.24.6/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.5/pyproject.toml` & `playwrightcapture-1.24.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.5"
+version = "1.24.6"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -37,16 +37,16 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 types-beautifulsoup4 = "^4.12.0.20240229"
 pytest = "^8.1.1"
-mypy = "^1.9.0"
-types-dateparser = "^1.1.4.20240331"
+mypy = "^1.10.0"
+types-dateparser = "^1.2.0.20240420"
 types-requests = "^2.31.0.20240406"
 types-pytz = "^2024.1.0.20240417"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playwrightcapture-1.24.5/PKG-INFO` & `playwrightcapture-1.24.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.5
+Version: 1.24.6
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

