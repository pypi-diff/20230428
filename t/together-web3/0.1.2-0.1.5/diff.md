# Comparing `tmp/together_web3-0.1.2.tar.gz` & `tmp/together_web3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together_web3-0.1.2.tar", max compression
+gzip compressed data, was "together_web3-0.1.5.tar", max compression
```

## Comparing `together_web3-0.1.2.tar` & `together_web3-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      854 2022-11-28 22:06:55.649513 together_web3-0.1.2/README.md
--rw-r--r--   0        0        0     2788 2022-11-28 22:07:09.721786 together_web3-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       46 2022-11-17 18:52:47.346426 together_web3-0.1.2/together_web3/__init__.py
--rw-r--r--   0        0        0      167 2022-11-17 18:52:47.346426 together_web3-0.1.2/together_web3/accounts.py
--rw-r--r--   0        0        0     8649 2022-11-28 22:06:55.649513 together_web3-0.1.2/together_web3/computer.py
--rw-r--r--   0        0        0     1315 2022-11-17 18:52:47.346426 together_web3-0.1.2/together_web3/coordinator.py
--rw-r--r--   0        0        0    13958 2022-11-28 22:06:55.649513 together_web3-0.1.2/together_web3/together.py
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 together_web3-0.1.2/setup.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 together_web3-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1177 2023-04-28 17:37:40.180065 together_web3-0.1.5/README.md
+-rw-r--r--   0        0        0     2806 2023-04-28 17:37:40.180065 together_web3-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/accounts.py
+-rw-r--r--   0        0        0    10298 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/computer.py
+-rw-r--r--   0        0        0     1315 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/coordinator.py
+-rw-r--r--   0        0        0    13998 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/together.py
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 together_web3-0.1.5/PKG-INFO
```

### Comparing `together_web3-0.1.2/pyproject.toml` & `together_web3-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "together-web3"
-version = "0.1.2"
+version = "0.1.5"
 description = ""
 authors = ["together <together@together.xyz>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/togethercomputer/web3.py"
 homepage = "https://github.com/togethercomputer/web3.py"
 keywords = [
@@ -42,14 +42,15 @@
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
 autopep8 = {version = "^1.7.0", allow-prereleases = true}
 ts2python = "0.6"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^5.1.1"
+build = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.isort]
```

### Comparing `together_web3-0.1.2/together_web3/computer.py` & `together_web3-0.1.5/together_web3/computer.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,21 +22,29 @@
 EventTypeNewBlock = "new-block"
 EventTypeResult = "result"
 OfferTypeInstanceAsk = "instance-ask"
 OfferTypeInstanceBid = "instance-bid"
 OfferTypeRemove = "remove"
 OfferTypeServiceAsk = "service-ask"
 OfferTypeServiceBid = "service-bid"
+PaymentChannelTypeDeposit = "deposit"
+PaymentChannelTypeWithdraw = "withdraw"
+PaymentChannelTypeOpenPaymentChannel = "open-payment-channel"
+RequestTypeAudioRecognition = "audio-recognition"
 RequestTypeImageModelInference = "image-model-inference"
+RequestTypeImageRecognition = "image-recognition"
 RequestTypeLanguageModelInference = "language-model-inference"
 RequestTypeShutdown = "shutdown"
 RequestTypeStatus = "status"
+ResultTypeError = "error"
 ResourceTypeInstance = "instance"
 ResourceTypeService = "service"
-ResultTypeError = "error"
+SubscriptionEvents = "events"
+TogetherHTTPProviderUrl = "https://computer.together.xyz"
+TogetherWebsocketProviderUrl = "wss://api.together.xyz/websocket"
 
 
 @dataclass
 class Job():
     """Base class for work fulfilled by a Service."""
     request_type: Optional[str]
 
@@ -91,14 +99,15 @@
     network_down: Optional[int] = None
     storage: Optional[List[Storage]] = None
 
 
 @dataclass
 class Service(Resource):
     service_name: str
+    options: Optional[Dict[str, str]]
 
 
 ############################################################
 # Resource prices
 
 @dataclass
 class ResourcePrice:
@@ -117,18 +126,20 @@
 
 
 ############################################################
 # Block format
 
 @dataclass
 class BlockHeader:
+    block_id: str
     block_previous: str
     block_height: int
     block_nonce: int
     market_address: Address
+    state_root: str
 
 
 ############################################################
 # Offers
 
 @dataclass
 class Offer:
@@ -152,15 +163,15 @@
     load_delay: Optional[int]
     high_water_mark: Optional[int]
     revenue_share: Optional[Dict[str, int]]
 
 
 @dataclass
 class ServiceBid(Offer):
-    deadline: Optional[datetime.datetime]
+    expires: Optional[datetime.datetime]
     service: Service
     max_service_price: ServicePrice
     job: Job
 
 
 @dataclass
 class InstanceAsk(Offer):
@@ -168,15 +179,15 @@
     instance_price: InstancePrice
     num_instances: int
     container_cached: Optional[List[str]]
 
 
 @dataclass
 class InstanceBid(Offer):
-    deadline: Optional[datetime.datetime]
+    expires: Optional[datetime.datetime]
     instance: Instance
     max_instance_price: InstancePrice
     num_instances: int
     container: Container
     supply_service: Optional[ServiceAsk]
 
 
@@ -281,14 +292,15 @@
 class Result:
     ask_address: str
     bid_address: str
     ask_offer_id: str
     bid_offer_id: str
     match_id: str
     partial: Optional[bool]
+    sequence: Optional[int]
     data: Dict[str, Any]
 
 
 @dataclass
 class LanguageModelInferenceChoice:
     # There are more fields here that aren't specified.
     # See the OpenAI API.
@@ -312,14 +324,15 @@
 
 ############################################################
 # Envelopes
 
 @dataclass
 class Envelope:
     signature: Optional[Signature]
+    version: Optional[int]
 
 
 @dataclass
 class OfferEnvelope(Envelope):
     offer: Offer
     offer_id: Optional[str]
 
@@ -354,19 +367,58 @@
 
 
 @dataclass
 class EventEnvelope(Envelope):
     events: List[Event]
 
 
+############################################################
+# Transactions
+
+@dataclass
+class Transaction:
+    match: MatchEnvelope
+    result: EventEnvelope
+    pass
+
+
 @dataclass
-class Block(BlockHeader, EventEnvelope):
+class BlockBody(EventEnvelope):
+    transaction: List[Transaction]
+
+
+@dataclass
+class Block(BlockHeader, BlockBody):
     pass
 
 
+@dataclass
+class LightTransaction:
+    market_address: Address
+    ask_address: Address
+    bid_address: Address
+    ask_signature: Signature
+    bid_signature: Signature
+    ask_offer_price: int
+    ask_offer_nonce: int
+    ask_offer_block_height: int
+    ask_offer_block_nonce: int
+    ask_offer_details_hash: ID
+    bid_offer_price: int
+    bid_offer_nonce: int
+    bid_offer_block_height: int
+    bid_offer_block_nonce: int
+    bid_offer_details_hash: ID
+    match_price: int
+    match_signature: Signature
+    result_data_hash: ID
+    result_signature: Signature
+    result_event_signature: Signature
+
+
 ############################################################
 # RPC
 
 class _RPC:
     together_updateOffer = RPCEndpoint("together_updateOffer")
     together_updateResult = RPCEndpoint("together_updateResult")
 
@@ -384,7 +436,19 @@
 
 class TogetherComputerProtocol(Protocol):
     def updateOffer(self, offer: Dict[str, Any], subscription_id: Optional[str]) -> str:
         pass
 
     def updateResult(self, offer: Dict[str, Any], subscription_id: Optional[str]) -> str:
         pass
+
+
+def parse_tags(input: str) -> Dict[str, str]:
+    tags: Dict[str, str] = {}
+    if not input:
+        return tags
+    for word in input.split():
+        if not word:
+            continue
+        kv = word.split("=")
+        tags[kv[0]] = "=".join(kv[1:])
+    return tags
```

### Comparing `together_web3-0.1.2/together_web3/coordinator.py` & `together_web3-0.1.5/together_web3/coordinator.py`

 * *Files identical despite different names*

### Comparing `together_web3-0.1.2/together_web3/together.py` & `together_web3-0.1.5/together_web3/together.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ResultEnvelope,
     ResultEvent,
     Service,
     ServiceBid,
     ServicePrice,
     TogetherComputer,
     TogetherComputerProtocol,
+    TogetherHTTPProviderUrl,
 )
 from .coordinator import TogetherCoordinator, TogetherCoordinatorProtocol
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -93,15 +94,15 @@
     _on_match_event: "List[Callable[[List[MatchEvent], List[Dict[str, Any]]], Union[None, Awaitable[None]]]]" = []
     _on_match_for_bid: "Dict[str, List[Callable[[Dict[str, Any]], None]]]" = {}
     _on_result_for_bid: "Dict[str, List[Future[Dict[str, Any]]]]" = {}
 
     def __init__(
         self,
         options: TogetherClientOptions = TogetherClientOptions(),
-        http_url: str = "https://computer.together.xyz",
+        http_url: str = TogetherHTTPProviderUrl,
         websocket_url: Optional[str] = None,
         **kwargs: Any
     ):
         self.http_url = http_url
         self.websocket_url = websocket_url if websocket_url else websocket_url_from_http_url(
             http_url)
         self.options = options
@@ -123,15 +124,15 @@
             self._subscription = asyncio.create_task(
                 self._handle_events(f"{rpc_namespace}_subscribe", "events", self._handle_event))
 
     async def _handle_events(self, method: str, event: str, handler: Callable[[Dict[str, Any]], Awaitable[None]]) -> None:
         while True:
             ws = None
             try:
-                ws = await asyncio.wait_for(connect(self.websocket_url), self.options.connect_timeout)
+                ws = await asyncio.wait_for(connect(self.websocket_url, max_size=10000000), self.options.connect_timeout)
                 await ws.send(f'{{"jsonrpc": "2.0", "id": 1, "method": "{method}", "params": ["{event}"]}}')
                 message = await ws.recv()
                 subscription_response = json.loads(message)
                 self._subscription_id = subscription_response["result"]
                 await self._handle_connect()
                 while True:
                     message = await asyncio.wait_for(ws.recv(), 1073741824)
```

### Comparing `together_web3-0.1.2/PKG-INFO` & `together_web3-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together-web3
-Version: 0.1.2
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/togethercomputer/web3.py
 License: MIT
 Keywords: NLP,vision,speech,deep,learning,transformer,pytorch,tensorflow,BERT,GPT-2
 Author: together
 Author-email: together@together.xyz
 Requires-Python: >=3.7.2,<3.11
@@ -42,8 +42,20 @@
 ### Generate an image
 
 ```console
 python examples/example.py "Rainbow unicorn" "StableDiffusion" \
   | grep image_base64 | cut -d\" -f4 | base64 -d > x.jpg && open x.jpg
 ```
 
+## Publish to PyPi
+
+GitHub repo > Releases > Draft a new Release > Choose a tag > Create new tag on publish >
+
+Name the tag using the current version from pyproject.toml with a "v" e.g. `v1.0.9`.
+
+> Publish Release
+
+In the repo toolbar select > Actions
+
+- Verify the publish workflow is running and completes successfully
+
```

