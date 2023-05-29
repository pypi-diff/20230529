# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.5.27-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.5.28-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,42 @@
-Zip file size: 3505098 bytes, number of entries: 40
--rw-r--r--  2.0 unx      567 b- defN 23-May-27 13:01 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-May-27 13:01 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-May-27 13:01 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-27 13:01 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 11491080 b- defN 23-May-27 13:01 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-May-27 13:01 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-May-27 13:01 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-May-27 13:01 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-May-27 13:01 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-May-27 13:01 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5727 b- defN 23-May-27 13:01 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     8697 b- defN 23-May-27 13:01 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    20516 b- defN 23-May-27 13:01 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-May-27 13:01 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-May-27 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    59005 b- defN 23-May-27 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    74102 b- defN 23-May-27 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39171 b- defN 23-May-27 13:01 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-27 13:01 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1912 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4163 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     4465 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6474 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2558 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     3710 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
--rw-r--r--  2.0 unx     1533 b- defN 23-May-27 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     4401 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4451 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6460 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2551 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3696 b- defN 23-May-27 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-May-27 13:01 fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-May-27 13:01 fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-27 13:01 fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4470 b- defN 23-May-27 13:01 fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/RECORD
-40 files, 11824104 bytes uncompressed, 3497554 bytes compressed:  70.4%
+Zip file size: 3505097 bytes, number of entries: 40
+-rw-r--r--  2.0 unx      567 b- defN 23-May-28 12:57 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-May-28 12:57 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-May-28 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-28 12:57 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 11491080 b- defN 23-May-28 12:57 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-May-28 12:57 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-May-28 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-May-28 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-May-28 12:57 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-May-28 12:57 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5727 b- defN 23-May-28 12:57 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     8697 b- defN 23-May-28 12:57 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    20516 b- defN 23-May-28 12:57 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-May-28 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-May-28 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    59005 b- defN 23-May-28 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    74102 b- defN 23-May-28 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39171 b- defN 23-May-28 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-28 12:57 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4163 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     4465 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6474 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2558 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     3710 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-May-28 12:51 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6460 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2551 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3696 b- defN 23-May-28 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-May-28 12:57 fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 23-May-28 12:57 fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-28 12:57 fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4470 b- defN 23-May-28 12:57 fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/RECORD
+40 files, 11824104 bytes uncompressed, 3497553 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -102,20 +102,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -15168,15 +15168,15 @@
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 defineMethod
 Default values must be specified for none or all arguments
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2310, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2308, please report a bug to PyTorch. 
 isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1951, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":647, please report a bug to PyTorch. 
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got:
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -165174,15 +165174,15 @@
 	mov    %rbx,%rdx
 	mov    %r15,%rsi
 	mov    %r12,%rdi
 	mov    %rax,0x48(%rsp)
 	call   14c4e0 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r12,%r8
 	lea    0x825005(%rip),%rcx        
-	mov    $0x906,%edx
+	mov    $0x904,%edx
 	lea    0x8248b9(%rip),%rsi        
 	lea    0x823cd6(%rip),%rdi        
 	call   14a6c0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	lea    0x40(%rsp),%rbx
 	mov    0x8(%rbp),%esi
 	mov    %rbx,%rdi
 	call   520880 <void split_embedding_grad_indice_weights_cpu_kernel<c10::Half, c10::Half>(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor)@@Base+0xac0>
@@ -895513,15 +895513,15 @@
 	mov    %r13,%rsi
 	mov    %r14,%rdi
 	lea    0x4fe610(%rip),%rax        
 	mov    %rax,0xa0(%rsp)
 	call   14c4e0 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x4ff92e(%rip),%rcx        
-	mov    $0x906,%edx
+	mov    $0x904,%edx
 	lea    0x4ff1e2(%rip),%rsi        
 	lea    0x4fe5ff(%rip),%rdi        
 	call   14a6c0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    %r13,%rsi
 	call   520610 <void split_embedding_grad_indice_weights_cpu_kernel<c10::Half, c10::Half>(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor)@@Base+0x850>
 	jmp    5220d8 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x6e8>
@@ -896574,15 +896574,15 @@
 	mov    %r12,%rsi
 	mov    %r14,%rdi
 	lea    0x4fd0e1(%rip),%rax        
 	mov    %rax,0x40(%rsp)
 	call   14c4e0 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x4fe402(%rip),%rcx        
-	mov    $0x906,%edx
+	mov    $0x904,%edx
 	lea    0x4fdcb6(%rip),%rsi        
 	lea    0x4fd0d3(%rip),%rdi        
 	call   14a6c0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	xchg   %ax,%ax
 	mov    %r12,%rsi
 	call   520610 <void split_embedding_grad_indice_weights_cpu_kernel<c10::Half, c10::Half>(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor)@@Base+0x850>
 	jmp    523620 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x1c30>
@@ -983670,15 +983670,15 @@
 	mov    %r12,%rdi
 	lea    0x4ab170(%rip),%rax        # a2b0b8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x258>
 	mov    %rbp,%rcx
 	lea    0x28(%rsp),%r8
 	mov    %rax,0x8(%rsp)
 	call   149e60 <c10::detail::_str_wrapper<char const*, unsigned long const&, char const*, unsigned long const&>::call(char const* const&, unsigned long const&, char const* const&, unsigned long const&)@plt>
 	mov    %r12,%rcx
-	mov    $0xdb,%edx
+	mov    $0xdd,%edx
 	lea    0x4a1bbf(%rip),%rsi        
 	lea    0x4a094c(%rip),%rdi        
 	call   14af70 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, std::string const&)@plt>
 	nopl   (%rax)
 	lock addl $0x1,0x8(%rax)
 	jmp    57fef3 <c10::Type::containedType(unsigned long) const@@Base+0x63>
 	mov    %rax,%r12
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -9934,15 +9934,15 @@
   0x00a21cb0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00a21cc0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00a21cd0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00a21ce0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
   0x00a21cf0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00a21d00 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00a21d10 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
-  0x00a21d20 655f696e 6c2e6822 3a323331 302c2070 e_inl.h":2310, p
+  0x00a21d20 655f696e 6c2e6822 3a323330 382c2070 e_inl.h":2308, p
   0x00a21d30 6c656173 65207265 706f7274 20612062 lease report a b
   0x00a21d40 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x00a21d50 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x00a21d60 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00a21d70 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00a21d80 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00a21d90 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.5.27
+Version: 2023.5.28
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fbgemm_gpu/__init__.py,sha256=hyPNE6QvlwUNM4PlyfKee7j7agkOF2SNoT3EQXJ-pe0,567
 fbgemm_gpu/_fbgemm_gpu_docs.py,sha256=ks59ZF1sbng7P2uhG_taag5310ml9N_y4jU0EDsUhXs,14920
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=rc49BZwtZuu8qsO5MENAlHeswgPUn35aM8Cgr3XtBE0,2747
 fbgemm_gpu/enums.py,sha256=Tg1pBJrcfSIWmWec2WCZkRuMwmCnepKrcACi3ZijZmk,818
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=Bb-jYIB0MGtxb09fn96L4IkyYNgGpGlj82odhi7NkV4,11491080
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=bRzxgwtCvRt702_Q_EzpH5qKo4Uatkd8BPdJiUNcYa4,11491080
 fbgemm_gpu/metrics.py,sha256=e5VnTatZjFqcgOfipH7Eqk5lsAkuxY2qsbil3Csy_yk,5648
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=n80gTkNwSA9k0dvJeZhVjzXC08c74o0G-u4MnKs7rek,2339
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=9MWBghoy5eajS4yleFWAMdi0LWV0nNbcIgCkqdkRP5g,2477
 fbgemm_gpu/quantize_comm.py,sha256=qONCevOTVA89K7vFJe-Bcc903lHsKDg6s661pTHCF2k,7682
 fbgemm_gpu/quantize_utils.py,sha256=pnZCkIeYxPnvwkIVsRdfPeGBLVXSpEdSsFLH2Ygk7D0,4005
 fbgemm_gpu/split_embedding_configs.py,sha256=o5RUPVwuuQx75T4QsvXKjMKAMQ915EXso8Wpyjgrhvg,5727
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=HH3xj7fgSvo6nytqaqiRqF0pnS8u0z6nBFvcROhwcgw,8697
@@ -30,11 +30,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=fBw0hDYHVaob9Pc2IC_XnpQ0jRStbG9R-IZqBnMywRM,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=z_INEdVlMxPi-rrq4W7oma6YnJF6EqHFIJeD1VdJNh0,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=YO8izH_FCVjxnhlf-Rx3uwTYrKJeERYEGki-QwnWmag,4451
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=5NeEd5Vx-cEpJMLTXFbJqlUtbKptFtx6lFpTSrd6xKA,6460
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=U8LroH3QA8U16dylYQ4UGTjEihOaZFbrZYqnqPfsuss,2551
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=qOeMzSHbEm74uOWD4W5r5UPZ1NpBqZefvYZS41_9kbE,4407
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=IjeKrN7_9l5SZppuc2WbOR8sv6JtRew5geHKKRIRexY,3696
-fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/METADATA,sha256=lKrd3uyqoM7xl7yol1V37KnXXPjcOy4yKD_eO8ACXug,2934
-fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
-fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.5.27.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/METADATA,sha256=EerBw9H3b7aTMeez2gkmJ4Pzs0udJb1XWqxfjY9xEQk,2934
+fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
+fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.5.28.dist-info/RECORD,,
```

