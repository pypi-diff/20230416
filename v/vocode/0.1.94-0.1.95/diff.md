# Comparing `tmp/vocode-0.1.94.tar.gz` & `tmp/vocode-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode-0.1.94.tar", max compression
+gzip compressed data, was "vocode-0.1.95.tar", max compression
```

## Comparing `vocode-0.1.94.tar` & `vocode-0.1.95.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1065 2023-03-28 17:29:00.108721 vocode-0.1.94/LICENSE
--rw-r--r--   0        0        0     8266 2023-04-12 08:05:58.013355 vocode-0.1.94/README.md
--rw-r--r--   0        0        0     2065 2023-04-15 15:38:08.420663 vocode-0.1.94/pyproject.toml
--rw-r--r--   0        0        0      308 2023-03-28 17:30:02.280446 vocode-0.1.94/vocode/__init__.py
--rw-r--r--   0        0        0     2390 2023-03-28 07:12:57.812230 vocode-0.1.94/vocode/helpers.py
--rw-r--r--   0        0        0     1536 2023-04-11 21:06:59.690563 vocode-0.1.94/vocode/streaming/agent/base_agent.py
--rw-r--r--   0        0        0     2007 2023-03-29 06:28:34.480507 vocode-0.1.94/vocode/streaming/agent/bot_sentiment_analyser.py
--rw-r--r--   0        0        0     6659 2023-04-11 17:15:11.306264 vocode-0.1.94/vocode/streaming/agent/chat_gpt_agent.py
--rw-r--r--   0        0        0      591 2023-04-11 17:15:11.306521 vocode-0.1.94/vocode/streaming/agent/echo_agent.py
--rw-r--r--   0        0        0     1467 2023-04-11 21:06:59.691054 vocode-0.1.94/vocode/streaming/agent/factory.py
--rw-r--r--   0        0        0     1481 2023-03-28 17:30:02.281854 vocode-0.1.94/vocode/streaming/agent/information_retrieval_agent.py
--rw-r--r--   0        0        0     5724 2023-04-11 17:15:11.307183 vocode-0.1.94/vocode/streaming/agent/llm_agent.py
--rw-r--r--   0        0        0     2053 2023-04-11 17:15:11.308601 vocode-0.1.94/vocode/streaming/agent/restful_user_implemented_agent.py
--rw-r--r--   0        0        0      684 2023-03-28 17:30:02.282322 vocode-0.1.94/vocode/streaming/agent/utils.py
--rw-r--r--   0        0        0     3259 2023-04-04 06:04:39.618650 vocode-0.1.94/vocode/streaming/client_backend/conversation.py
--rw-r--r--   0        0        0       96 2023-03-28 17:30:02.282460 vocode-0.1.94/vocode/streaming/constants.py
--rw-r--r--   0        0        0     3724 2023-04-12 18:22:27.897471 vocode-0.1.94/vocode/streaming/hosted_streaming_conversation.py
--rw-r--r--   0        0        0      476 2023-03-28 07:12:57.812101 vocode-0.1.94/vocode/streaming/input_device/base_input_device.py
--rw-r--r--   0        0        0     1648 2023-03-28 07:12:57.809750 vocode-0.1.94/vocode/streaming/input_device/microphone_input.py
--rw-r--r--   0        0        0      334 2023-03-28 07:12:57.811970 vocode-0.1.94/vocode/streaming/input_device/telephone_input.py
--rw-r--r--   0        0        0     5314 2023-04-13 19:53:16.083378 vocode-0.1.94/vocode/streaming/models/agent.py
--rw-r--r--   0        0        0      102 2023-03-28 17:30:02.283498 vocode-0.1.94/vocode/streaming/models/audio_encoding.py
--rw-r--r--   0        0        0      856 2023-04-03 01:45:30.651534 vocode-0.1.94/vocode/streaming/models/events.py
--rw-r--r--   0        0        0      299 2023-03-28 07:12:57.772953 vocode-0.1.94/vocode/streaming/models/message.py
--rw-r--r--   0        0        0     1455 2023-03-28 17:30:02.283821 vocode-0.1.94/vocode/streaming/models/model.py
--rw-r--r--   0        0        0     3700 2023-04-14 17:29:46.789838 vocode-0.1.94/vocode/streaming/models/synthesizer.py
--rw-r--r--   0        0        0     1806 2023-03-28 17:30:02.284366 vocode-0.1.94/vocode/streaming/models/telephony.py
--rw-r--r--   0        0        0     3254 2023-04-12 08:06:19.437996 vocode-0.1.94/vocode/streaming/models/transcriber.py
--rw-r--r--   0        0        0     1765 2023-04-04 06:04:39.619062 vocode-0.1.94/vocode/streaming/models/websocket.py
--rw-r--r--   0        0        0      396 2023-03-28 17:30:02.285240 vocode-0.1.94/vocode/streaming/output_device/base_output_device.py
--rw-r--r--   0        0        0     1015 2023-03-28 07:12:57.807120 vocode-0.1.94/vocode/streaming/output_device/speaker_output.py
--rw-r--r--   0        0        0      262 2023-03-28 07:12:57.809162 vocode-0.1.94/vocode/streaming/output_device/telephone_output.py
--rw-r--r--   0        0        0     1148 2023-04-04 06:04:39.619476 vocode-0.1.94/vocode/streaming/output_device/twilio_output_device.py
--rw-r--r--   0        0        0      800 2023-04-04 06:04:39.619698 vocode-0.1.94/vocode/streaming/output_device/websocket_output_device.py
--rw-r--r--   0        0        0    21220 2023-04-12 07:56:17.824251 vocode-0.1.94/vocode/streaming/streaming_conversation.py
--rw-r--r--   0        0        0    10570 2023-04-10 22:54:02.366120 vocode-0.1.94/vocode/streaming/synthesizer/azure_synthesizer.py
--rw-r--r--   0        0        0     7673 2023-04-11 21:06:59.693069 vocode-0.1.94/vocode/streaming/synthesizer/base_synthesizer.py
--rw-r--r--   0        0        0     2355 2023-04-12 08:05:58.014267 vocode-0.1.94/vocode/streaming/synthesizer/eleven_labs_synthesizer.py
--rw-r--r--   0        0        0     1448 2023-04-11 21:06:59.693827 vocode-0.1.94/vocode/streaming/synthesizer/factory.py
--rw-r--r--   0        0        0  6548060 2023-03-28 17:30:02.328281 vocode-0.1.94/vocode/streaming/synthesizer/filler_audio/typing-noise.wav
--rw-r--r--   0        0        0     3396 2023-04-11 21:06:59.694063 vocode-0.1.94/vocode/streaming/synthesizer/google_synthesizer.py
--rw-r--r--   0        0        0     1252 2023-04-14 17:21:46.738980 vocode-0.1.94/vocode/streaming/synthesizer/gtts_synthesizer.py
--rw-r--r--   0        0        0     2463 2023-04-11 21:06:59.694296 vocode-0.1.94/vocode/streaming/synthesizer/play_ht_synthesizer.py
--rw-r--r--   0        0        0     1795 2023-04-12 06:50:30.491534 vocode-0.1.94/vocode/streaming/synthesizer/rime_synthesizer.py
--rw-r--r--   0        0        0     1453 2023-04-14 17:19:36.773276 vocode-0.1.94/vocode/streaming/synthesizer/stream_elements_synthesizer.py
--rw-r--r--   0        0        0        0 2023-03-28 17:30:02.329443 vocode-0.1.94/vocode/streaming/telephony/__init__.py
--rw-r--r--   0        0        0      438 2023-03-28 17:30:02.330427 vocode-0.1.94/vocode/streaming/telephony/config_manager/base_config_manager.py
--rw-r--r--   0        0        0      609 2023-03-28 23:14:27.148000 vocode-0.1.94/vocode/streaming/telephony/config_manager/in_memory_config_manager.py
--rw-r--r--   0        0        0     1248 2023-03-28 17:30:02.331245 vocode-0.1.94/vocode/streaming/telephony/config_manager/redis_config_manager.py
--rw-r--r--   0        0        0      170 2023-03-28 17:30:02.331397 vocode-0.1.94/vocode/streaming/telephony/constants.py
--rw-r--r--   0        0        0     6799 2023-04-11 21:06:59.694996 vocode-0.1.94/vocode/streaming/telephony/conversation/call.py
--rw-r--r--   0        0        0     4136 2023-04-11 17:15:11.315392 vocode-0.1.94/vocode/streaming/telephony/conversation/outbound_call.py
--rw-r--r--   0        0        0     2802 2023-03-28 17:30:02.332164 vocode-0.1.94/vocode/streaming/telephony/conversation/zoom_dial_in.py
--rw-r--r--   0        0        0      106 2023-04-03 01:45:30.652609 vocode-0.1.94/vocode/streaming/telephony/hosted/exceptions.py
--rw-r--r--   0        0        0     2264 2023-03-28 17:30:02.332438 vocode-0.1.94/vocode/streaming/telephony/hosted/inbound_call_server.py
--rw-r--r--   0        0        0     1697 2023-03-28 17:30:02.332777 vocode-0.1.94/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py
--rw-r--r--   0        0        0     3032 2023-04-03 01:45:30.652914 vocode-0.1.94/vocode/streaming/telephony/hosted/outbound_call.py
--rw-r--r--   0        0        0     2458 2023-04-03 01:45:30.653149 vocode-0.1.94/vocode/streaming/telephony/hosted/zoom_dial_in.py
--rw-r--r--   0        0        0     5845 2023-04-11 21:06:59.695325 vocode-0.1.94/vocode/streaming/telephony/server/base.py
--rw-r--r--   0        0        0     2439 2023-04-11 21:06:59.695619 vocode-0.1.94/vocode/streaming/telephony/server/router/calls.py
--rw-r--r--   0        0        0      865 2023-04-04 06:04:39.620616 vocode-0.1.94/vocode/streaming/telephony/server/router/twiml.py
--rw-r--r--   0        0        0      150 2023-03-28 17:30:02.333925 vocode-0.1.94/vocode/streaming/telephony/templates/connect_call.xml
--rw-r--r--   0        0        0      653 2023-03-28 17:30:02.333757 vocode-0.1.94/vocode/streaming/telephony/templates.py
--rw-r--r--   0        0        0      434 2023-04-11 21:06:59.695870 vocode-0.1.94/vocode/streaming/telephony/twilio.py
--rw-r--r--   0        0        0     2220 2023-03-21 03:19:41.096039 vocode-0.1.94/vocode/streaming/telephony/zoom_dial_in.py
--rw-r--r--   0        0        0     3452 2023-04-12 08:03:51.421371 vocode-0.1.94/vocode/streaming/transcriber/assembly_ai_transcriber.py
--rw-r--r--   0        0        0     1241 2023-04-11 21:06:59.696653 vocode-0.1.94/vocode/streaming/transcriber/base_transcriber.py
--rw-r--r--   0        0        0     7975 2023-04-12 07:59:00.960353 vocode-0.1.94/vocode/streaming/transcriber/deepgram_transcriber.py
--rw-r--r--   0        0        0     1249 2023-04-12 08:05:58.014409 vocode-0.1.94/vocode/streaming/transcriber/factory.py
--rw-r--r--   0        0        0     4377 2023-04-12 08:00:45.683444 vocode-0.1.94/vocode/streaming/transcriber/google_transcriber.py
--rw-r--r--   0        0        0     4800 2023-04-12 08:05:58.014523 vocode-0.1.94/vocode/streaming/transcriber/rev_ai_transcriber.py
--rw-r--r--   0        0        0     3353 2023-04-11 23:13:05.536070 vocode-0.1.94/vocode/streaming/transcriber/whisper_cpp_transcriber.py
--rw-r--r--   0        0        0      216 2023-03-28 07:12:57.762251 vocode-0.1.94/vocode/streaming/user_implemented_agent/base_agent.py
--rw-r--r--   0        0        0      697 2023-03-28 07:12:57.762593 vocode-0.1.94/vocode/streaming/user_implemented_agent/restful_agent.py
--rw-r--r--   0        0        0     2183 2023-03-28 07:12:57.762008 vocode-0.1.94/vocode/streaming/user_implemented_agent/websocket_agent.py
--rw-r--r--   0        0        0     1768 2023-03-28 17:30:02.335417 vocode-0.1.94/vocode/streaming/utils/__init__.py
--rw-r--r--   0        0        0      125 2023-04-04 06:04:39.620775 vocode-0.1.94/vocode/streaming/utils/base_router.py
--rw-r--r--   0        0        0        0 2023-03-28 17:30:02.335448 vocode-0.1.94/vocode/streaming/utils/goodbye_embeddings/.gitkeep
--rw-r--r--   0        0        0     2237 2023-03-29 06:27:49.549508 vocode-0.1.94/vocode/streaming/utils/goodbye_model.py
--rw-r--r--   0        0        0     7782 2023-03-28 17:30:02.335881 vocode-0.1.94/vocode/streaming/utils/sse_client.py
--rw-r--r--   0        0        0     1085 2023-03-28 17:30:02.336058 vocode-0.1.94/vocode/streaming/utils/transcript.py
--rw-r--r--   0        0        0      233 2023-03-28 07:12:57.813897 vocode-0.1.94/vocode/turn_based/agent/base_agent.py
--rw-r--r--   0        0        0     1758 2023-04-11 23:08:06.680994 vocode-0.1.94/vocode/turn_based/agent/chat_gpt_agent.py
--rw-r--r--   0        0        0      155 2023-03-28 07:12:57.813754 vocode-0.1.94/vocode/turn_based/agent/echo_agent.py
--rw-r--r--   0        0        0      201 2023-03-28 07:12:57.817990 vocode-0.1.94/vocode/turn_based/input_device/base_input_device.py
--rw-r--r--   0        0        0     2040 2023-04-04 06:04:39.620961 vocode-0.1.94/vocode/turn_based/input_device/microphone_input.py
--rw-r--r--   0        0        0      185 2023-03-28 07:12:57.817099 vocode-0.1.94/vocode/turn_based/output_device/base_output_device.py
--rw-r--r--   0        0        0     1244 2023-04-04 06:04:39.621216 vocode-0.1.94/vocode/turn_based/output_device/speaker_output.py
--rw-r--r--   0        0        0     3579 2023-04-12 22:31:13.091927 vocode-0.1.94/vocode/turn_based/synthesizer/azure_synthesizer.py
--rw-r--r--   0        0        0      138 2023-03-28 07:12:57.815598 vocode-0.1.94/vocode/turn_based/synthesizer/base_synthesizer.py
--rw-r--r--   0        0        0     1733 2023-04-04 06:04:39.621772 vocode-0.1.94/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py
--rw-r--r--   0        0        0      409 2023-04-11 17:15:11.317870 vocode-0.1.94/vocode/turn_based/synthesizer/gtts_synthesizer.py
--rw-r--r--   0        0        0     1757 2023-04-14 18:44:08.059363 vocode-0.1.94/vocode/turn_based/synthesizer/play_ht_synthesizer.py
--rw-r--r--   0        0        0      973 2023-04-11 17:15:11.318340 vocode-0.1.94/vocode/turn_based/synthesizer/rime_synthesizer.py
--rw-r--r--   0        0        0      701 2023-04-14 17:25:24.206454 vocode-0.1.94/vocode/turn_based/synthesizer/stream_elements_synthesizer.py
--rw-r--r--   0        0        0      152 2023-03-28 07:12:57.812543 vocode-0.1.94/vocode/turn_based/transcriber/base_transcriber.py
--rw-r--r--   0        0        0     1532 2023-04-11 23:13:05.536284 vocode-0.1.94/vocode/turn_based/transcriber/whisper_cpp_transcriber.py
--rw-r--r--   0        0        0      770 2023-03-28 17:30:02.337446 vocode-0.1.94/vocode/turn_based/transcriber/whisper_transcriber.py
--rw-r--r--   0        0        0     1638 2023-03-28 07:12:57.817247 vocode-0.1.94/vocode/turn_based/turn_based_conversation.py
--rw-r--r--   0        0        0      872 2023-04-11 23:13:05.536499 vocode-0.1.94/vocode/utils/whisper_cpp/helpers.py
--rw-r--r--   0        0        0     2124 2023-04-11 23:13:05.536728 vocode-0.1.94/vocode/utils/whisper_cpp/whisper_params.py
--rw-r--r--   0        0        0    11497 1970-01-01 00:00:00.000000 vocode-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-28 17:29:00.108721 vocode-0.1.95/LICENSE
+-rw-r--r--   0        0        0     8266 2023-04-12 08:05:58.013355 vocode-0.1.95/README.md
+-rw-r--r--   0        0        0     2065 2023-04-16 02:36:25.106823 vocode-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0      308 2023-03-28 17:30:02.280446 vocode-0.1.95/vocode/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-16 02:29:23.736495 vocode-0.1.95/vocode/helpers.py
+-rw-r--r--   0        0        0     1543 2023-04-16 02:29:43.085893 vocode-0.1.95/vocode/streaming/agent/base_agent.py
+-rw-r--r--   0        0        0     2013 2023-04-16 02:34:07.911907 vocode-0.1.95/vocode/streaming/agent/bot_sentiment_analyser.py
+-rw-r--r--   0        0        0     6666 2023-04-16 02:29:49.146370 vocode-0.1.95/vocode/streaming/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      598 2023-04-16 02:29:55.603404 vocode-0.1.95/vocode/streaming/agent/echo_agent.py
+-rw-r--r--   0        0        0     1467 2023-04-11 21:06:59.691054 vocode-0.1.95/vocode/streaming/agent/factory.py
+-rw-r--r--   0        0        0     1481 2023-03-28 17:30:02.281854 vocode-0.1.95/vocode/streaming/agent/information_retrieval_agent.py
+-rw-r--r--   0        0        0     5731 2023-04-16 02:30:01.602687 vocode-0.1.95/vocode/streaming/agent/llm_agent.py
+-rw-r--r--   0        0        0     2060 2023-04-16 02:30:19.787530 vocode-0.1.95/vocode/streaming/agent/restful_user_implemented_agent.py
+-rw-r--r--   0        0        0      684 2023-03-28 17:30:02.282322 vocode-0.1.95/vocode/streaming/agent/utils.py
+-rw-r--r--   0        0        0     3259 2023-04-04 06:04:39.618650 vocode-0.1.95/vocode/streaming/client_backend/conversation.py
+-rw-r--r--   0        0        0       96 2023-03-28 17:30:02.282460 vocode-0.1.95/vocode/streaming/constants.py
+-rw-r--r--   0        0        0     3724 2023-04-12 18:22:27.897471 vocode-0.1.95/vocode/streaming/hosted_streaming_conversation.py
+-rw-r--r--   0        0        0      476 2023-03-28 07:12:57.812101 vocode-0.1.95/vocode/streaming/input_device/base_input_device.py
+-rw-r--r--   0        0        0     1638 2023-04-16 02:26:04.321472 vocode-0.1.95/vocode/streaming/input_device/microphone_input.py
+-rw-r--r--   0        0        0      334 2023-03-28 07:12:57.811970 vocode-0.1.95/vocode/streaming/input_device/telephone_input.py
+-rw-r--r--   0        0        0     5320 2023-04-16 02:28:10.013958 vocode-0.1.95/vocode/streaming/models/agent.py
+-rw-r--r--   0        0        0      102 2023-03-28 17:30:02.283498 vocode-0.1.95/vocode/streaming/models/audio_encoding.py
+-rw-r--r--   0        0        0      856 2023-04-03 01:45:30.651534 vocode-0.1.95/vocode/streaming/models/events.py
+-rw-r--r--   0        0        0      299 2023-03-28 07:12:57.772953 vocode-0.1.95/vocode/streaming/models/message.py
+-rw-r--r--   0        0        0     1455 2023-03-28 17:30:02.283821 vocode-0.1.95/vocode/streaming/models/model.py
+-rw-r--r--   0        0        0     3706 2023-04-16 02:34:16.026032 vocode-0.1.95/vocode/streaming/models/synthesizer.py
+-rw-r--r--   0        0        0     1806 2023-03-28 17:30:02.284366 vocode-0.1.95/vocode/streaming/models/telephony.py
+-rw-r--r--   0        0        0     3254 2023-04-12 08:06:19.437996 vocode-0.1.95/vocode/streaming/models/transcriber.py
+-rw-r--r--   0        0        0     1765 2023-04-04 06:04:39.619062 vocode-0.1.95/vocode/streaming/models/websocket.py
+-rw-r--r--   0        0        0      396 2023-03-28 17:30:02.285240 vocode-0.1.95/vocode/streaming/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1015 2023-03-28 07:12:57.807120 vocode-0.1.95/vocode/streaming/output_device/speaker_output.py
+-rw-r--r--   0        0        0      262 2023-03-28 07:12:57.809162 vocode-0.1.95/vocode/streaming/output_device/telephone_output.py
+-rw-r--r--   0        0        0     1148 2023-04-04 06:04:39.619476 vocode-0.1.95/vocode/streaming/output_device/twilio_output_device.py
+-rw-r--r--   0        0        0      800 2023-04-04 06:04:39.619698 vocode-0.1.95/vocode/streaming/output_device/websocket_output_device.py
+-rw-r--r--   0        0        0    21227 2023-04-16 02:29:35.185728 vocode-0.1.95/vocode/streaming/streaming_conversation.py
+-rw-r--r--   0        0        0    10583 2023-04-16 02:34:21.809757 vocode-0.1.95/vocode/streaming/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0     7708 2023-04-16 02:34:30.750962 vocode-0.1.95/vocode/streaming/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     2355 2023-04-12 08:05:58.014267 vocode-0.1.95/vocode/streaming/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0     1448 2023-04-11 21:06:59.693827 vocode-0.1.95/vocode/streaming/synthesizer/factory.py
+-rw-r--r--   0        0        0  6548060 2023-03-28 17:30:02.328281 vocode-0.1.95/vocode/streaming/synthesizer/filler_audio/typing-noise.wav
+-rw-r--r--   0        0        0     3396 2023-04-11 21:06:59.694063 vocode-0.1.95/vocode/streaming/synthesizer/google_synthesizer.py
+-rw-r--r--   0        0        0     1252 2023-04-14 17:21:46.738980 vocode-0.1.95/vocode/streaming/synthesizer/gtts_synthesizer.py
+-rw-r--r--   0        0        0     2463 2023-04-11 21:06:59.694296 vocode-0.1.95/vocode/streaming/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0     1795 2023-04-12 06:50:30.491534 vocode-0.1.95/vocode/streaming/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0     1453 2023-04-14 17:19:36.773276 vocode-0.1.95/vocode/streaming/synthesizer/stream_elements_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.329443 vocode-0.1.95/vocode/streaming/telephony/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-28 17:30:02.330427 vocode-0.1.95/vocode/streaming/telephony/config_manager/base_config_manager.py
+-rw-r--r--   0        0        0      609 2023-03-28 23:14:27.148000 vocode-0.1.95/vocode/streaming/telephony/config_manager/in_memory_config_manager.py
+-rw-r--r--   0        0        0     1248 2023-03-28 17:30:02.331245 vocode-0.1.95/vocode/streaming/telephony/config_manager/redis_config_manager.py
+-rw-r--r--   0        0        0      170 2023-03-28 17:30:02.331397 vocode-0.1.95/vocode/streaming/telephony/constants.py
+-rw-r--r--   0        0        0     6799 2023-04-11 21:06:59.694996 vocode-0.1.95/vocode/streaming/telephony/conversation/call.py
+-rw-r--r--   0        0        0     4136 2023-04-11 17:15:11.315392 vocode-0.1.95/vocode/streaming/telephony/conversation/outbound_call.py
+-rw-r--r--   0        0        0     2802 2023-03-28 17:30:02.332164 vocode-0.1.95/vocode/streaming/telephony/conversation/zoom_dial_in.py
+-rw-r--r--   0        0        0      106 2023-04-03 01:45:30.652609 vocode-0.1.95/vocode/streaming/telephony/hosted/exceptions.py
+-rw-r--r--   0        0        0     2264 2023-03-28 17:30:02.332438 vocode-0.1.95/vocode/streaming/telephony/hosted/inbound_call_server.py
+-rw-r--r--   0        0        0     1697 2023-03-28 17:30:02.332777 vocode-0.1.95/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py
+-rw-r--r--   0        0        0     3032 2023-04-03 01:45:30.652914 vocode-0.1.95/vocode/streaming/telephony/hosted/outbound_call.py
+-rw-r--r--   0        0        0     2458 2023-04-03 01:45:30.653149 vocode-0.1.95/vocode/streaming/telephony/hosted/zoom_dial_in.py
+-rw-r--r--   0        0        0     5851 2023-04-16 02:27:33.229170 vocode-0.1.95/vocode/streaming/telephony/server/base.py
+-rw-r--r--   0        0        0     2439 2023-04-11 21:06:59.695619 vocode-0.1.95/vocode/streaming/telephony/server/router/calls.py
+-rw-r--r--   0        0        0      865 2023-04-04 06:04:39.620616 vocode-0.1.95/vocode/streaming/telephony/server/router/twiml.py
+-rw-r--r--   0        0        0      150 2023-03-28 17:30:02.333925 vocode-0.1.95/vocode/streaming/telephony/templates/connect_call.xml
+-rw-r--r--   0        0        0      653 2023-03-28 17:30:02.333757 vocode-0.1.95/vocode/streaming/telephony/templates.py
+-rw-r--r--   0        0        0      434 2023-04-11 21:06:59.695870 vocode-0.1.95/vocode/streaming/telephony/twilio.py
+-rw-r--r--   0        0        0     2220 2023-03-21 03:19:41.096039 vocode-0.1.95/vocode/streaming/telephony/zoom_dial_in.py
+-rw-r--r--   0        0        0     3452 2023-04-12 08:03:51.421371 vocode-0.1.95/vocode/streaming/transcriber/assembly_ai_transcriber.py
+-rw-r--r--   0        0        0     1241 2023-04-11 21:06:59.696653 vocode-0.1.95/vocode/streaming/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     7975 2023-04-12 07:59:00.960353 vocode-0.1.95/vocode/streaming/transcriber/deepgram_transcriber.py
+-rw-r--r--   0        0        0     1249 2023-04-12 08:05:58.014409 vocode-0.1.95/vocode/streaming/transcriber/factory.py
+-rw-r--r--   0        0        0     4377 2023-04-12 08:00:45.683444 vocode-0.1.95/vocode/streaming/transcriber/google_transcriber.py
+-rw-r--r--   0        0        0     4800 2023-04-12 08:05:58.014523 vocode-0.1.95/vocode/streaming/transcriber/rev_ai_transcriber.py
+-rw-r--r--   0        0        0     3353 2023-04-11 23:13:05.536070 vocode-0.1.95/vocode/streaming/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      216 2023-03-28 07:12:57.762251 vocode-0.1.95/vocode/streaming/user_implemented_agent/base_agent.py
+-rw-r--r--   0        0        0      697 2023-03-28 07:12:57.762593 vocode-0.1.95/vocode/streaming/user_implemented_agent/restful_agent.py
+-rw-r--r--   0        0        0     2183 2023-03-28 07:12:57.762008 vocode-0.1.95/vocode/streaming/user_implemented_agent/websocket_agent.py
+-rw-r--r--   0        0        0     1768 2023-03-28 17:30:02.335417 vocode-0.1.95/vocode/streaming/utils/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-04 06:04:39.620775 vocode-0.1.95/vocode/streaming/utils/base_router.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.335448 vocode-0.1.95/vocode/streaming/utils/goodbye_embeddings/.gitkeep
+-rw-r--r--   0        0        0     2237 2023-03-29 06:27:49.549508 vocode-0.1.95/vocode/streaming/utils/goodbye_model.py
+-rw-r--r--   0        0        0     7782 2023-03-28 17:30:02.335881 vocode-0.1.95/vocode/streaming/utils/sse_client.py
+-rw-r--r--   0        0        0     1109 2023-04-16 02:27:08.021157 vocode-0.1.95/vocode/streaming/utils/transcript.py
+-rw-r--r--   0        0        0      233 2023-03-28 07:12:57.813897 vocode-0.1.95/vocode/turn_based/agent/base_agent.py
+-rw-r--r--   0        0        0     1758 2023-04-11 23:08:06.680994 vocode-0.1.95/vocode/turn_based/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      155 2023-03-28 07:12:57.813754 vocode-0.1.95/vocode/turn_based/agent/echo_agent.py
+-rw-r--r--   0        0        0      201 2023-03-28 07:12:57.817990 vocode-0.1.95/vocode/turn_based/input_device/base_input_device.py
+-rw-r--r--   0        0        0     2030 2023-04-16 02:26:10.297748 vocode-0.1.95/vocode/turn_based/input_device/microphone_input.py
+-rw-r--r--   0        0        0      185 2023-03-28 07:12:57.817099 vocode-0.1.95/vocode/turn_based/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1244 2023-04-04 06:04:39.621216 vocode-0.1.95/vocode/turn_based/output_device/speaker_output.py
+-rw-r--r--   0        0        0     3579 2023-04-12 22:31:13.091927 vocode-0.1.95/vocode/turn_based/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0      138 2023-03-28 07:12:57.815598 vocode-0.1.95/vocode/turn_based/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     1733 2023-04-04 06:04:39.621772 vocode-0.1.95/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0      409 2023-04-11 17:15:11.317870 vocode-0.1.95/vocode/turn_based/synthesizer/gtts_synthesizer.py
+-rw-r--r--   0        0        0     1757 2023-04-14 18:44:08.059363 vocode-0.1.95/vocode/turn_based/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0      973 2023-04-11 17:15:11.318340 vocode-0.1.95/vocode/turn_based/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0      701 2023-04-14 17:25:24.206454 vocode-0.1.95/vocode/turn_based/synthesizer/stream_elements_synthesizer.py
+-rw-r--r--   0        0        0      152 2023-03-28 07:12:57.812543 vocode-0.1.95/vocode/turn_based/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     1532 2023-04-11 23:13:05.536284 vocode-0.1.95/vocode/turn_based/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      770 2023-03-28 17:30:02.337446 vocode-0.1.95/vocode/turn_based/transcriber/whisper_transcriber.py
+-rw-r--r--   0        0        0     1638 2023-03-28 07:12:57.817247 vocode-0.1.95/vocode/turn_based/turn_based_conversation.py
+-rw-r--r--   0        0        0      872 2023-04-11 23:13:05.536499 vocode-0.1.95/vocode/utils/whisper_cpp/helpers.py
+-rw-r--r--   0        0        0     2124 2023-04-11 23:13:05.536728 vocode-0.1.95/vocode/utils/whisper_cpp/whisper_params.py
+-rw-r--r--   0        0        0    11547 1970-01-01 00:00:00.000000 vocode-0.1.95/PKG-INFO
```

### Comparing `vocode-0.1.94/LICENSE` & `vocode-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/README.md` & `vocode-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/pyproject.toml` & `vocode-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "vocode"
-version = "0.1.94"
+version = "0.1.95"
 description = "The all-in-one voice SDK"
 authors = ["Ajay Raj <ajay@vocode.dev>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/vocodedev/vocode-python"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pydantic = ">=1.9.0"
 python-dotenv = ">=0.21.1"
 typing-extensions = ">=3.10.0.2"
 websockets = "10.4"
 anyio = "3.6.2"
 certifi = "2022.12.7"
 cffi = "1.15.1"
```

### Comparing `vocode-0.1.94/vocode/helpers.py` & `vocode-0.1.95/vocode/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import List, Tuple, Union
 import sounddevice as sd
 from vocode.streaming.input_device.microphone_input import (
     MicrophoneInput as StreamingMicrophoneInput,
 )
 from vocode.streaming.output_device.speaker_output import (
     SpeakerOutput as StreamingSpeakerOutput,
 )
@@ -13,15 +13,15 @@
     SpeakerOutput as TurnBasedSpeakerOutput,
 )
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-def _get_device_prompt(device_infos: list[dict]) -> str:
+def _get_device_prompt(device_infos: List[dict]) -> str:
     return """Please select a device:
 {}
 Choice: """.format(
         "\n".join(
             f"{index}: {device['name']}" for index, device in enumerate(device_infos)
         )
     )
@@ -29,16 +29,16 @@
 
 def create_microphone_input_and_speaker_output(
     streaming: bool = True,
     use_default_devices=False,
     mic_sampling_rate=None,
     speaker_sampling_rate=None,
 ) -> Union[
-    tuple[StreamingMicrophoneInput, StreamingSpeakerOutput],
-    tuple[TurnBasedMicrophoneInput, TurnBasedSpeakerOutput],
+    Tuple[StreamingMicrophoneInput, StreamingSpeakerOutput],
+    Tuple[TurnBasedMicrophoneInput, TurnBasedSpeakerOutput],
 ]:
     device_infos = sd.query_devices()
     input_device_infos = list(
         filter(lambda device_info: device_info["max_input_channels"] > 0, device_infos)
     )
     output_device_infos = list(
         filter(lambda device_info: device_info["max_output_channels"] > 0, device_infos)
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/base_agent.py` & `vocode-0.1.95/vocode/streaming/agent/base_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import random
-from typing import Generator, Optional
+from typing import Generator, Optional, Tuple
 from vocode.streaming.models.agent import (
     AgentConfig,
     ChatGPTAgentConfig,
     LLMAgentConfig,
 )
 
 
@@ -21,15 +21,15 @@
         pass
 
     def respond(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
-    ) -> tuple[Optional[str], bool]:
+    ) -> Tuple[Optional[str], bool]:
         raise NotImplementedError
 
     def generate_response(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/bot_sentiment_analyser.py` & `vocode-0.1.95/vocode/streaming/agent/bot_sentiment_analyser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 from langchain.llms import OpenAI
 from langchain.prompts import PromptTemplate
 from pydantic import BaseModel
 
 from vocode import getenv
 
 TEMPLATE = """
@@ -19,15 +19,15 @@
     emotion: Optional[str] = None
     degree: float = 0.0
 
 
 class BotSentimentAnalyser:
     def __init__(
         self,
-        emotions: list[str],
+        emotions: List[str],
         model_name: str = "text-davinci-003",
         openai_api_key: Optional[str] = None,
     ):
         self.model_name = model_name
         openai_api_key = openai_api_key or getenv("OPENAI_API_KEY")
         if not openai_api_key:
             raise ValueError("OPENAI_API_KEY must be set in environment or passed in")
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/chat_gpt_agent.py` & `vocode-0.1.95/vocode/streaming/agent/chat_gpt_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from langchain.chains import ConversationChain
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import OpenAIChat
 from langchain.memory import ConversationBufferMemory
 from langchain.schema import ChatMessage, AIMessage
 import openai
 import json
-from typing import Generator, Optional
+from typing import Generator, Optional, Tuple
 
 from typing import Generator
 import logging
 from vocode import getenv
 
 from vocode.streaming.agent.base_agent import BaseAgent
 from vocode.streaming.models.agent import ChatGPTAgentConfig
@@ -80,15 +80,15 @@
         return self.conversation.predict(input=first_prompt)
 
     def respond(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
-    ) -> tuple[str, bool]:
+    ) -> Tuple[str, bool]:
         if is_interrupt and self.agent_config.cut_off_response:
             cut_off_response = self.get_cut_off_response()
             self.memory.chat_memory.add_user_message(human_input)
             self.memory.chat_memory.add_ai_message(cut_off_response)
             return cut_off_response, False
         self.logger.debug("LLM responding to human input")
         if self.is_first_response and self.first_response:
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/echo_agent.py` & `vocode-0.1.95/vocode/streaming/agent/echo_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Generator, Optional
+from typing import Generator, Optional, Tuple
 from vocode.streaming.agent.base_agent import BaseAgent
 
 
 class EchoAgent(BaseAgent):
     def respond(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
-    ) -> tuple[str, bool]:
+    ) -> Tuple[str, bool]:
         return human_input, False
 
     def generate_response(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/factory.py` & `vocode-0.1.95/vocode/streaming/agent/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/agent/information_retrieval_agent.py` & `vocode-0.1.95/vocode/streaming/agent/information_retrieval_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/agent/llm_agent.py` & `vocode-0.1.95/vocode/streaming/agent/llm_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional
+from typing import Optional, Tuple
 
 from langchain import OpenAI
 from langchain.llms import OpenAIChat
 from typing import Generator
 import logging
 from vocode import getenv
 
@@ -71,15 +71,15 @@
         return f"{self.recipient}: {human_input}\n{self.sender}: {response}"
 
     def respond(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
-    ) -> tuple[str, bool]:
+    ) -> Tuple[str, bool]:
         if is_interrupt and self.agent_config.cut_off_response:
             cut_off_response = self.get_cut_off_response()
             self.memory.append(self.get_memory_entry(human_input, cut_off_response))
             return cut_off_response, False
         self.logger.debug("LLM responding to human input")
         if self.is_first_response and self.first_response:
             self.logger.debug("First response is cached")
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/restful_user_implemented_agent.py` & `vocode-0.1.95/vocode/streaming/agent/restful_user_implemented_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..models.agent import (
     RESTfulUserImplementedAgentConfig,
     RESTfulAgentInput,
     RESTfulAgentOutput,
     RESTfulAgentOutputType,
     RESTfulAgentText,
 )
-from typing import Generator, Optional, cast
+from typing import Generator, Optional, Tuple, cast
 import requests
 import logging
 
 
 class RESTfulUserImplementedAgent(BaseAgent):
     def __init__(
         self,
@@ -26,15 +26,15 @@
         self.logger = logger or logging.getLogger(__name__)
 
     def respond(
         self,
         human_input,
         is_interrupt: bool = False,
         conversation_id: Optional[str] = None,
-    ) -> tuple[Optional[str], bool]:
+    ) -> Tuple[Optional[str], bool]:
         config = self.agent_config.respond
         try:
             agent_response = requests.request(
                 method=config.method,
                 url=config.url,
                 json=RESTfulAgentInput(
                     human_input=human_input, conversation_id=conversation_id
```

### Comparing `vocode-0.1.94/vocode/streaming/agent/utils.py` & `vocode-0.1.95/vocode/streaming/agent/utils.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/client_backend/conversation.py` & `vocode-0.1.95/vocode/streaming/client_backend/conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/hosted_streaming_conversation.py` & `vocode-0.1.95/vocode/streaming/hosted_streaming_conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/input_device/microphone_input.py` & `vocode-0.1.95/vocode/streaming/input_device/microphone_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             device=int(self.device_info["index"]),
             callback=self._stream_callback,
         )
         self.stream.start()
         self.queue = queue.Queue()
         self.microphone_gain = microphone_gain
 
-    def _stream_callback(self, in_data: np.ndarray[np.int16], *_args):
+    def _stream_callback(self, in_data: np.ndarray, *_args):
         if self.microphone_gain > 1:
             in_data = in_data * (2 ^ self.microphone_gain)
         else:
             in_data = in_data // (2 ^ self.microphone_gain)
         audio_bytes = in_data.tobytes()
         self.queue.put_nowait(audio_bytes)
```

### Comparing `vocode-0.1.94/vocode/streaming/models/agent.py` & `vocode-0.1.95/vocode/streaming/models/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 from enum import Enum
 
 from pydantic import validator
 
 from vocode.streaming.models.message import BaseMessage
 from .model import TypedModel, BaseModel
 
@@ -50,15 +50,15 @@
     end_conversation_on_goodbye: bool = False
     send_filler_audio: Union[bool, FillerAudioConfig] = False
     webhook_config: Optional[WebhookConfig] = None
     track_bot_sentiment: bool = False
 
 
 class CutOffResponse(BaseModel):
-    messages: list[BaseMessage] = [BaseMessage(text="Sorry?")]
+    messages: List[BaseMessage] = [BaseMessage(text="Sorry?")]
 
 
 class LLMAgentConfig(AgentConfig, type=AgentType.LLM.value):
     prompt_preamble: str
     expected_first_prompt: Optional[str] = None
     model_name: str = LLM_AGENT_DEFAULT_MODEL_NAME
     temperature: float = LLM_AGENT_DEFAULT_TEMPERATURE
@@ -78,15 +78,15 @@
 
 class InformationRetrievalAgentConfig(
     AgentConfig, type=AgentType.INFORMATION_RETRIEVAL.value
 ):
     recipient_descriptor: str
     caller_descriptor: str
     goal_description: str
-    fields: list[str]
+    fields: List[str]
     # TODO: add fields for IVR, voicemail
 
 
 class EchoAgentConfig(AgentConfig, type=AgentType.ECHO.value):
     pass
```

### Comparing `vocode-0.1.94/vocode/streaming/models/events.py` & `vocode-0.1.95/vocode/streaming/models/events.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/models/model.py` & `vocode-0.1.95/vocode/streaming/models/model.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/models/synthesizer.py` & `vocode-0.1.95/vocode/streaming/models/synthesizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from pydantic import BaseModel, validator
 
 from vocode.streaming.output_device.base_output_device import BaseOutputDevice
 from vocode.streaming.telephony.constants import (
     DEFAULT_AUDIO_ENCODING,
     DEFAULT_SAMPLING_RATE,
@@ -18,15 +18,15 @@
     GOOGLE = "synthesizer_google"
     ELEVEN_LABS = "synthesizer_eleven_labs"
     RIME = "synthesizer_rime"
     PLAY_HT = "synthesizer_play_ht"
 
 
 class SentimentConfig(BaseModel):
-    emotions: list[str] = ["angry", "friendly", "sad", "whispering"]
+    emotions: List[str] = ["angry", "friendly", "sad", "whispering"]
 
     @validator("emotions")
     def emotions_must_not_be_empty(cls, v):
         if len(v) == 0:
             raise ValueError("must have at least one emotion")
         return v
```

### Comparing `vocode-0.1.94/vocode/streaming/models/telephony.py` & `vocode-0.1.95/vocode/streaming/models/telephony.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/models/transcriber.py` & `vocode-0.1.95/vocode/streaming/models/transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/models/websocket.py` & `vocode-0.1.95/vocode/streaming/models/websocket.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/output_device/speaker_output.py` & `vocode-0.1.95/vocode/streaming/output_device/speaker_output.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/output_device/twilio_output_device.py` & `vocode-0.1.95/vocode/streaming/output_device/twilio_output_device.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/output_device/websocket_output_device.py` & `vocode-0.1.95/vocode/streaming/output_device/websocket_output_device.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/streaming_conversation.py` & `vocode-0.1.95/vocode/streaming/streaming_conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import queue
-from typing import Awaitable, Callable, Optional, Any
+from typing import Awaitable, Callable, Optional, Any, Tuple
 import logging
 import threading
 import time
 import random
 
 from vocode.streaming.agent.bot_sentiment_analyser import (
     BotSentimentAnalyser,
@@ -162,15 +162,15 @@
         self.transcriber.send_audio(chunk)
 
     async def send_messages_to_stream_async(
         self,
         messages,
         should_allow_human_to_cut_off_bot: bool,
         wait_for_filler_audio: bool = False,
-    ) -> tuple[str, bool]:
+    ) -> Tuple[str, bool]:
         messages_queue = queue.Queue()
         messages_done = threading.Event()
         speech_cut_off = threading.Event()
         seconds_per_chunk = TEXT_TO_SPEECH_CHUNK_SIZE_SECONDS
         chunk_size = (
             get_chunk_size_per_second(
                 self.synthesizer.get_synthesizer_config().audio_encoding,
@@ -246,15 +246,15 @@
             self.synthesizer_event_loop,
         )
 
     async def send_message_to_stream_async(
         self,
         message: BaseMessage,
         should_allow_human_to_cut_off_bot: bool,
-    ) -> tuple[str, bool]:
+    ) -> Tuple[str, bool]:
         self.is_current_synthesis_interruptable = should_allow_human_to_cut_off_bot
         stop_event = self.enqueue_stop_event()
         self.logger.debug("Synthesizing speech for message")
         seconds_per_chunk = TEXT_TO_SPEECH_CHUNK_SIZE_SECONDS
         chunk_size = (
             get_chunk_size_per_second(
                 self.synthesizer.get_synthesizer_config().audio_encoding,
```

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/azure_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/azure_synthesizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import re
-from typing import Any, Optional
+from typing import Any, List, Optional, Tuple
 from xml.etree import ElementTree
 import azure.cognitiveservices.speech as speechsdk
 from vocode import getenv
 
 from vocode.streaming.agent.bot_sentiment_analyser import BotSentiment
 from vocode.streaming.models.message import BaseMessage, SSMLMessage
 
@@ -104,15 +104,15 @@
         )
 
         self.voice_name = self.synthesizer_config.voice_name
         self.pitch = self.synthesizer_config.pitch
         self.rate = self.synthesizer_config.rate
         self.logger = logger or logging.getLogger(__name__)
 
-    def get_phrase_filler_audios(self) -> list[FillerAudio]:
+    def get_phrase_filler_audios(self) -> List[FillerAudio]:
         filler_phrase_audios = []
         for filler_phrase in FILLER_PHRASES:
             cache_key = "-".join(
                 (
                     str(filler_phrase.text),
                     str(self.synthesizer_config.type),
                     str(self.synthesizer_config.audio_encoding),
@@ -177,15 +177,15 @@
             voice_root = styled
         prosody = ElementTree.SubElement(voice_root, "prosody")
         prosody.set("pitch", f"{self.pitch}%")
         prosody.set("rate", f"{self.rate}%")
         prosody.text = message.strip()
         return ElementTree.tostring(ssml_root, encoding="unicode")
 
-    def synthesize_ssml(self, ssml: str) -> tuple[speechsdk.AudioDataStream, str]:
+    def synthesize_ssml(self, ssml: str) -> Tuple[speechsdk.AudioDataStream, str]:
         result = self.synthesizer.start_speaking_ssml_async(ssml).get()
         return speechsdk.AudioDataStream(result)
 
     def ready_synthesizer(self):
         connection = speechsdk.Connection.from_speech_synthesizer(self.synthesizer)
         connection.open(True)
```

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/base_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/base_synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Any, Generator, Callable, Optional
+from typing import Any, Generator, Callable, List, Optional
 import math
 import io
 import wave
 from nltk.tokenize import word_tokenize
 from nltk.tokenize.treebank import TreebankWordDetokenizer
 
 from vocode.streaming.agent.bot_sentiment_analyser import BotSentiment
@@ -101,15 +101,15 @@
 class BaseSynthesizer:
     def __init__(self, synthesizer_config: SynthesizerConfig):
         self.synthesizer_config = synthesizer_config
         if synthesizer_config.audio_encoding == AudioEncoding.MULAW:
             assert (
                 synthesizer_config.sampling_rate == 8000
             ), "MuLaw encoding only supports 8kHz sampling rate"
-        self.filler_audios: list[FillerAudio] = []
+        self.filler_audios: List[FillerAudio] = []
 
     def get_synthesizer_config(self) -> SynthesizerConfig:
         return self.synthesizer_config
 
     def get_typing_noise_filler_audio(self) -> FillerAudio:
         return FillerAudio(
             message=BaseMessage(text="<typing noise>"),
@@ -125,15 +125,15 @@
 
     def set_filler_audios(self, filler_audio_config: FillerAudioConfig):
         if filler_audio_config.use_phrases:
             self.filler_audios = self.get_phrase_filler_audios()
         elif filler_audio_config.use_typing_noise:
             self.filler_audios = [self.get_typing_noise_filler_audio()]
 
-    def get_phrase_filler_audios(self) -> list[FillerAudio]:
+    def get_phrase_filler_audios(self) -> List[FillerAudio]:
         return []
 
     def ready_synthesizer(self):
         pass
 
     # given the number of seconds the message was allowed to go until, where did we get in the message?
     def get_message_cutoff_from_total_response_length(
@@ -150,15 +150,15 @@
     ) -> str:
         words_per_second = words_per_minute / 60
         estimated_words_spoken = math.floor(words_per_second * seconds)
         tokens = word_tokenize(message.text)
         return TreebankWordDetokenizer().detokenize(tokens[:estimated_words_spoken])
 
     # returns a chunk generator and a thunk that can tell you what part of the message was read given the number of seconds spoken
-    # chunk generator must return tuple (bytes of size chunk_size, flag if it is the last chunk)
+    # chunk generator must return a ChunkResult, essentially a tuple (bytes of size chunk_size, flag if it is the last chunk)
     def create_speech(
         self,
         message: BaseMessage,
         chunk_size: int,
         bot_sentiment: Optional[BotSentiment] = None,
     ) -> SynthesisResult:
         raise NotImplementedError
```

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/eleven_labs_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/factory.py` & `vocode-0.1.95/vocode/streaming/synthesizer/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/filler_audio/typing-noise.wav` & `vocode-0.1.95/vocode/streaming/synthesizer/filler_audio/typing-noise.wav`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/google_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/google_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/gtts_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/gtts_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/play_ht_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/play_ht_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/rime_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/synthesizer/stream_elements_synthesizer.py` & `vocode-0.1.95/vocode/streaming/synthesizer/stream_elements_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/config_manager/in_memory_config_manager.py` & `vocode-0.1.95/vocode/streaming/telephony/config_manager/in_memory_config_manager.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/config_manager/redis_config_manager.py` & `vocode-0.1.95/vocode/streaming/telephony/config_manager/redis_config_manager.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/conversation/call.py` & `vocode-0.1.95/vocode/streaming/telephony/conversation/call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/conversation/outbound_call.py` & `vocode-0.1.95/vocode/streaming/telephony/conversation/outbound_call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/conversation/zoom_dial_in.py` & `vocode-0.1.95/vocode/streaming/telephony/conversation/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/hosted/inbound_call_server.py` & `vocode-0.1.95/vocode/streaming/telephony/hosted/inbound_call_server.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py` & `vocode-0.1.95/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/hosted/outbound_call.py` & `vocode-0.1.95/vocode/streaming/telephony/hosted/outbound_call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/hosted/zoom_dial_in.py` & `vocode-0.1.95/vocode/streaming/telephony/hosted/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/server/base.py` & `vocode-0.1.95/vocode/streaming/telephony/server/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Optional
+from typing import List, Optional
 from fastapi import APIRouter, Form, Response
 from pydantic import BaseModel
 from vocode import getenv
 from vocode.streaming.agent.base_agent import BaseAgent
 from vocode.streaming.agent.factory import AgentFactory
 from vocode.streaming.models.agent import AgentConfig
 from vocode.streaming.models.synthesizer import (
@@ -55,15 +55,15 @@
 
 
 class TelephonyServer:
     def __init__(
         self,
         base_url: str,
         config_manager: BaseConfigManager,
-        inbound_call_configs: list[InboundCallConfig] = [],
+        inbound_call_configs: List[InboundCallConfig] = [],
         transcriber_factory: TranscriberFactory = TranscriberFactory(),
         agent_factory: AgentFactory = AgentFactory(),
         synthesizer_factory: SynthesizerFactory = SynthesizerFactory(),
         logger: Optional[logging.Logger] = None,
     ):
         self.base_url = base_url
         self.logger = logger or logging.getLogger(__name__)
```

### Comparing `vocode-0.1.94/vocode/streaming/telephony/server/router/calls.py` & `vocode-0.1.95/vocode/streaming/telephony/server/router/calls.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/server/router/twiml.py` & `vocode-0.1.95/vocode/streaming/telephony/server/router/twiml.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/templates.py` & `vocode-0.1.95/vocode/streaming/telephony/templates.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/telephony/zoom_dial_in.py` & `vocode-0.1.95/vocode/streaming/telephony/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/assembly_ai_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/assembly_ai_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/base_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/base_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/deepgram_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/deepgram_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/factory.py` & `vocode-0.1.95/vocode/streaming/transcriber/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/google_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/google_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/rev_ai_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/rev_ai_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/transcriber/whisper_cpp_transcriber.py` & `vocode-0.1.95/vocode/streaming/transcriber/whisper_cpp_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/user_implemented_agent/restful_agent.py` & `vocode-0.1.95/vocode/streaming/user_implemented_agent/restful_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/user_implemented_agent/websocket_agent.py` & `vocode-0.1.95/vocode/streaming/user_implemented_agent/websocket_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/utils/__init__.py` & `vocode-0.1.95/vocode/streaming/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/utils/goodbye_model.py` & `vocode-0.1.95/vocode/streaming/utils/goodbye_model.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/utils/sse_client.py` & `vocode-0.1.95/vocode/streaming/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/streaming/utils/transcript.py` & `vocode-0.1.95/vocode/streaming/utils/transcript.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from typing import List
 from pydantic import BaseModel, Field
 from enum import Enum
 
 
 class Sender(str, Enum):
     HUMAN = "human"
     BOT = "bot"
@@ -16,15 +17,15 @@
     def to_string(self, include_timestamp: bool = False) -> str:
         if include_timestamp:
             return f"{self.sender.name}: {self.text} ({self.timestamp})"
         return f"{self.sender.name}: {self.text}"
 
 
 class Transcript(BaseModel):
-    messages: list[Message] = []
+    messages: List[Message] = []
     start_time: float = Field(default_factory=time.time)
 
     def to_string(self, include_timestamps: bool = False) -> str:
         return "\n".join(
             message.to_string(include_timestamp=include_timestamps)
             for message in self.messages
         )
```

### Comparing `vocode-0.1.94/vocode/turn_based/agent/chat_gpt_agent.py` & `vocode-0.1.95/vocode/turn_based/agent/chat_gpt_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/input_device/microphone_input.py` & `vocode-0.1.95/vocode/turn_based/input_device/microphone_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         )
         self.active = False
 
     @classmethod
     def from_default_device(cls, sampling_rate: int = None):
         return cls(sd.query_devices(kind="input"), sampling_rate)
 
-    def _stream_callback(self, in_data: np.ndarray[np.int16], *_args):
+    def _stream_callback(self, in_data: np.ndarray, *_args):
         if self.active:
             audio_bytes = in_data.tobytes()
             self.wave_writer.writeframes(audio_bytes)
 
     def create_buffer(self):
         in_memory_wav = io.BytesIO()
         wave_writer = wave.open(in_memory_wav, "wb")
```

### Comparing `vocode-0.1.94/vocode/turn_based/output_device/speaker_output.py` & `vocode-0.1.95/vocode/turn_based/output_device/speaker_output.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/synthesizer/azure_synthesizer.py` & `vocode-0.1.95/vocode/turn_based/synthesizer/azure_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py` & `vocode-0.1.95/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/synthesizer/play_ht_synthesizer.py` & `vocode-0.1.95/vocode/turn_based/synthesizer/play_ht_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/synthesizer/rime_synthesizer.py` & `vocode-0.1.95/vocode/turn_based/synthesizer/rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/synthesizer/stream_elements_synthesizer.py` & `vocode-0.1.95/vocode/turn_based/synthesizer/stream_elements_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/transcriber/whisper_cpp_transcriber.py` & `vocode-0.1.95/vocode/turn_based/transcriber/whisper_cpp_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/transcriber/whisper_transcriber.py` & `vocode-0.1.95/vocode/turn_based/transcriber/whisper_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/turn_based/turn_based_conversation.py` & `vocode-0.1.95/vocode/turn_based/turn_based_conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/utils/whisper_cpp/helpers.py` & `vocode-0.1.95/vocode/utils/whisper_cpp/helpers.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/vocode/utils/whisper_cpp/whisper_params.py` & `vocode-0.1.95/vocode/utils/whisper_cpp/whisper_params.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.94/PKG-INFO` & `vocode-0.1.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: vocode
-Version: 0.1.94
+Version: 0.1.95
 Summary: The all-in-one voice SDK
 Home-page: https://github.com/vocodedev/vocode-python
 License: MIT
 Author: Ajay Raj
 Author-email: ajay@vocode.dev
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: io
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: aiosignal (==1.3.1)
 Requires-Dist: anyio (==3.6.2)
```

