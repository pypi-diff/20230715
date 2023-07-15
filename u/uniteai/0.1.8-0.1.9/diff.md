# Comparing `tmp/uniteai-0.1.8.tar.gz` & `tmp/uniteai-0.1.9.tar.gz`

## Comparing `uniteai-0.1.8.tar` & `uniteai-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/.dir-locals.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/common.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/config.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/edit.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/llm_server.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/local_llm.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/lsp_server.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/openai.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/server.py
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/transcription.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/contrib/example.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.8/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.8/LICENSE
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.8/README.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uniteai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 uniteai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/.dir-locals.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/__init__.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/common.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/config.py
+-rw-r--r--   0        0        0    12010 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/edit.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/llm_server.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/local_llm.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/lsp_server.py
+-rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/openai.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/server.py
+-rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/transcription.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 uniteai-0.1.9/uniteai/contrib/example.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 uniteai-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 uniteai-0.1.9/README.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uniteai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 uniteai-0.1.9/PKG-INFO
```

### Comparing `uniteai-0.1.8/uniteai/common.py` & `uniteai-0.1.9/uniteai/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     CodeActionKind,
     CodeActionParams,
     Command,
     Position,
     Range,
     TextDocumentIdentifier,
     VersionedTextDocumentIdentifier,
+    OptionalVersionedTextDocumentIdentifier,
     TextEdit,
     WorkspaceEdit,
     DidChangeTextDocumentParams,
 )
 import logging
 
 
@@ -148,15 +149,15 @@
                    version: int,
                    start: Position,
                    end: Position,
                    new_text: str) -> WorkspaceEdit:
     ''' Build a `WorkspaceEdit` for pygls to send to LSP client. '''
     text_edit = TextEdit(range=Range(start=start, end=end), new_text=new_text)
     text_document_edit = {
-        'textDocument': VersionedTextDocumentIdentifier(uri=uri,
+        'textDocument': OptionalVersionedTextDocumentIdentifier(uri=uri,
                                                         version=version),
         'edits': [text_edit],
     }
     return WorkspaceEdit(document_changes=[text_document_edit])
 
 
 def workspace_edits(uri: str,
@@ -165,15 +166,15 @@
                     ) -> WorkspaceEdit:
     ''' Build a `WorkspaceEdit` for pygls to send to LSP client. '''
     text_edits = [
         TextEdit(range=Range(start=start, end=end), new_text=new_text)
         for start, end, new_text in start_end_text
     ]
     text_document_edit = {
-        'textDocument': VersionedTextDocumentIdentifier(uri=uri,
+        'textDocument': OptionalVersionedTextDocumentIdentifier(uri=uri,
                                                         version=version),
         'edits': text_edits,
     }
     return WorkspaceEdit(document_changes=[text_document_edit])
 
 
 def extract_range(doc: str, range: Range) -> str:
```

### Comparing `uniteai-0.1.8/uniteai/config.py` & `uniteai-0.1.9/uniteai/config.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.8/uniteai/edit.py` & `uniteai-0.1.9/uniteai/edit.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 Jobs for applying textual edits to the LSP client
 
 '''
 
 from typing import List, Union
 import pygls
 from pygls.server import LanguageServer
+from pygls.workspace import Workspace
 from lsprotocol.types import (
     ApplyWorkspaceEditParams,
     Range,
     Position,
 )
 
 from threading import Thread
 from queue import Queue, Empty
 import time
 from dataclasses import dataclass
 from uniteai.common import find_tag, workspace_edit, workspace_edits, mk_logger
 import logging
 
-log = mk_logger('edit', logging.WARN)
+log = mk_logger('edit', logging.DEBUG)
 
 
 ##################################################
 # Types
 
 
 @dataclass
@@ -172,15 +173,14 @@
                         failed_job = None
                         failed_count = 0
                     if not success:
                         failed_job = job
                         failed_count += 1
             time.sleep(self.job_delay)
 
-
 def _attempt_edit_job(ls: LanguageServer, job: LSPJob):
     if isinstance(job, InsertJob):
         return _attempt_insert_job(ls, job)
     if isinstance(job, BlockJob):
         return _attempt_block_job(ls, job)
     elif isinstance(job, DeleteJob):
         return _attempt_delete_job(ls, job)
@@ -192,15 +192,20 @@
     Try to execute a job that inserts some text. May fail if document versions
     don't match.
 
     '''
     log.debug('APPLYING INSERT')
     try:
         doc = ls.workspace.get_document(job.uri)
+        if not doc:
+            log.error(f'Document not managed by Workspace. Make sure this file type is managed by the client, so it sends `didOpen`. uri={job.uri}')
+            return False
+
         version = doc.version
+        log.debug(f'INSERT: uri={job.uri}, doc={doc}, version={version}')
         position = Position(job.line, job.column)
         edit = workspace_edit(job.uri,
                               version,
                               position,
                               position,
                               job.text)
         params = ApplyWorkspaceEditParams(edit=edit)
@@ -221,14 +226,17 @@
 
     Try to execute a job that deletes some regex. May fail if document versions
     don't match.
 
     '''
     try:
         doc = ls.workspace.get_document(job.uri)
+        if not doc:
+            log.error(f'Document not managed by Workspace. Make sure this file type is managed by the client, so it sends `didOpen`. uri={job.uri}')
+            return False
         version = doc.version
         doc_lines = doc.source.split('\n')
 
         # Collect positions of regexs
         failed_regexs = []
         start_end_texts = []
         for regex in job.regexs:
@@ -272,16 +280,20 @@
     a "block" demarcated by start and end tags. May fail if document versions
     don't match.
 
     '''
     log.debug('APPLYING BLOCK')
     try:
         doc = ls.workspace.get_document(job.uri)
+        if not doc:
+            log.error(f'Document not managed by Workspace. Make sure this file type is managed by the client, so it sends `didOpen`. uri={job.uri}. All docs: {ls.workspace.documents.keys()}')
+            return False
         version = doc.version
         doc_lines = doc.source.split('\n')
+        log.debug(f'BLOCK CONTEXT: uri={job.uri}, version={version}, doc={type(doc)}|{doc}, doc_source[:100]={doc.source[:100]}')
 
         m_start = find_tag(job.start_tag, doc_lines)
         m_end = find_tag(job.end_tag, doc_lines)
         if m_start and m_end:
             log.debug('BLOCK: found tags, applying edit')
             ix, s, e = m_start
             start_position = Position(ix, e)
```

### Comparing `uniteai-0.1.8/uniteai/llm_server.py` & `uniteai-0.1.9/uniteai/llm_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.8/uniteai/local_llm.py` & `uniteai-0.1.9/uniteai/local_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from uniteai.common import extract_range, find_block, mk_logger, get_nested
 from uniteai.server import Server
 
 
 START_TAG = ':START_LOCAL:'
 END_TAG = ':END_LOCAL:'
 NAME = 'local_llm'
-log = mk_logger(NAME, logging.DEBUG)
+log = mk_logger(NAME, logging.WARN)
 
 
 class LocalLLMActor(Actor):
     def __init__(self):
         log.debug('ACTOR INIT')
         self.is_running = False
         self.executor = ThreadPoolExecutor(max_workers=3)
@@ -242,14 +242,16 @@
 
     # CodeActions
     server.add_code_action(code_action_local_llm)
 
     @server.thread()
     @server.command('command.localLlmStream')
     def local_llm_stream(ls: Server, args):
+        if len(args) != 2:
+            log.error(f'command.localLlmStream: Wrong arguments, received: {args}')
         text_document = ls.converter.structure(args[0], TextDocumentIdentifier)
         range = ls.converter.structure(args[1], Range)
         uri = text_document.uri
         doc = ls.workspace.get_document(uri)
         doc_source = doc.source
 
         # Extract the highlighted region
```

### Comparing `uniteai-0.1.8/uniteai/lsp_server.py` & `uniteai-0.1.9/uniteai/lsp_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,18 +26,22 @@
 # different processes to report things as needed, in a way that can be easily
 # turned on and off per object of your attention.
 #
 # NOTE: Thespian has a domineering logging methodology. To customize their
 #       formatter, see: `thespian.system.simpleSystemBase`.
 #
 #       Also, https://github.com/thespianpy/Thespian/issues/73
+#
+# NOTE: VSCode thinks the server is erroring if it logs to stdout from the main
+#       thread, but spawned threads don't seem to have the same effect.
 
 logging.basicConfig(
-    stream=sys.stdout,
-    level=logging.DEBUG,  # Globally allow any level. Other loggers can narrow.
+    filename='log_file.log', # TODO: feature loggers still seem to report on stdout
+    # stream=sys.stdout,
+    level=logging.DEBUG,
 )
 
 # Quiet the libs a little
 logging.getLogger('pygls.feature_manager').setLevel(logging.WARN)
 logging.getLogger('pygls.protocol').setLevel(logging.WARN)
 logging.getLogger('Thespian').setLevel(logging.WARN)
 logging.getLogger('asyncio').setLevel(logging.WARN)
```

### Comparing `uniteai-0.1.8/uniteai/openai.py` & `uniteai-0.1.9/uniteai/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,14 +284,16 @@
         lambda params:
         code_action_chat_gpt(openai_chat_engine, openai_max_length, params))
 
     # Modify Server
     @server.thread()
     @server.command('command.openaiAutocompleteStream')
     def openai_autocomplete_stream(ls: Server, args):
+        if len(args) != 4:
+            log.error(f'command.openaiAutocompleteStream: Wrong arguments, received: {args}')
         text_document = ls.converter.structure(args[0], TextDocumentIdentifier)
         range = ls.converter.structure(args[1], Range)
         uri = text_document.uri
         doc = ls.workspace.get_document(uri)
         doc_source = doc.source
 
         # Determine engine, by checking for sentinel values to allow LSP client
```

### Comparing `uniteai-0.1.8/uniteai/server.py` & `uniteai-0.1.9/uniteai/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,31 @@
 from pygls.server import LanguageServer
 from lsprotocol.types import (
     CodeAction,
     CodeActionKind,
     CodeActionParams,
     Command,
     TextDocumentIdentifier,
+
+    TEXT_DOCUMENT_DID_OPEN,
+    DidOpenTextDocumentParams,
+    Diagnostic,
+    Range,
+    Position,
 )
 from pygls.protocol import default_converter
 from concurrent.futures import ThreadPoolExecutor
 from threading import Event
 from thespian.actors import ActorSystem
 import uniteai.edit as edit
+import logging
+from uniteai.common import mk_logger
 
+NAME = 'server.py'
+log = mk_logger(NAME, logging.DEBUG)
 
 ##################################################
 # Server
 
 class Server(LanguageServer):
     def __init__(self, name, version):
         super().__init__(name, version)
@@ -67,31 +77,41 @@
 def initialize():
     '''
     A Barebones pygls LSP Server.
     '''
     server = Server("uniteai", "0.1.0")
 
     @server.feature('workspace/didChangeConfiguration')
-    def workspace_did_change_configuration(ls: Server, *args):
+    def workspace_did_change_configuration(ls: Server, args):
         ''' There's a warning without this. '''
+        log.debug(f'workspace/didChangeConfiguration: args={args}')
         return []
 
+    @server.feature(TEXT_DOCUMENT_DID_OPEN)
+    async def did_open(ls: Server, params: DidOpenTextDocumentParams):
+        """Text document did open notification. It appears this does not
+        overwrite the default `didOpen` handler in pygls, so we can add extra
+        `didOpen` logic here."""
+        log.debug(f'Document did open: uri={params.text_document.uri}')
+
     @server.feature("textDocument/codeAction")
     def code_action(params: CodeActionParams) -> List[CodeAction]:
         ''' Code Actions are eg a list of options you can trigger in your
         client. Included modules can add to `server.code_actions` via
         `server.add_code_action`.  '''
         return [action(params) for action in server.code_actions]
 
     @server.thread()
     @server.command('command.stop')
     def stop(ls: Server, args):
         '''
         Tell ALL actors to stop.
         '''
+        if len(args) != 1:
+            log.error(f'command.stop: Wrong arguments, received: {args}')
         text_document = ls.converter.structure(args[0], TextDocumentIdentifier)
         uri = text_document.uri
         doc = ls.workspace.get_document(uri)
         doc_source = doc.source
 
         # Send a message to stop the stream
         actor_args = {
@@ -106,15 +126,17 @@
     # Add `command.stop` as a "Code Action" too (accessible from the dropdown
     # menu, eg `M-'`.
     server.add_code_action(code_action_stop)
     return server
 
 
 def code_action_stop(params: CodeActionParams):
+    text_document = params.text_document
     return CodeAction(
                 title='Stop Streaming Things',
                 kind=CodeActionKind.Refactor,
                 command=Command(
                     title='Stop Streaming Things',
-                    command='command.stop'
+                    command='command.stop',
+                    arguments=[text_document]
                 )
             )
```

### Comparing `uniteai-0.1.8/uniteai/transcription.py` & `uniteai-0.1.9/uniteai/transcription.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''
 
-Transcribe Speech.
+Speech-to-text
+
 
 '''
 
 from thespian.actors import Actor
 from typing import List
 import pygls
 from pygls.server import LanguageServer
@@ -48,15 +49,15 @@
 
 START_TAG = ':START_TRANSCRIPTION:'
 END_TAG = ':END_TRANSCRIPTION:'
 NAME = 'transcription'
 
 # A custom logger for just this feature. You can tune the log level to turn
 # on/off just this feature's logs.
-log = mk_logger(NAME, logging.WARN)
+log = mk_logger(NAME, logging.DEBUG)
 
 
 ##################################################
 # SpeechRecognition
 
 class SpeechRecognition:
     def __init__(self,
@@ -105,49 +106,38 @@
 
     def _warmup(self):
         ''' Warm up, intended for a separate thread. '''
         empty_audio = sr.AudioData(np.zeros(10), sample_rate=1, sample_width=1)
         self.recognize(empty_audio)
         logging.info('Warmed up transcription model')
 
+        # TODO: Transcription needs to be tuned better to deal with ambient
+        # noise, and appropriate volume levels
+        #
         logging.info('Adjusting thresholds for ambient noise')
         with sr.Microphone() as source:
             self.r.adjust_for_ambient_noise(source)
 
 
     def warmup(self):
         '''Load whisper model into memory.'''
         logging.info('Warming up whisper in separate thread')
         warmup_thread = Thread(target=self._warmup)
         warmup_thread.daemon = True
         warmup_thread.start()
 
-    def listen_worker(self, should_stop, listen_worker_is_running):
-        log.debug('STARTING L WORKER')
-        listen_worker_is_running.set()
-        with sr.Microphone() as source:
-            try:
-                while not should_stop.is_set():
-                    log.debug(f'LISTEN AUDIO. should_stop={should_stop.is_set()}')
-                    try:
-                        audio = self.r.listen(source, timeout=0.5)
-                        self.audio_queue.put(audio, block=False)
-                    except sr.WaitTimeoutError:
-                        pass
-            except KeyboardInterrupt:
-                pass
-
-        # Drain audio queue
-        try:
-            while True:
-                self.audio_queue.get(False)
-        except Empty:
-            pass
-        listen_worker_is_running.clear()
-        log.debug('DONE LISTENING')
+    def listen(self, should_stop):
+        def callback(r, audio):
+            log.debug('LISTENING CALLBACK called')
+            self.audio_queue.put(audio, block=False)
+        stop_listening_fn = self.r.listen_in_background(
+            sr.Microphone(),
+            callback
+        )
+        return stop_listening_fn
 
     def transcription_worker(self, uri, edits, should_stop,
                              transcription_worker_is_running):
         transcription_worker_is_running.set()
         running_transcription = ""
         while not should_stop.is_set():
             try:
@@ -160,21 +150,14 @@
 
             try:
                 x = self.recognize(audio)
                 if not x:
                     continue
 
                 x = x.strip()
-                # x = self.r.recognize_whisper(audio,
-                #                              model=self.model_size,
-                #                              load_options=dict(
-                #                                  device='cuda:0',
-                #                                  download_root=self.model_path
-                #                              ), language='english').strip()
-
                 log.debug(f'TRANSCRIPTION: {x}')
                 if filter_out(x):
                     continue
 
                 # Add space to respect next loop of transcription
                 running_transcription += x + ' '
                 job = BlockJob(
@@ -190,47 +173,42 @@
             self.audio_queue.task_done()
 
         cleanup_block(NAME, [START_TAG, END_TAG], uri, edits)
         transcription_worker_is_running.clear()
         log.debug('DONE TRANSCRIBING')
 
 
-
 ##################################################
 # Actor
 
 class TranscriptionActor(Actor):
     def __init__(self):
-        self.listen_worker_is_running = Event()
         self.transcription_worker_is_running = Event()
         self.should_stop = Event()
         self.tags = [START_TAG, END_TAG]
         self.speech_recognition = None  # set during initialization
         self.executor = ThreadPoolExecutor(max_workers=5)
-        self.listen_thread_future = None
         self.transcription_thread_future = None
 
-        # set during set_config
+        # set during set_config/start
         self.model_path = None
         self.model_size = None
         self.volume_threshold = None
+        self.stop_listening_fn = lambda x,y: None
 
     def receiveMessage(self, msg, sender):
         command = msg.get('command')
         edits = msg.get('edits')
-        lw_set = self.listen_worker_is_running.is_set()
         tw_set = self.transcription_worker_is_running.is_set()
         log.debug(f'''
 %%%%%%%%%%
 ACTOR RECV: {msg["command"]}
 ACTOR STATE:
-listen_worker is running={lw_set}.
 transcription_worker is running={tw_set}
 should_stop: {self.should_stop.is_set()}
-listen_thread_future: {self.listen_thread_future}
 transcription_thread_future: {self.transcription_thread_future}
 
 EDITS STATE:
 job_thread alive: {edits.job_thread.is_alive() if edits and edits.job_thread else "NOT STARTED"}
 %%%%%%%%%%
 ''')
 
@@ -268,15 +246,14 @@
             if self.model_type == 'vosk':
                 pass
 
             # Whisper
             if self.model_type == 'whisper':
                 self.model_size = config.transcription_model_size
 
-
         elif command == 'initialize':
             log.debug(f'INIT TYPE: {self.model_type}')
             self.speech_recognition = SpeechRecognition(
                 self.model_type,
 
                 # whisper
                 self.model_path,
@@ -284,58 +261,50 @@
                 self.volume_threshold
             )
 
             # load the model into GPU
             self.speech_recognition.warmup()
 
     def start(self, uri, cursor_pos, edits):
-        lw_set = self.listen_worker_is_running.is_set()
         tw_set = self.transcription_worker_is_running.is_set()
-        if lw_set or tw_set:
+        if tw_set:
             log.info(f'WARN: ON_START_BUT_RUNNING. '
-                     f'listen_worker is running={lw_set}. '
                      f'transcription_worker is running={tw_set}')
             return
         log.debug('ACTOR START')
         self.should_stop.clear()
 
         # Audio Listener
-        self.listen_thread_future = self.executor.submit(
-            self.speech_recognition.listen_worker,
-            self.should_stop, self.listen_worker_is_running)
+        self.stop_listening_fn = self.speech_recognition.listen(self.should_stop)
 
         # Transcriber
         self.transcription_thread_future = self.executor.submit(
             self.speech_recognition.transcription_worker,
             uri, edits, self.should_stop, self.transcription_worker_is_running)
 
         log.debug('START CAN RETURN')
 
     def stop(self):
         log.debug('ACTOR STOP')
-        lw_set = self.listen_worker_is_running.is_set()
         tw_set = self.transcription_worker_is_running.is_set()
-        if not lw_set or not tw_set:
+        if not tw_set:
             log.info('WARN: ON_STOP_BUT_STOPPED'
-                     f'listen_worker is running={lw_set}. '
                      f'transcription_worker is running={tw_set}')
+            return False
 
         self.should_stop.set()
-
-        if self.listen_thread_future:
-            log.debug('Waiting for audio `listen_thread_future` to terminate')
-            self.listen_thread_future.result()  # block, wait to finish
-            self.listen_thread_future = None  # reset
+        self.stop_listening_fn(wait_for_stop=False)
 
         if self.transcription_thread_future:
             log.debug('Waiting for audio `transcription_thread_future` to terminate')
             self.transcription_thread_future.result()  # block, wait to finish
             self.transcription_thread_future = None  # reset
 
         self.should_stop.clear()
+        self.stop_listening_fn = lambda x,y: None
         log.debug('FINALLY STOPPED')
 
 
 ##########
 # Util
 
 def filter_alphanum(x: str) -> str:
@@ -412,14 +381,16 @@
     # CodeActions
     server.add_code_action(code_action_transcribe)
 
     # Modify Server
     @server.thread()
     @server.command('command.transcribe')
     def transcribe_stream(ls: LanguageServer, args):
+        if len(args) != 2:
+            log.error(f'command.transcribe: Wrong arguments, received: {args}')
         # Prepare args
         text_document = ls.converter.structure(args[0], TextDocumentIdentifier)
         uri = text_document.uri
         doc = ls.workspace.get_document(uri)
         cursor_pos = ls.converter.structure(args[1], Position)
         actor_args = {
             'command': 'start',
```

### Comparing `uniteai-0.1.8/uniteai/contrib/example.py` & `uniteai-0.1.9/uniteai/contrib/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 START_TAG = ':START_EXAMPLE:'
 END_TAG = ':END_EXAMPLE:'
 NAME = 'example'
 
 # A custom logger for just this feature. You can tune the log level to turn
 # on/off just this feature's logs.
-log = mk_logger(NAME, logging.DEBUG)
+log = mk_logger(NAME, logging.WARN)
 
 
 class ExampleActor(Actor):
     def __init__(self):
         self.is_running = False
         self.executor = ThreadPoolExecutor(max_workers=3)
         self.current_future = None
@@ -85,17 +85,18 @@
         # Stop
         elif command == 'stop':
             self.stop()
 
         ##########
         # Set Config
         elif command == 'set_config':
-            self.start_digit = msg.get('start_digit')
-            self.end_digit = msg.get('end_digit')
-            self.delay = msg.get('delay')
+            config = msg['config']
+            self.start_digit = config.example_start_digit
+            self.end_digit = config.example_end_digit
+            self.delay = config.example_delay
 
     def start(self, uri, cursor_pos, engine, max_length, edits):
         if self.is_running:
             log.info('WARN: ON_START_BUT_RUNNING')
             return
         log.debug('ACTOR START')
 
@@ -219,26 +220,28 @@
 
     # Actor
     server.add_actor(NAME, ExampleActor)
 
     # Initialize configuration in Actor
     server.tell_actor(NAME, {
         'command': 'set_config',
-        **vars(config)  # argparse.Namespace -> dict
+        'config': config,
     })
 
     # CodeActions
     server.add_code_action(
         lambda params:
         code_action_example(start_digit, end_digit, delay, params))
 
     # Modify Server
     @server.thread()
     @server.command('command.exampleCounter')
     def example_counter(ls: Server, args):
+        if len(args) != 2:
+            log.error(f'command.exampleCounter: Wrong arguments, received: {args}')
         text_document = ls.converter.structure(args[0], TextDocumentIdentifier)
         cursor_pos = ls.converter.structure(args[1], Position)
         uri = text_document.uri
         doc = ls.workspace.get_document(uri)
         doc_source = doc.source
 
         # Send a message to start the stream
```

### Comparing `uniteai-0.1.8/LICENSE` & `uniteai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.8/pyproject.toml` & `uniteai-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uniteai"
-version = "0.1.8"
+version = "0.1.9"
 description = "AI, Inside your Editor."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [{ name = "Josh Freckleton"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
```

### Comparing `uniteai-0.1.8/PKG-INFO` & `uniteai-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniteai
-Version: 0.1.8
+Version: 0.1.9
 Summary: AI, Inside your Editor.
 Project-URL: Homepage, https://github.com/freckletonj/uniteai
 Project-URL: Bug Tracker, https://github.com/freckletonj/uniteai/issues
 Author: Josh Freckleton
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
@@ -42,177 +42,214 @@
 Provides-Extra: transcription
 Requires-Dist: openai-whisper; extra == 'transcription'
 Requires-Dist: pyaudio; extra == 'transcription'
 Requires-Dist: soundfile; extra == 'transcription'
 Requires-Dist: speechrecognition; extra == 'transcription'
 Description-Content-Type: text/markdown
 
-# uniteai
+<p align="center">
+  <img width="256" height="256" src="https://raw.githubusercontent.com/freckletonj/uniteai/master/icon.jpeg" alt='uniteai'>
+</p>
 
-Interact with local/cloud AIs via the editor you already use, directly inside the document you're editing.
+<p align="center">
+<em>UniteAI: Voice-to-text, Local LLM, and GPT, right in your editor.</em>
+</p>
 
-This is driven from a python backend, and therefore highly extensible. A key goal is to make this code simple, robust, and contributor-friendly, and to expand it to solving everything that's worth solving via this type of interface.
+---
+[![Package version](https://badge.fury.io/py/uniteai.svg)](https://pypi.python.org/pypi/uniteai)
 
-Please consider adding to `./contrib`utions, make a PR against the main library, add a [`.todo/042_my_feature.md`](./todo), or make an [Issue](https://github.com/freckletonj/uniteai/issues) with your cool concept.
+**Requirements:** Python 3
 
+**Editor:** VSCode(ium) or Emacs or any editor with LSP capabilities (most).
 
-|                        | **AI** | **You** |
-|:-----------------------|--------|---------|
-| Knows what you want    |        | ✓       |
-| Doesn't hallucinate    |        | ✓       |
-| Knows a ton            | ✓      |         |
-| Thinks super fast      | ✓      |         |
-| Easy to automate tasks | ✓      |         |
-| Supported in `uniteai` | ✓      | ✓       |
 
+## Screencast Demo
+
+[screencast.webm](https://github.com/freckletonj/uniteai/assets/8399149/6cc56405-bf8f-4b1c-89d3-dbe4ff0c794f)
 
 ## The Vision
 
-For those of us who wish, our interface with technology will increasingly be augmented/mediated by AI.
+### AIs, Why?
 
-We'll **create** code/books/emails/content/work-outputs via collaborating with AI.
+As we integrate more technology into our lives, it's becoming clear that our interactions with these systems will be more and more AI-mediated. This project envisions a future where:
 
-We'll **manage** tasks/processes via help from AI.
+1. **Creation:** We co-create code, books, emails, work outputs, and more with AI.
+2. **Management:** AI aids in task and process handling.
+3. **Learning:** We learn and explore new concepts with AI.
+4. **Entertainment:** Our leisure times are enhanced through AI interaction.
 
-We'll **learn and explore** via collaborating with AI.
+This project hopes build **A Good Interface**.
 
-We'll seek **entertainment** value from interacting with an AI.
 
-What does the ideal interface look like?
+### But why this project?
 
-This project seeks to answer that.
 
+* **The Human-AI Team:** feed off each others' strengths
 
-## Screencast Demo
+  |                        | **AI** | **You** |
+  |:-----------------------|--------|---------|
+  | Knows what you want    |        | ✓       |
+  | Doesn't hallucinate    |        | ✓       |
+  | Knows a ton            | ✓      |         |
+  | Thinks super fast      | ✓      |         |
+  | Easy to automate tasks | ✓      |         |
 
-[screencast.webm](https://github.com/freckletonj/uniteai/assets/8399149/77a5293a-6f49-4cc5-9d6e-3f3e11f97925)
+* **One-for-All AI Environment:** get your AI Stack in *one* environment, get synergy among the tools.
 
-## Capabilities
+* **Self-hosted AI Stack:** more control, better security and customization.
 
-|                                                 |   |
-|:------------------------------------------------|---|
-| **Features**                                    |   |
-| local voice-to-text                             | ✓ |
-| local LLM (eg Falcon)                           | ✓ |
-| ChatGPT & GPT API                               | ✓ |
-| Works via standard LSP                          | ✓ |
-| Only enable features you want                   | ✓ |
-|                                                 |   |
-| **Future**                                      |   |
-| Document retrieval & Embedding Indexing         | _ |
-| Prompt engineering / Assistants                 | _ |
-| Write-ahead for tab-completion                  | _ |
-| Contextualized on your files, repo, email, etc. | _ |
-| Contextualized on multiple highlighted regions  | _ |
-|                                                 |   |
-| **Editors**                                     |   |
-| emacs                                           | ✓ |
-| vscode                                          | _ |
-| vim                                             | _ |
-| jetbrains                                       | _ |
-| atom                                            | _ |
-|                                                 |   |
-| **Meta**                                        |   |
-| `contrib` dir for community contributions       | ✓ |
-| well documented                                 | ✓ |
-| robust simple code                              | ✓ |
+* **High speed communication:** Ultimate man-machine flow needs high-speed communication. Symbolic language is best served in a text-editor environment. Natural language integrates seamlessly via voice-to-text.
 
+* **Conclusion:** *Let's get a local AI stack cozy inside a text editor.*
 
-## Setup
 
-Setup code is crazy simple (see: [`doc/example_lsp_mode_config.el`](./doc/example_lsp_mode_config.el)), but I only use emacs (on ubuntu), and would love some help for the other environments.
+## Quickstart, installing Everything on Ubuntu
 
+You can install more granularly than *everything*, but we'll demo *everything* first.
 
-### Emacs
+The only platform-dependent dependency right now is `portaudio`, which I mention in the next section how to install for linux/mac.
 
-#### 1. Setup
+1.) Get: `uniteai_lsp`.
 
+```sh
+sudo apt install portaudio19-dev
+pip install uniteai[all]
+uniteai_lsp
 ```
-git clone git@github.com:freckletonj/uniteai
-cd uniteai/
-pip install -r requirements.txt
-sudo apt install portaudio19-dev  # if you want transcription
+
+It will prompt if it should make a default `.uniteai.yml` config for you. Update your preferences, including your OpenAI API key if you want that, and which local language model or transcription models you want.
+
+
+2.) *Optional:* Then start the longlived LLM server which offers your editor a connection to your local large language model.
+
+```sh
+uniteai_llm
 ```
 
 
-#### 2. Setup emacs's `init.el`
+3.) Install in your editor:
+
+* For **VSCode** get the [`uniteai` extension](https://marketplace.visualstudio.com/publishers/uniteai). Eg in VSCode, `Ctrl-P` then `ext install uniteai.uniteai` .
+
+* For **VSCodium**, VSCode Marketplace files are not compatible, so you'll need to either:
+
+  * Download the prepackaged [`uniteai.vsix`](./clients/vscode/) extension, then:
+    ```sh
+    codium --install-extension clients/vscode/uniteai.vsix
+    ```
+
+  * DIY:
+    ```sh
+    npm install -g @vscode/vsce
+    git clone https://github.com/freckletonj/uniteai
+    cd uniteai/clients/vscode
+    vsce package
+    codium --install-extension uniteai-version.vsix
+    ```
+
+* For **Emacs**, copy the [`lsp-mode` config](./clients/emacs/example_lsp_mode_config.el) to your `init.el`.
+
+* For other editors with LSP support (most do), we just need to copy the [emacs/vscode configuration](./clients), and translate it to your editor. Please submit a PR with new editor configs!
 
-* `lsp-mode`: `lsp-mode` is recommended because it allows multipe LSPs to run in parallel in the same buffer (eg `uniteai` and your python LSP). See [`doc/example_lsp_mode_config.el`](./doc/example_lsp_mode_config.el).
+## Granular installs
 
-* `EGlot`: See [`doc/example_eglot_config.el`](./doc/example_eglot_config.el):
+Still refer to the Quickstart section for the main workflow, such as calling `uniteai_lsp` to get your default config made.
 
+Your config determines what modules/features are loaded.
 
-#### 3. Optional: Run the local LLM server
+The following makes sure to get your dependencies for each feature.
 
+### Transcription dependencies
+
+```sh
+# Debian/Ubuntu
+sudo apt install portaudio19-dev  # needed by PyAudio
+
+# Mac
+brew install portaudio  # needed by PyAudio
+
+pip install uniteai[transcription]
+```
+
+### Local LLM dependencies
+
+```sh
+pip install uniteai[local_llm]
 ```
-uvicorn llm_server:app --port 8000
+
+### OpenAI/ChatGPT dependencies
+
+```sh
+pip install uniteai[openai]
 ```
 
-This reads your `.uniteai.yml` configuration  (example is in the repo) to find a Transformers-compatible model, eg Falcon, and will run it.
+## Keycombos
 
-I imagine if you point at the dir of any Transformers-compatible model, this should work.
+Your client configuration determines this, so if you are using the example client config examples in `./clients`:
 
+| VSCode      | Emacs   | Effect                                               |
+|:------------|:--------|:-----------------------------------------------------|
+| <lightbulb> | M-'     | Show Code Actions Menu                               |
+| Ctrl-Alt-g  | C-c l g | Send region to **GPT**, stream output to text buffer |
+| Ctrl-Alt-c  | C-c l c | Same, but **ChatGPT**                                |
+| Ctrl-Alt-l  | C-c l l | Same, but **Local (eg Falcon) model**                |
+| Ctrl-Alt-v  | C-c l v | Start **voice-to-text**                              |
+| Ctrl-Alt-s  | C-c l s | Whatevers streaming, stop it                         |
 
-#### 4. Give it a go.
 
-**Keycombos**
+*I'm still figuring out what's most ergonomic, so, I'm accepting feedback.*
 
-Your client configuration determines this, so if you are using the example client config examples in `./doc`:
 
-| Keycombo | Effect                                           |
-|:---------|:-------------------------------------------------|
-| M-'      | Show Code Actions Menu                           |
-|          |                                                  |
-| C-c l g  | Send region to GPT, stream output to text buffer |
-| C-c l c  | Same, but ChatGPT                                |
-|          |                                                  |
-| C-c l l  | Same, but local (eg Falcon) model                |
-|          |                                                  |
-| C-c l v  | Start transcribing from microphone               |
-|          |                                                  |
-| C-c l s  | Whatevers streaming, stop it                     |
+## Contributions
 
+### Why?
 
-### vscode
+Because there are **so many cool tools** to yet be added:
 
-Accepting contributions. See [`.doc/`](./doc) for examples in other editors, it's quite simple.
+* Image creation, eg: *"Write a bulleted plan for a Hero's Journey story about X, and make an image for each scene."*
 
+* Contextualize the AI via reading my emails via POP3, and possibly responding, eg: *"what was that thing my accountant told me not to forget?"*
 
-### vim
+* Ask my database natural language questions, eg: *"what were my top 10% customers' top 3 favorite products?"*
 
-Accepting contributions. See [`.doc/`](./doc) for examples in other editors, it's quite simple.
+* Write-ahead for tab-completion, eg: *"Once upon a ____".*
 
+* Chat with a PDF document, eg: *"what do the authors mean by X?"*
 
-### jetbrains
+* Do some searches, scrape the web, and upload it all into my db.
 
-Accepting contributions. See [`.doc/`](./doc) for examples in other editors, it's quite simple.
+* Sky's the limit.
 
 
-### atom
+### How?
 
-Accepting contributions. See [`.doc/`](./doc) for examples in other editors, it's quite simple.
+A Key goal of this project is to be **Contributor-Friendly**.
 
+* Make an [Issue](https://github.com/freckletonj/uniteai/issues) with your cool concept, or bug you found.
 
-## Misc
+* [`.todo/`](./todo) is a directory of community "tickets", eg [`.todo/042_my_cool_feature.md`](./todo). Make a ticket or take a ticket, and make a PR with your changes!
 
-### TODO
+* [`./todo/README.md`](./todo/README.md) gives some overview of the library, and advice on building against this library.
 
-See [`./todo/README.md`](./todo/README.md).
+* a [`./contrib`](./contrib) directory is where you can add your custom feature. See [`./uniteai/contrib/example.py`](./uniteai/contrib/example.py).
 
-At a high level:
+* `.uniteai.yml` configuration chooses which modules to load/not load.
 
-- [ ] support other editors
-- [ ] add cool features
+* The code is *well-documented*, *robust*, and *simple*, to reduce friction.
 
+* Adding a feature is as simple as writing some python code, and making use of `uniteai`'s library to directly handle issues like concurrency and communicating/modifying the text editor.
+
+
+## Misc
 
 ### Notes on Local LLMs
 
 The file [`./llm_server.py`](./llm_server.py) launches a TCP server in which the LLM weights are booted up. The `lsp_server` will make calls to this `llm_server`.
 
-The reason is that the `lsp_server` lifecycle is (generally*) managed by the text editor, and LLM features can be really slow to boot up. Especially if you're developing a feature, you do not want the LLM to keep being read into your GPU each time you restart the `lsp_server`.
+The reason is that the `lsp_server` lifecycle is (generally*) managed by the text editor, and LLM models can be really slow to boot up. Especially if you're developing a feature, you do not want the LLM to keep being read into your GPU each time you restart the `lsp_server`.
 
 `*` you don't have to let the editor manage the `lsp_server`. For instance, `eglot` in emacs allows you to launch it yourself, and then the editor client can just bind to the port.
 
 
 ### Falcon LLM Issue:
 
 If Falcon runs on multiple threads, its cache has an issue. You need a separate `modelling_RW.py` that makes sure it never tries to cache.
@@ -243,12 +280,12 @@
     return cos_cached, sin_cached
 ```
 
 A separate bitsandbytes issue remains unresolved, but is less serious than the above.
 https://github.com/h2oai/h2ogpt/issues/104
 https://github.com/TimDettmers/bitsandbytes/issues/162
 
-# License
+## License
 
 Copyright (c) Josh Freckleton. All rights reserved.
 
 Licensed under the [Apache-2.0](https://apache.org/licenses/LICENSE-2.0) license.
```

