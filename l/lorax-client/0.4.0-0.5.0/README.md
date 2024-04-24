# Comparing `tmp/lorax_client-0.4.0.tar.gz` & `tmp/lorax_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorax_client-0.4.0.tar", max compression
+gzip compressed data, was "lorax_client-0.5.0.tar", max compression
```

## Comparing `lorax_client-0.4.0.tar` & `lorax_client-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6812 2024-03-19 21:37:41.890076 lorax_client-0.4.0/README.md
--rw-r--r--   0        0        0      691 2024-03-23 00:14:37.308363 lorax_client-0.4.0/lorax/__init__.py
--rw-r--r--   0        0        0    26450 2024-03-22 17:14:38.649607 lorax_client-0.4.0/lorax/client.py
--rw-r--r--   0        0        0     2700 2023-12-02 22:28:06.724978 lorax_client-0.4.0/lorax/errors.py
--rw-r--r--   0        0        0    11062 2024-03-22 17:14:38.650136 lorax_client-0.4.0/lorax/types.py
--rw-r--r--   0        0        0      777 2024-03-23 00:14:28.634801 lorax_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 lorax_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6812 2024-03-19 21:37:41.890076 lorax_client-0.5.0/README.md
+-rw-r--r--   0        0        0      691 2024-04-24 16:22:05.614181 lorax_client-0.5.0/lorax/__init__.py
+-rw-r--r--   0        0        0    26684 2024-04-18 01:22:21.287788 lorax_client-0.5.0/lorax/client.py
+-rw-r--r--   0        0        0     2892 2024-04-18 01:22:21.289915 lorax_client-0.5.0/lorax/errors.py
+-rw-r--r--   0        0        0    11461 2024-04-16 22:25:03.736784 lorax_client-0.5.0/lorax/types.py
+-rw-r--r--   0        0        0      780 2024-04-24 16:22:28.817803 lorax_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7742 1970-01-01 00:00:00.000000 lorax_client-0.5.0/PKG-INFO
```

### Comparing `lorax_client-0.4.0/README.md` & `lorax_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lorax_client-0.4.0/lorax/__init__.py` & `lorax_client-0.5.0/lorax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from lorax.client import Client, AsyncClient, MergedAdapters
```

### Comparing `lorax_client-0.4.0/lorax/client.py` & `lorax_client-0.5.0/lorax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,23 @@
             self.base_url,
             json=request.dict(by_alias=True),
             headers=self.headers,
             cookies=self.cookies,
             timeout=self.timeout,
         )
 
-        # TODO: expose better error messages for 422 and similar errors
-        payload = resp.json()
+        try:
+            payload = resp.json()
+        except requests.JSONDecodeError as e:
+            # If the status code is success-like, reset it to 500 since the server is sending an invalid response.
+            if 200 <= resp.status_code < 400:
+                resp.status_code = 500
+
+            payload = {"message": e.msg}
+
         if resp.status_code != 200:
             raise parse_error(resp.status_code, payload)
 
         return Response(**payload[0])
 
     def generate_stream(
         self,
```

### Comparing `lorax_client-0.4.0/lorax/errors.py` & `lorax_client-0.5.0/lorax/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,20 +50,25 @@
 
 class NotSupportedError(Exception):
     def __init__(self, model_id: str):
         message = f"Model `{model_id}` is not available for inference with this client."
         super(NotSupportedError, self).__init__(message)
 
 
-# Unknown error
-class UnknownError(Exception):
+class UnprocessableEntityError(Exception):
     def __init__(self, message: str):
         super().__init__(message)
 
 
+# Unknown error
+class UnknownError(Exception):
+    def __init__(self, message: str, code: int):
+        super().__init__(f"Error status {code}: {message}")
+
+
 def parse_error(status_code: int, payload: Dict[str, str]) -> Exception:
     """
     Parse error given an HTTP status code and a json payload
 
     Args:
         status_code (`int`):
             HTTP status code
@@ -71,33 +76,35 @@
             Json payload
 
     Returns:
         Exception: parsed exception
 
     """
     # Try to parse a LoRAX error
-    message = payload["error"]
-    if "error_type" in payload:
-        error_type = payload["error_type"]
-        if error_type == "generation":
-            return GenerationError(message)
-        if error_type == "incomplete_generation":
-            return IncompleteGenerationError(message)
-        if error_type == "overloaded":
-            return OverloadedError(message)
-        if error_type == "validation":
-            return ValidationError(message)
+    message = payload.get("error", "")
+
+    error_type = payload.get("error_type", "")
+    if error_type == "generation":
+        return GenerationError(message)
+    if error_type == "incomplete_generation":
+        return IncompleteGenerationError(message)
+    if error_type == "overloaded":
+        return OverloadedError(message)
+    if error_type == "validation":
+        return ValidationError(message)
 
     # Try to parse a APIInference error
     if status_code == 400:
         return BadRequestError(message)
     if status_code == 403 or status_code == 424:
         return ShardNotReadyError(message)
     if status_code == 504:
         return ShardTimeoutError(message)
     if status_code == 404:
         return NotFoundError(message)
     if status_code == 429:
         return RateLimitExceededError(message)
+    if status_code == 422:
+        return UnprocessableEntityError(message)
 
     # Fallback to an unknown error
-    return UnknownError(message)
+    return UnknownError(message, status_code)
```

### Comparing `lorax_client-0.4.0/lorax/types.py` & `lorax_client-0.5.0/lorax/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from pydantic import BaseModel, validator, Field, ConfigDict
+from pydantic import BaseModel, field_validator, model_validator, Field, ConfigDict
 from typing import Optional, List, Dict, Any, OrderedDict, Union
 
 from lorax.errors import ValidationError
 
 
 ADAPTER_SOURCES = ["hub", "local", "s3", "pbase"]
 MERGE_STRATEGIES = ["linear", "ties", "dare_linear", "dare_ties"]
@@ -12,48 +12,48 @@
 
 class MergedAdapters(BaseModel):
     # IDs of the adapters to merge
     ids: List[str]
     # Weights of the adapters to merge
     weights: List[float]
     # Merge strategy
-    merge_strategy: Optional[str]
+    merge_strategy: Optional[str] = None
     # Density
     density: float
     # Majority sign method
-    majority_sign_method: Optional[str]
+    majority_sign_method: Optional[str] = None
 
-    @validator("ids")
+    @field_validator("ids")
     def validate_ids(cls, v):
         if not v:
             raise ValidationError("`ids` cannot be empty")
         return v
 
-    @validator("weights")
+    @field_validator("weights")
     def validate_weights(cls, v, values):
-        ids = values["ids"]
+        ids = values.data["ids"]
         if not v:
             raise ValidationError("`weights` cannot be empty")
         if len(ids) != len(v):
             raise ValidationError("`ids` and `weights` must have the same length")
         return v
 
-    @validator("merge_strategy")
+    @field_validator("merge_strategy")
     def validate_merge_strategy(cls, v):
         if v is not None and v not in MERGE_STRATEGIES:
             raise ValidationError(f"`merge_strategy` must be one of {MERGE_STRATEGIES}")
         return v
 
-    @validator("density")
+    @field_validator("density")
     def validate_density(cls, v):
         if v < 0 or v > 1.0:
             raise ValidationError("`density` must be >= 0.0 and <= 1.0")
         return v
 
-    @validator("majority_sign_method")
+    @field_validator("majority_sign_method")
     def validate_majority_sign_method(cls, v):
         if v is not None and v not in MAJORITY_SIGN_METHODS:
             raise ValidationError(f"`majority_sign_method` must be one of {MAJORITY_SIGN_METHODS}")
         return v
 
 
 class ResponseFormatType(str, Enum):
@@ -65,203 +65,199 @@
 
     type: ResponseFormatType
     schema_spec: Union[Dict[str, Any], OrderedDict] = Field(alias="schema")
 
 
 class Parameters(BaseModel):
     # The ID of the adapter to use
-    adapter_id: Optional[str]
+    adapter_id: Optional[str] = None
     # The source of the adapter to use
-    adapter_source: Optional[str]
+    adapter_source: Optional[str] = None
     # Adapter merge parameters
-    merged_adapters: Optional[MergedAdapters]
+    merged_adapters: Optional[MergedAdapters] = None
     # API token for accessing private adapters
-    api_token: Optional[str]
+    api_token: Optional[str] = None
     # Activate logits sampling
     do_sample: bool = False
     # Maximum number of generated tokens
     max_new_tokens: Optional[int] = None
     # Whether to ignore the EOS token during generation
     ignore_eos_token: bool = False
     # The parameter for repetition penalty. 1.0 means no penalty.
     # See [this paper](https://arxiv.org/pdf/1909.05858.pdf) for more details.
     repetition_penalty: Optional[float] = None
     # Whether to prepend the prompt to the generated text
     return_full_text: bool = False
     # Stop generating tokens if a member of `stop_sequences` is generated
     stop: List[str] = []
     # Random sampling seed
-    seed: Optional[int]
+    seed: Optional[int] = None
     # The value used to module the logits distribution.
-    temperature: Optional[float]
+    temperature: Optional[float] = None
     # The number of highest probability vocabulary tokens to keep for top-k-filtering.
-    top_k: Optional[int]
+    top_k: Optional[int] = None
     # If set to < 1, only the smallest set of most probable tokens with probabilities that add up to `top_p` or
     # higher are kept for generation.
-    top_p: Optional[float]
+    top_p: Optional[float] = None
     # truncate inputs tokens to the given size
-    truncate: Optional[int]
+    truncate: Optional[int] = None
     # Typical Decoding mass
     # See [Typical Decoding for Natural Language Generation](https://arxiv.org/abs/2202.00666) for more information
-    typical_p: Optional[float]
+    typical_p: Optional[float] = None
     # Generate best_of sequences and return the one if the highest token logprobs
-    best_of: Optional[int]
+    best_of: Optional[int] = None
     # Watermarking with [A Watermark for Large Language Models](https://arxiv.org/abs/2301.10226)
     watermark: bool = False
     # Get generation details
     details: bool = False
     # Get decoder input token logprobs and ids
     decoder_input_details: bool = False
     # The number of highest probability vocabulary tokens to return as alternative tokens in the generation result
-    return_k_alternatives: Optional[int]
+    return_k_alternatives: Optional[int] = None
     # Optional response format specification to constrain the generated text
-    response_format: Optional[ResponseFormat]
+    response_format: Optional[ResponseFormat] = None
 
-    @validator("adapter_id")
-    def valid_adapter_id(cls, v, values):
-        merged_adapters = values.get("merged_adapters")
-        if v is not None and merged_adapters is not None:
+    @model_validator(mode="after")
+    def valid_adapter_id(self):
+        adapter_id = self.adapter_id
+        merged_adapters = self.merged_adapters
+        if adapter_id is not None and merged_adapters is not None:
             raise ValidationError("you must specify at most one of `adapter_id` or `merged_adapters`")
-        return v
+        return self
 
-    @validator("adapter_source")
+    @field_validator("adapter_source")
     def valid_adapter_source(cls, v):
         if v is not None and v not in ADAPTER_SOURCES:
             raise ValidationError(f"`adapter_source` must be one of {ADAPTER_SOURCES}")
         return v
 
-    @validator("best_of")
+    @field_validator("best_of")
     def valid_best_of(cls, field_value, values):
         if field_value is not None:
             if field_value <= 0:
                 raise ValidationError("`best_of` must be strictly positive")
-            if field_value > 1 and values["seed"] is not None:
+            if field_value > 1 and values.data["seed"] is not None:
                 raise ValidationError("`seed` must not be set when `best_of` is > 1")
             sampling = (
-                values["do_sample"]
-                | (values["temperature"] is not None)
-                | (values["top_k"] is not None)
-                | (values["top_p"] is not None)
-                | (values["typical_p"] is not None)
+                values.data["do_sample"]
+                | (values.data["temperature"] is not None)
+                | (values.data["top_k"] is not None)
+                | (values.data["top_p"] is not None)
+                | (values.data["typical_p"] is not None)
             )
             if field_value > 1 and not sampling:
                 raise ValidationError("you must use sampling when `best_of` is > 1")
 
         return field_value
 
-    @validator("repetition_penalty")
+    @field_validator("repetition_penalty")
     def valid_repetition_penalty(cls, v):
         if v is not None and v <= 0:
             raise ValidationError("`repetition_penalty` must be strictly positive")
         return v
 
-    @validator("seed")
+    @field_validator("seed")
     def valid_seed(cls, v):
         if v is not None and v < 0:
             raise ValidationError("`seed` must be positive")
         return v
 
-    @validator("temperature")
+    @field_validator("temperature")
     def valid_temp(cls, v):
         if v is not None and v <= 0:
             raise ValidationError("`temperature` must be strictly positive")
         return v
 
-    @validator("top_k")
+    @field_validator("top_k")
     def valid_top_k(cls, v):
         if v is not None and v <= 0:
             raise ValidationError("`top_k` must be strictly positive")
         return v
 
-    @validator("top_p")
+    @field_validator("top_p")
     def valid_top_p(cls, v):
         if v is not None and (v <= 0 or v >= 1.0):
             raise ValidationError("`top_p` must be > 0.0 and < 1.0")
         return v
 
-    @validator("truncate")
+    @field_validator("truncate")
     def valid_truncate(cls, v):
         if v is not None and v <= 0:
             raise ValidationError("`truncate` must be strictly positive")
         return v
 
-    @validator("typical_p")
+    @field_validator("typical_p")
     def valid_typical_p(cls, v):
         if v is not None and (v <= 0 or v >= 1.0):
             raise ValidationError("`typical_p` must be > 0.0 and < 1.0")
         return v
 
-    @validator("return_k_alternatives")
+    @field_validator("return_k_alternatives")
     def valid_return_k_alternatives(cls, v):
         if v is not None and v <= 0:
             raise ValidationError("`return_k_alternatives` must be strictly positive")
         return v
 
 
 class Request(BaseModel):
     # Prompt
     inputs: str
     # Generation parameters
-    parameters: Optional[Parameters]
+    parameters: Optional[Parameters] = None
     # Whether to stream output tokens
     stream: bool = False
 
-    @validator("inputs")
+    @field_validator("inputs")
     def valid_input(cls, v):
         if not v:
             raise ValidationError("`inputs` cannot be empty")
         return v
 
-    @validator("stream")
+    @field_validator("stream")
     def valid_best_of_stream(cls, field_value, values):
-        parameters = values["parameters"]
-        if (
-            parameters is not None
-            and parameters.best_of is not None
-            and parameters.best_of > 1
-            and field_value
-        ):
-            raise ValidationError(
-                "`best_of` != 1 is not supported when `stream` == True"
-            )
+        parameters = values.data["parameters"]
+        if parameters is not None and parameters.best_of is not None and parameters.best_of > 1 and field_value:
+            raise ValidationError("`best_of` != 1 is not supported when `stream` == True")
         return field_value
 
 
 # Decoder input tokens
 class InputToken(BaseModel):
     # Token ID from the model tokenizer
     id: int
     # Token text
     text: str
     # Logprob
     # Optional since the logprob of the first token cannot be computed
-    logprob: Optional[float]
+    logprob: Optional[float] = None
+
 
 # Alternative Tokens
 class AlternativeToken(BaseModel):
     # Token ID from the model tokenizer
     id: int
     # Token text
     text: str
     # Logprob
     logprob: float
 
+
 # Generated tokens
 class Token(BaseModel):
     # Token ID from the model tokenizer
     id: int
     # Token text
     text: str
     # Logprob
     logprob: float
     # Is the token a special token
     # Can be used to ignore tokens when concatenating
     special: bool
     # Alternative tokens
-    alternative_tokens: Optional[List[AlternativeToken]]
+    alternative_tokens: Optional[List[AlternativeToken]] = None
 
 
 # Generation finish reason
 class FinishReason(str, Enum):
     # number of generated tokens == `max_new_tokens`
     Length = "length"
     # the model generated its end of sequence token
@@ -275,15 +271,15 @@
     # Generated text
     generated_text: str
     # Generation finish reason
     finish_reason: FinishReason
     # Number of generated tokens
     generated_tokens: int
     # Sampling seed if sampling was activated
-    seed: Optional[int]
+    seed: Optional[int] = None
     # Decoder input tokens, empty if decoder_input_details is False
     prefill: List[InputToken]
     # Generated tokens
     tokens: List[Token]
 
 
 # `generate` details
@@ -291,52 +287,55 @@
     # Generation finish reason
     finish_reason: FinishReason
     # Number of prompt tokens
     prompt_tokens: int
     # Number of generated tokens
     generated_tokens: int
     # Sampling seed if sampling was activated
-    seed: Optional[int]
+    seed: Optional[int] = None
     # Decoder input tokens, empty if decoder_input_details is False
     prefill: List[InputToken]
     # Generated tokens
     tokens: List[Token]
     # Additional sequences when using the `best_of` parameter
-    best_of_sequences: Optional[List[BestOfSequence]]
+    best_of_sequences: Optional[List[BestOfSequence]] = None
 
 
 # `generate` return value
 class Response(BaseModel):
     # Generated text
     generated_text: str
     # Generation details
-    details: Optional[Details]
+    details: Optional[Details] = None
 
 
 # `generate_stream` details
 class StreamDetails(BaseModel):
     # Generation finish reason
     finish_reason: FinishReason
     # Number of prompt tokens
     prompt_tokens: int
     # Number of generated tokens
     generated_tokens: int
     # Sampling seed if sampling was activated
-    seed: Optional[int]
+    seed: Optional[int] = None
 
 
 # `generate_stream` return value
 class StreamResponse(BaseModel):
     # Generated token
     token: Token
     # Complete generated text
     # Only available when the generation is finished
-    generated_text: Optional[str]
+    generated_text: Optional[str] = None
     # Generation details
     # Only available when the generation is finished
-    details: Optional[StreamDetails]
+    details: Optional[StreamDetails] = None
 
 
 # Inference API currently deployed model
 class DeployedModel(BaseModel):
     model_id: str
     sha: str
+
+    # Suppress pydantic warning over `model_id` field.
+    model_config = ConfigDict(protected_namespaces=())
```

### Comparing `lorax_client-0.4.0/pyproject.toml` & `lorax_client-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "lorax-client"
 packages = [
     {include = "lorax"}
 ]
-version = "0.4.0"
+version = "0.5.0"
 description = "LoRAX Python Client"
 license = "Apache-2.0"
 authors = ["Travis Addair <travis@predibase.com>", "Olivier Dehaene <olivier@huggingface.co>"]
 maintainers = ["Travis Addair <travis@predibase.com>"]
 readme = "README.md"
 homepage = "https://github.com/predibase/lorax"
 repository = "https://github.com/predibase/lorax"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.10"
+pydantic = "> 2, < 3"
 aiohttp = "^3.8"
 huggingface-hub = ">= 0.12, < 1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-asyncio = "^0.17.2"
 pytest-cov = "^3.0.0"
```

### Comparing `lorax_client-0.4.0/PKG-INFO` & `lorax_client-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lorax-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: LoRAX Python Client
 Home-page: https://github.com/predibase/lorax
 License: Apache-2.0
 Author: Travis Addair
 Author-email: travis@predibase.com
 Maintainer: Travis Addair
 Maintainer-email: travis@predibase.com
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: huggingface-hub (>=0.12,<1.0)
-Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: pydantic (>2,<3)
 Project-URL: Repository, https://github.com/predibase/lorax
 Description-Content-Type: text/markdown
 
 # LoRAX Python Client
 
 LoRAX Python client provides a convenient way of interfacing with a
 `lorax` instance running in your environment.
```

