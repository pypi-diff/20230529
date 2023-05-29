# Comparing `tmp/chiakilisp-1.4.0rc7-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27319 bytes, number of entries: 19
+Zip file size: 27670 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
--rw-r--r--  2.0 unx    14553 b- defN 23-May-28 20:46 chiakilisp/lexer.py
+-rw-r--r--  2.0 unx    15250 b- defN 23-May-29 18:13 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
 -rw-r--r--  2.0 unx     3311 b- defN 23-May-27 10:34 chiakilisp/utils.py
--rw-r--r--  2.0 unx     7391 b- defN 23-May-28 13:22 chiakilisp/corelib/core.cl
+-rw-r--r--  2.0 unx     7503 b- defN 23-May-29 18:33 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
--rw-r--r--  2.0 unx    31150 b- defN 23-May-27 22:02 chiakilisp/models/expression.py
+-rw-r--r--  2.0 unx    31965 b- defN 23-May-29 18:31 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
 -rw-r--r--  2.0 unx     4001 b- defN 23-May-28 20:48 chiakilisp/models/literal.py
 -rw-r--r--  2.0 unx     2123 b- defN 23-May-27 22:28 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    13359 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/RECORD
-19 files, 98499 bytes uncompressed, 24771 bytes compressed:  74.9%
+-rwxr-xr-x  2.0 unx    13359 b- defN 23-May-29 18:41 chiakilisp-1.4.0rc8.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-29 18:41 chiakilisp-1.4.0rc8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 18:41 chiakilisp-1.4.0rc8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-29 18:41 chiakilisp-1.4.0rc8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-29 18:41 chiakilisp-1.4.0rc8.dist-info/RECORD
+19 files, 100123 bytes uncompressed, 25122 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc7.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc8.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc7.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc8.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc7.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc8.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc7.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc8.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc7.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chiakilisp/lexer.py

```diff
@@ -15,16 +15,16 @@
     """
     Lexer is the class that takes the source code, then produces a list of tokens
     """
 
     _source_code: str  # <----------------------------------- source code context
     _source_code_file_name: str  # <----------------------- source code file name
     _pointer: int = 0  # <------------------------------ default pointer position
-    _tokens: List[Token]  # <----------------------- list of the populated Tokens
-    _line_num, _char_num = 1, 0  # <------------ initial pointer position in file
+    _tokens: List[Token]  # <------------------------------ populated Tokens list
+    _line_num, _char_num, _start_num = 1, 1, 1  # <---- initial pointer positions
 
     def _raise_syntax_error(self, message: str) -> None:
 
         """A shortcut for future that helps to throw a SyntaxError"""
 
         raise SyntaxError(f'{":".join(map(str, self.pos()))}: {message}')
 
@@ -48,75 +48,87 @@
 
         self._char_num += 1
 
     def _increment_line_number_with_char_number_reset(self) -> None:
 
         """Increments line number by 1 and resets character number"""
 
-        self._char_num = 0
+        self._char_num = 1
         self._line_num += 1
 
+    def _start(self) -> None:
+
+        """Assign self._start_num to current self._char_num value"""
+
+        self._start_num = self._char_num
+
     def pos(self) -> tuple:
 
         """Returns a tuple containing current char and line number"""
 
-        return tuple((self._source_code_file_name, self._line_num, self._char_num))
+        return tuple((self._source_code_file_name, self._line_num, self._start_num))
 
     def lex(self) -> None:  # pylint: disable=R0912, disable=R0915  # maybe refactor
 
         """Process the given source code, thus produces a list of Token instances"""
 
         while self._can_be_advanced():
 
             if self._current_char_is_semicolon() or \
                     (self._current_char_is_hash() and
                         self._next_char_is_exclamation_mark()):
+                self._start()
                 self._advance()
                 while self._can_be_advanced():
                     if self._current_char_is_nl():
                         break
                     self._advance()
                 self._advance()
                 self._increment_line_number_with_char_number_reset()
 
             elif (self._current_char_is_hash()
                   and self._next_char_is_opening_paren()):
+                self._start()
                 self._advance()
                 self._increment_char_number()
                 self._tokens.append(Token(Token.InlineFunMarker,  '#{', self.pos()))
 
             elif (self._current_char_is_hash()
                   and self._next_char_is_underscore()):
+                self._start()
                 self._advance()
                 self._advance()
                 self._increment_char_number()
                 self._increment_char_number()
                 self._tokens.append(Token(Token.CommentedMarker,  '#_', self.pos()))
 
             elif (self._current_char_is_hash()
                   and self._next_char_is_cr_opening_paren()):
+                self._start()
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'setty', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif (self._current_char_is_hash()
                   and self._next_char_is_sq_opening_paren()):
+                self._start()
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
                 self._tokens.append(Token(Token.OpeningParen,     '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,   'tuply', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_number() \
                     or (self._current_char_is_sign()
                         and self._next_char_is_number()):
+                self._start()
                 value = self._current_char()
                 self._advance()
                 self._increment_char_number()
                 while self._can_be_advanced():
                     if self._current_char_is_number() \
                             or self._current_char_is_dot():
                         value += self._current_char()
@@ -129,14 +141,15 @@
                 elif re.match(r'^(-)?\d+(\.\d+)?$', value):
                     self._tokens.append(Token(Token.Number, value, self.pos()))
                 else:
                     self._raise_syntax_error(f'Invalid float syntax: {value}.')
 
             elif self._current_char_is_letter() \
                     or self._current_char_is_colon():
+                self._start()
                 value = self._current_char()
                 self._advance()
                 self._increment_char_number()
                 while self._can_be_advanced():
                     if self._current_char_is_letter() or \
                             self._current_char_is_number():
                         value += self._current_char()
@@ -158,14 +171,15 @@
                     self._tokens.append(Token(Token.Boolean, value, self.pos()))
                 elif re.match(r'^\.{2}\d+$', value):  # make it equivalent for 0..2
                     self._tokens.append(Token(Token.Slice, value, self.pos()))
                 else:
                     self._tokens.append(Token(Token.Identifier, value, self.pos()))
 
             elif self._current_char_is_double_quote():
+                self._start()
                 value = ''
                 while self._can_be_advanced():
                     self._advance()
                     self._increment_char_number()
                     if self._current_char() == '\\':
                         self._advance()
                         self._increment_char_number()
@@ -181,50 +195,58 @@
                     else:
                         self._tokens.append(Token(Token.String, value,  self.pos()))
                         break
                 self._advance()  # <--- call _advance() to skip the leading '"' char
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_opening_paren():
+                self._start()
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_closing_paren():
+                self._start()
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_cr_opening_paren():
+                self._start()
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'dicty', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_cr_closing_paren():
+                self._start()
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_sq_opening_paren():
+                self._start()
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'listy', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_sq_closing_paren():
+                self._start()
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_char_is_nl():
+                self._start()
                 self._advance()
                 self._increment_line_number_with_char_number_reset()  # go a newline
 
             else:
+                self._start()
                 self._advance()  # call _advance() to skip over the extra characters
                 self._increment_char_number()  # <-- increment character num as well
 
     def _advance(self) -> None:
 
         """Advances char pointer"""
 
@@ -251,15 +273,16 @@
 
         return self._pointer < len(self._source_code)
 
     def _current_char_is_nl(self) -> bool:
 
         """Returns whether current character is a newline character"""
 
-        return self._current_char() == '\n'
+        return self._current_char() == '\n' \
+            or self._current_char() == '\r\n'  # support for MSWindows
 
     def _current_char_is_sign(self) -> bool:
 
         """Returns whether current character is a number sign: +, -"""
 
         return self._current_char() in ['+', '-']
```

## chiakilisp/corelib/core.cl

```diff
@@ -125,14 +125,17 @@
 (defn get-in (& args)        ;; Goes through full path to get an item
  (when args
   (let ((coll path default) args)
         (cond (>= (count args) 2)
               (functools/reduce (fn (acc n)
                                   (get acc n default)) path coll)))))
 
+(defn str*                   ;; Behaves the same as str in Clojure
+ (& parts) (.join "" (map #(str %) parts)))
+
 (defn cons                   ;; Behaves the same as cons in Clojure
  (first-item others)
  (when (list? others)
   (let (new-list [first-item]) (.extend new-list others) new-list)))
 
 (defn assoc                  ;; Behaves the same as assoc in Clojure
  (collection key value)
```

## chiakilisp/models/expression.py

```diff
@@ -30,20 +30,28 @@
 
 class ArityError(SyntaxError):
 
     """Stub class to display that there is an arity error"""
 
 
 NE_ASSERT = get_assertion_closure(NameError)  # <--------- raises NameError
-TE_ASSERT = get_assertion_closure(TypeError)  # <--------- raises TypeError
 SE_ASSERT = get_assertion_closure(SyntaxError)  # <----- raises SyntaxError
 RE_ASSERT = get_assertion_closure(RuntimeError)  # <--- raises RuntimeError
 
+# MANAGED_ERRORS are required to properly raise exceptions, while executing
+# an expressions
+# However, we can't guarantee that in case of broken Python 3.x module user
+# tries to import those exceptions are raised properly.
+# 'NameError' may occur if module tries to reference non-existent variable;
+# 'SyntaxError' may occur if module contains some sort of the syntax error;
+# 'RuntimeError' may occur if module tries to call to (i.e.) virtual method
+
 MANAGED_ERRORS = (
-    Py3xError, ArityError, NameError, TypeError, SyntaxError, RuntimeError)
+    Py3xError, ArityError,
+    NameError, SyntaxError, RuntimeError)  # tuple may be updated in future
 
 
 def IDENTIFIER_ASSERT(lit: Literal, message: str) -> None:
 
     """Handy shortcut to make assertion that Literal is Identifier"""
 
     SE_ASSERT(lit.token().position(), lit.token().is_identifier(), message)
@@ -162,25 +170,25 @@
 
             fn_valid, _, fn_why = integrity_spec_rule.valid(c_arguments)  # first, validate function integrity
             SE_ASSERT(where, fn_valid,                                                    f'{name}: {fn_why}')
 
             if can_take_extras:
                 if len(c_arguments) > positional_parameters_length:
                     e_arguments = c_arguments[positional_parameters_length:]
-                    c_arguments = c_arguments[:positional_parameters_length] + (e_arguments,)  # new args list
+                    c_arguments = c_arguments[:positional_parameters_length] + (e_arguments,)  # complete list
                 else:
                     c_arguments = c_arguments + (tuple(),)  # <- if extras are possible but missing, set to ()
 
             fn = {}  # <----------------------------------------------- initialize new computation environment
             fn.update(environ)  # <--------------------------------------------- update it with the global one
+            fn.update({'kwargs': kwargs})  # <--------------------------- update environment with keyword args
             fn.update(dict(zip(names, c_arguments)))  # <-------------- associate parameters with their values
-            fn.update({'kwargs': kwargs})  # <---------------------- update environment with keyword arguments
-            return [node.execute(fn, False) for node in body][-1]  # then return the last _computation_ result
+            return [node.execute(fn, False) for node in body][-1]  # <- and return the last computation result
 
-        return handle  # <-------- return the closure that will be a good handle for the user defined function
+        return handle  # <---------- return a closure that will be a good handle for the user defined function
 
     def execute(self, environ: dict, top: bool = True) -> Any:
 
         """Execute here - is to return Python 3 value related to the expression: string, number, and vice versa"""
 
         head: Literal
 
@@ -190,15 +198,15 @@
         get = environ.get('get')  # <------- some features like destructing or keyword-as-fn will require core/get
         first = environ.get('first')  # <----- some feature like inline function or others will require core/first
 
         head, *tail = self.nodes()
 
         where = head.token().position()  # <------------ when make assertions on expression head, this can be used
 
-        if head.token().type() == Token.Keyword:
+        if head.token().type() == Token.Keyword:  # if the head of expression is a keyword, evaluate call to `get`
             RE_ASSERT(where, get,   "Expression[execute]: unable to use keyword as a function without `core/get`")
             SE_ASSERT(where, len(tail) >= 1,  'Expression[execute]: keyword must be followed by at least one arg')
             SE_ASSERT(where, len(tail) <= 2,   'Expression[execute]: keyword can be followed by at most two args')
             collection, default = tail if len(tail) == 2 else (tail[0], Nil)  # <--- define collection and default
             return get(
                 collection.execute(environ, False), head.execute(environ, False), default.execute(environ, False))
 
@@ -316,15 +324,20 @@
                       hasattr(handle_instance, '__class__'),
                       'Expression[execute]: dot-form: use object/method, module/method to invoke a static method')
             handle_alias = handle_instance.__class__.__name__  # <------------- get the actual instance class name
             handle_method: Callable = getattr(handle_instance, method_name, NotFound)  # <-- get the method handle
             NE_ASSERT(where,
                       handle_method is not NotFound,
                       f"Expression[execute]: dot-form: the '{handle_alias}' object has no method '{method_name}'")
-            return handle_method(*(node.execute(environ, False) for node in method_args))  # <- return last result
+            try:
+                return handle_method(*(node.execute(environ, False) for node in method_args))  # <- catch an error
+            except Exception as _err_:
+                if not isinstance(_err_, MANAGED_ERRORS):
+                    raise Py3xError(f'{":".join(map(str, where))}: {_err_.__class__.__name__}: {_err_.__str__()}')
+                raise _err_  # re-raise the error if it is managed, raise Py3xError if its arbitrary Python 3x one
 
         if head.token().value() == 'if':
             arity = TAIL_IS_VALID(tail, 'if', where,                             'Expression[execute]: if: {why}')
             cond, true, false = (tail if arity == 3 else tail + [Nil])  # <-- tolerate missing false-branch for if
             return true.execute(environ, False) if cond.execute(environ, False) else false.execute(environ, False)
 
         if head.token().value() == 'when':
```

## Comparing `chiakilisp-1.4.0rc7.data/scripts/chiakilang` & `chiakilisp-1.4.0rc8.data/scripts/chiakilang`

 * *Files identical despite different names*

## Comparing `chiakilisp-1.4.0rc7.dist-info/METADATA` & `chiakilisp-1.4.0rc8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc7
+Version: 1.4.0rc8
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
```

## Comparing `chiakilisp-1.4.0rc7.dist-info/RECORD` & `chiakilisp-1.4.0rc8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 chiakilisp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/lexer.py,sha256=7f7q6iWpjkh8NIogYnRa4Ea2YVJsVZwl7WyjP_cWIQs,14553
+chiakilisp/lexer.py,sha256=9Cs0bCNLQ2dSKEhc7WFE8KlyHMkzuYicdGDI1ewtEmo,15250
 chiakilisp/parser.py,sha256=aPAa3U8D28DO15NzwUliLTOZeCaQEu5giOpzCnPBSs8,5943
 chiakilisp/runtime.py,sha256=J69abrFy4RdcA6oU9z2Pv4ok4A7h5X8lR9VM1l28kk4,1378
 chiakilisp/spec.py,sha256=4_hvO1HYm3RGnky1q85q72we1L3wpjufDgoVU_kcTwk,11225
 chiakilisp/utils.py,sha256=lYwdSJY_y5QEBAM9rEd02Z9ra9ZADJ_yO8JIfsS2WAM,3311
-chiakilisp/corelib/core.cl,sha256=dzLuHsn9URABl8Sj-XHLweHsj-tntjuPl8O2m2Emoy8,7391
+chiakilisp/corelib/core.cl,sha256=l2MMYjUrAAaOIGwrK_1H2Y0dOrVzR1Bjre6JrmgeG0w,7503
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/models/expression.py,sha256=T2R6S3pMAJxmcrjbmxueyDfzAUE8aOzbTutNV-451y4,31150
+chiakilisp/models/expression.py,sha256=jkGqmdnJuP49kP6MJaAynZVp3xF3kY0yoqqWoXULcJ4,31965
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
 chiakilisp/models/literal.py,sha256=Dg5tqdDWzuaW0NvxtZpHP9CQAvTDDjB4eJGMFuxWImc,4001
 chiakilisp/models/token.py,sha256=1ks0qk_t-V-EaLu_LhjEeHx2hrPa_bbyIsqHxdFeAeU,2123
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc7.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
-chiakilisp-1.4.0rc7.dist-info/METADATA,sha256=qhhwNsZeOFcXAZnK5d736xYmTcPskYWjvW1H4nXfZVc,1408
-chiakilisp-1.4.0rc7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc7.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc7.dist-info/RECORD,,
+chiakilisp-1.4.0rc8.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
+chiakilisp-1.4.0rc8.dist-info/METADATA,sha256=qDBtupv0y17gq28-N3Hha9-wnpVrl7NvgosovF8eatE,1408
+chiakilisp-1.4.0rc8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc8.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc8.dist-info/RECORD,,
```

