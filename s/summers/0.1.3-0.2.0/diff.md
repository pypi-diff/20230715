# Comparing `tmp/summers-0.1.3-py3-none-any.whl.zip` & `tmp/summers-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8293 bytes, number of entries: 9
+Zip file size: 8395 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx     3225 b- defN 23-Jul-14 10:41 summers/__init__.py
 -rw-rw-r--  2.0 unx      354 b- defN 23-Jul-15 02:41 summers/cc.py
 -rw-rw-r--  2.0 unx     3371 b- defN 23-Jul-15 02:41 summers/di.py
 -rw-rw-r--  2.0 unx     1996 b- defN 23-Jul-15 02:41 summers/sc_imp.py
 -rw-rw-r--  2.0 unx     4092 b- defN 23-Jul-15 02:41 summers/sc_txt.py
--rw-rw-r--  2.0 unx     5227 b- defN 23-Jul-15 09:19 summers-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 09:19 summers-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-15 09:19 summers-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      660 b- defN 23-Jul-15 09:19 summers-0.1.3.dist-info/RECORD
-9 files, 19025 bytes uncompressed, 7173 bytes compressed:  62.3%
+-rw-rw-r--  2.0 unx     5405 b- defN 23-Jul-15 09:37 summers-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 09:37 summers-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-15 09:37 summers-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      660 b- defN 23-Jul-15 09:37 summers-0.2.0.dist-info/RECORD
+9 files, 19203 bytes uncompressed, 7275 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: summers/sc_imp.py
 Comment: 
 
 Filename: summers/sc_txt.py
 Comment: 
 
-Filename: summers-0.1.3.dist-info/METADATA
+Filename: summers-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: summers-0.1.3.dist-info/WHEEL
+Filename: summers-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: summers-0.1.3.dist-info/top_level.txt
+Filename: summers-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: summers-0.1.3.dist-info/RECORD
+Filename: summers-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `summers-0.1.3.dist-info/METADATA` & `summers-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summers
-Version: 0.1.3
+Version: 0.2.0
 Summary: 一个遵循整洁架构风格的 python 依赖注入框架 // A dependency injection framework like Spring (java framework), it conforms to a clean architecture style.
 Home-page: https://github.com/tuijs/summers
 Author: weiyi
 Author-email: 272654394@qq.com
 License: UNKNOWN
 Keywords: dependency injection,clean architecture,DI,IOC,DDD,依赖注入,整洁架构,领域驱动设计
 Platform: UNKNOWN
@@ -22,23 +22,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Summers
 
-Summers 是一款遵循 `整洁架构` 风格的 python 语言的 `依赖注入框架`, 主要参考了 java `spring` 框架进行设计和实现. 它很好地解决了 python 语言面向接口/抽象编程, 便捷地实现解耦.
+Summers 是一款遵循 `整洁架构` 风格的 python 语言的 `依赖注入框架`, 主要参考了 java `spring` 框架进行设计和实现 (也是个人由 java 转 python 后对 spring 的致敬之作). 它很好地解决了 python 语言面向接口/抽象编程, 便捷地实现解耦.
 
 框架的主要组成:
 
-- Summers: 依赖注入, 主要技术有: 反射, 装饰器, 单例, 动态导入等
-- Parser: 扫描解析器, 主要技术有: 正则表达式
+- Summers: 依赖注入, 主要技术有: `反射`, `装饰器`, `单例`, `动态导入` 等
+- Parser: 扫描解析器, 主要技术有: `正则表达式`
 - CleanArch: 整洁架构校验器
 
-使用过程中， 若有问题疑问， 可以在 <https://github.com/tuijs/summers/issues> 提 issue.
+声明: `该框架不涉及任何业务代码， 是一个纯粹的侵入性低的依赖注入框架`. 使用过程中， 若有问题疑问， 可以在 <https://github.com/tuijs/summers/issues> 提 issue.
 
 ## 1.快速入门
 
 ### 1.1 配置注解/装饰器
 
 注解是基于整洁架构分层风格来命名的, 主要包括:
 
@@ -114,19 +114,19 @@
 ```
 
 ### 1.2 配置及启动主程序
 
 
 #### 1.2.1 安装 summers
 
-已发布至 pypi: https://pypi.org/project/summers/0.1.3/
+已发布至 pypi: https://pypi.org/project/summers/0.2.0/
 
 ```python
 # 安装 summers 框架
-pip install summers==0.1.3
+pip install summers==0.2.0
 ```
 
 #### 1.2.2 普通应用程序
 
 可以直接 new 具体的实现类获取该实例, 框架也会自动注入依赖的对象, 但不建议这么用, 这违反了解耦的初衷.
 
 ```python
```

## Comparing `summers-0.1.3.dist-info/RECORD` & `summers-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 summers/__init__.py,sha256=-fggyGoWCQPgDwbwvAvgwyDtl5wZBdQyImpyWEprdmk,3225
 summers/cc.py,sha256=L1jCssoO0_YD0U2pxgBHFQdlnmVX6z3ZYEt36Gd9Kv4,354
 summers/di.py,sha256=idT-D_hOZCfeU6dppbuEiOJP_Zs7i867eLIYHWxQ0WA,3371
 summers/sc_imp.py,sha256=Q08Srd29Sfa5hnhdqsTetfX7yweYmD96YmARbWqzT4I,1996
 summers/sc_txt.py,sha256=siQUPEg5TFuOfRlavKRlllLRfpfWD2qfsUSOspfMV7I,4092
-summers-0.1.3.dist-info/METADATA,sha256=J6Wei2f7NtuJNQKg2mjJQSooG0a8ulUkaPk7D8W08Ko,5227
-summers-0.1.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-summers-0.1.3.dist-info/top_level.txt,sha256=k6Qomaj62_zErR8OF1SCi5dxZXAMHqM8Ayr27DcWJC0,8
-summers-0.1.3.dist-info/RECORD,,
+summers-0.2.0.dist-info/METADATA,sha256=2EqWuOFx74Wp4002HGRcpBxk20Vei6QCzOzsaWeXkYo,5405
+summers-0.2.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+summers-0.2.0.dist-info/top_level.txt,sha256=k6Qomaj62_zErR8OF1SCi5dxZXAMHqM8Ayr27DcWJC0,8
+summers-0.2.0.dist-info/RECORD,,
```

