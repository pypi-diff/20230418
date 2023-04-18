# Comparing `tmp/archytas-0.1.0.tar.gz` & `tmp/archytas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.1.0.tar", max compression
+gzip compressed data, was "archytas-0.2.0.tar", max compression
```

## Comparing `archytas-0.1.0.tar` & `archytas-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      334 2023-04-14 14:34:59.436097 archytas-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-14 13:14:38.430129 archytas-0.1.0/archytas/__init__.py
--rw-r--r--   0        0        0     3118 2023-04-14 15:02:51.864528 archytas-0.1.0/archytas/agent.py
--rw-r--r--   0        0        0      513 2023-04-14 15:08:54.164570 archytas-0.1.0/archytas/auth.py
--rw-r--r--   0        0        0     2651 2023-04-14 13:14:38.430129 archytas-0.1.0/archytas/prompt.py
--rw-r--r--   0        0        0     4906 2023-04-14 13:14:38.430129 archytas-0.1.0/archytas/react.py
--rw-r--r--   0        0        0      939 2023-04-14 15:09:52.894770 archytas-0.1.0/archytas/repl.py
--rw-r--r--   0        0        0    12059 2023-04-14 13:14:38.430129 archytas-0.1.0/archytas/tools.py
--rw-r--r--   0        0        0      729 2023-04-14 14:43:33.141350 archytas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 archytas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2577 2023-04-18 18:03:59.444618 archytas-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/agent.py
+-rw-r--r--   0        0        0      513 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/auth.py
+-rw-r--r--   0        0        0     6701 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/demo_tools.py
+-rw-r--r--   0        0        0     3229 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/prompt.py
+-rw-r--r--   0        0        0     5548 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/react.py
+-rw-r--r--   0        0        0     1005 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/repl.py
+-rw-r--r--   0        0        0    17317 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/tool_utils.py
+-rw-r--r--   0        0        0     1561 2023-04-18 18:03:59.444618 archytas-0.2.0/archytas/tools.py
+-rw-r--r--   0        0        0      729 2023-04-18 18:03:59.448618 archytas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 archytas-0.2.0/PKG-INFO
```

### Comparing `archytas-0.1.0/archytas/agent.py` & `archytas-0.2.0/archytas/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import logging
-import os
-import toml
+# get openai key from environment or .openai.toml file
+from archytas.auth import add_openai_auth; add_openai_auth()
 import openai
+import logging
 from openai.error import Timeout, APIError, APIConnectionError, RateLimitError, ServiceUnavailableError, InvalidRequestError
 from tenacity import before_sleep_log, retry as tenacity_retry, retry_if_exception_type as retry_if, stop_after_attempt, wait_exponential
 from typing import TypedDict, Literal
 
 
 from rich.spinner import Spinner
 from rich.live import Live
@@ -27,14 +27,16 @@
     user = 'user'
 class Message(TypedDict):
     role: Literal['system', 'assistant', 'user']
     content: str
 
 class Agent:
     def __init__(self, *, model:str='gpt-4', prompt:str="You are a helpful assistant."):
+
+
         self.model = model
         self.system_message: Message = {"role": Role.system, "content": prompt }
         self.messages = []
 
     def query(self, message:str) -> str:
         """Send a user query to the agent. Returns the agent's response"""
         self.messages.append({"role": Role.user, "content": message})
```

### Comparing `archytas-0.1.0/archytas/auth.py` & `archytas-0.2.0/archytas/auth.py`

 * *Files identical despite different names*

### Comparing `archytas-0.1.0/archytas/prompt.py` & `archytas-0.2.0/archytas/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from archytas.tools import get_tool_prompt_description
+from typing import Callable
+from archytas.tool_utils import get_tool_prompt_description, get_tool_names
 
 
 prelude = 'You are the ReAct (Reason & Action) assistant. You act as an interface between a user and the system. Your job is to help the user to complete their tasks.'
 
 tool_intro = '# Tools\nYou have access to the following tools which can help you in your job:'
 
 system_tools = f"""
@@ -14,21 +15,24 @@
     the fail_task tool is used to indicate that you have failed to complete the task. You should use this tool to communicate the reason for the failure to the user. Do not call this tool unless you have given a good effort to complete the task.
     _input_: the reason for the failure
 """.strip()
 
 
 #TODO: there should be some way to give an example relevant to the environment/tools...
 #      or use a system tool for the example
-formatting = f"""
+def formatting(tool_names:list[str]) -> str:
+    tool_names += ['final_answer', 'fail_task']
+    tools_list = ', '.join(tool_names)
+    return f"""
 # Formatting
 Every response you generate should EXACTLY follow this JSON format:
 
 {{
   "thought"    : # you should always think about what you need to do
-  "tool"       : # the name of the tool.  This must be one of: [search, calculator, ask_user, final_answer, fail_task]
+  "tool"       : # the name of the tool. This must be one of: {{{tools_list}}}
   "tool_input" : # the input to the tool
 }}
 
 Do not include any text outside of this JSON object. The user will not be able to see it. You can communicate with the user through the "thought" field or the ask_user tool.
 The tool input must be a valid JSON blob (i.e. null, string, number, boolean, array, or object). The input type will depend on which tool you select, so make sure to follow the instructions for each tool.
 
 For example, if the user asked you what the square-root of 2, you would use the calculator like so:
@@ -43,15 +47,29 @@
 # Notes
 - assume any time based knowledge you have is out of date, and should be looked up. Things like the current date, current world leaders, celebrities ages, etc.
 - You are not very good at arithmetic, so you should generally use tools to do arithmetic for you.
 - The user cannot see your thoughts. If you want to communicate to tell the user something, it should be via the ask_user or final_answer tools.
 """.strip()
 
 
-def build_prompt(tools: list):
+def build_prompt(tools: list[Callable]) -> str:
+    """
+    Build the prompt for the ReAct agent
+    
+    Args:
+        tools (list): A list of tools to use. Each tool should have the @tool decorator. applied.
+    
+    Returns:
+        str: The prompt for the ReAct agent
+    """
+    # collect all the tool names (including class.method names)
+    tool_names = [name for tool in tools for name in get_tool_names(tool)]
+    
     chunks = [prelude, tool_intro]
     for tool in tools:
         chunks.append(get_tool_prompt_description(tool))
-    chunks.extend([system_tools+'\n', formatting+'\n', notes])
+    chunks.append(system_tools+'\n')
+    chunks.append(formatting(tool_names)+'\n')
+    chunks.append(notes)
     return '\n\n'.join(chunks)
```

### Comparing `archytas-0.1.0/archytas/react.py` & `archytas-0.2.0/archytas/react.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from archytas.agent import Agent
 from archytas.prompt import build_prompt
-from archytas.tools import make_tool_dict
+from archytas.tools import ask_user
+from archytas.tool_utils import make_tool_dict
 import json
 from rich import print
 
 
 class FailedTaskError(Exception): ...
 
 class ReActAgent:
-    def __init__(self, *, model:str='gpt-4', tools:list=None, max_errors:int|None=3, max_react_steps:int|None=None, verbose:bool=False):
+    def __init__(self, *, model:str='gpt-4', tools:list=None, allow_ask_user:bool=True, max_errors:int|None=3, max_react_steps:int|None=None, verbose:bool=False):
+        """
+        Create a ReAct agent
+        
+        Args:
+            model (str): The model to use. Defaults to 'gpt-4'. Recommended not to change this. gpt-3.5-turbo doesn't follow the prompt format.
+            tools (list): A list of tools to use. Defaults to None. If None, only the system tools (final_answer, fail_task) will be used.
+            allow_ask_user (bool): Whether to include the ask_user tool, which allows the model to ask the user for clarification. Defaults to True.
+            """
 
         # create a dictionary for looking up tools by name
         tools = tools or []
+        if allow_ask_user: 
+            tools.append(ask_user)
         self.tools = make_tool_dict(tools)
 
         # create the prompt with the tools
         self.prompt = build_prompt(tools)
         self._agent = Agent(model=model, prompt=self.prompt)
 
         # react settings
```

### Comparing `archytas-0.1.0/archytas/tools.py` & `archytas-0.2.0/archytas/tool_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,261 @@
 import inspect
 from docstring_parser import parse as parse_docstring
 from rich import traceback; traceback.install(show_locals=True)
 from textwrap import indent
-from typing import Callable
+from typing import Callable, Any
+import functools
 
 import pdb
 
 
 #TODO: separate system tools from library tools from user tools
 #      ideally system tools will have no library dependencies
 
+#TODO: parse extra long manual page from doc string. man_page can be seen by calling man <tool_name>
+# man_page:str|None=None
+# wrapper._man_page = man_page
 
 
 def tool(*, name:str|None=None):
     """
-    Converts a function into a tool for ReAct agents to use.
+    Decorator to convert a function into a tool for ReAct agents to use.
+
+    Usage:
+    ```
+        @tool()
+        def my_tool(arg:type) -> type:
+            '''
+            Short description of the tool
+
+            Long description of the tool
+
+            Args:
+                arg (type): Description of the argument
+
+            Returns:
+                type: Description of the return value
+
+            Examples:
+                optional description of the example
+                >>> my_tool(arg)
+                result
+            '''
+    ```
+    """
+    def decorator(func:Callable):
+        # check that the decorator is being applied to a function
+        if not inspect.isfunction(func):
+            raise TypeError(f"tool decorator can only be applied to functions or classes. Got {func} of type {type(func)}")
+        
+        # determine if function, or class method, and return the appropriate wrapper
+        if is_class_method(func):
+            return make_method_tool_wrapper(func, name)
+        else:
+            return make_func_tool_wrapper(func, name)
+
+    return decorator
+
+
+def toolset(*, name:str|None=None):
     """
-    def decorator(func):
-        args_list, ret, desc = get_tool_signature(func)
-        def wrapper(args:dict|list|str|int|bool|None):
-            
-            if isinstance(args, dict):
-                result = func(**args)
-            elif isinstance(args, list):
-                result = func(*args)
-            elif isinstance(args, (str, int, bool)):
-                result = func(args)
-            elif args is None:
-                result = func()
-            else:
-                raise TypeError(f"args must be a dict, list, str, int, bool, or None. Got {type(args)}")
-
-            #TODO: structure input args so they can be used to call the function
-            # args = validate_tool_call(func, args, args_list)
-            
-            # result = func(**args)
-
-            #convert the result to a string if it is not already a string
-            if not isinstance(result, str):
-                result = str(result)
-
-            return result
-        #attach usage description to the wrapper function
-        wrapper._name = name if name else func.__name__
-        wrapper._is_tool = True
-        wrapper._args_list = args_list
-        wrapper._ret = ret
-        wrapper._desc = desc
+    Decorator used to convert a class into a toolset for ReAct agents to use.
 
+    Usage:
+    ```
+        @toolset()
+        class MyToolset:
+            '''
+            description of the toolset
+            '''
+
+            def __init__(self, arg1, arg2, ...):
+                # initialize the toolset, set up state, etc.
+                # if has no required arguments, can pass class constructor to agent's list of tools
+                # if has required arguments, must pass an instance to agent's list of tools
+
+            @tool()
+            def my_tool(self, arg:type) -> type:
+                '''
+                Short description of the tool method
+
+                Long description of the tool method
+
+                Args:
+                    arg (type): Description of the argument
+
+                Returns:
+                    type: Description of the return value
+
+                Examples:
+                    optional description of the example
+                    >>> my_tool(arg)
+                    result
+                '''
+
+            @tool()
+            def my_other_tool(self, arg:type) -> type:
+                '''<tool docstring>'''
+    ```
+    """
+    def decorator(cls:type):
+        if not inspect.isclass(cls):
+            raise TypeError(f"toolset decorator can only be applied to classes. Got {cls} of type {type(cls)}")
+
+        #basically just add metadata, and return the class
+        #metadata should include a list of the class's tool methods
+
+        #get the list of @tool methods in the class
+        methods = inspect.getmembers(cls, predicate=inspect.isfunction)
+        methods = [method for name, method in methods if is_tool(method)]
+
+        # get the class docstring description
+        docstring = inspect.getdoc(cls)
+
+        @functools.wraps(cls)
+        def wrapper(*args, **kwargs):
+            # create an instance of the class
+            c = cls(*args, **kwargs)
+
+            # attach the metadata to the instance
+            c._name = name if name else cls.__name__
+            c._is_class_tool_instance = True
+            c._docstring = docstring
+            c._tool_methods = methods
+
+            return c
+
+        # attach the metadata to the class
+        wrapper._name = name if name else cls.__name__
+        wrapper._is_class_tool = True
+        wrapper._docstring = docstring
+        wrapper._tool_methods = methods
+        
         return wrapper
     
     return decorator
 
 
-def get_tool_prompt_description(func):
-    #check that this function has the @tool decorator attached
-    if not hasattr(func, '_is_tool'):
-        raise ValueError(f"Function {func.__name__} does not have the @tool decorator attached")
-    
+
+def make_func_tool_wrapper(func:Callable, name:str|None=None):
+    def wrapper(args:dict|list|str|int|float|bool|None):
+        """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
+        
+        if isinstance(args, dict):
+            result = func(**args)
+        elif isinstance(args, list):
+            result = func(*args)
+        elif isinstance(args, (str, int, float, bool)):
+            result = func(args)
+        elif args is None:
+            result = func()
+        else:
+            raise TypeError(f"args must be a valid json object type (dict, list, str, int, float, bool, or None). Got {type(args)}")
+
+        #convert the result to a string if it is not already a string
+        if not isinstance(result, str):
+            result = str(result)
+
+        return result
+    
+    #attach usage description to the wrapper function
+    args_list, ret, desc = get_tool_signature(func)
+
+    wrapper._name = name if name else func.__name__
+    wrapper._is_function_tool = True
+    wrapper._args_list = args_list
+    wrapper._ret = ret
+    wrapper._desc = desc
+
+    return wrapper
+
+def make_method_tool_wrapper(func:Callable, name:str|None=None):
+    def wrapper(self, args:dict|list|str|int|float|bool|None):
+        """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
+        
+        if isinstance(args, dict):
+            result = func(self, **args)
+        elif isinstance(args, list):
+            result = func(self, *args)
+        elif isinstance(args, (str, int, float, bool)):
+            result = func(self, args)
+        elif args is None:
+            result = func(self)
+        else:
+            raise TypeError(f"args must be a valid json object type (dict, list, str, int, float, bool, or None). Got {type(args)}")
+
+        #convert the result to a string if it is not already a string
+        if not isinstance(result, str):
+            result = str(result)
+
+        return result
+    
+    #attach usage description to the wrapper function
+    args_list, ret, desc = get_tool_signature(func)
+
+    wrapper._name = name if name else func.__name__
+    wrapper._is_method_tool = True
+    wrapper._args_list = args_list
+    wrapper._ret = ret
+    wrapper._desc = desc
+
+    return wrapper
+
+
+
+def is_class_method(func:Callable) -> bool:
+    """checks if a function is part of a class, or a standalone function"""
+    assert inspect.isfunction(func), f"is_class_method can only be used on functions. Got {func}"
+    return func.__qualname__ != func.__name__
+
+def is_tool(obj:Callable|type) -> bool:
+    """checks if an object is a tool function, tool method, or tool class (may not be an instance of a class tool)"""
+    return hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool') or hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance')
+        
+
+def get_tool_name(obj:Callable|type) -> str:
+    """Get the name of the tool, either from the @tool _name field, or the __name__ attribute"""
+    assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
+    return getattr(obj, '_name')
+
+def get_tool_names(obj:Callable|type) -> list[str]:
+    """
+    Get the tool name, or all method names if tool is a class tool
+    """
+    assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
+    
+    if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
+        cls_name = get_tool_name(obj)
+
+        #construct names as cls_name.method_name
+        names = [f"{cls_name}.{get_tool_name(method)}" for method in obj._tool_methods]
+
+        return names
+    
+    #otherwise, just return the name of the tool
+    return [get_tool_name(obj)]
+
+
+
+def get_tool_prompt_description(obj:Callable|type|Any):
+    if hasattr(obj, '_is_class_tool'):
+        return get_tool_class_prompt_description(obj)
+    if hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool'):
+        return get_tool_func_prompt_description(obj)
+    if hasattr(obj, '_is_class_tool_instance'):
+        return get_tool_class_prompt_description(obj)
+
+    raise TypeError(f"get_tool_prompt_description can only be used on @tools. Got {obj}")
+
+def get_tool_func_prompt_description(func:Callable):
+    assert is_tool(func), f"Function {func.__name__} does not have the @tool decorator attached"
+    assert inspect.isfunction(func), f"get_tool_func_prompt_description can only be used on functions. Got {func}"
+
     #get the list of arguments
+    
     args_list = func._args_list
     ret_name, ret_type, ret_description = func._ret
     short_desc, long_desc, examples = func._desc
 
     
     chunks = []
     tab = "    "
@@ -94,47 +287,93 @@
             if arg_default:
                 chunks.append(f", optional")
             chunks.append(f") {arg_desc}")
         chunks.append(f"\n{tab}}}")
 
     #################### OUTPUT ####################
     chunks.append("\n    _output_: ")
-    chunks.append(f"({ret_type.__name__}) {ret_description}")
+    if ret_type is None:
+        chunks.append("None")
+    else:
+        chunks.append(f"({ret_type.__name__}) {ret_description}")
 
 
     ############### EXAMPLES ###############
     #TODO: examples need to be parsed...
 
 
     return ''.join(chunks)
 
 
+def get_tool_class_prompt_description(cls:type):
+    """
+    Get the prompt description for a class tool, including all of its tool methods
+    
+    class description is as follows:
+      class_name (class):
+          full unmodified class docstring
+          methods:
+              <get_tool_func_prompt_description for each method>
+
+    Args:
+        cls (type|Any): The class tool to get the description for, or an instance of a class tool
+    
+    Returns:
+        str: The prompt description for the class tool
+    """
+    assert hasattr(cls, '_is_class_tool') or hasattr(cls, '_is_class_tool_instance'), f"class or instance {cls} does not have the @tool decorator attached"
+
+
+    chunks = []
+    tab = "    "
+
+    ############### NAME/DESCRIPTION ###############
+    chunks.append(f"{cls._name} (class):\n")
+    if cls._docstring:
+        chunks.append(f"{indent(cls._docstring, tab)}\n\n")
+
+    #################### METHODS ####################
+    chunks.append(f"{tab}methods:\n")
+    for method in cls._tool_methods:
+        method_str = get_tool_func_prompt_description(method)
+        chunks.append(f"{indent(method_str, tab*2)}\n\n")
+
+    #strip trailing whitespace
+    return ''.join(chunks).rstrip()
+
 
 
-def get_tool_signature(func) -> tuple[list[tuple[str, type, str|None, str|None]], tuple[str|None, type|None, str|None], tuple[str, str|None, list[str]]]:
+
+def get_tool_signature(func:Callable) -> tuple[list[tuple[str, type, str|None, str|None]], tuple[str|None, type|None, str|None], tuple[str, str|None, list[str]]]:
     """
     Check that the docstring and function signature match for a tool function, and return all function information.
 
     Args:
         func (function): The function to check and extract information from
+        ignore_self (bool): If True, ignore the first argument of the function if it is named 'self'
 
     Returns:
         args_list: A list of tuples (name, type, description, default) for each argument
         ret: A tuple (name, type, description) for the return value
         desc: A tuple (short_description, long_description, examples) from the docstring for the function
     """
+    assert inspect.isfunction(func), f"get_tool_signature can only be used on functions. Got {func}"
+
     # get the function signature from the function and the docstring
     docstring = parse_docstring(func.__doc__)
     signature = inspect.signature(func)
 
+    # determine if self needs to be ignored
+    ignore_self: bool = is_class_method(func)
+
     # Extract argument information from the docstring
     docstring_args = {arg.arg_name: (arg.type_name, arg.description, arg.default) for arg in docstring.params}
 
-    # Extract argument information from the signature
-    signature_args = {k: v.annotation for k, v in signature.parameters.items()}
+    # Extract argument information from the signature (ignore self from class methods)
+    signature_args = {k: v.annotation for i, (k, v) in enumerate(signature.parameters.items()) if not (i == 0 and ignore_self and k == 'self')}
 
     # Check if the docstring argument names match the signature argument names
     if set(docstring_args.keys()) != set(signature_args.keys()):
         raise ValueError(f"Docstring argument names do not match function signature argument names for function '{func.__name__}'")
 
     # Check if the docstring argument types match the signature argument types
     for arg_name, arg_type in signature_args.items():
@@ -145,238 +384,95 @@
     # Generate a list of tuples (name, type, description, default) for each argument
     #TODO: use the signature to determine if an argument is optional or not
     args_list = [(arg_name, signature_args[arg_name], arg_desc, arg_default) for arg_name, (arg_type, arg_desc, arg_default) in docstring_args.items()]
 
     # get the return type and description
     signature_ret_type = signature.return_annotation
 
-    docstring.returns
-    docstring_ret_type = docstring.returns.type_name
+    # # if docstring.returns:
+    # if signature_ret_type == inspect.Signature.empty and docstring.returns is None:
+    #     ...
+    try:
+        docstring_ret_type = docstring.returns.type_name
+    except AttributeError:
+        docstring_ret_type = '_empty'
     if signature_ret_type.__name__ != docstring_ret_type:
         raise ValueError(f"Docstring return type '{docstring_ret_type}' does not match function signature return type '{signature_ret_type.__name__}' for function '{func.__name__}'")
     
     # get the return type and description
-    ret = (docstring.returns.return_name, signature_ret_type, docstring.returns.description)
+    if docstring.returns is None:
+        ret = (None, None, None)
+    else:
+        ret = (docstring.returns.return_name, signature_ret_type, docstring.returns.description)
 
     # get the docstring description and examples
     examples = [example.description for example in docstring.examples]
     desc = (docstring.short_description, docstring.long_description, examples)
     
     return args_list, ret, desc
 
 
-# def validate_tool_call(func, args:dict|str, args_list) -> dict:
-#     if isinstance(args, str):
-#         #coerce the string to the correct type
-#         pdb.set_trace()
-#         name, type, desc, default = args_list[0]
-#         pdb.set_trace()
-#         args = {name: type(args)}
-
-#     #validate that the arguments are correct for this tool
-#     for arg_name, arg_type, arg_desc in args_list:
-#         if arg_name not in args:
-#             raise ValueError(f"Missing argument '{arg_name}' for tool '{func.__name__}'")
-
-#         if not isinstance(args[arg_name], arg_type):
-#             raise ValueError(f"Argument '{arg_name}' for tool '{func.__name__}' must be of type {arg_type.__name__}, got {type(args[arg_name]).__name__}")
-    
-#     return args
-
 
-def make_tool_dict(tools:list[Callable]) -> dict[str, Callable]:
+def make_tool_dict(tools:list[Callable|type|Any]) -> dict[str, Callable]:
     """
     Create a dictionary of tools from a list of tool functions.
 
     Tries to use the '_name' attribute of the @tool function, otherwise uses the function name.
 
     Args:
-        tools (list[Callable]): A list of tool functions
+        tools (list[Callable|type|Any]): A list of tool functions, or tool classes, or instances of tool classes.
 
     Returns:
-        dict[str, Callable]: A dictionary of tools
+        dict[str, Callable]: A dictionary of tools. Class methods of class tools are included as separate functions.
     """
+    #TODO: extract methods from any class tools
     tool_dict = {}
     for tool in tools:
-        name = getattr(tool, '_name', tool.__name__)
-        if name in tool_dict:
-            raise ValueError(f"Tool name '{name}' is already in use")
-        tool_dict[name] = tool
-    return tool_dict
-
-
-
-
-from easyrepl import readl
-@tool()
-def ask_user(query:str) -> str:
-    """
-    Ask the user a question and get their response. 
-    
-    You should ask the user a question if you do not have enough information to complete the task, and there is no suitable tool to help you.
-    
-    Args:
-        query (str): The question to ask the user
-
-    Returns:
-        str: The user's response
-    """
-    return readl(prompt=f'{query} ')
-
-
+        assert is_tool(tool), f"make_tool_dict can only be used on tools. Got {tool}"
+        name = getattr(tool, '_name')
+        
+        
+        if hasattr(tool, '_is_function_tool'):
+            if name in tool_dict:
+                raise ValueError(f"Tool name '{name}' is already in use")
+            tool_dict[name] = tool
+            continue
+        
+        if hasattr(tool, '_is_method_tool'):
+            #TODO: not sure if methods should be allowed since they need usually need a class instance...
+            raise NotImplementedError("Free-floating tool methods are not yet supported")
+            pdb.set_trace()
+        
+
+        # handle if instance of class or class itself
+        if hasattr(tool, '_is_class_tool'):
+            instance = tool()
+        else:
+            assert hasattr(tool, '_is_class_tool_instance'), f"Tool {tool} is not a function, method, or class tool"
+            instance = tool
+
+        for _, method in inspect.getmembers(instance, predicate=inspect.ismethod):
+            if not hasattr(method, '_name'):
+                continue
+            method_name = f'{name}.{method._name}'
+            if method_name in tool_dict:
+                raise ValueError(f"Tool name '{method_name}' is already in use")
+            tool_dict[method_name] = method
 
-from datetime import datetime as dt
-import pytz
-@tool()
-def datetime(format:str='%Y-%m-%d %H:%M:%S %Z', timezone:str='UTC') -> str:
-    """
-    Get the current date and time. 
-    
-    Args:
-        format (str, optional): The format to return the date and time in. Defaults to '%Y-%m-%d %H:%M:%S %Z'.
-        timezone (str, optional): The timezone to return the date and time in. Defaults to 'UTC'.
-
-    Returns:
-        str: The current date and time in the specified format
-    """
-    # TODO: See https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for more information.
-    # TODO: list of valid timezones: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
-    
-    tz = pytz.timezone(timezone)
-    return dt.now(tz).strftime(format)
-
-
-@tool()
-def timestamp() -> float:
-    """
-    Returns the current unix timestamp in seconds
-    
-    Returns:
-        float: The current unix timestamp in seconds 
-
-    Examples:
-        >>> timestamp()
-        1681445698.726113
-    """
-    return dt.now().timestamp()
-
-
-
-
-@tool()
-def fib_n(n:int) -> int:
-    """
-    generate the nth fibonacci number
-
-    Args:
-        n (int): The index of the fibonacci number to get
-
-    Returns:
-        int: The nth fibonacci number
-
-    Examples:
-        >>> fib_n(10)
-        55
-        >>> fib_n(20)
-        6765
-    """
-    n0 = 0
-    n1 = 1
-    for _ in range(n):
-        n0, n1 = n1, n0 + n1
-
-    return n0
-
-
-
-@tool()
-def example_tool(arg1:int, arg2:str='', arg3:dict=None) -> int:
-    """
-    Simple 1 sentence description of the tool
-
-    More detailed description of the tool. This can be multiple lines.
-    Explain more what the tool does, and what it is used for.
-
-    Args:
-        arg1 (int): Description of the first argument.
-        arg2 (str): Description of the second argument. Defaults to ''.
-        arg3 (dict): Description of the third argument. Defaults to {}.
-
-    Returns:
-        int: Description of the return value
-
-    Examples:
-        >>> example_tool(1, 'hello', {'a': 1, 'b': 2})
-        3
-        >>> example_tool(2, 'world', {'a': 1, 'b': 2})
-        4
-    """
-    return 42
-
-@tool()
-def calculator(expression:str) -> float:
-    """
-    A simple calculator tool. Can perform basic arithmetic
-
-    Expressions must contain exactly:
-    - one left operand. Can be a float or integer
-    - one operation. Can be one of + - * / ^ %
-    - one right operand. Can be a float or integer
-
-    multiple chained operations are not currently supported.
-
-    Expressions may not contain parentheses, or multiple operations. 
-    If you want to do a complex calculation, you must do it in multiple steps.
 
-    Args:
-        expression (str): A string containing a mathematical expression.
+    return tool_dict
 
-    Returns:
-        float: The result of the calculation
-    
-    Examples:
-        >>> calculator('22/7')
-        3.142857142857143
-        >>> calculator('3.24^2')
-        10.4976
-        >>> calculator('3.24+2.5')
-        5.74
-    """
-
-    #ensure that only one operation is present
-    ops = [c for c in expression if c in '+-*/^%']
-    if len(ops) > 1:
-        raise ValueError(f"Invalid expression, too many operators. Expected exactly one of '+ - * / ^ %', found {', '.join(ops)}")
-    if len(ops) == 0:
-        raise ValueError(f"Invalid expression, no operation found. Expected one of '+ - * / ^ %'")
-    
-    op = ops[0]
-
-    _a, _b = expression.split(op)
-    a = float(_a)
-    b = float(_b)
-
-    if op == '+':
-        return a+b
-    elif op == '-':
-        return a-b
-    elif op == '*':
-        return a*b
-    elif op == '/':
-        return a/b
-    elif op == '^':
-        return a**b
-    elif op == '%':
-        return a%b
-    
 
 
 
 def test():
-    for t in [ask_user, datetime, timestamp, fib_n, example_tool, calculator]:
+    from archytas.tools import ask_user, datetime_tool, timestamp
+    from archytas.demo_tools import fib_n, example_tool, calculator, Jackpot
+    
+    for t in [ask_user, datetime_tool, timestamp, fib_n, example_tool, calculator, Jackpot]:
         print(get_tool_prompt_description(t))
         print()
 
 
 
 if __name__ == '__main__':
     test()
```

### Comparing `archytas-0.1.0/pyproject.toml` & `archytas-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.1.0"
+version = "0.2.0"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
 "Bug Tracker" = "https://github.com/jataware/archytas/issues"
```

