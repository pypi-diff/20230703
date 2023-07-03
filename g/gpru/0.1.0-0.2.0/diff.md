# Comparing `tmp/gpru-0.1.0.tar.gz` & `tmp/gpru-0.2.0.tar.gz`

## Comparing `gpru-0.1.0.tar` & `gpru-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/__about__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/__init__.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/_client.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/_logger.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/_api.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/_utils.py
--rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2022_03_01.py
--rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2022_06_01.py
--rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2023_03_15.py
--rw-r--r--   0        0        0    59066 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2023_06_01.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/py.typed
--rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/stable_2022_12_01.py
--rw-r--r--   0        0        0    49153 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/stable_2023_05_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/__init__.py
--rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/py.typed
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.1.0/LICENSE
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 gpru-0.1.0/README.md
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 gpru-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 gpru-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/__about__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/__init__.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/_client.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/_logger.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/_api.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/_utils.py
+-rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2022_03_01.py
+-rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2022_06_01.py
+-rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2023_03_15.py
+-rw-r--r--   0        0        0    59066 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2023_06_01.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/py.typed
+-rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/stable_2022_12_01.py
+-rw-r--r--   0        0        0    49153 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/stable_2023_05_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/__init__.py
+-rw-r--r--   0        0        0    58302 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/py.typed
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 gpru-0.2.0/README.md
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 gpru-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 gpru-0.2.0/PKG-INFO
```

### Comparing `gpru-0.1.0/gpru/_client.py` & `gpru-0.2.0/gpru/_client.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/exceptions.py` & `gpru-0.2.0/gpru/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/_api.py` & `gpru-0.2.0/gpru/azure/_api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/preview_2022_03_01.py` & `gpru-0.2.0/gpru/azure/preview_2022_03_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/preview_2022_06_01.py` & `gpru-0.2.0/gpru/azure/preview_2022_06_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/preview_2023_03_15.py` & `gpru-0.2.0/gpru/azure/preview_2023_03_15.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/preview_2023_06_01.py` & `gpru-0.2.0/gpru/azure/preview_2023_06_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/stable_2022_12_01.py` & `gpru-0.2.0/gpru/azure/stable_2022_12_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/azure/stable_2023_05_15.py` & `gpru-0.2.0/gpru/azure/stable_2023_05_15.py`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/gpru/openai/api.py` & `gpru-0.2.0/gpru/openai/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,200 +1,241 @@
-"""Client implementation for the OpenAI API version `1.2.0`."""
+"""Client implementation for the OpenAI API version `2.0.0`."""
 
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Union
 
 from httpx._config import DEFAULT_TIMEOUT_CONFIG
 from httpx._types import TimeoutTypes
 from pydantic import BaseModel, Field
 
 from gpru._client import kwargs_for_uploading, request_factory, stream_factory
 
 
 class Error(BaseModel):
-    message: Optional[str] = None
-    type: Optional[str] = None
-    param: Optional[str] = None
-    code: Optional[str] = None
+    type: Optional[str]
+    message: Optional[str]
+    param: Optional[str]
+    code: Optional[str]
 
 
 class ErrorResponse(BaseModel):
     error: Error
 
 
-class Logprobs(BaseModel):
-    tokens: Optional[List[str]] = None
-    token_logprobs: Optional[List[float]] = None
-    top_logprobs: Optional[List[Dict[str, Any]]] = None
-    text_offset: Optional[List[int]] = None
+class ChatCompletionModel(str, Enum):
+    GPT_4 = "gpt-4"
+    GPT_4_0314 = "gpt-4-0314"
+    GPT_4_0613 = "gpt-4-0613"
+    GPT_4_32K = "gpt-4-32k"
+    GPT_4_32K_0314 = "gpt-4-32k-0314"
+    GPT_4_32K_0613 = "gpt-4-32k-0613"
+    GPT_35_TURBO = "gpt-3.5-turbo"
+    GPT_35_TURBO_16K = "gpt-3.5-turbo-16k"
+    GPT_35_TURBO_0301 = "gpt-3.5-turbo-0301"
+    GPT_35_TURBO_0613 = "gpt-3.5-turbo-0613"
+    GPT_35_TURBO_16K_0613 = "gpt-3.5-turbo-16k-0613"
 
 
-class Choice(BaseModel):
-    text: Optional[str] = None
-    index: Optional[int] = None
-    logprobs: Optional[Logprobs] = None
-    finish_reason: Optional[str] = None
+class Role(str, Enum):
+    """The role of the messages author."""
 
+    SYSTEM = "system"
+    USER = "user"
+    ASSISTANT = "assistant"
+    FUNCTION = "function"
 
-class Usage(BaseModel):
-    prompt_tokens: int
-    completion_tokens: int
-    total_tokens: int
 
+class FunctionCall(BaseModel):
+    """The name and arguments of a function that should be called, as generated by the
+    model.
+    """
 
-class Completion(BaseModel):
-    id: str
-    object: str
-    created: int
-    model: str
-    choices: List[Choice]
-    usage: Optional[Usage] = None
+    name: str
+    """The name of the function to call."""
+    arguments: str
+    """
+    The arguments to call the function with, as generated by the model in JSON format.
 
-    @property
-    def texts(self) -> List[str]:
+    Notes
+    -----
+    The model does not always generate valid JSON, and may hallucinate parameters not
+    defined by your function schema. Validate the arguments in your code before calling
+    your function.
+    """
+
+
+class Message(BaseModel):
+    role: Role
+    """The role of the messages author."""
+    content: str
+    """
+    The contents of the message.
+
+    `content` is required for all messages, and may be null for assistant messages with
+    function calls.
+    """
+    name: Optional[str] = None
+    """
+    The name of the author of this message.
+
+    `name` is required if role is `function`, and it should be the name of the function
+    whose response is in the `content`. May contain a-z, A-Z, 0-9, and underscores, with
+    a maximum length of 64 characters.
+    """
+    function_call: Optional[FunctionCall] = None
+    """The name and arguments of a function that should be called, as generated by the
+    model.
+    """
+
+
+class SystemMessage(Message):
+    """A system message."""
+
+    def __init__(self, content: str):
         """
-        List of texts from the choices.
+        Create a system message.
 
-        Returns
-        -------
-        List[str]
-            List of texts.
+        Parameters
+        ----------
+        content : str
+            The contents of the message.
         """
-        return [c.text for c in self.choices if c.text is not None]
+        super().__init__(role=Role.SYSTEM, content=content)
 
-    @property
-    def text(self) -> str:
+
+class UserMessage(Message):
+    """A user message."""
+
+    def __init__(self, content: str, name: Optional[str] = None):
         """
-        The concatenation of the generated texts.
+        Create a user message.
 
-        Returns
-        -------
-        str
-            Concatenated texts.
+        Parameters
+        ----------
+        content : str
+            The contents of the message.
+        name : Optional[str], optional
+            The name of the author of this message.
         """
-        return "".join(self.texts)
+        super().__init__(role=Role.USER, content=content, name=name)
 
 
-class CompletionRequest(BaseModel):
-    """The contents of the request to create completion."""
+class AssistantMessage(Message):
+    """An assistant message."""
 
-    model: str
+    def __init__(self, content: str):
+        """
+        Create an assistant message.
+
+        Parameters
+        ----------
+        content : str
+            The contents of the message.
+        """
+        super().__init__(role=Role.ASSISTANT, content=content)
+
+
+class FunctionMessage(Message):
+    """A function message."""
+
+    def __init__(self, content: str, function_call: Optional[FunctionCall] = None):
+        """
+        Create an assistant message.
+
+        Parameters
+        ----------
+        content : str
+            The contents of the message.
+        function_call: Optional[FunctionCall], optional
+            The name and arguments of a function that should be called, as generated by
+            the model.
+        """
+        super().__init__(
+            role=Role.FUNCTION, content=content, function_call=function_call
+        )
+
+
+class Function(BaseModel):
+    name: str
     """
-    ID of the model to use.
+    The name of the function to be called.
 
-    Examples
-    --------
-    - `model="text-davinci-003"`
+    Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length of
+    64.
     """
-    prompt: Optional[
-        Union[str, List[str], List[int], List[List[int]]]
-    ] = "<|endoftext|>"
+    description: Optional[str] = None
+    """A description of what the function does, used by the model to choose when and how
+    to call the function.
     """
-    The prompt(s) to generate completions for, encoded as a string, array of strings,
-    array of tokens, or array of token arrays.
+    parameters: Dict[str, Any]
+    """
+    The parameters the functions accepts, described as a JSON Schema object.
 
-    Notes
-    -----
-    `"<|endoftext|>"` is the document separator that the model sees during training, so
-    if a prompt is not specified the model will generate as if from the beginning of a
-    new document.
+    To describe a function that accepts no parameters, provide the value
+    `{"type": "object", "properties": {}}`.
 
-    Examples
+    See Also
     --------
-    - `prompt="This is a test."`
-    - `prompt=["This is a test."]`
-    - `prompt=[1212, 318, 257, 1332, 13]`
-    - `prompt=[[1212, 318, 257, 1332, 13]]`
+    - [Official Guide](https://platform.openai.com/docs/guides/gpt/function-calling)
+    - [JSON Schema](https://json-schema.org/understanding-json-schema/)
     """
-    suffix: Optional[str] = None
-    """
-    The suffix that comes after a completion of inserted text.
 
-    Examples
-    --------
-    - `suffix="test."`
-    """
-    max_tokens: Optional[int] = Field(16, ge=0)
-    """
-    The maximum number of [tokens](https://platform.openai.com/tokenizer) to generate in
-    the completion.
 
-    The token count of your prompt plus `max_tokens` cannot exceed the model's context
-    length. Most models have a context length of 2048 tokens (except for the newest
-    models, which support 4096).
+class ChatCompletionRequest(BaseModel):
+    model: Union[str, ChatCompletionModel]
+    """
+    ID of the model to use.
 
-    Examples
-    --------
-    - `max_tokens=16`
+    See the [model endpoint compatibility](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+    table for details on which models work with the Chat API.
+    """
+    messages: List[Message] = Field(..., min_items=1)
+    """A list of messages comprising the conversation so far."""
+    functions: Optional[List[Function]] = Field(None, min_items=1)
+    """A list of functions the model may generate JSON inputs for."""
+    function_call: Union[str, Dict[str, str], None] = None
+    """
+    Controls how the model responds to function calls.
+
+    "none" means the model does not call a function, and responds to the end-user.
+    "auto" means the model can pick between an end-user or calling a function.
+    Specifying a particular function via `{"name": "my_function"}` forces the model to
+    call that function. "none" is the default when no functions are present. "auto" is
+    the default if functions are present.
     """
     temperature: Optional[float] = Field(1.0, ge=0.0, le=2.0)
     """
     What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make
     the output more random, while lower values like 0.2 will make it more focused and
     deterministic.
 
     We generally recommend altering this or `top_p` but not both.
-
-    Examples
-    --------
-    - `temperature=1.0`
     """
     top_p: Optional[float] = Field(1.0, ge=0.0, le=1.0)
     """
     An alternative to sampling with temperature, called nucleus sampling, where the
-    model considers the results of the tokens with `top_p` probability mass. So 0.1
-    means only the tokens comprising the top 10% probability mass are considered.
+    model considers the results of the tokens with top_p probability mass. So 0.1 means
+    only the tokens comprising the top 10% probability mass are considered.
 
     We generally recommend altering this or `temperature` but not both.
-
-    Examples
-    --------
-    - `top_p=1.0`
     """
     n: Optional[int] = Field(1, ge=1, le=128)
-    """
-    How many completions to generate for each prompt.
-
-    Notes
-    -----
-    Because this parameter generates many completions, it can quickly consume your token
-    quota. Use carefully and ensure that you have reasonable settings for `max_tokens`
-    and `stop`.
-
-    Examples
-    --------
-    - `n=1`
-    """
+    """How many chat completion choices to generate for each input message."""
     stream: Optional[bool] = False
-    """Whether to stream back partial progress."""
-    logprobs: Optional[int] = Field(None, ge=0, le=5)
-    """
-    Include the log probabilities on the `logprobs` most likely tokens, as well the
-    chosen tokens.
-
-    For example, if `logprobs` is 5, the API will return a list of the 5 most likely
-    tokens. The API will always return the `logprob` of the sampled token, so there may
-    be up to `logprobs+1` elements in the response. The maximum value for `logprobs` is
-    5. If you need more than this, please contact us through our
-    [Help center](https://help.openai.com)
-    and describe your use case.
-    """
-    echo: Optional[bool] = False
-    """Echo back the prompt in addition to the completion."""
+    """If set, partial message deltas will be sent, like in ChatGPT."""
     stop: Optional[Union[str, List[str]]] = None
-    r"""
-    Up to 4 sequences where the API will stop generating further tokens.
-
-    The returned text will not contain the stop sequence.
+    """Up to 4 sequences where the API will stop generating further tokens."""
+    max_tokens: Optional[int] = None
+    """
+    The maximum number of [tokens](https://platform.openai.com/tokenizer) to generate in
+    the chat completion.
 
-    Examples
-    --------
-    - `stop="\n"`
-    - `stop=["\n"]`
+    The total length of input tokens and generated tokens is limited by the model's
+    context length.
     """
     presence_penalty: Optional[float] = Field(0.0, ge=-2.0, le=2.0)
     """
     Number between -2.0 and 2.0. Positive values penalize new tokens based on whether
     they appear in the text so far, increasing the model's likelihood to talk about new
     topics.
 
@@ -208,84 +249,75 @@
     existing frequency in the text so far, decreasing the model's likelihood to repeat
     the same line verbatim.
 
     See Also
     --------
     [Parameter details](https://platform.openai.com/docs/api-reference/parameter-details)
     """
-    best_of: Optional[int] = Field(1, ge=0, le=20)
-    """
-    Generates `best_of` completions server-side and returns the "best" (the one with the
-    highest log probability per token). Results cannot be streamed.
-
-    When used with `n`, `best_of` controls the number of candidate completions and `n`
-    specifies how many to return - `best_of` must be greater than `n`.
-
-    Notes
-    -----
-    Because this parameter generates many completions, it can quickly consume your token
-    quota. Use carefully and ensure that you have reasonable settings for `max_tokens`
-    and `stop`.
-    """
     logit_bias: Optional[Dict[str, Any]] = None
     """
-    Modify the likelihood of specified tokens appearing in the completion. Accepts a
-    json object that maps tokens (specified by their token ID in the GPT tokenizer) to
-    an associated bias value from -100 to 100.
-
-    You can use this [tokenizer tool](https://platform.openai.com/tokenizer) (which
-    works for both GPT-2 and GPT-3) to convert text to token IDs. Mathematically,
-    the bias is added to the logits generated by the model prior to sampling. The exact
-    effect will vary per model, but values between -1 and 1 should decrease or increase
-    likelihood of selection; values like -100 or 100 should result in a ban or exclusive
-    selection of the relevant token.
+    Modify the likelihood of specified tokens appearing in the completion.
 
-    As an example, you can pass `{"50256": -100}` to prevent the `<|endoftext|>` token
-    from being generated.
+    Accepts a json object that maps tokens (specified by their token ID in the
+    tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is
+    added to the logits generated by the model prior to sampling. The exact effect will
+    vary per model, but values between -1 and 1 should decrease or increase likelihood
+    of selection; values like -100 or 100 should result in a ban or exclusive selection
+    of the relevant token.
     """
     user: Optional[str] = None
     """
     A unique identifier representing your end-user, which can help OpenAI to monitor and
     detect abuse.
 
     See Also
     --------
     [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
-
-    Examples
-    --------
-    - `user="user-1234"`
     """
 
 
-class Role(str, Enum):
-    """The role of the author of this message."""
-
-    SYSTEM = "system"
-    USER = "user"
-    ASSISTANT = "assistant"
-
-
 class ChatCompletionMessage(BaseModel):
     role: Role
-    content: str
+    """The role of the author of this message."""
+    content: Optional[str] = None
+    """The contents of the message."""
+    function_call: Optional[FunctionCall] = None
+    """The name and arguments of a function that should be called, as generated by the
+    model.
+    """
 
 
 class ChatCompletionDeltaMessage(BaseModel):
     role: Optional[Role] = None
     """The role of the author of this message."""
     content: Optional[str] = None
-    """The contents of the message."""
+    """The contents of the chunk message."""
+    function_call: Optional[FunctionCall] = None
+    """The name and arguments of a function that should be called, as generated by the
+    model.
+    """
+
+
+class FinishReason(str, Enum):
+    STOP = "stop"
+    LENGTH = "length"
+    FUNCTION_CALL = "function_call"
 
 
 class ChatChoice(BaseModel):
     index: Optional[int] = None
     message: Optional[ChatCompletionMessage] = None
     delta: Optional[ChatCompletionDeltaMessage] = None
-    finish_reason: Optional[str] = None
+    finish_reason: Optional[FinishReason] = None
+
+
+class Usage(BaseModel):
+    prompt_tokens: int
+    completion_tokens: int
+    total_tokens: int
 
 
 class ChatCompletion(BaseModel):
     id: str
     object: str
     created: int
     model: str
@@ -310,15 +342,15 @@
         List of message contents from the choices.
 
         Returns
         -------
         List[str]
             List of message contents
         """
-        return [m.content for m in self.messages]
+        return [m.content for m in self.messages if m.content is not None]
 
     @property
     def content(self) -> str:
         """
         The concatenation of the generated message contents.
 
         Returns
@@ -344,83 +376,47 @@
                 continue
             if choice.delta.content is None:
                 continue
             content += choice.delta.content
         return content
 
 
-class Message(BaseModel):
-    role: Role
-    """The role of the author of this message."""
-    content: str
-    """The contents of the message."""
-    name: Optional[str] = None
-    """The name of the user in a multi-user chat."""
-
-
-class SystemMessage(Message):
-    """A system message."""
-
-    def __init__(self, content: str):
-        """
-        Create a system message.
-
-        Parameters
-        ----------
-        content : str
-            The contents of the message.
-        """
-        super().__init__(role=Role.SYSTEM, content=content)
-
-
-class UserMessage(Message):
-    """A user message."""
+class CompletionModel(str, Enum):
+    TEXT_DAVINCI_003 = "text-davinci-003"
+    TEXT_DAVINCI_002 = "text-davinci-002"
+    TEXT_DAVINCI_001 = "text-davinci-001"
+    CODE_DAVINCI_002 = "code-davinci-002"
+    TEXT_CURIE_001 = "text-curie-001"
+    TEXT_BABBAGE_001 = "text-babbage-001"
+    TEXT_ADA_001 = "text-ada-001"
 
-    def __init__(self, content: str):
-        """
-        Create a user message.
 
-        Parameters
-        ----------
-        content : str
-            The contents of the message.
-        """
-        super().__init__(role=Role.USER, content=content)
-
-
-class AssistantMessage(Message):
-    """An assistant message."""
-
-    def __init__(self, content: str):
-        """
-        Create an assistant message.
-
-        Parameters
-        ----------
-        content : str
-            The contents of the message.
-        """
-        super().__init__(role=Role.ASSISTANT, content=content)
-
-
-class ChatCompletionRequest(BaseModel):
-    model: str
+class CompletionRequest(BaseModel):
+    model: Union[str, CompletionModel]
+    """ID of the model to use."""
+    prompt: Union[str, List[str], List[int], List[List[int]], None] = "<|endoftext|>"
     """
-    ID of the model to use.
+    The prompt(s) to generate completions for, encoded as a string, array of strings,
+    array of tokens, or array of token arrays.
 
-    See the [model endpoint compatibility table](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-    for details on which models work with the Chat API.
+    Notes
+    -----
+    `"<|endoftext|>"` is the document separator that the model sees during training, so
+    if a prompt is not specified the model will generate as if from the beginning of a
+    new document.
     """
-    messages: List[Message] = Field(..., min_items=1)
+    suffix: Optional[str] = None
+    """The suffix that comes after a completion of inserted text."""
+    max_tokens: Optional[int] = Field(16, ge=0)
     """
-    The messages to generate chat completions for, in the chat format.
+    The maximum number of [tokens](https://platform.openai.com/tokenizer) to generate in
+    the completion.
 
-    See Also
-    --------
-    [Chat completions - Introduction](https://platform.openai.com/docs/guides/chat/introduction)
+    The token count of your prompt plus `max_tokens` cannot exceed the model's context
+    length.
     """
     temperature: Optional[float] = Field(1.0, ge=0.0, le=2.0)
     """
     What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make
     the output more random, while lower values like 0.2 will make it more focused and
     deterministic.
 
@@ -431,25 +427,42 @@
     An alternative to sampling with temperature, called nucleus sampling, where the
     model considers the results of the tokens with `top_p` probability mass. So 0.1
     means only the tokens comprising the top 10% probability mass are considered.
 
     We generally recommend altering this or `temperature` but not both.
     """
     n: Optional[int] = Field(1, ge=1, le=128)
-    """How many chat completion choices to generate for each input message."""
+    """
+    How many completions to generate for each prompt.
+
+    Notes
+    -----
+    Because this parameter generates many completions, it can quickly consume your token
+    quota. Use carefully and ensure that you have reasonable settings for `max_tokens`
+    and `stop`.
+    """
     stream: Optional[bool] = False
-    """If set, partial message deltas will be sent, like in ChatGPT."""
-    stop: Optional[Union[str, List[str]]] = None
-    """Up to 4 sequences where the API will stop generating further tokens."""
-    max_tokens: Optional[int] = None
+    """Whether to stream back partial progress."""
+    logprobs: Optional[int] = Field(None, ge=0, le=5)
     """
-    The maximum number of tokens allowed for the generated answer.
+    Include the log probabilities on the `logprobs` most likely tokens, as well the
+    chosen tokens.
 
-    By default, the number of tokens the model can return will be (4096 - prompt
-    tokens).
+    For example, if `logprobs` is 5, the API will return a list of the 5 most likely
+    tokens. The API will always return the `logprob` of the sampled token, so there may
+    be up to `logprobs+1` elements in the response The maximum value for `logprobs` is
+    5.
+    """
+    echo: Optional[bool] = False
+    """Echo back the prompt in addition to the completion."""
+    stop: Union[str, List[str], None] = None
+    """
+    Up to 4 sequences where the API will stop generating further tokens.
+
+    The returned text will not contain the stop sequence.
     """
     presence_penalty: Optional[float] = Field(0.0, ge=-2.0, le=2.0)
     """
     Number between -2.0 and 2.0. Positive values penalize new tokens based on whether
     they appear in the text so far, increasing the model's likelihood to talk about new
     topics.
 
@@ -463,45 +476,76 @@
     existing frequency in the text so far, decreasing the model's likelihood to repeat
     the same line verbatim.
 
     See Also
     --------
     [Parameter details](https://platform.openai.com/docs/api-reference/parameter-details)
     """
+    best_of: Optional[int] = Field(1, ge=0, le=20)
+    """
+    Generates `best_of` completions server-side and returns the "best" (the one with the
+    highest log probability per token). Results cannot be streamed.
+
+    When used with `n`, `best_of` controls the number of candidate completions and `n`
+    specifies how many to return - `best_of` must be greater than `n`.
+
+    Notes
+    -----
+    Because this parameter generates many completions, it can quickly consume your token
+    quota. Use carefully and ensure that you have reasonable settings for `max_tokens`
+    and `stop`.
+    """
     logit_bias: Optional[Dict[str, Any]] = None
     """
-    Modify the likelihood of specified tokens appearing in the completion.
+    Modify the likelihood of specified tokens appearing in the completion. Accepts a
+    json object that maps tokens (specified by their token ID in the GPT tokenizer) to
+    an associated bias value from -100 to 100.
 
-    Accepts a json object that maps tokens (specified by their token ID in the
-    tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is
-    added to the logits generated by the model prior to sampling. The exact effect will
-    vary per model, but values between -1 and 1 should decrease or increase likelihood
-    of selection; values like -100 or 100 should result in a ban or exclusive selection
-    of the relevant token.
+    You can use this [tokenizer tool](https://platform.openai.com/tokenizer?view=bpe)
+    (which works for both GPT-2 and GPT-3) to convert text to token IDs. Mathematically,
+    the bias is added to the logits generated by the model prior to sampling. The exact
+    effect will vary per model, but values between -1 and 1 should decrease or increase
+    likelihood of selection; values like -100 or 100 should result in a ban or exclusive
+    selection of the relevant token.
+
+    As an example, you can pass `{"50256": -100}` to prevent the `<|endoftext|>` token
+    from being generated.
     """
     user: Optional[str] = None
     """
     A unique identifier representing your end-user, which can help OpenAI to monitor and
     detect abuse.
 
     See Also
     --------
     [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
-
-    Examples
-    --------
-    - `user="user-1234"`
     """
 
 
-class Edit(BaseModel):
+class Logprobs(BaseModel):
+    tokens: Optional[List[str]] = None
+    token_logprobs: Optional[List[float]] = None
+    top_logprobs: Optional[List[Dict[str, Any]]] = None
+    text_offset: Optional[List[int]] = None
+
+
+class Choice(BaseModel):
+    text: Optional[str] = None
+    index: Optional[int] = None
+    logprobs: Optional[Logprobs] = None
+    finish_reason: Optional[FinishReason] = None  # can't be FUNCTION_CALL
+
+
+class Completion(BaseModel):
+    id: str
     object: str
     created: int
+    model: str
     choices: List[Choice]
-    usage: Usage
+    usage: Optional[Usage] = None
 
     @property
     def texts(self) -> List[str]:
         """
         List of texts from the choices.
 
         Returns
@@ -515,27 +559,27 @@
     def text(self) -> str:
         """
         The concatenation of the generated texts.
 
         Returns
         -------
         str
-            Concatenated text.
+            Concatenated texts.
         """
         return "".join(self.texts)
 
 
-class EditRequest(BaseModel):
-    model: str
-    """
-    ID of the model to use.
+class EditModel(str, Enum):
+    TEXT_DAVINCI_EDIT_001 = "text-davinci-edit-001"
+    CODE_DAVINCI_EDIT_001 = "code-davinci-edit-001"
 
-    You can use the `text-davinci-edit-001` or `code-davinci-edit-001` model with this
-    endpoint.
-    """
+
+class EditRequest(BaseModel):
+    model: Union[str, EditModel]
+    """ID of the model to use."""
     input: Optional[str] = ""
     """The input text to use as a starting point for the edit."""
     instruction: str
     """The instruction that tells the model how to edit the prompt."""
     n: Optional[int] = Field(1, ge=1, le=20)
     """How many edits to generate for the input and instruction."""
     temperature: Optional[float] = Field(1.0, ge=0.0, le=2.0)
@@ -552,22 +596,43 @@
     model considers the results of the tokens with top_p probability mass. So 0.1 means
     only the tokens comprising the top 10% probability mass are considered.
 
     We generally recommend altering this or `temperature` but not both.
     """
 
 
-class ImageDatum(BaseModel):
-    url: Optional[str] = None
-    b64_json: Optional[str] = None
+class Edit(BaseModel):
+    object: str
+    created: int
+    choices: List[Choice]
+    usage: Usage
 
+    @property
+    def texts(self) -> List[str]:
+        """
+        List of texts from the choices.
 
-class ImageList(BaseModel):
-    created: int
-    data: List[ImageDatum]
+        Returns
+        -------
+        List[str]
+            List of texts.
+        """
+        return [c.text for c in self.choices if c.text is not None]
+
+    @property
+    def text(self) -> str:
+        """
+        The concatenation of the generated texts.
+
+        Returns
+        -------
+        str
+            Concatenated text.
+        """
+        return "".join(self.texts)
 
 
 class ImageSize(str, Enum):
     """The size of the generated images."""
 
     SQUARE_256 = "256x256"
     SQUARE_512 = "512x512"
@@ -583,18 +648,14 @@
 
 class ImageRequest(BaseModel):
     prompt: str = Field(..., max_length=1000)
     """
     A text description of the desired image(s).
 
     The maximum length is 1000 characters.
-
-    Examples
-    --------
-    - `prompt="A cute baby sea otter"`
     """
     n: Optional[int] = Field(1, ge=1, le=10)
     """
     The number of images to generate.
 
     Must be between 1 and 10.
     """
@@ -606,45 +667,47 @@
     """
     A unique identifier representing your end-user, which can help OpenAI to monitor and
     detect abuse.
 
     See Also
     --------
     [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
-
-    Examples
-    --------
-    - `user="user-1234"`
     """
 
 
-class ImageEditing(BaseModel):
+class ImageDatum(BaseModel):
+    url: Optional[str] = None
+    b64_json: Optional[str] = None
+
+
+class ImageList(BaseModel):
+    created: int
+    data: List[ImageDatum]
+
+
+class ImageEditRequest(BaseModel):
     image: Path
     """
-    The image to edit.
+    The path of image to edit.
 
     Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image
     must have transparency, which will be used as the mask.
     """
     mask: Optional[Path] = None
     """
-    An additional image whose fully transparent areas (e.g. where alpha is zero)
+    An additional path of image whose fully transparent areas (e.g. where alpha is zero)
     indicate where `image` should be edited.
 
     Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.
     """
     prompt: str = Field(..., max_length=1000)
     """
     A text description of the desired image(s).
 
     The maximum length is 1000 characters.
-
-    Examples
-    --------
-    - `prompt="A cute baby sea otter wearing a beret"`
     """
     n: Optional[int] = Field(1, ge=1, le=10)
     """
     The number of images to generate.
 
     Must be between 1 and 10.
     """
@@ -656,25 +719,21 @@
     """
     A unique identifier representing your end-user, which can help OpenAI to monitor and
     detect abuse.
 
     See Also
     --------
     [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
-
-    Examples
-    --------
-    - `user="user-1234"`
     """
 
 
-class ImageVariation(BaseModel):
+class ImageVariationRequest(BaseModel):
     image: Path
     """
-    The image to use as the basis for the variation(s).
+    The path of image to use as the basis for the variation(s).
 
     Must be a valid PNG file, less than 4MB, and square.
     """
     n: Optional[int] = Field(1, ge=1, le=10)
     """
     The number of images to generate.
 
@@ -688,18 +747,40 @@
     """
     A unique identifier representing your end-user, which can help OpenAI to monitor and
     detect abuse.
 
     See Also
     --------
     [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
+    """
+
 
-    Examples
+class EmbeddingModel(str, Enum):
+    TEXT_EMBEDDING_ADA_002 = "text-embedding-ada-002"
+
+
+class EmbeddingRequest(BaseModel):
+    model: Union[str, EmbeddingModel]
+    """ID of the model to use."""
+    input: Union[str, List[str], List[int], List[List[int]]]
+    """
+    Input text to embed, encoded as a string or array of tokens.
+
+    To embed multiple inputs in a single request, pass an array of strings or array of
+    token arrays. Each input must not exceed the max input tokens for the model (8191
+    tokens for `text-embedding-ada-002`).
+    """
+    user: Optional[str] = None
+    """
+    A unique identifier representing your end-user, which can help OpenAI to monitor and
+    detect abuse.
+
+    See Also
     --------
-    - `user="user-1234"`
+    [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
     """
 
 
 class EmbeddingDatum(BaseModel):
     index: int
     object: str
     embedding: List[float]
@@ -725,93 +806,35 @@
         -------
         List[List[float]]
             List of embeddings.
         """
         return [d.embedding for d in self.data]
 
 
-class EmbeddingRequest(BaseModel):
-    model: str
-    """ID of the model to use."""
-    input: Union[str, List[str], List[int], List[List[int]]]
-    """
-    Input text to get embeddings for, encoded as a string or array of tokens.
-
-    To get embeddings for multiple inputs in a single request, pass an array of strings
-    or array of token arrays. Each input must not exceed 8192 tokens in length.
-
-    Examples
-    --------
-    - `input="This is a test."`
-    - `input=["This is a test."]`
-    - `input=[1212, 318, 257, 1332, 13]`
-    - `input=[[1212, 318, 257, 1332, 13]]`
-    """
-    user: Optional[str] = None
-    """
-    A unique identifier representing your end-user, which can help OpenAI to monitor and
-    detect abuse.
-
-    See Also
-    --------
-    [End-user IDs](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids)
-
-    Examples
-    --------
-    - `user="user-1234"`
-    """
-
-
-class TranscriptionJson(BaseModel):
-    text: str
-
-
-class Segment(BaseModel):
-    id: int
-    seek: int
-    start: float
-    end: float
-    text: str
-    tokens: List[int]
-    temperature: float
-    avg_logprob: float
-    compression_ratio: float
-    no_speech_prob: float
-    transient: bool
-
-
-class TranscriptionVerboseJson(BaseModel):
-    task: str
-    language: str
-    duration: float
-    segments: List[Segment]
-    text: str
+class AudioModel(str, Enum):
+    WHISPER_1 = "whisper-1"
 
 
 class TranscriptionFormat(str, Enum):
     """The format of the transcript output."""
 
     JSON = "json"
     TEXT = "text"
     SRT = "srt"
     VERBOSE_JSON = "verbose_json"
     VTT = "vtt"
 
 
 class TranscriptionRequest(BaseModel):
     file: Path
-    """The audio file to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a,
-    wav, or webm.
-    """
-    model: str
-    """
-    ID of the model to use.
-
-    Only `whisper-1` is currently available.
+    """The path of audio file to transcribe, in one of these formats: mp3, mp4, mpeg,
+    mpga, m4a, wav, or webm.
     """
+    model: Union[str, AudioModel]
+    """ID of the model to use."""
     prompt: Optional[str] = None
     """
     An optional text to guide the model's style or continue a previous audio segment.
 
     The [prompt](https://platform.openai.com/docs/guides/speech-to-text/prompting)
     should match the audio language.
     """
@@ -831,25 +854,47 @@
     The language of the input audio.
 
     Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
     format will improve accuracy and latency.
     """
 
 
+class TranscriptionJson(BaseModel):
+    text: str
+
+
+class Segment(BaseModel):
+    id: int
+    seek: int
+    start: float
+    end: float
+    text: str
+    tokens: List[int]
+    temperature: float
+    avg_logprob: float
+    compression_ratio: float
+    no_speech_prob: float
+    transient: bool
+
+
+class TranscriptionVerboseJson(BaseModel):
+    task: str
+    language: str
+    duration: float
+    segments: List[Segment]
+    text: str
+
+
 class TranslationRequest(BaseModel):
     file: Path
-    """The audio file to translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a,
-    wav, or webm.
-    """
-    model: str
-    """
-    ID of the model to use.
-
-    Only `whisper-1` is currently available.
+    """The path of audio file to translate, in one of these formats: mp3, mp4, mpeg,
+    mpga, m4a, wav, or webm.
     """
+    model: Union[str, AudioModel]
+    """ID of the model to use."""
     prompt: Optional[str] = None
     """
     An optional text to guide the model's style or continue a previous audio segment.
 
     The [prompt](https://platform.openai.com/docs/guides/speech-to-text/prompting)
     should be in English.
     """
@@ -879,74 +924,29 @@
 
 class FileList(BaseModel):
     object: str
     data: List[File]
 
     @property
     def ids(self) -> List[str]:
-        """
-        List of file IDs.
-
-        Returns
-        -------
-        List[str]
-            List of file IDs.
-        """
+        """List of file IDs."""
         return [d.id for d in self.data]
 
 
 class DeletionResult(BaseModel):
     id: str
     object: str
     deleted: bool
 
 
-class FineTuneEvent(BaseModel):
-    object: str
-    created_at: int
-    level: str
-    message: str
-
-
-class FineTuneEventList(BaseModel):
-    object: str
-    data: List[FineTuneEvent]
-
-
-class FineTune(BaseModel):
-    id: str
-    object: str
-    created_at: int
-    updated_at: int
-    model: str
-    fine_tuned_model: Optional[str] = None
-    organization_id: str
-    status: str
-    hyperparams: Dict[str, Any]
-    training_files: List[File]
-    validation_files: List[File]
-    result_files: List[File]
-    events: Optional[List[FineTuneEvent]] = None
-
-
-class FineTuneList(BaseModel):
-    object: str
-    data: List[FineTune]
-
-    @property
-    def ids(self) -> List[str]:
-        """
-        List of fine-tune job IDs.
-
-        Returns
-        -------
-        List[str]
-            List of fine-tune job IDs.
-        """
-        return [d.id for d in self.data]
+class FineTuneModel(str, Enum):
+    ADA = "ada"
+    BABBAGE = "babbage"
+    CURIE = "curie"
+    DAVINCI = "davinci"
 
 
 class FineTuneRequest(BaseModel):
     training_file: str
     """
     The ID of an uploaded file that contains training data.
 
@@ -961,28 +961,28 @@
     --------
     [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning/creating-training-data)
     """
     validation_file: Optional[str] = None
     """
     The ID of an uploaded file that contains validation data.
 
-    If you provide this file, the data is used to generate validation
-    metrics periodically during fine-tuning. These metrics can be viewed in the
-    [fine-tuning results file](https://platform.openai.com/docs/guides/fine-tuning/analyzing-your-fine-tuned-model)
+    If you provide this file, the data is used to generate validation metrics
+    periodically during fine-tuning. These metrics can be viewed in the
+    [fine-tuning results file](https://platform.openai.com/docs/guides/fine-tuning/analyzing-your-fine-tuned-model).
     Your train and validation data should be mutually exclusive.
 
-    Your dataset must be formatted as a JSONL file, where each validation
-    example is a JSON object with the keys "prompt" and "completion".
-    Additionally, you must upload your file with the purpose `fine-tune`.
+    Your dataset must be formatted as a JSONL file, where each validation example is a
+    JSON object with the keys "prompt" and "completion". Additionally, you must upload
+    your file with the purpose `fine-tune`.
 
     See Also
     --------
     [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning/creating-training-data)
     """
-    model: Optional[str] = "curie"
+    model: Union[str, FineTuneModel, None] = FineTuneModel.CURIE
     """
     The name of the base model to fine-tune.
 
     You can select one of "ada", "babbage", "curie", "davinci", or a fine-tuned model
     created after 2022-04-21.
 
     See Also
@@ -1063,14 +1063,52 @@
     A string of up to 40 characters that will be added to your fine-tuned model name.
 
     For example, a `suffix` of "custom-model-name" would produce a model name like
     `ada:ft-your-org:custom-model-name-2022-02-15-04-21-04`.
     """
 
 
+class FineTuneEvent(BaseModel):
+    object: str
+    created_at: int
+    level: str
+    message: str
+
+
+class FineTune(BaseModel):
+    id: str
+    object: str
+    created_at: int
+    updated_at: int
+    model: str
+    fine_tuned_model: Optional[str] = None
+    organization_id: str
+    status: str
+    hyperparams: Dict[str, Any]
+    training_files: List[File]
+    validation_files: List[File]
+    result_files: List[File]
+    events: Optional[List[FineTuneEvent]] = None
+
+
+class FineTuneList(BaseModel):
+    object: str
+    data: List[FineTune]
+
+    @property
+    def ids(self) -> List[str]:
+        """List of fine-tune job IDs."""
+        return [d.id for d in self.data]
+
+
+class FineTuneEventList(BaseModel):
+    object: str
+    data: List[FineTuneEvent]
+
+
 class ModelPermission(BaseModel):
     id: str
     object: str
     created: int
     allow_create_engine: bool
     allow_sampling: bool
     allow_logprobs: bool
@@ -1094,43 +1132,64 @@
 
 class ModelList(BaseModel):
     object: str
     data: List[Model]
 
     @property
     def ids(self) -> List[str]:
-        """
-        List of model IDs.
-
-        Returns
-        -------
-        List[str]
-            List of model IDs.
-        """
+        """List of model IDs."""
         return [d.id for d in self.data]
 
 
+class ModerationModel(str, Enum):
+    TEXT_MODERATION_LATEST = "text-moderation-latest"
+    TEXT_MODERATION_STABLE = "text-moderation-stable"
+
+
+class ModerationRequest(BaseModel):
+    input: Union[str, List[str]]
+    """The input text to classify."""
+    model: Optional[
+        Union[str, ModerationModel]
+    ] = ModerationModel.TEXT_MODERATION_LATEST
+    """
+    The default is `ModerationModel.TEXT_MODERATION_LATEST` which will be automatically
+    upgraded over time. This ensures you are always using our most accurate model. If
+    you use `ModerationModel.TEXT_MODERATION_STABLE`, we will provide advanced notice
+    before updating the model. Accuracy of `ModerationModel.TEXT_MODERATION_STABLE` may
+    be slightly lower than for `ModerationModel.TEXT_MODERATION_LATEST`.
+    """
+
+
 class Categories(BaseModel):
     hate: bool
     hate_threatening: bool = Field(..., alias="hate/threatening")
     self_harm: bool = Field(..., alias="self-harm")
+    self_harm_instructions: Optional[bool] = Field(alias="self-harm/instructions")
+    self_harm_intent: Optional[bool] = Field(alias="self-harm/intent")
     sexual: bool
     sexual_minors: bool = Field(..., alias="sexual/minors")
     violence: bool
     violence_graphic: bool = Field(..., alias="violence/graphic")
+    harassment: Optional[bool]
+    harassment_threatening: Optional[bool] = Field(alias="harassment/threatening")
 
 
 class CategoryScores(BaseModel):
     hate: float
     hate_threatening: float = Field(..., alias="hate/threatening")
     self_harm: float = Field(..., alias="self-harm")
+    self_harm_instructions: Optional[float] = Field(alias="self-harm/instructions")
+    self_harm_intent: Optional[float] = Field(alias="self-harm/intent")
     sexual: float
     sexual_minors: float = Field(..., alias="sexual/minors")
     violence: float
     violence_graphic: float = Field(..., alias="violence/graphic")
+    harassment: Optional[float]
+    harassment_threatening: Optional[float] = Field(alias="harassment/threatening")
 
 
 class ModerationResult(BaseModel):
     flagged: bool
     """Set to `True` if the model classifies the content as violating OpenAI's usage
     policies, `False` otherwise.
     """
@@ -1153,52 +1212,32 @@
 
 class Moderation(BaseModel):
     id: str
     model: str
     results: List[ModerationResult]
 
 
-class ModerationRequest(BaseModel):
-    input: Union[str, List[str]]
-    """The input text to classify."""
-    model: Optional[str] = "text-moderation-latest"
-    """
-    Two content moderations models are available: `text-moderation-stable` and `text-
-    moderation-latest`.
-
-    The default is `text-moderation-latest` which will be automatically upgraded over
-    time. This ensures you are always using our most accurate model. If you use `text-
-    moderation-stable`, we will provide advanced notice before updating the model.
-    Accuracy of `text-moderation-stable` may be slightly lower than for `text-
-    moderation-latest`.
-    """
-
-
 class OpenAiApi:
     """
-    Client implementation for the OpenAI API version `1.2.0`.
+    Client implementation for the OpenAI API version `2.0.0`.
 
     See Also
     --------
     [Official API specification](https://github.com/openai/openai-openapi/blob/master/openapi.yaml)
-
-    Notes
-    -----
-    Clients for deprecated APIs are not implemented.
     """
 
     def __init__(
         self,
         key: str,
         organization_id: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
         base_url: Optional[str] = "https://api.openai.com/v1",
     ) -> None:
         """
-        Initialize a client for the OpenAI API version `1.2.0`.
+        Initialize a client for the OpenAI API version `2.0.0`.
 
         Parameters
         ----------
         key : str
             API key for authentication, which can be found on the [API Keys page](https://platform.openai.com/account/api-keys).
         organization_id : Optional[str]
             Optional value used to specify which organization's subscription quota is
@@ -1230,263 +1269,260 @@
         self, key: str, organization_id: Optional[str]
     ) -> Dict[str, str]:
         headers = {"Authorization": f"Bearer {key}"}
         if organization_id is not None:
             headers["OpenAI-Organization"] = organization_id
         return headers
 
-    def create_completion(
-        self, completion_request: CompletionRequest
-    ) -> Union[Generator[Completion, None, None], Completion]:
+    def create_chat_completion(
+        self, req: ChatCompletionRequest
+    ) -> Union[Generator[ChatCompletion, None, None], ChatCompletion]:
         """
-        Create a completion for the provided prompt and parameters.
+        Create a model response for the given chat conversation.
 
         Parameters
         ----------
-        completion_request : CompletionRequest
-            Specification of the completion to create.
+        req : ChatCompletionRequest
+            Specification of the chat completion to create.
 
         Returns
         -------
-        Union[Generator[Completion, None, None], Completion]:
-            Generator that streams the `Completion` if `completion_request.stream` is
-            `True`, or created `Completion` instance otherwise.
+        Union[Generator[ChatCompletion, None, None], ChatCompletion]
+            Generator that streams the `ChatCompletion` if `req.stream` is `True`, or
+            created `ChatCompletion` instance otherwise.
 
         See Also
         --------
-        [Official API reference](https://platform.openai.com/docs/api-reference/completions/create)
+        [Official API reference](https://platform.openai.com/docs/api-reference/chat/create)
         """
         kwargs = {
             "method": "POST",
-            "path": "/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "path": "/chat/completions",
+            "json": req.dict(exclude_none=True),
         }
 
-        if completion_request.stream is True:
-            return self._stream(Completion, **kwargs)  # type: ignore[return-value]
+        if req.stream is True:
+            return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return ChatCompletion.parse_obj(response.json())
 
-    def create_chat_completion(
-        self, chat_completion_request: ChatCompletionRequest
-    ) -> Union[Generator[ChatCompletion, None, None], ChatCompletion]:
+    def create_completion(
+        self, req: CompletionRequest
+    ) -> Union[Generator[Completion, None, None], Completion]:
         """
-        Create a completion for the chat message.
+        Create a completion for the provided prompt and parameters.
 
         Parameters
         ----------
-        chat_completion_request : ChatCompletionRequest
-            Specification of the chat completion to create.
+        req : CompletionRequest
+            Specification of the completion to create.
 
         Returns
         -------
-        Union[Generator[ChatCompletion, None, None], ChatCompletion]
-            Generator that streams the `ChatCompletion` if
-            `chat_completion_request.stream` is `True`, or created `ChatCompletion`
-            instance otherwise.
+        Union[Generator[Completion, None, None], Completion]:
+            Generator that streams the `Completion` if `req.stream` is `True`, or
+            created `Completion` instance otherwise.
 
         See Also
         --------
-        [Official API reference](https://platform.openai.com/docs/api-reference/chat/create)
+        [Official API reference](https://platform.openai.com/docs/api-reference/completions/create)
         """
         kwargs = {
             "method": "POST",
-            "path": "/chat/completions",
-            "json": chat_completion_request.dict(exclude_none=True),
+            "path": "/completions",
+            "json": req.dict(exclude_none=True),
         }
 
-        if chat_completion_request.stream is True:
-            return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
+        if req.stream is True:
+            return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return ChatCompletion.parse_obj(response.json())
+        return Completion.parse_obj(response.json())
 
-    def create_edit(self, edit_request: EditRequest) -> Edit:
+    def create_edit(self, req: EditRequest) -> Edit:
         """
         Create a new edit for the provided input, instruction, and parameters.
 
         Parameters
         ----------
-        edit_request : EditRequest
+        req : EditRequest
             Specification of the edit to create.
 
         Returns
         -------
         Edit
             Created `Edit` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/edits/create)
         """
-        response = self._request(
-            "POST", "/edits", json=edit_request.dict(exclude_none=True)
-        )
+        response = self._request("POST", "/edits", json=req.dict(exclude_none=True))
         return Edit.parse_obj(response.json())
 
-    def create_images(self, image_request: ImageRequest) -> ImageList:
+    def create_images(self, req: ImageRequest) -> ImageList:
         """
         Create images given a prompt.
 
         Parameters
         ----------
-        image_request: ImageRequest
+        req: ImageRequest
             Specification of the images to create.
 
         Returns
         -------
         ImageList
             Created `ImageList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create)
         """
         response = self._request(
-            "POST", "/images/generations", json=image_request.dict(exclude_none=True)
+            "POST", "/images/generations", json=req.dict(exclude_none=True)
         )
         return ImageList.parse_obj(response.json())
 
-    def edit_image(self, image_editing: ImageEditing) -> ImageList:
+    def edit_image(self, req: ImageEditRequest) -> ImageList:
         """
         Create edited or extended images given an original image and a prompt.
 
         Parameters
         ----------
-        image_editing : ImageEditing
+        req : ImageEditRequest
             Specification of the images to create.
 
         Returns
         -------
         ImageList
             Edited or extended `ImageList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create-edit)
         """
-        response = self._request(
-            "POST", "/images/edits", **kwargs_for_uploading(image_editing)
-        )
+        response = self._request("POST", "/images/edits", **kwargs_for_uploading(req))
         return ImageList.parse_obj(response.json())
 
-    def create_image_variation(self, image_variation: ImageVariation) -> ImageList:
+    def create_image_variation(self, req: ImageVariationRequest) -> ImageList:
         """
         Create a variation of a given image.
 
         Parameters
         ----------
-        image_variation : ImageVariation
+        req : ImageVariationRequest
             Specification of the images to create.
 
         Returns
         -------
         ImageList
             Created `ImageList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create-variation)
         """
         response = self._request(
-            "POST", "/images/variations", **kwargs_for_uploading(image_variation)
+            "POST", "/images/variations", **kwargs_for_uploading(req)
         )
         return ImageList.parse_obj(response.json())
 
-    def create_embedding(self, embedding_request: EmbeddingRequest) -> Embedding:
+    def create_embedding(self, req: EmbeddingRequest) -> Embedding:
         """
         Create an embedding vector representing the input text.
 
         Parameters
         ----------
-        embedding_request : EmbeddingRequest
+        req : EmbeddingRequest
             Specification of the embedding to create.
 
         Returns
         -------
         Embedding
             Created `Embedding` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/embeddings/create)
         """
         response = self._request(
-            "POST", "/embeddings", json=embedding_request.dict(exclude_none=True)
+            "POST", "/embeddings", json=req.dict(exclude_none=True)
         )
         return Embedding.parse_obj(response.json())
 
     def transcribe_audio(
-        self, transcription_request: TranscriptionRequest
+        self, req: TranscriptionRequest
     ) -> Union[TranscriptionJson, TranscriptionVerboseJson, str]:
         """
         Transcribe audio into the input language.
 
         Parameters
         ----------
-        transcription_request : TranscriptionRequest
+        req : TranscriptionRequest
             Specification of the transcription to create.
 
         Returns
         -------
         Union[TranscriptionJson, TranscriptionVerboseJson, str]
-            Created `TranscriptionJson` instance if
-            `transcription_request.response_format` is `TranscriptionFormat.JSON`,
-            created `TranscriptionVerboseJson` instance if
-            `transcription_request.response_format` is
-            `TranscriptionFormat.VERBOSE_JSON`, or `str` otherwise.
+            Created `TranscriptionJson` instance if `req.response_format` is
+            `TranscriptionFormat.JSON`, created `TranscriptionVerboseJson` instance if
+            `req.response_format` is `TranscriptionFormat.VERBOSE_JSON`, or `str`
+            otherwise.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/audio/create)
         """
         response = self._request(
             "POST",
             "/audio/transcriptions",
-            **kwargs_for_uploading(transcription_request),
+            **kwargs_for_uploading(req),
         )
 
-        if transcription_request.response_format is TranscriptionFormat.JSON:
+        if req.response_format is TranscriptionFormat.JSON:
             return TranscriptionJson.parse_obj(response.json())
 
-        if transcription_request.response_format is TranscriptionFormat.VERBOSE_JSON:
+        if req.response_format is TranscriptionFormat.VERBOSE_JSON:
             return TranscriptionVerboseJson.parse_obj(response.json())
 
         # text, srt or vtt
         return str(response.text)
 
     def translate_audio(
-        self, translation_request: TranslationRequest
+        self, req: TranslationRequest
     ) -> Union[TranscriptionJson, TranscriptionVerboseJson, str]:
         """
-        Translate audio into into English.
+        Translate audio into English.
 
         Parameters
         ----------
-        translation_request : TranslationRequest
-            Specification of the transcription to create.
+        req : TranslationRequest
+            Specification of the translation to create.
 
         Returns
         -------
         Union[TranscriptionJson, TranscriptionVerboseJson, str]
-            Created `Edit` instance.
+            Created `TranscriptionJson` instance if `req.response_format` is
+            `TranscriptionFormat.JSON`, created `TranscriptionVerboseJson` instance if
+            `req.response_format` is `TranscriptionFormat.VERBOSE_JSON`, or `str`
+            otherwise.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/audio/create)
         """
         response = self._request(
-            "POST", "/audio/translations", **kwargs_for_uploading(translation_request)
+            "POST", "/audio/translations", **kwargs_for_uploading(req)
         )
 
-        if translation_request.response_format is TranscriptionFormat.JSON:
+        if req.response_format is TranscriptionFormat.JSON:
             return TranscriptionJson.parse_obj(response.json())
 
-        if translation_request.response_format is TranscriptionFormat.VERBOSE_JSON:
+        if req.response_format is TranscriptionFormat.VERBOSE_JSON:
             return TranscriptionVerboseJson.parse_obj(response.json())
 
         # text, srt or vtt
         return str(response.text)
 
     def list_files(self) -> FileList:
         """
@@ -1532,55 +1568,55 @@
         [Official API reference](https://platform.openai.com/docs/api-reference/files/upload)
         """
         data = {"purpose": purpose}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
         return File.parse_obj(response.json())
 
-    def get_file(self, file_id: str) -> File:
+    def delete_file(self, file_id: str) -> DeletionResult:
         """
-        Return information about a specific file.
+        Delete a file.
 
         Parameters
         ----------
         file_id : str
             ID of the file.
 
         Returns
         -------
-        File
-            Specified `File` instance.
+        DeletionResult
+            `DeletionResult` instance.
 
         See Also
         --------
-        [Official API reference](https://platform.openai.com/docs/api-reference/files/retrieve)
+        [Official API reference](https://platform.openai.com/docs/api-reference/files/delete)
         """
-        response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        response = self._request("DELETE", f"/files/{file_id}")
+        return DeletionResult.parse_obj(response.json())
 
-    def delete_file(self, file_id: str) -> DeletionResult:
+    def get_file(self, file_id: str) -> File:
         """
-        Delete a file.
+        Return information about a specific file.
 
         Parameters
         ----------
         file_id : str
             ID of the file.
 
         Returns
         -------
-        DeletionResult
-            `DeletionResult` instance.
+        File
+            Specified `File` instance.
 
         See Also
         --------
-        [Official API reference](https://platform.openai.com/docs/api-reference/files/delete)
+        [Official API reference](https://platform.openai.com/docs/api-reference/files/retrieve)
         """
-        response = self._request("DELETE", f"/files/{file_id}")
-        return DeletionResult.parse_obj(response.json())
+        response = self._request("GET", f"/files/{file_id}")
+        return File.parse_obj(response.json())
 
     def download_file(self, file_id: str) -> str:
         """
         Return the contents of the specified file.
 
         Parameters
         ----------
@@ -1595,57 +1631,57 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/files/retrieve-content)
         """
         response = self._request("GET", f"/files/{file_id}/content")
         return str(response.text)
 
-    def list_fine_tunes(self) -> FineTuneList:
-        """
-        List your organization's fine-tuning jobs.
-
-        Returns
-        -------
-        FineTuneList
-            `FineTuneList` instance.
-
-        See Also
-        --------
-        [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/list)
-        """
-        response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
-
-    def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
+    def create_fine_tune(self, req: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given dataset.
 
         Response includes details of the enqueued job including job status and the name
         of the fine-tuned models once complete.
 
         Parameters
         ----------
-        fine_tune_request : FineTuneRequest
+        req : FineTuneRequest
             Specification of the fine-tune job to create.
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
 
         See Also
         --------
         - [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/create)
         - [Learn more about Fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=req.dict(exclude_none=True)
         )
         return FineTune.parse_obj(response.json())
 
+    def list_fine_tunes(self) -> FineTuneList:
+        """
+        List your organization's fine-tuning jobs.
+
+        Returns
+        -------
+        FineTuneList
+            `FineTuneList` instance.
+
+        See Also
+        --------
+        [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/list)
+        """
+        response = self._request("GET", "/fine-tunes")
+        return FineTuneList.parse_obj(response.json())
+
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get info about the fine-tune job.
 
         Parameters
         ----------
         fine_tune_id : str
@@ -1776,35 +1812,35 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/delete-model)
         """
         response = self._request("DELETE", f"/models/{model_id}")
         return DeletionResult.parse_obj(response.json())
 
-    def create_moderation(self, moderation_request: ModerationRequest) -> Moderation:
+    def create_moderation(self, req: ModerationRequest) -> Moderation:
         """
         Classify if text violates OpenAI's Content Policy.
 
         Notes
         -----
         OpenAI will continuously upgrade the moderation endpoint's underlying model.
         Therefore, custom policies that rely on `category_scores` may need recalibration
         over time.
 
         Parameters
         ----------
-        moderation_request : ModerationRequest
+        req : ModerationRequest
             Specification of the moderation to create.
 
         Returns
         -------
         Moderation
             Created `Moderation` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/moderations/create)
         """
         response = self._request(
-            "POST", "/moderations", json=moderation_request.dict(exclude_none=True)
+            "POST", "/moderations", json=req.dict(exclude_none=True)
         )
         return Moderation.parse_obj(response.json())
```

### Comparing `gpru-0.1.0/.gitignore` & `gpru-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/LICENSE` & `gpru-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/README.md` & `gpru-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,20 +42,27 @@
 **Notes** Before anything else, you must ensure that the [API key](https://platform.openai.com/account/api-keys) is set as an environment variable named `OPENAI_API_KEY`.
 
 Here is an example of [chat completion](https://platform.openai.com/docs/api-reference/chat/create), also known as [ChatGPT](https://chat.openai.com/).
 
 ```python
 import os
 
-from gpru.openai.api import ChatCompletionRequest, OpenAiApi, UserMessage
+from gpru.openai.api import (
+    ChatCompletionModel,
+    ChatCompletionRequest,
+    OpenAiApi,
+    UserMessage,
+)
 
 key = os.environ["OPENAI_API_KEY"]
 api = OpenAiApi(key)
 
-req = ChatCompletionRequest(model="gpt-3.5-turbo", messages=[UserMessage("Hello!")])
+req = ChatCompletionRequest(
+    model=ChatCompletionModel.GPT_35_TURBO, messages=[UserMessage("Hello!")]
+)
 chat_completion = api.create_chat_completion(req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
 
 ### Azure OpenAI API
```

### Comparing `gpru-0.1.0/pyproject.toml` & `gpru-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpru-0.1.0/PKG-INFO` & `gpru-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpru
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unofficial Python client library for the OpenAI and Azure OpenAI APIs
 Project-URL: Documentation, https://github.com/sincekmori/gpru#readme
 Project-URL: Issues, https://github.com/sincekmori/gpru/issues
 Project-URL: Source, https://github.com/sincekmori/gpru
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -76,20 +76,27 @@
 **Notes** Before anything else, you must ensure that the [API key](https://platform.openai.com/account/api-keys) is set as an environment variable named `OPENAI_API_KEY`.
 
 Here is an example of [chat completion](https://platform.openai.com/docs/api-reference/chat/create), also known as [ChatGPT](https://chat.openai.com/).
 
 ```python
 import os
 
-from gpru.openai.api import ChatCompletionRequest, OpenAiApi, UserMessage
+from gpru.openai.api import (
+    ChatCompletionModel,
+    ChatCompletionRequest,
+    OpenAiApi,
+    UserMessage,
+)
 
 key = os.environ["OPENAI_API_KEY"]
 api = OpenAiApi(key)
 
-req = ChatCompletionRequest(model="gpt-3.5-turbo", messages=[UserMessage("Hello!")])
+req = ChatCompletionRequest(
+    model=ChatCompletionModel.GPT_35_TURBO, messages=[UserMessage("Hello!")]
+)
 chat_completion = api.create_chat_completion(req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
 
 ### Azure OpenAI API
```

