# Comparing `tmp/nonebot-plugin-chatgpt-plus-0.8.4.tar.gz` & `tmp/nonebot-plugin-chatgpt-plus-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.4.tar", last modified: Wed Apr 12 09:14:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.5.tar", last modified: Tue Apr 18 16:32:22 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-plus-0.8.4.tar` & `nonebot-plugin-chatgpt-plus-0.8.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/LICENSE
--rw-r--r--   0        0        0     6921 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/README.md
--rw-r--r--   0        0        0    13268 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/__init__.py
--rw-r--r--   0        0        0    14117 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/chatgpt.py
--rw-r--r--   0        0        0     1032 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/config.py
--rw-r--r--   0        0        0      892 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/data.py
--rw-r--r--   0        0        0     5678 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/utils.py
--rw-r--r--   0        0        0      725 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     7318 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/LICENSE
+-rw-r--r--   0        0        0     6831 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/README.md
+-rw-r--r--   0        0        0    13362 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/__init__.py
+-rw-r--r--   0        0        0    12072 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/chatgpt.py
+-rw-r--r--   0        0        0     1043 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/config.py
+-rw-r--r--   0        0        0      873 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/data.py
+-rw-r--r--   0        0        0     5678 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/utils.py
+-rw-r--r--   0        0        0      725 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     7228 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.5/PKG-INFO
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/LICENSE` & `nonebot-plugin-chatgpt-plus-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/README.md` & `nonebot-plugin-chatgpt-plus-0.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置（在 **ARM** 平台，可能必须使用 `CHATGPT_SESSION_TOKEN` 登录）
 
 > ⚠️ **Windows** 系统下需要在 `.env.dev` 文件中设置 `FASTAPI_RELOAD=false`
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
-| CHATGPT_PUID | 否 | 空字符串 | ChatGPT PLUS账号的puid，使用官方API必填 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
 | CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
```

#### html2text {}

```diff
@@ -18,18 +18,17 @@
 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
 ('nonebot_plugin_chatgpt_plus')  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®ï¼å¨ **ARM**
 å¹³å°ï¼å¯è½å¿é¡»ä½¿ç¨ `CHATGPT_SESSION_TOKEN` ç»å½ï¼ > â ï¸
 **Windows** ç³»ç»ä¸éè¦å¨ `.env.dev` æä»¶ä¸­è®¾ç½®
 `FASTAPI_RELOAD=false` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:--
 --:|:----:|:----:| | CHATGPT_SESSION_TOKEN | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT ç
-session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_PUID | å¦ | ç©ºå­ç¬¦ä¸²
-| ChatGPT PLUSè´¦å·çpuidï¼ä½¿ç¨å®æ¹APIå¿å¡« | | CHATGPT_MODEL | å¦ |
-ç©ºå­ç¬¦ä¸² | æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` |
-| CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
+session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸²
+| æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
+CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
 å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
 True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
 å¦ | 30 | session_token èªå¨å·æ°é´éï¼åä½ï¼åé | |
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/__init__.py` & `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,31 @@
     from nonebot_plugin_htmlrender import md_to_pic
 
 
 __zx_plugin_name__ = "ChatGPT-PLUS"
 __plugin_meta__ = PluginMetadata(
     name="ChatGPT-PLUS",
     description="ChatGPT PLUS插件",
-    usage=f"触发方式：{'@bot ' if config.chatgpt_to_me else ''}{config.chatgpt_command} 触发",
-    extra={
-        "unique_name": "chatgpt-plus",
-        "example": """
+    usage=f"""触发方式：{'@bot ' if config.chatgpt_to_me else ''}{config.chatgpt_command} 触发
 刷新会话/刷新对话	重置会话记录，开始新的对话
 导出会话/导出对话	导出当前会话记录
 导入会话/导入对话 + 会话ID + 父消息ID(可选)	将会话记录导入，这会替换当前的会话
 保存会话/保存对话 + 会话名称	将当前会话保存
 查看会话/查看对话	查看已保存的所有会话
 切换会话/切换对话 + 会话名称	切换到指定的会话
 回滚会话/回滚对话	返回到之前的会话，输入数字可以返回多个会话，但不可以超过最大支持数量
 人格设定/设置人格 + 名称 使用人格预设
+查看人格/查询人格   查看已有的人格预设列表
 清空会话/清空对话   清空所有会话（超级用户）
-查看人格/查询人格   查看已有的人格预设（超级用户）
+查看人格/查询人格 + 名称   查看已有的人格预设（超级用户）
 人格设定/设置人格 + 名称 + 人格信息 编辑人格信息（超级用户）
 刷新token   强制刷新token（超级用户）""",
+    extra={
+        "unique_name": "chatgpt-plus",
+        "example": """@bot 人格设定 香草""",
         "author": "A-kirami",
         "version": "0.8.1",
     },
 )
 __plugin_settings__ = {
     "level": 5,
     "default_status": True,
@@ -62,15 +63,14 @@
         "gpt3",
         "gpt4",
     ],
 }
 
 chat_bot = Chatbot(
     token=setting.token or config.chatgpt_session_token,
-    puid=setting.puid or config.chatgpt_puid,
     model=config.chatgpt_model,
     account=config.chatgpt_account,
     password=config.chatgpt_password,
     api=config.chatgpt_api,
     proxies=config.chatgpt_proxies,
     presets=setting.presets,
     timeout=config.chatgpt_timeout,
@@ -254,22 +254,18 @@
 
 
 @refresh.handle()
 @scheduler.scheduled_job("interval", minutes=config.chatgpt_refresh_interval)
 async def refresh_session() -> None:
     await chat_bot.refresh_session()
     setting.token = chat_bot.session_token
-    if config.chatgpt_puid:
-        await chat_bot.refresh_session_puid()
-        setting.puid = chat_bot.plus_puid
     setting.save()
     session.save_sessions()
     logger.opt(colors=True).debug(
         f"\ntoken: {setting.token}"
-        f"\npuid: {setting.puid}"
     )
 
 clear = on_command("清空对话", aliases={"清空会话"}, block=True, rule=to_me(), permission=SUPERUSER, priority=1)
 
 
 @clear.handle()
 async def clear_session() -> None:
@@ -323,23 +319,26 @@
             session[event] = chat_bot.conversation_id, chat_bot.parent_id
         except Exception as e:
             error = f"{type(e).__name__}: {e}"
             logger.opt(exception=e).error(f"ChatGPT request failed: {error}")
             await set_preset.finish(
                 f"请求 ChatGPT 服务器时出现问题，请稍后再试\n错误信息: {error}", reply_message=True
             )
-        await set_preset.finish(msg, reply_message=True)
+        await set_preset.send(msg, reply_message=True)
+        await chat_bot(**session[event]).edit_title(session.id(event=event))
 
-query = on_command("查看人格", aliases={"查询人格"}, block=True, rule=to_me(), permission=SUPERUSER, priority=1)
+query = on_command("查看人格", aliases={"查询人格"}, block=True, rule=to_me(), priority=1)
 
 
 @query.handle()
-async def query_preset(event: MessageEvent, arg: Message = CommandArg()):
+async def query_preset(bot: Bot, event: MessageEvent, arg: Message = CommandArg()):
     preset = arg.extract_plain_text().strip()
     if not preset:
         msg = "人格如下：\n"
         msg += "、".join(setting.presets.keys())
         await query.finish(msg, reply_message=True)
     if setting.presets.get(preset):
+        if event.get_user_id() not in bot.config.superusers:
+            await query.finish("权限不足", reply_message=True)
         await query.finish(f"名称：{preset}\n人格设定：{setting.presets.get(preset)}", reply_message=True)
     else:
         await query.finish("人格设定不存在", reply_message=True)
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/chatgpt.py` & `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/chatgpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
 SESSION_TOKEN_KEY = "__Secure-next-auth.session-token"
-PLUS_PUID_KEY = "_puid"
 CF_CLEARANCE_KEY = "cf_clearance"
 
 class Chatbot:
     def __init__(
         self,
         *,
         token: str = "",
-        puid: str = "",
         model: str = "text-davinci-002-render-sha",
         account: str = "",
         password: str = "",
         api: str = "https://chat.openai.com/",
         proxies: Optional[str] = None,
         presets: dict = {},
         timeout: int = 10,
     ) -> None:
         self.session_token = token
-        self.plus_puid = puid
         self.model = model
         self.account = account
         self.password = password
         self.api_url = api
         self.proxies = proxies
         self.timeout = timeout
         self.authorization = ""
@@ -48,16 +45,16 @@
 
         if self.session_token:
             self.auto_auth = False
         elif self.account and self.password:
             self.auto_auth = True
         else:
             raise ValueError("至少需要配置 session_token 或者 account 和 password")
-        if self.api_url.startswith('https://chat.openai.com') and not self.plus_puid:
-            raise ValueError("使用官方API请配置puid")
+        if self.api_url.startswith('https://chat.openai.com'):
+            raise ValueError("无法使用官方API，请使用第三方API")
 
     def __call__(
         self, conversation_id: Optional[str] = None, parent_id: Optional[str] = None, played_name: Optional[str] = None
     ) -> Self:
         self.conversation_id = conversation_id[-1] if conversation_id else None
         self.parent_id = parent_id[-1] if parent_id else self.id
         self.played_name = played_name
@@ -125,24 +122,22 @@
             "model": self.model,
             "timezone_offset_min": -480,
         }
 
     async def get_chat_response(self, prompt: str) -> str:
         if not self.authorization:
             await self.refresh_session()
+            if not self.authorization:
+                return "Token获取失败，请检查配置或API是否可用"
         async with httpx.AsyncClient(proxies=self.proxies) as client:
-            cookies = {
-                PLUS_PUID_KEY:self.plus_puid,
-            }
             async with client.stream(
                 "POST",
                 urljoin(self.api_url, "backend-api/conversation"),
                 headers=self.headers,
                 json=self.get_payload(prompt),
-                cookies=cookies,
                 timeout=self.timeout,
             ) as response:
                 if response.status_code == 429:
                     msg = ""
                     _buffer = bytearray()
                     async for chunk in response.aiter_bytes():
                         _buffer.extend(chunk)
@@ -161,41 +156,39 @@
                     return "会话不存在"
                 if response.is_error:
                     _buffer = bytearray()
                     async for chunk in response.aiter_bytes():
                         _buffer.extend(chunk)
                     resp_text = _buffer.decode()
                     logger.opt(colors=True).error(
-                        f"非预期的响应内容: <r>HTTP{response.status_code}</r> {escape_tag(resp_text)}"
+                        f"非预期的响应内容: <r>HTTP{response.status_code}</r> {resp_text}"
                     )
-                    return f"ChatGPT 服务器返回了非预期的内容: HTTP{response.status_code}\n{escape_tag(resp_text)}"
+                    return f"ChatGPT 服务器返回了非预期的内容: HTTP{response.status_code}\n{resp_text[:256]}"
                 data_list = []
                 async for line in response.aiter_lines():
                     if line.startswith("data:"):
                         data = line[6:]
                         if data.startswith("{"):
                             try:
                                 data_list.append(json.loads(data))
                             except Exception as e:
                                 logger.warning(f"ChatGPT数据解析未知错误：{e}: {data}")
                 if not data_list:
-                    return "ChatGPT 服务器未返回任何内容:"
+                    return "ChatGPT 服务器未返回任何内容"
                 idx = -1
                 while data_list[idx]["error"]:
                     idx -= 1
                 response = data_list[idx]
                 self.parent_id = response["message"]["id"]
                 self.conversation_id = response["conversation_id"]
                 return response["message"]["content"]["parts"][0]
 
     async def edit_title(self, title: str) -> bool:
         cookies = {
             SESSION_TOKEN_KEY: self.session_token,
-            PLUS_PUID_KEY:self.plus_puid,
-            CF_CLEARANCE_KEY: "cf_clearance"
         }
         async with httpx.AsyncClient(
             cookies=cookies,
             headers=self.headers,
             proxies=self.proxies,
             timeout=self.timeout,
         ) as client:
@@ -215,21 +208,18 @@
             else:
                 return False
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
                 f"编辑标题失败: <r>HTTP{response.status_code}</r> {response.text}"
             )
             return f"编辑标题失败，{e}"
-        
 
     async def gen_title(self) -> str:
         cookies = {
             SESSION_TOKEN_KEY: self.session_token,
-            PLUS_PUID_KEY:self.plus_puid,
-            CF_CLEARANCE_KEY: "cf_clearance"
         }
         async with httpx.AsyncClient(
             cookies=cookies,
             headers=self.headers,
             proxies=self.proxies,
             timeout=self.timeout,
         ) as client:
@@ -249,23 +239,21 @@
             else:
                 return resp.get('message')
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
                 f"生成标题失败: <r>HTTP{response.status_code}</r> {response.text}"
             )
             return f"生成标题失败，{e}"
-        
+
     async def refresh_session(self) -> None:
         if self.auto_auth:
             await self.login()
         else:
             cookies = {
                 SESSION_TOKEN_KEY: self.session_token,
-                PLUS_PUID_KEY:self.plus_puid,
-                CF_CLEARANCE_KEY: "cf_clearance"
             }
             async with httpx.AsyncClient(
                 cookies=cookies,
                 proxies=self.proxies,
                 timeout=self.timeout,
             ) as client:
                 response = await client.get(
@@ -280,66 +268,27 @@
                 )
                 self.authorization = response.json()["accessToken"]
             except Exception as e:
                 logger.opt(colors=True, exception=e).error(
                     f"刷新会话失败: <r>HTTP{response.status_code}</r> {response.text}"
                 )
 
-
-    async def refresh_session_puid(self) -> None:
-        cookies = {
-            PLUS_PUID_KEY:self.plus_puid
-        }
+    async def login(self) -> None:
         async with httpx.AsyncClient(
-            cookies=cookies,
-            headers=self.headers,
             proxies=self.proxies,
             timeout=self.timeout,
         ) as client:
-            response = await client.get(
-                urljoin(self.api_url, "backend-api/models"),
-                headers={
-                    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Safari/605.1.15",
-                },
-            )
-        try:
-            self.plus_puid = (
-                response.cookies.get(PLUS_PUID_KEY) or self.plus_puid
-            )
-        except Exception as e:
-            logger.opt(colors=True, exception=e).error(
-                f"刷新puid失败: <r>HTTP{response.status_code}</r> {response.text}"
+            response = await client.post(
+                "https://chat.loli.vet/api/auth/login",
+                files={
+                    "username": self.account,
+                    "password": self.password
+                }
             )
-
-    async def login(self) -> None:
-        if self.plus_puid:
-            try:
-                from OpenAIAuth import Authenticator
-                auth = Authenticator(email_address=self.account, password=self.password, puid=self.plus_puid, proxy=self.proxies)
-                auth.begin()
-                cookies = auth.session.cookies
-                self.session_token = cookies.get(SESSION_TOKEN_KEY)
+            if response.status_code == 200:
+                session_token =  response.cookies.get(SESSION_TOKEN_KEY)
+                self.session_token = session_token
                 self.auto_auth = False
                 logger.opt(colors=True).info("ChatGPT 登录成功！")
                 await self.refresh_session()
-            except Exception as e:
-                logger.error(f"ChatGPT 登陆错误!  {e}")
-        else:
-            async with httpx.AsyncClient(
-                proxies=self.proxies,
-                timeout=self.timeout,
-            ) as client:
-                response = await client.post(
-                    "https://chat.loli.vet/api/auth/login",
-                    files={
-                        "username": self.account,
-                        "password": self.password
-                    }
-                )
-                if response.status_code == 200:
-                    session_token =  response.cookies.get(SESSION_TOKEN_KEY)
-                    self.session_token = session_token
-                    self.auto_auth = False
-                    logger.opt(colors=True).info("ChatGPT 登录成功！")
-                    await self.refresh_session()
-                else:
-                    logger.error(f"ChatGPT 登陆错误! {response.text}")
+            else:
+                logger.error(f"ChatGPT 登陆错误! {response.text}")
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/config.py` & `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from nonebot import get_driver
 from pydantic import BaseModel, Extra
 
 
 class Config(BaseModel, extra=Extra.ignore):
     chatgpt_session_token: str = ""
-    chatgpt_puid: str = ""
     chatgpt_model: str = ""
     chatgpt_account: str = ""
     chatgpt_password: str = ""
     chatgpt_cd_time: int = 60
     chatgpt_notice: bool = True
+    chatgpt_auto_refresh: bool = True
     chatgpt_proxies: Optional[str] = None
     chatgpt_refresh_interval: int = 30
     chatgpt_command: Union[str, List[str]] = ""
     chatgpt_to_me: bool = True
     chatgpt_timeout: int = 30
     chatgpt_api: str = "https://chat.loli.vet/"
     chatgpt_image: bool = False
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/data.py` & `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     import json
 
 
 class Setting(BaseModel):
     session: Dict[str, Dict[str, Any]] = Field(default_factory=dict)
     presets: Dict[str, str] = Field(default_factory=dict)
     token: str = ""
-    puid: str = ""
 
     __file_path: Path = config.chatgpt_data / "setting.json"
 
     @property
     def file_path(self) -> Path:
         return self.__class__.__file_path
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/utils.py` & `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/pyproject.toml` & `nonebot-plugin-chatgpt-plus-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-chatgpt-plus"
-version = "0.8.4"
+version = "0.8.5"
 description = "NoneBot2 plugin for AI chat"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.4/PKG-INFO` & `nonebot-plugin-chatgpt-plus-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-plus
-Version: 0.8.4
+Version: 0.8.5
 Summary: NoneBot2 plugin for AI chat
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Project-URL: Repository, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Description-Content-Type: text/markdown
@@ -87,15 +87,14 @@
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置（在 **ARM** 平台，可能必须使用 `CHATGPT_SESSION_TOKEN` 登录）
 
 > ⚠️ **Windows** 系统下需要在 `.env.dev` 文件中设置 `FASTAPI_RELOAD=false`
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
-| CHATGPT_PUID | 否 | 空字符串 | ChatGPT PLUS账号的puid，使用官方API必填 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
 | CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.5 Summary:
 NoneBot2 plugin for AI chat License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 AkashiCoin/nonebot-plugin-chatgpt-plus Project-URL: Repository, https://
 github.com/AkashiCoin/nonebot-plugin-chatgpt-plus Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -24,18 +24,17 @@
 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
 ('nonebot_plugin_chatgpt_plus')  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®ï¼å¨ **ARM**
 å¹³å°ï¼å¯è½å¿é¡»ä½¿ç¨ `CHATGPT_SESSION_TOKEN` ç»å½ï¼ > â ï¸
 **Windows** ç³»ç»ä¸éè¦å¨ `.env.dev` æä»¶ä¸­è®¾ç½®
 `FASTAPI_RELOAD=false` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:--
 --:|:----:|:----:| | CHATGPT_SESSION_TOKEN | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT ç
-session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_PUID | å¦ | ç©ºå­ç¬¦ä¸²
-| ChatGPT PLUSè´¦å·çpuidï¼ä½¿ç¨å®æ¹APIå¿å¡« | | CHATGPT_MODEL | å¦ |
-ç©ºå­ç¬¦ä¸² | æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` |
-| CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
+session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸²
+| æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
+CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
 å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
 True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
 å¦ | 30 | session_token èªå¨å·æ°é´éï¼åä½ï¼åé | |
```

