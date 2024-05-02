# Comparing `tmp/ipex_llm-2.1.0b20240430-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240501-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5310290 bytes, number of entries: 188
+Zip file size: 5310317 bytes, number of entries: 188
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,47 +38,47 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-30 15:07 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-30 15:07 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   470528 b- defN 24-Apr-30 15:07 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   853504 b- defN 24-Apr-30 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-Apr-30 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-Apr-30 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-30 15:07 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   530432 b- defN 24-Apr-30 15:07 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   496128 b- defN 24-Apr-30 15:07 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   471040 b- defN 24-Apr-30 15:07 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   556032 b- defN 24-Apr-30 15:07 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   530944 b- defN 24-Apr-30 15:07 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   549888 b- defN 24-Apr-30 15:07 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   525312 b- defN 24-Apr-30 15:07 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   586752 b- defN 24-Apr-30 15:07 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   561664 b- defN 24-Apr-30 15:07 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-30 15:07 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   524288 b- defN 24-Apr-30 15:07 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-30 15:07 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-30 15:07 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-30 15:07 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-30 15:07 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-30 15:07 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-Apr-30 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-30 15:07 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   561152 b- defN 24-Apr-30 15:07 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-01 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-01 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   470528 b- defN 24-May-01 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   853504 b- defN 24-May-01 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-01 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-01 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-01 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   530432 b- defN 24-May-01 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   496128 b- defN 24-May-01 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   471040 b- defN 24-May-01 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   556032 b- defN 24-May-01 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   530944 b- defN 24-May-01 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   549888 b- defN 24-May-01 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   525312 b- defN 24-May-01 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   586752 b- defN 24-May-01 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   561664 b- defN 24-May-01 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-01 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   524288 b- defN 24-May-01 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-01 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-01 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-01 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-01 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-01 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-01 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-01 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   561152 b- defN 24-May-01 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -176,15 +176,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240430.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240430.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5125 b- defN 24-Apr-30 15:07 ipex_llm-2.1.0b20240430.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-30 15:07 ipex_llm-2.1.0b20240430.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-30 15:07 ipex_llm-2.1.0b20240430.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-30 15:07 ipex_llm-2.1.0b20240430.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17824 b- defN 24-Apr-30 15:07 ipex_llm-2.1.0b20240430.dist-info/RECORD
-188 files, 12952053 bytes uncompressed, 5281810 bytes compressed:  59.2%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240501.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240501.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5125 b- defN 24-May-01 15:08 ipex_llm-2.1.0b20240501.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-01 15:08 ipex_llm-2.1.0b20240501.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-01 15:08 ipex_llm-2.1.0b20240501.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-01 15:08 ipex_llm-2.1.0b20240501.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17824 b- defN 24-May-01 15:08 ipex_llm-2.1.0b20240501.dist-info/RECORD
+188 files, 12952053 bytes uncompressed, 5281837 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -537,29 +537,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240501.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240501.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240501.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240501.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240501.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240501.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240430.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240501.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,17 +6375,18 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	add    $0x663108,%eax
-   180005639:	add    %al,(%rax)
-   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
+   180005634:	mov    0x32(%rcx),%ds
+   180005637:	data16 add %al,(%rax)
+   18000563a:	add    %al,(%rax)
+   18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800551e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055800
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000551e8
@@ -111728,15 +111728,15 @@
    18005e7fa:	add    $0x180,%eax
    18005e7ff:	add    %dh,0x76(%rax)
    18005e802:	add    $0x180,%eax
    18005e807:	add    %bh,0x76(%rax)
    18005e80a:	add    $0x180,%eax
    18005e80f:	add    %al,(%rax)
    18005e811:	add    %al,(%rax)
-   18005e813:	add    %al,0x663108(%rip)        # 0x1806c1921
+   18005e813:	add    %cl,0x663259(%rdi)
    18005e819:	add    %al,(%rax)
    18005e81b:	add    %cl,0x50000000(%rip)        # 0x1d005e821
    18005e821:	add    (%rax),%eax
    18005e823:	add    %ah,(%rax)
    18005e825:	repnz add $0x5de2000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:28 2024
+Time/Date		Wed May  1 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,18 +5058,18 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	add    $0x8,%al
-   1800049d6:	xor    %esp,0x0(%rsi)
-   1800049d9:	add    %al,(%rax)
-   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
+   1800049d4:	mov    0x32(%rcx),%ds
+   1800049d7:	data16 add %al,(%rax)
+   1800049da:	add    %al,(%rax)
+   1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c948
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d200
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c948
@@ -123136,15 +123136,17 @@
    1800660bd:	add    %al,(%rax)
    1800660bf:	add    %bh,0x18005f6(%rax)
    1800660c5:	add    %al,(%rax)
    1800660c7:	add    %al,%al
    1800660c9:	testb  $0x0,0x180(%rip)        # 0x180066250
    1800660d0:	add    %al,(%rax)
    1800660d2:	add    %al,(%rax)
-   1800660d4:	add    $0x663108,%eax
+   1800660d4:	(bad)
+   1800660d5:	pop    %rcx
+   1800660d6:	xor    0x0(%rsi),%ah
    1800660d9:	add    %al,(%rax)
    1800660db:	add    %cl,0x50000000(%rip)        # 0x1d00660e1
    1800660e1:	add    (%rax),%eax
    1800660e3:	add    %al,0x53040006(,%rbp,2)
    1800660ea:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b148
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:03:31 2024
+Time/Date		Wed May  1 15:07:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b600
 SizeOfInitializedData	00000000000bf800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b148
@@ -117188,18 +117188,17 @@
    18006472a:	add    $0x180,%eax
    18006472f:	add    %dh,-0x2a(%rax)
    180064732:	add    $0x180,%eax
    180064737:	add    %bh,-0x2a(%rax)
    18006473a:	add    $0x180,%eax
    18006473f:	add    %al,(%rax)
    180064741:	add    %al,(%rax)
-   180064743:	add    %al,0x8(%rbx)
-   180064746:	xor    %esp,0x0(%rsi)
-   180064749:	add    %al,(%rax)
-   18006474b:	add    %cl,0x50000000(%rip)        # 0x1d0064751
+   180064743:	add    %bl,0x6632(%rdx,%rbx,2)
+   18006474a:	add    %al,(%rax)
+   18006474c:	or     $0x50000000,%eax
    180064751:	add    (%rax),%eax
    180064753:	add    %ah,(%rax)
    180064755:	push   %rcx
    180064756:	(bad)
    180064757:	add    %ah,(%rax)
    180064759:	cmp    (%rsi),%eax
 	...
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800553f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:04:29 2024
+Time/Date		Wed May  1 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055a00
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000553f8
@@ -111831,16 +111831,17 @@
    18005e7da:	add    $0x180,%eax
    18005e7df:	add    %dh,0x76(%rax)
    18005e7e2:	add    $0x180,%eax
    18005e7e7:	add    %bh,0x76(%rax)
    18005e7ea:	add    $0x180,%eax
    18005e7ef:	add    %al,(%rax)
    18005e7f1:	add    %al,(%rax)
-   18005e7f3:	add    %bh,0x8(%rbp)
-   18005e7f6:	xor    %esp,0x0(%rsi)
+   18005e7f3:	add    %dl,%cl
+   18005e7f5:	pop    %rcx
+   18005e7f6:	xor    0x0(%rsi),%ah
    18005e7f9:	add    %al,(%rax)
    18005e7fb:	add    %cl,0x50000000(%rip)        # 0x1d005e801
    18005e801:	add    (%rax),%eax
    18005e803:	add    %ah,(%rax)
    18005e805:	repnz add $0x5e02000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062938
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:03:32 2024
+Time/Date		Wed May  1 15:07:09 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062938
@@ -128639,18 +128639,19 @@
    18006bff7:	add    %al,%al
    18006bff9:	push   %rsi
    18006bffa:	(bad)
    18006bffb:	addb   $0x0,(%rcx)
    18006bffe:	add    %al,(%rax)
    18006c000:	add    %al,(%rax)
    18006c002:	add    %al,(%rax)
-   18006c004:	or     %r14b,(%rcx)
-   18006c007:	data16 add %al,(%rax)
-   18006c00a:	add    %al,(%rax)
-   18006c00c:	or     $0x50000000,%eax
+   18006c004:	popf
+   18006c005:	pop    %rdx
+   18006c006:	xor    0x0(%rsi),%ah
+   18006c009:	add    %al,(%rax)
+   18006c00b:	add    %cl,0x50000000(%rip)        # 0x1d006c011
    18006c011:	add    (%rax),%eax
    18006c013:	add    %al,-0x4d7bfffa(%rsp,%rcx,8)
    18006c01a:	(bad)
 	...
    18006c07f:	add    %bh,%al
    18006c081:	iret
    18006c082:	(bad)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005cb58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:04:29 2024
+Time/Date		Wed May  1 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d400
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005cb58
@@ -123256,18 +123256,18 @@
    18006609d:	add    %al,(%rax)
    18006609f:	add    %bh,0x18005f6(%rax)
    1800660a5:	add    %al,(%rax)
    1800660a7:	add    %al,%al
    1800660a9:	testb  $0x0,0x180(%rip)        # 0x180066230
    1800660b0:	add    %al,(%rax)
    1800660b2:	add    %al,(%rax)
-   1800660b4:	jge    0x1800660be
-   1800660b6:	xor    %esp,0x0(%rsi)
-   1800660b9:	add    %al,(%rax)
-   1800660bb:	add    %cl,0x50000000(%rip)        # 0x1d00660c1
+   1800660b4:	rcrb   %cl,0x32(%rcx)
+   1800660b7:	data16 add %al,(%rax)
+   1800660ba:	add    %al,(%rax)
+   1800660bc:	or     $0x50000000,%eax
    1800660c1:	add    (%rax),%eax
    1800660c3:	add    %al,0x55040006(,%rbp,2)
    1800660ca:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
    180066102:	(bad)
    180066103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180061648
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:03:32 2024
+Time/Date		Wed May  1 15:07:09 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000061648
@@ -127298,18 +127298,19 @@
    18006a0d6:	add    %al,(%rax)
    18006a0d8:	shlb   $1,(%rsi)
    18006a0da:	(bad)
    18006a0db:	addb   $0x0,(%rcx)
    18006a0de:	add    %al,(%rax)
    18006a0e0:	add    %al,(%rax)
    18006a0e2:	add    %al,(%rax)
-   18006a0e4:	or     %r14b,(%rcx)
-   18006a0e7:	data16 add %al,(%rax)
-   18006a0ea:	add    %al,(%rax)
-   18006a0ec:	or     $0x50000000,%eax
+   18006a0e4:	popf
+   18006a0e5:	pop    %rdx
+   18006a0e6:	xor    0x0(%rsi),%ah
+   18006a0e9:	add    %al,(%rax)
+   18006a0eb:	add    %cl,0x50000000(%rip)        # 0x1d006a0f1
    18006a0f1:	add    (%rax),%eax
    18006a0f3:	add    %al,(%rax)
    18006a0f5:	lods   %ds:(%rsi),%eax
    18006a0f6:	(bad)
    18006a0f7:	add    %al,(%rax)
    18006a0f9:	lahf
    18006a0fa:	(bad)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b868
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:04:29 2024
+Time/Date		Wed May  1 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b868
@@ -121930,16 +121930,17 @@
    180064181:	(bad)
    180064182:	add    $0x180,%eax
    180064187:	add    %dl,%al
    180064189:	(bad)
    18006418a:	add    $0x180,%eax
    18006418f:	add    %al,(%rax)
    180064191:	add    %al,(%rax)
-   180064193:	add    %bh,0x8(%rbp)
-   180064196:	xor    %esp,0x0(%rsi)
+   180064193:	add    %dl,%dl
+   180064195:	pop    %rcx
+   180064196:	xor    0x0(%rsi),%ah
    180064199:	add    %al,(%rax)
    18006419b:	add    %cl,0x50000000(%rip)        # 0x1d00641a1
    1800641a1:	add    (%rax),%eax
    1800641a3:	add    %al,(%rax)
    1800641a5:	rex.WRX (bad)
    1800641a7:	add    %al,(%rax)
    1800641a9:	rex.X (bad)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180068aa8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:03:32 2024
+Time/Date		Wed May  1 15:07:09 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069000
 SizeOfInitializedData	00000000000c8200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000068aa8
@@ -137914,18 +137914,19 @@
    180071c27:	add    %al,%al
    180071c29:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180071c2a:	(bad)
    180071c2b:	addb   $0x0,(%rcx)
    180071c2e:	add    %al,(%rax)
    180071c30:	add    %al,(%rax)
    180071c32:	add    %al,(%rax)
-   180071c34:	or     %r14b,(%rcx)
-   180071c37:	data16 add %al,(%rax)
-   180071c3a:	add    %al,(%rax)
-   180071c3c:	or     $0x50000000,%eax
+   180071c34:	popf
+   180071c35:	pop    %rdx
+   180071c36:	xor    0x0(%rsi),%ah
+   180071c39:	add    %al,(%rax)
+   180071c3b:	add    %cl,0x50000000(%rip)        # 0x1d0071c41
    180071c41:	add    (%rax),%eax
    180071c43:	add    %dl,%al
    180071c45:	sub    $0x21d00007,%eax
    180071c4a:	(bad)
 	...
    180071c7f:	add    %al,0x31(%rax)
    180071c82:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062d58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:04:29 2024
+Time/Date		Wed May  1 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063400
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062d58
@@ -132533,18 +132533,18 @@
    18006ccf7:	add    %al,%al
    18006ccf9:	push   %rsi
    18006ccfa:	(bad)
    18006ccfb:	addb   $0x0,(%rcx)
    18006ccfe:	add    %al,(%rax)
    18006cd00:	add    %al,(%rax)
    18006cd02:	add    %al,(%rax)
-   18006cd04:	jge    0x18006cd0e
-   18006cd06:	xor    %esp,0x0(%rsi)
-   18006cd09:	add    %al,(%rax)
-   18006cd0b:	add    %cl,0x50000000(%rip)        # 0x1d006cd11
+   18006cd04:	rcrl   $1,0x32(%rcx)
+   18006cd07:	data16 add %al,(%rax)
+   18006cd0a:	add    %al,(%rax)
+   18006cd0c:	or     $0x50000000,%eax
    18006cd11:	add    (%rax),%eax
    18006cd13:	add    %dl,%al
    18006cd15:	fiadds (%rsi)
    18006cd17:	add    %dl,%al
    18006cd19:	movb   $0x0,(%rsi)
 	...
    18006cd80:	rex loop 0x18006cd89
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:28 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,17 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	add    $0x8,%al
-   180004a36:	xor    %esp,0x0(%rsi)
+   180004a34:	(bad)
+   180004a35:	pop    %rcx
+   180004a36:	xor    0x0(%rsi),%ah
    180004a39:	add    %al,(%rax)
    180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b658
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005be00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b658
@@ -121795,15 +121795,15 @@
    1800641a1:	(bad)
    1800641a2:	add    $0x180,%eax
    1800641a7:	add    %dl,%al
    1800641a9:	(bad)
    1800641aa:	add    $0x180,%eax
    1800641af:	add    %al,(%rax)
    1800641b1:	add    %al,(%rax)
-   1800641b3:	add    %al,0x663108(%rip)        # 0x1806c72c1
+   1800641b3:	add    %cl,0x663259(%rdi)
    1800641b9:	add    %al,(%rax)
    1800641bb:	add    %cl,0x50000000(%rip)        # 0x1d00641c1
    1800641c1:	add    (%rax),%eax
    1800641c3:	add    %al,(%rax)
    1800641c5:	rex.WRX (bad)
    1800641c7:	add    %al,(%rax)
    1800641c9:	rex (bad)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,15 +25509,17 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	add    $0x663108,%eax
+   140014ac4:	(bad)
+   140014ac5:	pop    %rcx
+   140014ac6:	xor    0x0(%rsi),%ah
    140014ac9:	add    %al,(%rax)
    140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:04:55 2024
+Time/Date		Wed May  1 15:04:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189047,15 +189047,17 @@
    140093ee5:	add    %al,(%rax)
    140093ee7:	add    %al,(%rax)
    140093ee9:	cltd
    140093eea:	or     %al,0x1(%rax)
    140093eed:	add    %al,(%rax)
    140093eef:	add    %al,(%rax)
    140093ef1:	add    %al,(%rax)
-   140093ef3:	add    %dl,0x663108(%rdi)
+   140093ef3:	add    %ch,%ch
+   140093ef5:	pop    %rcx
+   140093ef6:	xor    0x0(%rsi),%ah
    140093ef9:	add    %al,(%rax)
    140093efb:	add    %cl,-0x34000000(%rip)        # 0x10c093f01
    140093f01:	add    (%rax),%eax
    140093f03:	add    %dl,-0x6ffff68d(%rax)
    140093f09:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,15 +24136,17 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	add    $0x663108,%eax
+   140013ef4:	(bad)
+   140013ef5:	pop    %rcx
+   140013ef6:	xor    0x0(%rsi),%ah
    140013ef9:	add    %al,(%rax)
    140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,15 +24679,17 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	add    $0x663108,%eax
+   140013fc4:	(bad)
+   140013fc5:	pop    %rcx
+   140013fc6:	xor    0x0(%rsi),%ah
    140013fc9:	add    %al,(%rax)
    140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,15 +40341,15 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %al,0x663108(%rip)        # 0x140682231
+   14001f123:	add    %cl,0x663259(%rdi)
    14001f129:	add    %al,(%rax)
    14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32229,15 +32229,15 @@
    1400191e5:	add    %al,(%rax)
    1400191e7:	add    %al,(%rax)
    1400191e9:	push   %rbp
    1400191ea:	add    %eax,0x1(%rax)
    1400191ed:	add    %al,(%rax)
    1400191ef:	add    %al,(%rax)
    1400191f1:	add    %al,(%rax)
-   1400191f3:	add    %al,0x663108(%rip)        # 0x14067c301
+   1400191f3:	add    %cl,0x663259(%rdi)
    1400191f9:	add    %al,(%rax)
    1400191fb:	add    %cl,0x20000000(%rip)        # 0x160019201
    140019201:	add    (%rax),%eax
    140019203:	add    %dh,%al
    140019205:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:04:28 2024
+Time/Date		Wed May  1 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32355,18 +32355,19 @@
    1400191c5:	add    %al,(%rax)
    1400191c7:	add    %al,(%rax)
    1400191c9:	push   %rbp
    1400191ca:	add    %eax,0x1(%rax)
    1400191cd:	add    %al,(%rax)
    1400191cf:	add    %al,(%rax)
    1400191d1:	add    %al,(%rax)
-   1400191d3:	add    %bh,0x31(%rax,%rcx,1)
-   1400191d7:	data16 add %al,(%rax)
-   1400191da:	add    %al,(%rax)
-   1400191dc:	or     $0x20000000,%eax
+   1400191d3:	add    %dl,%cl
+   1400191d5:	pop    %rcx
+   1400191d6:	xor    0x0(%rsi),%ah
+   1400191d9:	add    %al,(%rax)
+   1400191db:	add    %cl,0x20000000(%rip)        # 0x1600191e1
    1400191e1:	add    (%rax),%eax
    1400191e3:	add    %dh,-0x5f(%rax)
    1400191e6:	add    %eax,(%rax)
    1400191e8:	jo     0x14001917b
    1400191ea:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:28 2024
+Time/Date		Wed May  1 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27178,16 +27178,15 @@
    140015fe0:	push   $0x1400123
    140015fe5:	add    %al,(%rax)
    140015fe7:	add    %dh,0x23(%rax)
    140015fea:	add    %eax,0x1(%rax)
    140015fed:	add    %al,(%rax)
    140015fef:	add    %al,(%rax)
    140015ff1:	add    %al,(%rax)
-   140015ff3:	add    %al,(%rax,%rcx,1)
-   140015ff6:	xor    %esp,0x0(%rsi)
+   140015ff3:	add    %cl,0x663259(%rsi)
    140015ff9:	add    %al,(%rax)
    140015ffb:	add    %cl,-0x70000000(%rip)        # 0xd0016001
    140016001:	add    (%rax),%eax
    140016003:	add    %ch,%al
    140016005:	add    %eax,%gs:(%rax)
    140016008:	call   0x140016160
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:04:28 2024
+Time/Date		Wed May  1 15:03:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27305,18 +27305,19 @@
    140015fc0:	push   $0x1400123
    140015fc5:	add    %al,(%rax)
    140015fc7:	add    %dh,0x23(%rax)
    140015fca:	add    %eax,0x1(%rax)
    140015fcd:	add    %al,(%rax)
    140015fcf:	add    %al,(%rax)
    140015fd1:	add    %al,(%rax)
-   140015fd3:	add    %bh,0x31(%rax,%rcx,1)
-   140015fd7:	data16 add %al,(%rax)
-   140015fda:	add    %al,(%rax)
-   140015fdc:	or     $0x90000000,%eax
+   140015fd3:	add    %dl,%al
+   140015fd5:	pop    %rcx
+   140015fd6:	xor    0x0(%rsi),%ah
+   140015fd9:	add    %al,(%rax)
+   140015fdb:	add    %cl,-0x70000000(%rip)        # 0xd0015fe1
    140015fe1:	add    (%rax),%eax
    140015fe3:	add    %ch,0x65(%rax)
    140015fe6:	add    %eax,(%rax)
    140015fe8:	push   $0x155
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:28 2024
+Time/Date		Wed May  1 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28462,16 +28462,15 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %al,(%rax,%rcx,1)
-   1400170e6:	xor    %esp,0x0(%rsi)
+   1400170e3:	add    %cl,0x663259(%rsi)
    1400170e9:	add    %al,(%rax)
    1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rdx,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:04:28 2024
+Time/Date		Wed May  1 15:03:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28607,18 +28607,19 @@
    1400170ad:	add    %al,(%rax)
    1400170af:	add    %cl,0x1400133(%rax)
    1400170b5:	add    %al,(%rax)
    1400170b7:	add    %dl,0x1400133(%rax)
    1400170bd:	add    %al,(%rax)
    1400170bf:	add    %al,(%rax)
    1400170c1:	add    %al,(%rax)
-   1400170c3:	add    %bh,0x31(%rax,%rcx,1)
-   1400170c7:	data16 add %al,(%rax)
-   1400170ca:	add    %al,(%rax)
-   1400170cc:	or     $0x90000000,%eax
+   1400170c3:	add    %dl,%al
+   1400170c5:	pop    %rcx
+   1400170c6:	xor    0x0(%rsi),%ah
+   1400170c9:	add    %al,(%rax)
+   1400170cb:	add    %cl,-0x70000000(%rip)        # 0xd00170d1
    1400170d1:	add    (%rax),%eax
    1400170d3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170d7:	add    %ch,0x1(%rsi,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
    140017103:	rex add %eax,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32576,15 +32576,15 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %al,0x663108(%rip)        # 0x14067c421
+   140019313:	add    %cl,0x663259(%rdi)
    140019319:	add    %al,(%rax)
    14001931b:	add    %cl,0x20000000(%rip)        # 0x160019321
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 30 15:04:29 2024
+Time/Date		Wed May  1 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32701,16 +32701,17 @@
    1400192e5:	add    %al,(%rax)
    1400192e7:	add    %al,(%rax)
    1400192e9:	push   %rbp
    1400192ea:	add    %eax,0x1(%rax)
    1400192ed:	add    %al,(%rax)
    1400192ef:	add    %al,(%rax)
    1400192f1:	add    %al,(%rax)
-   1400192f3:	add    %bh,0x8(%rbp)
-   1400192f6:	xor    %esp,0x0(%rsi)
+   1400192f3:	add    %dl,%cl
+   1400192f5:	pop    %rcx
+   1400192f6:	xor    0x0(%rsi),%ah
    1400192f9:	add    %al,(%rax)
    1400192fb:	add    %cl,0x20000000(%rip)        # 0x160019301
    140019301:	add    (%rax),%eax
    140019303:	add    %bh,%ah
    140019305:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:28 2024
+Time/Date		Wed May  1 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,18 +4028,18 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	add    $0x8,%al
-   180004606:	xor    %esp,0x0(%rsi)
-   180004609:	add    %al,(%rax)
-   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
+   180004604:	mov    0x32(%rcx),%ds
+   180004607:	data16 add %al,(%rax)
+   18000460a:	add    %al,(%rax)
+   18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062b48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 15:02:29 2024
+Time/Date		Wed May  1 15:02:39 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062b48
@@ -132428,15 +132428,17 @@
    18006cd17:	add    %al,%al
    18006cd19:	push   %rsi
    18006cd1a:	(bad)
    18006cd1b:	addb   $0x0,(%rcx)
    18006cd1e:	add    %al,(%rax)
    18006cd20:	add    %al,(%rax)
    18006cd22:	add    %al,(%rax)
-   18006cd24:	add    $0x663108,%eax
+   18006cd24:	(bad)
+   18006cd25:	pop    %rcx
+   18006cd26:	xor    0x0(%rsi),%ah
    18006cd29:	add    %al,(%rax)
    18006cd2b:	add    %cl,0x50000000(%rip)        # 0x1d006cd31
    18006cd31:	add    (%rax),%eax
    18006cd33:	add    %dl,%al
    18006cd35:	fiadds (%rsi)
    18006cd37:	add    %dl,%al
    18006cd39:	(bad)
```

## Comparing `ipex_llm-2.1.0b20240430.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240501.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240430.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240501.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240430.dist-info/METADATA` & `ipex_llm-2.1.0b20240501.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240430
+Version: 2.1.0b20240501
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240430) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240501) ; extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
 Requires-Dist: numpy (==1.26.4) ; extra == 'llama-index'
 Requires-Dist: sentencepiece ; extra == 'llama-index'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'llama-index'
@@ -51,47 +51,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240430) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240430) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240501) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240501) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240430) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240430) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240501) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240501) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240430) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240430) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240501) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240501) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240430.dist-info/RECORD` & `ipex_llm-2.1.0b20240501.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -38,46 +38,46 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=PfuIt-eGZnbAbLhz4DNFf7IaVPw5-6IYJwgKg9zx-Fc,36352
-ipex_llm/libs/bloom.dll,sha256=ffDIMFLQHGdRK70V_kTeh8jgzHiASBnXnjcZ-s-k3yY,470528
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=TwJUvJIh5s6GauXD7qkwX5ir3WlS6esx60TvSUWtyTg,853504
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=6BrtcbRJr5jTMy_N_bGYgwhqiXkf6J74KrSp5LT6fU4,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=Gt0fRb7vaE7uO-xjxbtgakyNeeR3OtBUXA8MTGOjj7Y,844288
-ipex_llm/libs/gptneox-api.dll,sha256=trK7YdOlvubRUluHyyhJpCyLZuN7MdLrMCqAu3XZveU,24576
-ipex_llm/libs/gptneox.dll,sha256=xxF2i4HaLEdENpI5GzcLq9FVfwCmgnqVzilxEzJYauM,530432
-ipex_llm/libs/libbloom_avx.dll,sha256=SrfJSkAZQXLDhQklNitLQH4OM3BZ93kEW2zAQyvzJSc,496128
-ipex_llm/libs/libbloom_vnni.dll,sha256=YsccpxT2Hd4mO4WxU7hXhjJU_3L9k96-D3gu6xmjtB4,471040
-ipex_llm/libs/libgptneox_avx.dll,sha256=6Cxbz0eKAG1iiKI0ESoJ7Y0fiU4BNjxbdRIOqyOgmPM,556032
-ipex_llm/libs/libgptneox_vnni.dll,sha256=_b4dxd1sr4zrYXuMnU2OW5AnCmT6G6YyDCyHOuTSipE,530944
-ipex_llm/libs/libllama_avx.dll,sha256=vaxQ4etXgYBjdAgCz13_x-YeNMJSQ5MSykDIkPADQlQ,549888
-ipex_llm/libs/libllama_vnni.dll,sha256=oaQm5bhK5SUJFxXjx5g8qb89WZ0dEvAwrRSFe_6nDSs,525312
-ipex_llm/libs/libstarcoder_avx.dll,sha256=h0P_FmBAScS4XxswsuK37NpQVPGWb0anBN6qDtEVRNc,586752
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=hXZ7hei1S0_MpADs3xSIeQ72xUsyAZFfM0jIQoQBERE,561664
-ipex_llm/libs/llama-api.dll,sha256=t7iUAjWaPLkCOi4KS8_KEdImvA1UzNOvBtwPK-lI6bI,25088
-ipex_llm/libs/llama.dll,sha256=_yqf9yK__Hgu0RhxkdjquUWC7H19dH5pNNbP_owyh5g,524288
-ipex_llm/libs/main-bloom.exe,sha256=TSKmrN32Hu5K0RliHOI-FWrdqFJmWmFAuR6DTbkvRSI,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=Yy6vR6fGrllNn55j91RiR03t1fOggeIvM1Qs1bRuOKE,726016
-ipex_llm/libs/main-gptneox.exe,sha256=7hYBMWDy2wGw6kLKPH7ZQtSMH0bitHS-lEVhqrNlkYA,98816
-ipex_llm/libs/main-llama.exe,sha256=dMLrtYniW1B5HbRgRdlBOBIaC3-9zRNDdZgZQzb0Qss,99840
-ipex_llm/libs/main-starcoder.exe,sha256=X8v_L4L2ZDNuw1N2aJoZh6W0ZkPkSoJ50B21CZRAXAo,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=EINAHxZJ2oQfLjanWXlMBpY3B0SDIRhwGMYQknuTols,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=fb2jyn-6cIOI9eSCGxPDR87ONNfsywlNDhPieaETxFI,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=qutFk2vtc6QpaECuLAnV8eUFaDxKcZK7YvRE6PQtGAI,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=LntD7yDBXgU9Mmymkn405vl4BvapDkAnYtr6LIEryuA,104448
-ipex_llm/libs/quantize-llama.exe,sha256=923doHfvqVOC7YFqjPzCUt3Qfv5nqI5TbDeuNmdeYBA,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=hA_yu5CdgXoa2tJ78I-M5YDztgsaOAN5E35E8SheRqs,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=eZLrs_8YLslj8lfSy-ZwvPUL7Tc531lQyCxRs5pj3Vs,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=3vQPnTTOQgzsjMBRWNj0XFBhLwhstwCLFK6-YGoiI9w,128512
-ipex_llm/libs/starcoder-api.dll,sha256=pTRAJe9zxoWMmBRrNcmHlTXv5DbOsqhWVo0mRkfMuo8,21504
-ipex_llm/libs/starcoder.dll,sha256=U8iwOJ4uN2881tHbzWSie3r2LesZck2rzKFfptZJBLM,561152
+ipex_llm/libs/bloom-api.dll,sha256=vA2hMI_Qvoq4CDvTtLzXAoDhVeVY511Hnil6dffzM1o,36352
+ipex_llm/libs/bloom.dll,sha256=TyL1LyG0-slunVk3U4gc2YM_PJJ9OWBiYKoAEM9W3Co,470528
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=6HcPk1WQqlozDX5Isfv3M13aVWX28uu6BD54hBj7Hdk,853504
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=z-xDU3suNLDV0VOU6H4qD6RkJRuqG9LcKLRgYYAbDe0,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=nHlJb0wCVLnGdBGxFym89Ppm7R4e4Lkb8YUyuZub9UU,844288
+ipex_llm/libs/gptneox-api.dll,sha256=DyFZSDhtx-5JUpxVfrHqU71qL38COFAN7CoS8w1ANa0,24576
+ipex_llm/libs/gptneox.dll,sha256=95DWp_F3i9Xgj3GBM3fUt_0o_TE1B1wLH5yyqBvaRuo,530432
+ipex_llm/libs/libbloom_avx.dll,sha256=GP7XCzSQt5-ZP-hpzL0WjkiWfog5HlrAu1mHIs6N6_A,496128
+ipex_llm/libs/libbloom_vnni.dll,sha256=6toDPBvTCSmh98kmVcdXz52MLLcUVAd_JhUKiU-jRQg,471040
+ipex_llm/libs/libgptneox_avx.dll,sha256=os4r2zBk2p1uExpGRdWSVtI-JMJfN28rEgtbSOJh4fs,556032
+ipex_llm/libs/libgptneox_vnni.dll,sha256=qyl0-HtLJOqgdLUCvBwgpt-vFrtk-48fTIsQIBzzoWM,530944
+ipex_llm/libs/libllama_avx.dll,sha256=OQoPTZa9MKpIQ9uTuZlVF7LpNjEDpu8SdVcLNmr7u-o,549888
+ipex_llm/libs/libllama_vnni.dll,sha256=CAyioHD1WNbax-XNCsYkyO1KRGB-_-L2WS08VRjm_d8,525312
+ipex_llm/libs/libstarcoder_avx.dll,sha256=ZSreB3zfe0j0N1Uh3KrSKqxQp-RGJFIS2qISb22eK88,586752
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=ccrV5EYEbGXYpcJurDCfvqH2iGvA30lt7C5G_0JsmCw,561664
+ipex_llm/libs/llama-api.dll,sha256=C7Ez46rT3bAK0McnHEBzyKTjpvkILK89-e6euljTPXE,25088
+ipex_llm/libs/llama.dll,sha256=HYGcOUL8_fny7EQhZTyOQta2eH8QZ1_QwZSubToiDRs,524288
+ipex_llm/libs/main-bloom.exe,sha256=oIFbeRp3cHwJfgYm1ynk0Y1-uVbqRQGF9J0daUpmmyY,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=rFu7iO1G5uL05lg8M0gUbCKySxs3E3Mop5xTSBUAMK4,726016
+ipex_llm/libs/main-gptneox.exe,sha256=zyhm_Ff4m9fNZPmrYQQ0ERxGRAIVU8X674qLWSvxizU,98816
+ipex_llm/libs/main-llama.exe,sha256=1iilwZmCihz177mQ-OhQjcXDiODQChv2lueyuioY4VQ,99840
+ipex_llm/libs/main-starcoder.exe,sha256=6EMHUdBezjJd6tMEXIQjtrUcMD-TSCYEFH7LAGLHsdY,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=IfFsXHWRVi_lq0stiQ-Tn7qLcTiGC90zlT2HlTX3YN8,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=BgOou1O2SgcQu_Kiqrco3GhqRcbmtVPSL-TYqbrC94E,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=tb-PwmuXQVVorabDwb4N7-oJzjkMcz3NtXRdzcyMSjE,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=Uz9HjHkfY_Qoe8WJgMceBjKu6iVqYSYdKWEBXSMe34k,104448
+ipex_llm/libs/quantize-llama.exe,sha256=ZoB1c98EpJFennVZW-6suPeEjqEHD2O2ANDMu2MVfV8,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=ffUc-TXnOKQq8B82HoQCmXh1Nu1bFmCS9hIMBo0RrcY,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=YXOzUgJr7MbKdYS1Jk_TpT6oU5uoIK8jPcMML_rFo3s,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=6UUDzQMZYLgb7g5Wob50Bt3kMV-lYJp21ETeGZPCAOs,128512
+ipex_llm/libs/starcoder-api.dll,sha256=kQk-nWss1BwyP4PtttGE915g-rpXxNHOI2IIhz3nmTM,21504
+ipex_llm/libs/starcoder.dll,sha256=7JzGOEbpj_zSWU-Ojo_aUg2GaO0VJ49agjF2_eP3rwM,561152
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
@@ -175,14 +175,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240430.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240430.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240430.dist-info/METADATA,sha256=OjjAe-q2XfxJo5GBQlkUMoce0DBl0oPcwzke4UOYXio,5125
-ipex_llm-2.1.0b20240430.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240430.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240430.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240430.dist-info/RECORD,,
+ipex_llm-2.1.0b20240501.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240501.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240501.dist-info/METADATA,sha256=ENY6k8RO2APV01rHjep32uEkN3nduVhJbLJVZzQ2sbM,5125
+ipex_llm-2.1.0b20240501.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240501.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240501.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240501.dist-info/RECORD,,
```

