# Comparing `tmp/langchain_utils-0.3.9.tar.gz` & `tmp/langchain_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.9.tar", max compression
+gzip compressed data, was "langchain_utils-0.4.0.tar", max compression
```

## Comparing `langchain_utils-0.3.9.tar` & `langchain_utils-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     7895 2023-04-12 05:34:44.784594 langchain_utils-0.3.9/README.md
--rw-r--r--   0        0        0       22 2023-04-12 05:41:16.700285 langchain_utils-0.3.9/langchain_utils/__init__.py
--rw-r--r--   0        0        0      222 2023-04-12 05:33:55.491462 langchain_utils-0.3.9/langchain_utils/config.py
--rwxr-xr-x   0        0        0     2632 2023-04-12 05:40:57.099678 langchain_utils-0.3.9/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.9/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2662 2023-04-12 05:41:02.430563 langchain_utils-0.3.9/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     2528 2023-04-12 05:21:34.707838 langchain_utils-0.3.9/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.9/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1922 2023-04-12 05:00:54.153184 langchain_utils-0.3.9/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.9/langchain_utils/prompts.py
--rw-r--r--   0        0        0     7841 2023-04-12 05:25:48.783743 langchain_utils-0.3.9/langchain_utils/utils.py
--rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.9/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1747 2023-04-12 05:41:16.699453 langchain_utils-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     8933 1970-01-01 00:00:00.000000 langchain_utils-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    12824 2023-05-03 03:03:42.597279 langchain_utils-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 09:24:45.089914 langchain_utils-0.4.0/langchain_utils/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.0/langchain_utils/config.py
+-rw-r--r--   0        0        0     4476 2023-05-29 09:15:45.189121 langchain_utils-0.4.0/langchain_utils/document_loaders.py
+-rwxr-xr-x   0        0        0     3130 2023-04-17 03:23:31.837819 langchain_utils-0.4.0/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     4844 2023-05-29 09:18:35.763289 langchain_utils-0.4.0/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3721 2023-04-17 03:23:31.791685 langchain_utils-0.4.0/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     4101 2023-05-03 03:00:37.545180 langchain_utils-0.4.0/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.0/langchain_utils/get_word_prompt.py
+-rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.0/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.0/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.0/langchain_utils/prompts.py
+-rw-r--r--   0        0        0    10484 2023-05-03 02:59:26.472452 langchain_utils-0.4.0/langchain_utils/utils.py
+-rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.0/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     3314 2023-05-29 08:59:46.652209 langchain_utils-0.4.0/langchain_utils/utils_doc_loaders.py
+-rw-r--r--   0        0        0     1891 2023-05-29 09:24:45.087373 langchain_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13900 1970-01-01 00:00:00.000000 langchain_utils-0.4.0/PKG-INFO
```

### Comparing `langchain_utils-0.3.9/langchain_utils/get_html_prompt.py` & `langchain_utils-0.4.0/langchain_utils/get_html_prompt.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,45 @@
 """
 Author : Xinyuan Chen <45612704+tddschn@users.noreply.github.com>
 Date   : 2023-04-09
 """
 
 import sys
 
-from . import __version__
-from .utils import (
+from langchain_utils import __version__
+from langchain_utils.utils import (
     deliver_prompts,
     get_word_count,
     deliver_prompts,
     html_source_info,
     save_stdin_to_tempfile,
+    save_clipboard_to_tempfile,
+    get_default_chunk_size,
 )
-from .loaders import load_html
-from .config import DEFAULT_HTML_WHAT
-from .utils_argparse import get_get_prompt_base_arg_parser
+from langchain_utils.loaders import load_html
+from langchain_utils.config import DEFAULT_HTML_WHAT
+from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(
-        description='Get a prompt from html files'
+    parser = get_get_prompt_base_arg_parser(description='Get a prompt from html files')
+
+    parser.add_argument(
+        'path',
+        help='Paths to the html files, or stdin if not provided',
+        metavar='PATH',
+        type=str,
+        default=None,
+        nargs='*',
     )
 
     parser.add_argument(
-        'path', help='Paths to the html files, or stdin if not provided', metavar='PATH', type=str, default=None, nargs='*'
+        '-C', '--from-clipboard', help='Load text from clipboard', action='store_true'
     )
 
     parser.add_argument(
         '-w',
         '--what',
         help='Initial knowledge you want to insert before the PDF content in the prompt',
         type=str,
@@ -41,16 +50,19 @@
         '-M',
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
 
     args = parser.parse_args()
-    if not args.path:
+    if args.from_clipboard:
+        args.path = [save_clipboard_to_tempfile()]
+    elif not args.path:
         args.path = [save_stdin_to_tempfile()]
+    args.chunk_size = get_default_chunk_size(args.model)
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
@@ -70,29 +82,32 @@
         merged = Document(
             page_content=all_text,
             # metadata=docs[0].metadata,
             # metadata={
             #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
             # },
         )
-    documents = [merged] if args.merge else docs # type: ignore
+    documents = [merged] if args.merge else docs  # type: ignore
     num_docs = len(documents)
-    if args.split or word_count > args.chunk_size * 0.75:
+    if args.no_split:
+        needs_splitting = False
+    elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
         what=args.what,
-        documents=documents, # type: ignore
+        documents=documents,  # type: ignore
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=html_source_info,
         dry_run=args.dry_run,
+        raw_triple_quotes=args.raw,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.9/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.4.0/langchain_utils/get_word_prompt.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,118 +2,113 @@
 """
 Author : Xinyuan Chen <45612704+tddschn@users.noreply.github.com>
 Date   : 2023-04-09
 """
 
 import sys
 
-from . import __version__
-from .utils import (
+from langchain_utils import __version__
+from langchain_utils.utils import (
     deliver_prompts,
     get_word_count,
     deliver_prompts,
-    pymupdf_doc_page_info,
-    convert_str_slice_notation_to_slice,
+    general_document_source_info,
+    get_percentage_non_ascii,
+    get_token_count,
+    get_default_chunk_size,
 )
-from .loaders import load_pdf
-from .config import DEFAULT_PDF_WHAT
-from .utils_argparse import get_get_prompt_base_arg_parser
+from langchain_utils.loaders import load_word, UnstructuredLoadingMode
+from langchain_utils.config import DEFAULT_GENERAL_WHAT
+from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(
-        description='Get a prompt consisting the text content of a PDF file'
-    )
+    parser = get_get_prompt_base_arg_parser(description='Get a prompt from text files')
 
     parser.add_argument(
-        'pdf_path', help='Path to the PDF file', metavar='PDF Path', type=str
+        'word_path',
+        help='Path to the Word document',
+        metavar='Word Document Path',
+        type=str,
     )
     parser.add_argument(
-        '-p',
-        '--pages',
-        help='Only include specified page numbers',
-        type=int,
-        nargs='+',
-        default=None,
+        '-u', '--unstructured-loading-mode', type=str, choices=UnstructuredLoadingMode.__args__, default='single', help='Unstructured loading mode'  # type: ignore
     )
+
     parser.add_argument(
-        '-l',
-        '--page-slice',
-        help='Use Python slice syntax to select page numbers (e.g. 1:3, 1:10:2, etc.)',
+        '-w',
+        '--what',
+        help='Initial knowledge you want to insert before the PDF content in the prompt',
         type=str,
-        default=None,
+        default=DEFAULT_GENERAL_WHAT,
     )
     parser.add_argument(
         '-M',
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
-    parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
-        type=str,
-        default=DEFAULT_PDF_WHAT,
-    )
 
     args = parser.parse_args()
+    args.chunk_size = get_default_chunk_size(args.model)
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
-    print(f'Loading PDF from {args.pdf_path} ...', file=sys.stderr)
-    docs = load_pdf(args.pdf_path)
-    num_whole_pdf_pages = len(docs)
-    if args.pages and args.page_slice:
-        print(
-            'Please specify either --pages or --page-slice, not both',
-            file=sys.stderr,
-        )
-        sys.exit(1)
-    if args.pages:
-        args.pages = [p for p in args.pages if p <= num_whole_pdf_pages and p > 0]
-        docs = [doc for doc in docs if doc.metadata['page_number'] in args.pages]
-    if args.page_slice:
-        args.pages = list(x + 1 for x in list(range(num_whole_pdf_pages))[convert_str_slice_notation_to_slice(args.page_slice)])
-        docs = [doc for doc in docs if doc.metadata['page_number'] in args.pages]
+    print(f'Loading Word document from {args.word_path} ...', file=sys.stderr)
+    docs = load_word(args.word_path)
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
+    char_count = len(all_text)
     print(
-        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
+        f'Loaded {len(docs)} Documents. Word count: {word_count} Char count: {char_count}',
         file=sys.stderr,
     )
+    if args.print_percentage_non_ascii:
+        print(
+            f'Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%',
+            file=sys.stderr,
+        )
+        token_count = get_token_count(all_text)
+        print(f'Token count: {token_count}', file=sys.stderr)
+        print(f'Token / Word: {token_count / word_count:.2f}', file=sys.stderr)
+        print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
+        return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
-            metadata={
-                k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
-            },
+            metadata={k: v for k, v in docs[0].metadata.items() if k in {'source'}},
         )
-    if args.split or word_count > args.chunk_size * 0.75:
+    documents = [merged] if args.merge else docs  # type: ignore
+    num_docs = len(documents)
+    if args.no_split:
+        needs_splitting = False
+    elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
         what=args.what,
-        documents=[merged] if args.merge else docs,  # type: ignore
+        documents=documents,  # type: ignore
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
+        should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
-        extra_chunk_info_fn=pymupdf_doc_page_info,
+        extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
+        raw_triple_quotes=args.raw,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.9/langchain_utils/get_text_prompt.py` & `langchain_utils-0.4.0/langchain_utils/get_text_prompt.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 """
 Author : Xinyuan Chen <45612704+tddschn@users.noreply.github.com>
 Date   : 2023-04-09
 """
 
 import sys
 
-from . import __version__
-from .utils import (
+from langchain_utils import __version__
+from langchain_utils.utils import (
     deliver_prompts,
     get_word_count,
     deliver_prompts,
     general_document_source_info,
     save_stdin_to_tempfile,
+    save_clipboard_to_tempfile,
+    get_token_count,
+    get_percentage_non_ascii,
+    get_default_chunk_size,
 )
-from .loaders import load_text
-from .config import DEFAULT_GENERAL_WHAT
-from .utils_argparse import get_get_prompt_base_arg_parser
+from langchain_utils.loaders import load_text
+from langchain_utils.config import DEFAULT_GENERAL_WHAT
+from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(
-        description='Get a prompt from text files'
+    parser = get_get_prompt_base_arg_parser(description='Get a prompt from text files')
+
+    parser.add_argument(
+        'path',
+        help='Paths to the text files, or stdin if not provided',
+        metavar='PATH',
+        type=str,
+        default=None,
+        nargs='*',
     )
 
     parser.add_argument(
-        'path', help='Paths to the text files, or stdin if not provided', metavar='PATH', type=str, default=None, nargs='*'
+        '-C', '--from-clipboard', help='Load text from clipboard', action='store_true'
     )
 
     parser.add_argument(
         '-w',
         '--what',
         help='Initial knowledge you want to insert before the PDF content in the prompt',
         type=str,
@@ -41,58 +52,75 @@
         '-M',
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
 
     args = parser.parse_args()
-    if not args.path:
+    if args.from_clipboard:
+        args.path = [save_clipboard_to_tempfile()]
+    elif not args.path:
         args.path = [save_stdin_to_tempfile()]
+    args.chunk_size = get_default_chunk_size(args.model)
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
     print(f'Loading text file(s) from {args.path} ...', file=sys.stderr)
     docs = [load_text(p)[0] for p in args.path]
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
+    char_count = len(all_text)
     print(
         f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
     )
+    if args.print_percentage_non_ascii:
+        print(
+            f'Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%',
+            file=sys.stderr,
+        )
+        token_count = get_token_count(all_text)
+        print(f'Token count: {token_count}', file=sys.stderr)
+        print(f'Token / Word: {token_count / word_count:.2f}', file=sys.stderr)
+        print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
+        return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
             # metadata=docs[0].metadata,
             # metadata={
             #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
             # },
         )
-    documents = [merged] if args.merge else docs # type: ignore
+    documents = [merged] if args.merge else docs  # type: ignore
     num_docs = len(documents)
-    if args.split or word_count > args.chunk_size * 0.75:
+    if args.no_split:
+        needs_splitting = False
+    elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
         what=args.what,
-        documents=documents, # type: ignore
+        documents=documents,  # type: ignore
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
+        raw_triple_quotes=args.raw,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.9/langchain_utils/get_url_prompt.py` & `langchain_utils-0.4.0/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 #!/usr/bin/env python3
 """
 Author : Xinyuan Chen <45612704+tddschn@users.noreply.github.com>
 Date   : 2023-04-09
+Purpose: Get a prompt consisting Title and Transcript of a YouTube Video
 """
 
 import sys
 
 from . import __version__
 from .utils import (
     deliver_prompts,
+    format_date,
     get_word_count,
     deliver_prompts,
-    general_document_source_info,
+    get_default_chunk_size,
+    get_percentage_non_ascii,
+    get_token_count,
 )
-from .loaders import load_url
-from .config import DEFAULT_URL_WHAT
+from .loaders import load_youtube_url
 from .utils_argparse import get_get_prompt_base_arg_parser
 
 
 def get_args():
     """Get command-line arguments"""
 
     parser = get_get_prompt_base_arg_parser(
-        description='Get a prompt consisting the text content of a webpage'
+        description='Get a prompt consisting Title and Transcript of a YouTube Video'
     )
 
-    parser.add_argument('url', help='URL to the webpage', metavar='URL', type=str)
-    parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
-        type=str,
-        default=DEFAULT_URL_WHAT,
-    )
-    parser.add_argument(
-        '-M',
-        '--merge',
-        help='Merge contents of all pages before processing',
-        action='store_true',
-    )
-    parser.add_argument(
-        '-j',
-        '--javascript',
-        help='Use JavaScript to render the page',
-        action='store_true',
-    )
+    parser.add_argument('youtube_url', metavar='YouTube URL', help='YouTube URL')
 
     args = parser.parse_args()
+    args.youtube_url = args.youtube_url.split('&')[0]
+    args.chunk_size = get_default_chunk_size(args.model)
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
-
-    print(f'Loading webpage from {args.url} ...', file=sys.stderr)
-    docs = load_url(urls=[args.url], javascript=args.javascript)
-    texts = [doc.page_content for doc in docs]
-    all_text = '\n'.join(texts)
-    word_count = get_word_count((all_text))
+    print(f'Loading transcript from {args.youtube_url} ...', file=sys.stderr)
+    docs = load_youtube_url(args.youtube_url)
     print(
-        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
+        f'Loaded transcript. Word count: {get_word_count((t := docs[0].page_content))} Char count: {len(t)}',
         file=sys.stderr,
     )
-    if args.merge:
-        from langchain.docstore.document import Document
-
-        merged = Document(
-            page_content=all_text,
-            # metadata={
-            #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
-            # },
+    texts = [doc.page_content for doc in docs]
+    all_text = '\n'.join(texts)
+    word_count = get_word_count((all_text))
+    char_count = len(all_text)
+    if args.print_percentage_non_ascii:
+        print(
+            f'Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%',
+            file=sys.stderr,
         )
-    if args.split or word_count > args.chunk_size * 0.75:
+        token_count = get_token_count(all_text)
+        print(f'Token count: {token_count}', file=sys.stderr)
+        print(f'Token / Word: {token_count / word_count:.2f}', file=sys.stderr)
+        print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
+        return
+
+    metadata = docs[0].metadata
+    title = metadata['title']
+    author = metadata['author']
+    publish_date = format_date(metadata['publish_date'])
+    what = f'''the transcript of a YouTube video titled "{title}" uploaded by "{author}" on {publish_date}'''
+    print(f'Title: {title}', file=sys.stderr)
+    print(f'Author: {author}', file=sys.stderr)
+    print(f'Publish date: {publish_date}', file=sys.stderr)
+    if args.no_split:
+        needs_splitting = False
+    elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
-        what=args.what,
-        documents=[merged] if args.merge else docs,  # type: ignore
+        what=what,
+        documents=docs,
+        should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
-        should_be_only_one_doc=True,
         chunk_size=args.chunk_size,
-        extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
+        raw_triple_quotes=args.raw,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.9/langchain_utils/loaders.py` & `langchain_utils-0.4.0/langchain_utils/loaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 #!/usr/bin/env python3
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
+
+from langchain_utils.utils import extract_github_info, get_github_file_raw_url
+from langchain_utils.config import (
+    TESSERACT_OCR_DEFAULT_LANG,
+)
 
 if TYPE_CHECKING:
     from langchain.docstore.document import Document
 
 
 def load_youtube_url(youtube_url: str) -> list['Document']:
     from langchain.document_loaders import YoutubeLoader
 
-    loader = YoutubeLoader.from_youtube_channel(youtube_url, add_video_info=True)
+    loader = YoutubeLoader.from_youtube_url(youtube_url, add_video_info=True)
     docs = loader.load()
     return docs
 
 
-def load_pdf(pdf_path: str) -> list['Document']:
-    from langchain.document_loaders import PyMuPDFLoader
+def load_pdf(
+    pdf_path: str,
+    use_ocr_if_no_text_detected_on_page: bool = False,
+    ocr_language: str = TESSERACT_OCR_DEFAULT_LANG,
+) -> list['Document']:
+    if use_ocr_if_no_text_detected_on_page:
+        from langchain_utils.document_loaders import PyMuPDFLoaderWithFallbackOCR
 
-    loader = PyMuPDFLoader(pdf_path)
-    docs = loader.load()
+        loader_cls = PyMuPDFLoaderWithFallbackOCR
+        load_kwargs = {'ocr_language': ocr_language}
+    else:
+        from langchain.document_loaders import PyMuPDFLoader
+
+        loader_cls = PyMuPDFLoader
+        load_kwargs = {}
+
+    loader = loader_cls(pdf_path)
+    docs = loader.load(**load_kwargs)
     return docs
 
 
 def load_url(urls: list[str], javascript: bool = False) -> list['Document']:
     from langchain.document_loaders import UnstructuredURLLoader, SeleniumURLLoader
 
     if javascript:
@@ -42,20 +60,53 @@
 
     partition_html(url='https://mp.weixin.qq.com/s/FsrDnCFKGD-FzP5YD76tbA')
     loader = loader_class(urls=urls, **kwargs)
     docs = loader.load()
 
     return docs
 
+
 def load_text(path: str, encoding: str | None = None) -> list['Document']:
     from langchain.document_loaders import TextLoader
 
     loader = TextLoader(path, encoding=encoding)
     docs = loader.load()
     return docs
 
-def load_html(path: str, open_encoding: str | None = None, bs_kwargs: dict | None = None) -> list['Document']:
+
+def load_html(
+    path: str, open_encoding: str | None = None, bs_kwargs: dict | None = None
+) -> list['Document']:
     from langchain.document_loaders import BSHTMLLoader
 
     loader = BSHTMLLoader(path, open_encoding=open_encoding, bs_kwargs=bs_kwargs)
     docs = loader.load()
-    return docs
+    return docs
+
+
+UnstructuredLoadingMode = Literal["single", "elements"]
+
+
+def load_word(path: str, mode: UnstructuredLoadingMode = "single") -> list['Document']:
+    # UnstructuredWordDocumentLoader
+    from langchain.document_loaders import UnstructuredWordDocumentLoader
+
+    loader = UnstructuredWordDocumentLoader(path, mode=mode)
+    docs = loader.load()
+    return docs
+
+
+def load_github_raw(
+    github_url: str, github_revision: str = 'master', github_path: str = 'README.md'
+) -> list['Document']:
+    from langchain.requests import TextRequestsWrapper
+    from langchain.docstore.document import Document
+
+    github_info = extract_github_info(github_url)
+    if github_info is None:
+        raise ValueError(f'Invalid GitHub URL: {github_url}')
+    github_info |= {'revision': github_revision, 'file_path': github_path}
+    url = get_github_file_raw_url(**github_info)
+    text = TextRequestsWrapper().get(url)
+
+    docs = [Document(page_content=text, metadata={'url': url})]
+    return docs
```

### Comparing `langchain_utils-0.3.9/langchain_utils/utils.py` & `langchain_utils-0.4.0/langchain_utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 from typing import TYPE_CHECKING, Callable, NoReturn
 import sys
 from .prompts import (
+    RAW_TRIPLE_QUOTES_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED,
 )
 
 
 if TYPE_CHECKING:
@@ -78,14 +79,15 @@
 def html_source_info(document: 'Document') -> str:
     metadata = document.metadata
     if 'source' in metadata:
         return f', Title: {metadata["title"]}, Source: {metadata["source"]}'
     else:
         return ''
 
+
 def general_document_source_info(document: 'Document') -> str:
     metadata = document.metadata
     if 'source' in metadata:
         return f', Source: {metadata["source"]}'
     else:
         return ''
 
@@ -125,21 +127,29 @@
     needs_splitting: bool = False,
     copy: bool = True,
     edit: bool = False,
     chunk_size: int = 2000,
     extra_chunk_info_fn: Callable[['Document'], str] = lambda doc: '',
     dry_run: bool = False,
     parts: list[int] | None = None,
+    raw_triple_quotes: bool = False,
 ):
     from langchain.prompts import PromptTemplate
 
     def deliver_single_doc(document: 'Document'):
-        prompt = PromptTemplate.from_template(REPLY_OK_IF_YOU_READ_TEMPLATE)
+        if raw_triple_quotes:
+            template = RAW_TRIPLE_QUOTES_TEMPLATE
+        else:
+            template = REPLY_OK_IF_YOU_READ_TEMPLATE
+        prompt = PromptTemplate.from_template(template)
         content = document.page_content
-        formatted_prompt = prompt.format(what=what, content=content)
+        if raw_triple_quotes:
+            formatted_prompt = prompt.format(content=content)
+        else:
+            formatted_prompt = prompt.format(what=what, content=content)
 
         def edit_prompt(formatted_prompt: str = formatted_prompt):
             formatted_prompt_path = save_str_to_tempfile(
                 formatted_prompt, suffix='.txt'
             )
             open_file(formatted_prompt_path)
             print(
@@ -161,28 +171,37 @@
 
                 pyperclip.copy(formatted_prompt)
                 print('Prompt copied to clipboard.', file=sys.stderr)
         else:
             print(formatted_prompt)
 
     def deliver_multiple_docs(documents: list['Document']):
+        if len(documents) == 1:
+            deliver_single_doc(documents[0])
+            return
         if edit:
             print(f'Please copy the prompts after each edits.', file=sys.stderr)
         for i, doc in enumerate(documents):
             num_chunks = len(documents)
-            if i == 0:
+            if raw_triple_quotes:
+                template = RAW_TRIPLE_QUOTES_TEMPLATE
+                prompt = PromptTemplate.from_template(template)
+            elif i == 0:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST
                 )
             else:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED
                 ).partial(x=str(i + 1))
             content = doc.page_content
-            formatted_prompt = prompt.format(what=what, content=content)
+            if raw_triple_quotes:
+                formatted_prompt = prompt.format(content=content)
+            else:
+                formatted_prompt = prompt.format(what=what, content=content)
             if dry_run:
                 print(
                     f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}{extra_chunk_info_fn(doc)}: '
                 )
                 continue
             if edit:
                 input(
@@ -236,8 +255,75 @@
     import shutil
     import sys
 
     with tempfile.NamedTemporaryFile(delete=False) as temp_file:
         with open(temp_file.name, 'w') as f:
             shutil.copyfileobj(sys.stdin, f)
         temp_file_path = temp_file.name
-    return temp_file_path
+    return temp_file_path
+
+
+def save_clipboard_to_tempfile() -> str:
+    # create a temp file and save stdin to it, and return the tempfile path
+    import tempfile
+    import pyperclip
+    import sys
+
+    with tempfile.NamedTemporaryFile(delete=False) as temp_file:
+        with open(temp_file.name, 'w') as f:
+            f.write(pyperclip.paste())
+        temp_file_path = temp_file.name
+    return temp_file_path
+
+
+def get_percentage_non_ascii(s: str) -> float:
+    return sum(1 for c in s if ord(c) >= 128) / len(s)
+
+
+def get_default_chunk_size(model: str | None = None) -> int:
+    from langchain_utils.config import MODEL_TO_CONTEXT_LENGTH_MAPPING, DEFAULT_MODEL
+
+    if model not in MODEL_TO_CONTEXT_LENGTH_MAPPING:
+        model = DEFAULT_MODEL
+    return MODEL_TO_CONTEXT_LENGTH_MAPPING[model] // 2
+
+
+def extract_github_info(url: str) -> dict[str, str] | None:
+    import re
+
+    # Define a regular expression to match GitHub URLs
+    pattern = (
+        r"^https?://github\.com/([^/]+)/([^/]+)(?:/(?:tree|blob)/([^/]+)(?:/(.+))?)?$"
+    )
+
+    # Use the regular expression to extract the URL components
+    match = re.match(pattern, url)
+    if match:
+        repo_owner = match.group(1)
+        repo_name = match.group(2)
+        revision = (
+            match.group(3) or "master"
+        )  # Use "main" as the default revision if not provided
+        file_path = (
+            match.group(4) or "README.md"
+        )  # Use "README.md" as the default file path if not provided
+
+        return {
+            "repo_owner": repo_owner,
+            "repo_name": repo_name,
+            "revision": revision,
+            "file_path": file_path,
+        }
+
+    return None
+
+
+def get_github_file_raw_url(
+    repo_owner: str,
+    repo_name: str,
+    revision: str = 'master',
+    file_path: str = 'README.md',
+):
+    # Construct the raw URL for the README.md file
+    raw_url = f"https://raw.githubusercontent.com/{repo_owner}/{repo_name}/{revision}/{file_path}"
+
+    return raw_url
```

### Comparing `langchain_utils-0.3.9/langchain_utils/utils_argparse.py` & `langchain_utils-0.4.0/langchain_utils/utils_argparse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
-from . import __version__
+from langchain_utils import __version__
+from langchain_utils.config import MODEL_TO_CONTEXT_LENGTH_MAPPING, DEFAULT_MODEL
 
 
 def get_get_prompt_base_arg_parser(description: str) -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description=description,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
@@ -22,33 +23,50 @@
     )
     parser.add_argument(
         '-m',
         '--model',
         help='Model to use',
         metavar='model',
         type=str,
-        default='gpt-3.5-turbo',
+        default=DEFAULT_MODEL,
     )
     parser.add_argument(
         '-S',
-        '--split',
-        help='Split the prompt into multiple parts',
+        '--no-split',
+        help='Do not split the prompt into multiple parts (use this if the model has a really large context size)',
         action='store_true',
     )
     parser.add_argument(
         '-s',
         '--chunk-size',
-        help='Chunk size when splitting transcript, also used to determine whether to split',
+        help='Chunk size when splitting transcript, also used to determine whether to split, defaults to 1/2 of the context length limit of the model',
         metavar='chunk_size',
         type=int,
-        default=2000,
+        # default to 1/2 of the context length limit
+        # default=MODEL_TO_CONTEXT_LENGTH_MAPPING[DEFAULT_MODEL] // 2,
+        # default=2000,
+        default=None,
     )
     parser.add_argument(
         '-P',
         '--parts',
         help='Parts to select in the processes list of Documents',
         type=int,
         nargs='+',
         default=None,
     )
+
+    parser.add_argument(
+        '-r',
+        '--raw',
+        help='Wraps the content in triple quotes with no extra text',
+        action='store_true',
+    )
+
+    parser.add_argument(
+        '--print-percentage-non-ascii',
+        help='Print percentage of non-ascii characters',
+        action='store_true',
+    )
+
     parser.add_argument('-n', '--dry-run', help='Dry run', action='store_true')
     return parser
```

### Comparing `langchain_utils-0.3.9/pyproject.toml` & `langchain_utils-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
@@ -14,42 +14,46 @@
 [tool.poetry.scripts]
 get-youtube-transcript-prompt = "langchain_utils.get_youtube_transcript_prompt:main"
 ytprompt = "langchain_utils.get_youtube_transcript_prompt:main"
 get-url-prompt = "langchain_utils.get_url_prompt:main"
 urlprompt = "langchain_utils.get_url_prompt:main"
 get-text-prompt = "langchain_utils.get_text_prompt:main"
 textprompt = "langchain_utils.get_text_prompt:main"
+get-word-prompt = "langchain_utils.get_word_prompt:main"
+wordprompt = "langchain_utils.get_word_prompt:main"
 get-html-prompt = "langchain_utils.get_html_prompt:main"
 htmlprompt = "langchain_utils.get_html_prompt:main"
 get-pdf-prompt = "langchain_utils.get_pdf_prompt:main"
 pdfprompt = "langchain_utils.get_pdf_prompt:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langchain = "^0.0.135"
+langchain = "^0.0.177"
 youtube-transcript-api = "^0.5.0"
 pytube = "^12.1.3"
 pyperclip = "^1.8.2"
 tiktoken = "^0.3.3"
 pymupdf = "^1.21.1"
 # must use this version of unstructured, or it won't be able to parse certain htmls
 unstructured = "0.5.2"
 selenium = "^4.8.3"
 bs4 = "^0.0.1"
+tqdm = "^4.65.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
 rich = "^13.3.3"
 pyinstrument = "^4.4.0"
 icecream = "^2.1.3"
 pytest = "^7.3.0"
+jinja2 = "^3.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langchain_utils-0.3.9/PKG-INFO` & `langchain_utils-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,212 @@
-Metadata-Version: 2.1
-Name: langchain-utils
-Version: 0.3.9
-Summary: 
-Home-page: https://github.com/tddschn/langchain-utils
-License: MIT
-Keywords: langchain,utils,LLM,prompts,CLI
-Author: Teddy Xinyuan Chen
-Author-email: 45612704+tddschn@users.noreply.github.com
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: langchain (>=0.0.135,<0.0.136)
-Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
-Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: pytube (>=12.1.3,<13.0.0)
-Requires-Dist: selenium (>=4.8.3,<5.0.0)
-Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Requires-Dist: unstructured (==0.5.2)
-Requires-Dist: youtube-transcript-api (>=0.5.0,<0.6.0)
-Project-URL: Bug Tracker, https://github.com/tddschn/langchain-utils/issues
-Project-URL: Repository, https://github.com/tddschn/langchain-utils
-Description-Content-Type: text/markdown
-
 # langchain-utils
 
 LangChain Utilities
 
-
 - [langchain-utils](#langchain-utils)
   - [Prompt generation using LangChain document loaders](#prompt-generation-using-langchain-document-loaders)
+    - [Demos](#demos)
     - [`urlprompt`](#urlprompt)
     - [`pdfprompt`](#pdfprompt)
     - [`ytprompt`](#ytprompt)
     - [`textprompt`](#textprompt)
     - [`htmlprompt`](#htmlprompt)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Develop](#develop)
 
-
 ## Prompt generation using LangChain document loaders
 
+Do you find yourself frequently copy-pasting texts from the web / PDFs / other documents into ChatGPT?
+
+If yes, these tools are for you!
+
 Optimized to feed into a chat interface (like ChatGPT) manually in one or multiple (to get around context length limits) goes.
 
+Basically, the prompts generated look like this:
+
+```python
+REPLY_OK_IF_YOU_READ_TEMPLATE = '''
+Below is {what}, reply "OK" if you read:
+
+"""
+{content}
+"""
+'''.strip()
+```
+
+You can feed it directly to a chat interface like ChatGPT, and ask follow up questions about it.
+
+See [`prompts.py`](./langchain_utils/prompts.py) for other variations.
+
+### Demos
+
+- Loading `https://github.com/tddschn/langchain-utils` and copy to clipboard:
+
+<!-- create a video tag with https://user-images.githubusercontent.com/45612704/231729153-341bd962-28cc-40a3-af8b-91e038ccaf6c.mp4 -->
+
+<video src="https://user-images.githubusercontent.com/45612704/231729153-341bd962-28cc-40a3-af8b-91e038ccaf6c.mp4" controls width="100%"></video>
+
+- Load 3 pages of a pdf file, open each part for inspection before copying, and optionally merge 3 pages into 2 prompts that wouldn't go over the `gpt-3.5-turbo`'s context length limit with langchain's `TokenTextSplitter`.
+
+<!-- for https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4 -->
+
+<video src="https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4" controls width="100%"></video>
+
 ### `urlprompt`
 
 ```
 $ urlprompt --help
 
-usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
-                 [-w WHAT] [-M] [-j]
+usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
+                 [-n] [-w WHAT] [-M] [-j] [-g] [--github-path GITHUB_PATH]
+                 [--github-revision GITHUB_REVISION]
                  URL
 
 Get a prompt consisting the text content of a webpage
 
 positional arguments:
   URL                   URL to the webpage
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
-  -S, --split           Split the prompt into multiple parts (default: False)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
   -n, --dry-run         Dry run (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         webpage)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -j, --javascript      Use JavaScript to render the page (default: False)
+  -g, --github          Load the raw file from a GitHub URL (default: False)
+  --github-path GITHUB_PATH
+                        Path to the GitHub file (default: README.md)
+  --github-revision GITHUB_REVISION
+                        Revision for the GitHub file (default: master)
 
 ```
-
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
-usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-P PARTS [PARTS ...]] [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
+usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
+                 [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
-  -S, --split           Split the prompt into multiple parts (default: False)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
   -s chunk_size, --chunk-size chunk_size
-                        Chunk size when splitting transcript, also used to determine whether to split (default: 2000)
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
-                        Parts to select in the processes list of Documents (default: None)
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
   -n, --dry-run         Dry run (default: False)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
   -l PAGE_SLICE, --page-slice PAGE_SLICE
-                        Use Python slice syntax to select page numbers (e.g. 1:3, 1:10:2, etc.) (default: None)
-  -M, --merge           Merge contents of all pages before processing (default: False)
-  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a PDF file)
+                        Use Python slice syntax to select page numbers (e.g.
+                        1:3, 1:10:2, etc.) (default: None)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the content of a PDF
+                        file)
 
 ```
-
 ### `ytprompt`
 
 ```
 $ ytprompt --help
 
-usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
+usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
+                [-n]
                 YouTube URL
 
 Get a prompt consisting Title and Transcript of a YouTube Video
 
 positional arguments:
   YouTube URL           YouTube URL
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
-  -S, --split           Split the prompt into multiple parts (default: False)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
   -n, --dry-run         Dry run (default: False)
 
 ```
-
 ### `textprompt`
 
 ```
 $ textprompt --help
 
 usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
+                  [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from text files
 
 positional arguments:
   PATH                  Paths to the text files, or stdin if not provided
                         (default: None)
@@ -163,37 +214,46 @@
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
-  -S, --split           Split the prompt into multiple parts (default: False)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
   -n, --dry-run         Dry run (default: False)
+  -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         document)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
-```
-
 
+```
 ### `htmlprompt`
 
 ```
 $ htmlprompt --help
 
 usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
+                  [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from html files
 
 positional arguments:
   PATH                  Paths to the html files, or stdin if not provided
                         (default: None)
@@ -201,30 +261,39 @@
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
-  -S, --split           Split the prompt into multiple parts (default: False)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
   -n, --dry-run         Dry run (default: False)
+  -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the text content of a
                         html file)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
 
-
 ```
+
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
 
 ```
@@ -233,15 +302,14 @@
 
 ### [pip](https://pypi.org/project/langchain-utils/)
 
 ```
 $ pip install langchain-utils
 ```
 
-
 ## Develop
 
 ```
 $ git clone https://github.com/tddschn/langchain-utils.git
 $ cd langchain-utils
 $ poetry install
-```
+```
```

