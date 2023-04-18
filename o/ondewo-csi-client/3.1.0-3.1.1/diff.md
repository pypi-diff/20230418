# Comparing `tmp/ondewo-csi-client-3.1.0.tar.gz` & `tmp/ondewo-csi-client-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-csi-client-3.1.0.tar", last modified: Sat Apr 15 09:21:31 2023, max compression
+gzip compressed data, was "ondewo-csi-client-3.1.1.tar", last modified: Tue Apr 18 09:43:05 2023, max compression
```

## Comparing `ondewo-csi-client-3.1.0.tar` & `ondewo-csi-client-3.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7365 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6526 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.357195 ondewo-csi-client-3.1.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/ondewo/csi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/ondewo/csi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1370 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      872 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/ondewo/csi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3151 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/services/conversations.py
--rw-rw-r--   0 root         (0) root         (0)      879 2023-04-15 09:20:13.000000 ondewo-csi-client-3.1.0/ondewo/csi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    16912 2023-04-15 09:21:12.000000 ondewo-csi-client-3.1.0/ondewo/csi/conversation_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    18957 2023-04-15 09:21:12.000000 ondewo-csi-client-3.1.0/ondewo/csi/conversation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 09:21:31.358195 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7365 2023-04-15 09:21:31.000000 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-15 09:21:31.000000 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 09:21:31.000000 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-15 09:21:31.000000 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-15 09:21:31.000000 ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-04-15 09:21:31.359195 ondewo-csi-client-3.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1902 2023-04-15 09:21:16.000000 ondewo-csi-client-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1370 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      872 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3151 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services/conversations.py
+-rw-rw-r--   0 root         (0) root         (0)      879 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    16188 2023-04-18 09:39:40.000000 ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    19025 2023-04-18 09:39:40.000000 ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1902 2023-04-18 09:39:44.000000 ondewo-csi-client-3.1.1/setup.py
```

### Comparing `ondewo-csi-client-3.1.0/LICENSE` & `ondewo-csi-client-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/PKG-INFO` & `ondewo-csi-client-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.1.0
+Version: 3.1.1
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.0 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.1 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `ondewo-csi-client-3.1.0/README.md` & `ondewo-csi-client-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/client/client.py` & `ondewo-csi-client-3.1.1/ondewo/csi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/client/client_config.py` & `ondewo-csi-client-3.1.1/ondewo/csi/client/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/client/services/conversations.py` & `ondewo-csi-client-3.1.1/ondewo/csi/client/services/conversations.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/client/services_container.py` & `ondewo-csi-client-3.1.1/ondewo/csi/client/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/conversation_pb2.py` & `ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from ondewo.nlu import session_pb2 as ondewo_dot_nlu_dot_session__pb2
 from ondewo.t2s import text_to_speech_pb2 as ondewo_dot_t2s_dot_text__to__speech__pb2
 from ondewo.s2t import speech_to_text_pb2 as ondewo_dot_s2t_dot_speech__to__text__pb2
 from ondewo.nlu import context_pb2 as ondewo_dot_nlu_dot_context__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dondewo/csi/conversation.proto\x12\nondewo.csi\x1a\x1bgoogle/protobuf/empty.proto\x1a\x17google/rpc/status.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x18ondewo/nlu/session.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x18ondewo/nlu/context.proto\x1a\x19google/protobuf/any.proto\"~\n\x0bS2sPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0fs2t_pipeline_id\x18\x02 \x01(\t\x12\x16\n\x0enlu_project_id\x18\x03 \x01(\t\x12\x19\n\x11nlu_language_code\x18\x04 \x01(\t\x12\x17\n\x0ft2s_pipeline_id\x18\x05 \x01(\t\"\x1b\n\rS2sPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"\x19\n\x17ListS2sPipelinesRequest\"F\n\x18ListS2sPipelinesResponse\x12*\n\tpipelines\x18\x01 \x03(\x0b\x32\x17.ondewo.csi.S2sPipeline\"\x86\x01\n\x10S2sStreamRequest\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x04 \x01(\x08\x12#\n\x1binitial_intent_display_name\x18\x05 \x01(\t\"\xd1\x01\n\x11S2sStreamResponse\x12\x42\n\x16\x64\x65tect_intent_response\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DetectIntentResponseH\x00\x12=\n\x13synthetize_response\x18\x02 \x01(\x0b\x32\x1e.ondewo.t2s.SynthesizeResponseH\x00\x12-\n\x0bsip_trigger\x18\x03 \x01(\x0b\x32\x16.ondewo.csi.SipTriggerH\x00\x42\n\n\x08response\"\xc7\x01\n\nSipTrigger\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ondewo.csi.SipTrigger.SipTriggerType\x12(\n\x07\x63ontent\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"Z\n\x0eSipTriggerType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06HANGUP\x10\x01\x12\x12\n\x0eHUMAN_HANDOVER\x10\x02\x12\x0c\n\x08SEND_NOW\x10\x03\x12\t\n\x05PAUSE\x10\x04\"\x95\x01\n\x1b\x43heckUpstreamHealthResponse\x12&\n\ns2t_status\x18\x01 \x01(\x0b\x32\x12.google.rpc.Status\x12&\n\nnlu_status\x18\x02 \x01(\x0b\x32\x12.google.rpc.Status\x12&\n\nt2s_status\x18\x03 \x01(\x0b\x32\x12.google.rpc.Status\"\x16\n\x14\x43ontrolStreamRequest\"J\n\x15\x43ontrolStreamResponse\x12\x31\n\x0e\x63ontrol_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"L\n\x17SetControlStatusRequest\x12\x31\n\x0e\x63ontrol_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"\x88\x01\n\x18SetControlStatusResponse\x12\x35\n\x12old_control_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\x12\x35\n\x12new_control_status\x18\x02 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"\x84\x01\n\x12\x43ondtionValueUnion\x12\x13\n\tint_value\x18\x01 \x01(\x03H\x00\x12\x15\n\x0b\x66loat_value\x18\x02 \x01(\x02H\x00\x12\x34\n\x0e\x64\x61tetime_value\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x42\x0c\n\nUnionOneof\"C\n\tCondition\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ConditionType\x12\r\n\x05value\x18\x02 \x01(\t\"\xfb\x02\n\x1f\x43ontrolMessageServiceParameters\x12/\n\nt2s_config\x18\x01 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfigH\x00\x12\x39\n\ns2t_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x12\x13\n\x0btransfer_id\x18\x03 \x01(\t\x12\x11\n\twav_files\x18\x04 \x03(\x0c\x12\x0c\n\x04text\x18\x05 \x01(\t\x12$\n\x07\x63ontext\x18\x06 \x01(\x0b\x32\x13.ondewo.nlu.Context\x12\x12\n\nsession_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontext_name\x18\x08 \x01(\t\x12.\n\x0f\x63ondition_start\x18\t \x01(\x0b\x32\x15.ondewo.csi.Condition\x12,\n\rcondition_end\x18\n \x01(\x0b\x32\x15.ondewo.csi.ConditionB\x08\n\x06\x63onfig\"\xc2\x01\n\x0e\x43ontrolMessage\x12\x36\n\x07service\x18\x01 \x01(\x0e\x32%.ondewo.csi.ControlMessageServiceName\x12\x37\n\x06method\x18\x02 \x01(\x0e\x32\'.ondewo.csi.ControlMessageServiceMethod\x12?\n\nparameters\x18\x03 \x01(\x0b\x32+.ondewo.csi.ControlMessageServiceParameters*+\n\rControlStatus\x12\x06\n\x02OK\x10\x00\x12\x12\n\x0e\x45MERGENCY_STOP\x10\x01*l\n\x19\x43ontrolMessageServiceName\x12\x0f\n\x0bUNKNOWNNAME\x10\x00\x12\x0e\n\nondewo_s2t\x10\x01\x12\x0e\n\nondewo_t2s\x10\x02\x12\x0e\n\nondewo_nlu\x10\x03\x12\x0e\n\nondewo_sip\x10\x04*\x85\x03\n\x1b\x43ontrolMessageServiceMethod\x12\x11\n\rUNKNOWNMETHOD\x10\x00\x12\x11\n\rupdate_config\x10\x01\x12\x0f\n\x0bundo_config\x10\x02\x12\x10\n\x0creset_config\x10\x03\x12\x0c\n\x08\x65nd_call\x10\x04\x12\x11\n\rtransfer_call\x10\x05\x12\x12\n\x0eplay_wav_files\x10\x06\x12\r\n\tplay_text\x10\x07\x12\x08\n\x04mute\x10\x08\x12\x0b\n\x07un_mute\x10\t\x12\x1d\n\x19stop_all_control_messages\x10\n\x12\x0f\n\x0btrain_agent\x10\x0b\x12\x16\n\x12\x63\x61ncel_train_agent\x10\x0c\x12\x12\n\x0e\x64\x65lete_session\x10\r\x12\x17\n\x13\x64\x65lete_all_contexts\x10\x0e\x12\x12\n\x0e\x63reate_context\x10\x0f\x12\x12\n\x0eupdate_context\x10\x10\x12\x12\n\x0e\x64\x65lete_context\x10\x11\x12\x11\n\rdetect_intent\x10\x12*\\\n\rConditionType\x12\x0e\n\nUNKNOWTYPE\x10\x00\x12\r\n\timmediate\x10\x01\x12\x0c\n\x08\x64uration\x10\x02\x12\x0c\n\x08\x64\x61tetime\x10\x03\x12\x10\n\x0cinteractions\x10\x04\x32\xfa\x05\n\rConversations\x12\x46\n\x11\x43reateS2sPipeline\x12\x17.ondewo.csi.S2sPipeline\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x0eGetS2sPipeline\x12\x19.ondewo.csi.S2sPipelineId\x1a\x17.ondewo.csi.S2sPipeline\"\x00\x12\x46\n\x11UpdateS2sPipeline\x12\x17.ondewo.csi.S2sPipeline\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x11\x44\x65leteS2sPipeline\x12\x19.ondewo.csi.S2sPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2sPipelines\x12#.ondewo.csi.ListS2sPipelinesRequest\x1a$.ondewo.csi.ListS2sPipelinesResponse\"\x00\x12N\n\tS2sStream\x12\x1c.ondewo.csi.S2sStreamRequest\x1a\x1d.ondewo.csi.S2sStreamResponse\"\x00(\x01\x30\x01\x12X\n\x13\x43heckUpstreamHealth\x12\x16.google.protobuf.Empty\x1a\'.ondewo.csi.CheckUpstreamHealthResponse\"\x00\x12[\n\x10GetControlStream\x12 .ondewo.csi.ControlStreamRequest\x1a!.ondewo.csi.ControlStreamResponse\"\x00\x30\x01\x12_\n\x10SetControlStatus\x12#.ondewo.csi.SetControlStatusRequest\x1a$.ondewo.csi.SetControlStatusResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dondewo/csi/conversation.proto\x12\nondewo.csi\x1a\x1bgoogle/protobuf/empty.proto\x1a\x17google/rpc/status.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x18ondewo/nlu/session.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x18ondewo/nlu/context.proto\x1a\x19google/protobuf/any.proto\"~\n\x0bS2sPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0fs2t_pipeline_id\x18\x02 \x01(\t\x12\x16\n\x0enlu_project_id\x18\x03 \x01(\t\x12\x19\n\x11nlu_language_code\x18\x04 \x01(\t\x12\x17\n\x0ft2s_pipeline_id\x18\x05 \x01(\t\"\x1b\n\rS2sPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"\x19\n\x17ListS2sPipelinesRequest\"F\n\x18ListS2sPipelinesResponse\x12*\n\tpipelines\x18\x01 \x03(\x0b\x32\x17.ondewo.csi.S2sPipeline\"\x86\x01\n\x10S2sStreamRequest\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x04 \x01(\x08\x12#\n\x1binitial_intent_display_name\x18\x05 \x01(\t\"\xd1\x01\n\x11S2sStreamResponse\x12\x42\n\x16\x64\x65tect_intent_response\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DetectIntentResponseH\x00\x12=\n\x13synthesize_response\x18\x02 \x01(\x0b\x32\x1e.ondewo.t2s.SynthesizeResponseH\x00\x12-\n\x0bsip_trigger\x18\x03 \x01(\x0b\x32\x16.ondewo.csi.SipTriggerH\x00\x42\n\n\x08response\"\xc7\x01\n\nSipTrigger\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ondewo.csi.SipTrigger.SipTriggerType\x12(\n\x07\x63ontent\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"Z\n\x0eSipTriggerType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06HANGUP\x10\x01\x12\x12\n\x0eHUMAN_HANDOVER\x10\x02\x12\x0c\n\x08SEND_NOW\x10\x03\x12\t\n\x05PAUSE\x10\x04\"\x95\x01\n\x1b\x43heckUpstreamHealthResponse\x12&\n\ns2t_status\x18\x01 \x01(\x0b\x32\x12.google.rpc.Status\x12&\n\nnlu_status\x18\x02 \x01(\x0b\x32\x12.google.rpc.Status\x12&\n\nt2s_status\x18\x03 \x01(\x0b\x32\x12.google.rpc.Status\"\x16\n\x14\x43ontrolStreamRequest\"J\n\x15\x43ontrolStreamResponse\x12\x31\n\x0e\x63ontrol_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"L\n\x17SetControlStatusRequest\x12\x31\n\x0e\x63ontrol_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"\x88\x01\n\x18SetControlStatusResponse\x12\x35\n\x12old_control_status\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\x12\x35\n\x12new_control_status\x18\x02 \x01(\x0e\x32\x19.ondewo.csi.ControlStatus\"C\n\tCondition\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.ondewo.csi.ConditionType\x12\r\n\x05value\x18\x02 \x01(\t\"\xfb\x02\n\x1f\x43ontrolMessageServiceParameters\x12/\n\nt2s_config\x18\x01 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfigH\x00\x12\x39\n\ns2t_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x12\x13\n\x0btransfer_id\x18\x03 \x01(\t\x12\x11\n\twav_files\x18\x04 \x03(\x0c\x12\x0c\n\x04text\x18\x05 \x01(\t\x12$\n\x07\x63ontext\x18\x06 \x01(\x0b\x32\x13.ondewo.nlu.Context\x12\x12\n\nsession_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontext_name\x18\x08 \x01(\t\x12.\n\x0f\x63ondition_start\x18\t \x01(\x0b\x32\x15.ondewo.csi.Condition\x12,\n\rcondition_end\x18\n \x01(\x0b\x32\x15.ondewo.csi.ConditionB\x08\n\x06\x63onfig\"\xc2\x01\n\x0e\x43ontrolMessage\x12\x36\n\x07service\x18\x01 \x01(\x0e\x32%.ondewo.csi.ControlMessageServiceName\x12\x37\n\x06method\x18\x02 \x01(\x0e\x32\'.ondewo.csi.ControlMessageServiceMethod\x12?\n\nparameters\x18\x03 \x01(\x0b\x32+.ondewo.csi.ControlMessageServiceParameters*+\n\rControlStatus\x12\x06\n\x02OK\x10\x00\x12\x12\n\x0e\x45MERGENCY_STOP\x10\x01*l\n\x19\x43ontrolMessageServiceName\x12\x0f\n\x0bUNKNOWNNAME\x10\x00\x12\x0e\n\nondewo_s2t\x10\x01\x12\x0e\n\nondewo_t2s\x10\x02\x12\x0e\n\nondewo_nlu\x10\x03\x12\x0e\n\nondewo_sip\x10\x04*\x85\x03\n\x1b\x43ontrolMessageServiceMethod\x12\x11\n\rUNKNOWNMETHOD\x10\x00\x12\x11\n\rupdate_config\x10\x01\x12\x0f\n\x0bundo_config\x10\x02\x12\x10\n\x0creset_config\x10\x03\x12\x0c\n\x08\x65nd_call\x10\x04\x12\x11\n\rtransfer_call\x10\x05\x12\x12\n\x0eplay_wav_files\x10\x06\x12\r\n\tplay_text\x10\x07\x12\x08\n\x04mute\x10\x08\x12\x0b\n\x07un_mute\x10\t\x12\x1d\n\x19stop_all_control_messages\x10\n\x12\x0f\n\x0btrain_agent\x10\x0b\x12\x16\n\x12\x63\x61ncel_train_agent\x10\x0c\x12\x12\n\x0e\x64\x65lete_session\x10\r\x12\x17\n\x13\x64\x65lete_all_contexts\x10\x0e\x12\x12\n\x0e\x63reate_context\x10\x0f\x12\x12\n\x0eupdate_context\x10\x10\x12\x12\n\x0e\x64\x65lete_context\x10\x11\x12\x11\n\rdetect_intent\x10\x12*\\\n\rConditionType\x12\x0e\n\nUNKNOWTYPE\x10\x00\x12\r\n\timmediate\x10\x01\x12\x0c\n\x08\x64uration\x10\x02\x12\x0c\n\x08\x64\x61tetime\x10\x03\x12\x10\n\x0cinteractions\x10\x04\x32\xfa\x05\n\rConversations\x12\x46\n\x11\x43reateS2sPipeline\x12\x17.ondewo.csi.S2sPipeline\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x0eGetS2sPipeline\x12\x19.ondewo.csi.S2sPipelineId\x1a\x17.ondewo.csi.S2sPipeline\"\x00\x12\x46\n\x11UpdateS2sPipeline\x12\x17.ondewo.csi.S2sPipeline\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x11\x44\x65leteS2sPipeline\x12\x19.ondewo.csi.S2sPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2sPipelines\x12#.ondewo.csi.ListS2sPipelinesRequest\x1a$.ondewo.csi.ListS2sPipelinesResponse\"\x00\x12N\n\tS2sStream\x12\x1c.ondewo.csi.S2sStreamRequest\x1a\x1d.ondewo.csi.S2sStreamResponse\"\x00(\x01\x30\x01\x12X\n\x13\x43heckUpstreamHealth\x12\x16.google.protobuf.Empty\x1a\'.ondewo.csi.CheckUpstreamHealthResponse\"\x00\x12[\n\x10GetControlStream\x12 .ondewo.csi.ControlStreamRequest\x1a!.ondewo.csi.ControlStreamResponse\"\x00\x30\x01\x12_\n\x10SetControlStatus\x12#.ondewo.csi.SetControlStatusRequest\x1a$.ondewo.csi.SetControlStatusResponse\"\x00\x62\x06proto3')
 
 _CONTROLSTATUS = DESCRIPTOR.enum_types_by_name['ControlStatus']
 ControlStatus = enum_type_wrapper.EnumTypeWrapper(_CONTROLSTATUS)
 _CONTROLMESSAGESERVICENAME = DESCRIPTOR.enum_types_by_name['ControlMessageServiceName']
 ControlMessageServiceName = enum_type_wrapper.EnumTypeWrapper(_CONTROLMESSAGESERVICENAME)
 _CONTROLMESSAGESERVICEMETHOD = DESCRIPTOR.enum_types_by_name['ControlMessageServiceMethod']
 ControlMessageServiceMethod = enum_type_wrapper.EnumTypeWrapper(_CONTROLMESSAGESERVICEMETHOD)
@@ -75,15 +75,14 @@
 _S2SSTREAMRESPONSE = DESCRIPTOR.message_types_by_name['S2sStreamResponse']
 _SIPTRIGGER = DESCRIPTOR.message_types_by_name['SipTrigger']
 _CHECKUPSTREAMHEALTHRESPONSE = DESCRIPTOR.message_types_by_name['CheckUpstreamHealthResponse']
 _CONTROLSTREAMREQUEST = DESCRIPTOR.message_types_by_name['ControlStreamRequest']
 _CONTROLSTREAMRESPONSE = DESCRIPTOR.message_types_by_name['ControlStreamResponse']
 _SETCONTROLSTATUSREQUEST = DESCRIPTOR.message_types_by_name['SetControlStatusRequest']
 _SETCONTROLSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['SetControlStatusResponse']
-_CONDTIONVALUEUNION = DESCRIPTOR.message_types_by_name['CondtionValueUnion']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _CONTROLMESSAGESERVICEPARAMETERS = DESCRIPTOR.message_types_by_name['ControlMessageServiceParameters']
 _CONTROLMESSAGE = DESCRIPTOR.message_types_by_name['ControlMessage']
 _SIPTRIGGER_SIPTRIGGERTYPE = _SIPTRIGGER.enum_types_by_name['SipTriggerType']
 S2sPipeline = _reflection.GeneratedProtocolMessageType('S2sPipeline', (_message.Message,), {
   'DESCRIPTOR' : _S2SPIPELINE,
   '__module__' : 'ondewo.csi.conversation_pb2'
@@ -164,21 +163,14 @@
 SetControlStatusResponse = _reflection.GeneratedProtocolMessageType('SetControlStatusResponse', (_message.Message,), {
   'DESCRIPTOR' : _SETCONTROLSTATUSRESPONSE,
   '__module__' : 'ondewo.csi.conversation_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.csi.SetControlStatusResponse)
   })
 _sym_db.RegisterMessage(SetControlStatusResponse)
 
-CondtionValueUnion = _reflection.GeneratedProtocolMessageType('CondtionValueUnion', (_message.Message,), {
-  'DESCRIPTOR' : _CONDTIONVALUEUNION,
-  '__module__' : 'ondewo.csi.conversation_pb2'
-  # @@protoc_insertion_point(class_scope:ondewo.csi.CondtionValueUnion)
-  })
-_sym_db.RegisterMessage(CondtionValueUnion)
-
 Condition = _reflection.GeneratedProtocolMessageType('Condition', (_message.Message,), {
   'DESCRIPTOR' : _CONDITION,
   '__module__' : 'ondewo.csi.conversation_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.csi.Condition)
   })
 _sym_db.RegisterMessage(Condition)
 
@@ -196,22 +188,22 @@
   })
 _sym_db.RegisterMessage(ControlMessage)
 
 _CONVERSATIONS = DESCRIPTOR.services_by_name['Conversations']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _CONTROLSTATUS._serialized_start=2366
-  _CONTROLSTATUS._serialized_end=2409
-  _CONTROLMESSAGESERVICENAME._serialized_start=2411
-  _CONTROLMESSAGESERVICENAME._serialized_end=2519
-  _CONTROLMESSAGESERVICEMETHOD._serialized_start=2522
-  _CONTROLMESSAGESERVICEMETHOD._serialized_end=2911
-  _CONDITIONTYPE._serialized_start=2913
-  _CONDITIONTYPE._serialized_end=3005
+  _CONTROLSTATUS._serialized_start=2231
+  _CONTROLSTATUS._serialized_end=2274
+  _CONTROLMESSAGESERVICENAME._serialized_start=2276
+  _CONTROLMESSAGESERVICENAME._serialized_end=2384
+  _CONTROLMESSAGESERVICEMETHOD._serialized_start=2387
+  _CONTROLMESSAGESERVICEMETHOD._serialized_end=2776
+  _CONDITIONTYPE._serialized_start=2778
+  _CONDITIONTYPE._serialized_end=2870
   _S2SPIPELINE._serialized_start=307
   _S2SPIPELINE._serialized_end=433
   _S2SPIPELINEID._serialized_start=435
   _S2SPIPELINEID._serialized_end=462
   _LISTS2SPIPELINESREQUEST._serialized_start=464
   _LISTS2SPIPELINESREQUEST._serialized_end=489
   _LISTS2SPIPELINESRESPONSE._serialized_start=491
@@ -230,18 +222,16 @@
   _CONTROLSTREAMREQUEST._serialized_end=1288
   _CONTROLSTREAMRESPONSE._serialized_start=1290
   _CONTROLSTREAMRESPONSE._serialized_end=1364
   _SETCONTROLSTATUSREQUEST._serialized_start=1366
   _SETCONTROLSTATUSREQUEST._serialized_end=1442
   _SETCONTROLSTATUSRESPONSE._serialized_start=1445
   _SETCONTROLSTATUSRESPONSE._serialized_end=1581
-  _CONDTIONVALUEUNION._serialized_start=1584
-  _CONDTIONVALUEUNION._serialized_end=1716
-  _CONDITION._serialized_start=1718
-  _CONDITION._serialized_end=1785
-  _CONTROLMESSAGESERVICEPARAMETERS._serialized_start=1788
-  _CONTROLMESSAGESERVICEPARAMETERS._serialized_end=2167
-  _CONTROLMESSAGE._serialized_start=2170
-  _CONTROLMESSAGE._serialized_end=2364
-  _CONVERSATIONS._serialized_start=3008
-  _CONVERSATIONS._serialized_end=3770
+  _CONDITION._serialized_start=1583
+  _CONDITION._serialized_end=1650
+  _CONTROLMESSAGESERVICEPARAMETERS._serialized_start=1653
+  _CONTROLMESSAGESERVICEPARAMETERS._serialized_end=2032
+  _CONTROLMESSAGE._serialized_start=2035
+  _CONTROLMESSAGE._serialized_end=2229
+  _CONVERSATIONS._serialized_start=2873
+  _CONVERSATIONS._serialized_end=3635
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-csi-client-3.1.0/ondewo/csi/conversation_pb2_grpc.py` & `ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,21 +203,23 @@
         }</samp>
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetControlStream(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get the control stream to control sip, t2s, s2t etc. during a conversation
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetControlStatus(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Send a message on the control stream to control sip, t2s, s2t etc. during a conversation
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ConversationsServicer_to_server(servicer, server):
     rpc_method_handlers = {
```

### Comparing `ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/PKG-INFO` & `ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.1.0
+Version: 3.1.1
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.0 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.1 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `ondewo-csi-client-3.1.0/ondewo_csi_client.egg-info/SOURCES.txt` & `ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.0/setup.py` & `ondewo-csi-client-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 long_description: str = read_file('README.md')
 requires: List[str] = read_requirements('requirements.txt')
 
 setup(
     name="ondewo-csi-client",
-    version='3.1.0',
+    version='3.1.1',
     author="ONDEWO GbmH",
     author_email="office@ondewo.com",
     description="Provides endpoints and messages for gRPC communication to the ONDEWO CSI server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-csi-client-python",
     packages=[
```

