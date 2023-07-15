# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar", last modified: Fri Jul 14 07:27:24 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar", last modified: Sat Jul 15 02:49:05 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.1/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    26051 2023-07-14 06:14:48.823684 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15847 2023-07-14 06:52:57.572497 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    17941 2023-07-14 05:24:38.854386 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    38151 2023-07-14 07:24:58.878281 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6326 2023-07-14 06:15:38.350677 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      728 2023-07-14 07:27:24.444210 nonebot_plugin_stable_diffusion_diao-0.3.9.1/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.2/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    26312 2023-07-15 02:38:33.308037 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15932 2023-07-15 02:22:12.577508 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17940 2023-07-15 02:42:00.196730 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11298 2023-07-15 02:23:36.589787 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    38132 2023-07-15 02:28:37.087912 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4417 2023-07-15 02:39:45.240818 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-07-15 02:49:05.693126 nonebot_plugin_stable_diffusion_diao-0.3.9.2/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.2/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
                            type=str, help="使用的lora", dest="lora")
 aidraw_parser.add_argument("-hr",
                            type=float, help="高清修复倍率", dest="hiresfix_scale")
 aidraw_parser.add_argument("-m",
                            type=str, help="更换模型", dest="model")
 aidraw_parser.add_argument("-match_off","-match-off",
                            action="store_true", help="关闭自动匹配", dest="match")
+aidraw_parser.add_argument("-sr_on","-sr-on",
+                           action="store_true", help="图片生产后再次超分", dest="sr")
 
 
 async def get_message_at(data: str) -> int:
     '''
     获取at列表
     :param data: event.json()
     '''
@@ -190,14 +192,15 @@
         if args.match or not config.auto_match:
             pass
         elif redis_client:
             r2 = redis_client[1]
             try:
                 tag = ""
                 if r2.exists("lora"):
+                    model_info = ""
                     all_lora_dict = r2.get("lora")
                     all_emb_dict = r2.get("emb")
                     all_backend_lora_list = ast.literal_eval(all_lora_dict.decode("utf-8"))
                     all_backend_emb_list = ast.literal_eval(all_emb_dict.decode("utf-8"))
                     cur_backend_lora_list = all_backend_lora_list[fifo.backend_name]
                     cur_backend_emb_list = all_backend_emb_list[fifo.backend_name]
                     if fifo.backend_name in all_backend_lora_list and all_backend_lora_list[fifo.backend_name] is None:
@@ -213,38 +216,40 @@
                     tag_index = -1
                     for tag in org_tag_list:
                         tag_index += 1
                         index = -1
                         for lora in list(cur_backend_lora_list.values()):
                             index += 1
                             if re.search(tag, lora, re.IGNORECASE):
-                                info_ = f"自动找到的lora模型: {lora}"
-                                fifo.extra_info += f"{info_}\n"
-                                logger.info(info_)
+                                model_info_ = f"自动找到的lora模型: {lora}\n"
+                                model_info += model_info_
+                                logger.info(model_info_)
                                 new_tags_list.append(f"<lora:{lora}:0.9>, ")
                                 tags_list.pop(org_tag_list.index(tag))
                                 break
                     tag_index = -1
                     for tag in org_tag_list:
                         tag_index += 1
                         index = -1
                         for emb in list(cur_backend_emb_list.values()):
                             index += 1
                             if re.search(tag, emb, re.IGNORECASE):
                                 new_tags_list.append(emb)
-                                info_ = f"自动找到的嵌入式模型: {emb}, "
-                                fifo.extra_info += f"{info_}\n"
-                                logger.info(info_)
+                                model_info_ += f"自动找到的嵌入式模型: {emb}, \n"
+                                model_info += model_info_
+                                logger.info(model_info_)
                                 tags_list.pop(org_tag_list.index(tag))
                                 break
                     if len(new_tags_list) >2:
                         new_tags_list = []
                         tags_list = org_tag_list
-                        fifo.extra_info += "↑以上模型未生效↑\n"
+                        fifo.extra_info += "自动匹配到的模型过多\n已关闭自动匹配功能"
+                        model_info = ""
                         raise RuntimeError("匹配到很多lora")
+                    fifo.extra_info += f"{model_info}\n"
             except Exception as e:
                 logger.warning(f"tag自动匹配失效,出现问题的: {tag}\n或者是prompt里自动匹配到的模型过多")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
             tags_list: str = await prepocess_tags(tags_list)
         except Exception as e:
             logger.debug(str(e))
@@ -315,16 +320,19 @@
         tags_list += lora_msg + emb_msg
         if args.no_trans:  # 不希望翻译的tags
             tags_list = tags_list + args.no_trans
         if not args.override:
             global pre_tags
             pre_tags = basetag + await config.get_value(group_id, "tags")
             pre_ntags = lowQuality
-            fifo.tags = pre_tags + "," + tags_list + "," + ",".join(new_tags_list) + style_tag
-            fifo.ntags = pre_ntags + fifo.ntags + style_ntag
+        else:
+            pre_tags = ""
+            pre_ntags = ""
+        fifo.tags = pre_tags + "," + tags_list + "," + ",".join(new_tags_list) + style_tag
+        fifo.ntags = pre_ntags + fifo.ntags + style_ntag
         if redis_client:
             tags_list_ = tags_to_list(tags_list)
             r1 = redis_client[0]
             pipe = r1.pipeline()
             pipe.rpush("prompts", str(tags_list_))
             pipe.rpush(fifo.user_id, str(dict(fifo)))
             pipe.execute()
@@ -487,26 +495,24 @@
                         )
             try:
                 if len(fifo.extra_info) != 0:
                     fifo.extra_info += "\n使用'-match_off'参数以关闭自动匹配功能\n"
                 message_data = await bot.send(event=event, 
                                           message=pic_message+f"模型:{os.path.basename(fifo.model)}\n{fifo.img_hash}", 
                                           at_sender=True, 
-                                          reply_message=True
             ) if (
                     await config.get_value(fifo.group_id, "pure")) or (
                     await config.get_value(fifo.group_id, "pure") is None and config.novelai_pure) else (
                     await send_forward_msg(bot=bot, event=event, name=nickname, uin=id, msgs=im)
                 )
 
             except ActionFailed:
                 message_data = await bot.send(event=event, 
                                              message=pic_message, 
                                              at_sender=True, 
-                                             reply_message=True
                                 )
 
             revoke = await config.get_value(fifo.group_id, "revoke")
             if revoke:
                 message_id = message_data["message_id"]
                 loop = get_running_loop()
                 loop.call_later(
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         man_shape: str = None,
         model: str = "",
         sampler: None or str = None,
         backend_index: str = None,
         disable_hr: bool = False if config.novelai_hr else True,
         hiresfix_scale: float = None,
         event: MessageEvent = None,
+        sr: bool = False,
         **kwargs,
     ):
         """
         AI绘画的核心部分,将与服务器通信的过程包装起来,并方便扩展服务器类型
 
         :user_id: 用户id,必须
         :group_id: 群聊id,如果是私聊则应置为0,必须
@@ -125,14 +126,15 @@
                            "controlnet_model": ""
                            }
         self.backend_info: dict = None
         self.task_type: str = None
         self.img_hash = None
         self.extra_info = ""
         self.audit_info = ""
+        self.sr = sr or config.novelai_SuperRes_generate
         
         # 数值合法检查
         if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
         if self.noise < 0 or self.noise > 1:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         "hr_upscaler": "Lanczos",  # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
         "hr_second_pass_steps": 7,  # 高清修复步数, 个人建议7是个不错的选择, 速度质量都不错
     } # 以上为个人推荐值
     novelai_SuperRes_MaxPixels: int = 2000  # 超分最大像素值, 对应(值)^2, 为了避免有人用超高分辨率的图来超分导致爆显存(
     novelai_SuperRes_generate: bool = False  # 图片生成后是否再次进行一次超分
     novelai_SuperRes_generate_payload: dict = {
         "upscaling_resize": 1.2,  # 超分倍率, 为长宽分辨率各X1.2
-        "upscaler_1": "Lanczos",  # 第一次超分使用的方法
+        "upscaler_1": "ScuNET",  # 第一次超分使用的方法
         "upscaler_2": "R-ESRGAN 4x+ Anime6B",  # 第二次超分使用的方法
-        "extras_upscaler_2_visibility": 0.7  # 第二层upscaler力度
+        "extras_upscaler_2_visibility": 0.6  # 第二层upscaler力度
     } # 以上为个人推荐值
     novelai_ControlNet_post_method: int = 0
     novelai_size_org: int = 640  # 最大分辨率
     if novelai_hr:
         novelai_size: int = novelai_size_org
     else:
         novelai_size: int = novelai_size_org * novelai_hr_payload["hr_scale"]
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     label = ""
     # 判读是否进行图片审核
     h = await config.get_value(fifo.group_id, "h")
     nsfw_count = 0
     for i in img_bytes:
         # try:
         if isinstance(fifo.event, PrivateMessageEvent):
-            if config.novelai_SuperRes_generate:
+            if fifo.sr:
                 try:
                     from ..extension.sd_extra_api_func import super_res_api_func
                     resp_tuple = await super_res_api_func(i, 3)
                     i = resp_tuple[0]
                 except:
                     logger.debug("超分API失效")
             if save_img_:
@@ -62,15 +62,15 @@
             try:
                 label, h_value, fifo.audit_info = await check_safe(i, fifo)
             except RuntimeError as e:
                 logger.error(f"NSFWAPI调用失败，错误代码为{e.args}")
                 label = "unknown"
             if label in ["safe", "general", "sensitive"]:
                 label = "_safe"
-                if config.novelai_SuperRes_generate:
+                if fifo.sr:
                     try:
                         from ..extension.sd_extra_api_func import super_res_api_func
                         resp_tuple = await super_res_api_func(i, 3)
                         for i in resp_tuple:
                             i = resp_tuple[0]
                     except:
                         pass
@@ -111,15 +111,15 @@
                                                              message=f"URL发送失败, 私聊消息发送失败, 请先加好友\n{fifo.img_hash}"
                                                              )
                                 except ActionFailed:
                                     await send_qr_code(bot, fifo, img_url)
                 elif htype == 3:
                     await send_qr_code(bot, fifo, img_url)
         else:
-            if config.novelai_SuperRes_generate:
+            if fifo.sr:
                 try:
                     from ..extension.sd_extra_api_func import super_res_api_func
                     resp_tuple = await super_res_api_func(i, 3)
                     i = resp_tuple[0]
                 except:
                     logger.debug("超分API失效")
             if save_img_:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     img_bytes = img_bytes.getvalue()
     img_base64 = base64.b64encode(img_bytes).decode("utf-8")
 # "data:image/jpeg;base64," + 
     payload = {"image": img_base64}
     payload.update(config.novelai_SuperRes_generate_payload)
     if upsale:
         payload["upscaling_resize"] = upsale
-    resp_tuple = await sd_LoadBalance(task_type="txt2img")
+    resp_tuple = await sd_LoadBalance()
     async with aiohttp.ClientSession() as session:
         api_url = "http://" + resp_tuple[1][0] + "/sdapi/v1/extra-single-image"
         async with session.post(url=api_url, json=payload) as resp:
             if resp.status not in [200, 201]:
                 raise RuntimeError
             else:
                 resp_json = await resp.json()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import aiohttp
 import asyncio 
 import random
 from nonebot import logger
 from ..config import config, redis_client
 import time
 from tqdm import tqdm
-from datetime import datetime
 
 import ast
 import traceback
 import aiofiles
 import json
 import os
 
@@ -41,16 +40,14 @@
     return vram_usage
 
 
 async def sd_LoadBalance():
     '''
     分别返回可用后端索引, 后端对应ip和名称(元组), 显存占用
     '''
-    current_date = datetime.now().date()
-    day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
     backend_url_dict = config.novelai_backend_url_dict
     reverse_dict = {value: key for key, value in backend_url_dict.items()}
     tasks = []
     is_avaiable = 0
     status_dict = {}
     ava_url = None
     n = -1
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.1/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.1"
+version = "0.3.9.2"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

