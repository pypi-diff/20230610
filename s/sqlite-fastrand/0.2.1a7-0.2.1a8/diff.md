# Comparing `tmp/sqlite_fastrand-0.2.1a7-py3-none-win_amd64.whl.zip` & `tmp/sqlite_fastrand-0.2.1a8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 619132 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 18:18 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      323 b- defN 23-Jun-07 18:18 sqlite_fastrand/__init__.py
--rw-rw-rw-  2.0 fat  1148928 b- defN 23-Jun-07 18:18 sqlite_fastrand/fastrand0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-07 18:18 sqlite_fastrand/version.py
--rw-rw-rw-  2.0 fat      535 b- defN 23-Jun-07 18:18 sqlite_fastrand-0.2.1a7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-07 18:18 sqlite_fastrand-0.2.1a7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-07 18:18 sqlite_fastrand-0.2.1a7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      669 b- defN 23-Jun-07 18:18 sqlite_fastrand-0.2.1a7.dist-info/RECORD
-8 files, 1150659 bytes uncompressed, 617954 bytes compressed:  46.3%
+Zip file size: 619134 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 20:48 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      323 b- defN 23-Jun-10 20:48 sqlite_fastrand/__init__.py
+-rw-rw-rw-  2.0 fat  1148928 b- defN 23-Jun-10 20:48 sqlite_fastrand/fastrand0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 20:48 sqlite_fastrand/version.py
+-rw-rw-rw-  2.0 fat      535 b- defN 23-Jun-10 20:48 sqlite_fastrand-0.2.1a8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 20:48 sqlite_fastrand-0.2.1a8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-10 20:48 sqlite_fastrand-0.2.1a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      669 b- defN 23-Jun-10 20:48 sqlite_fastrand-0.2.1a8.dist-info/RECORD
+8 files, 1150659 bytes uncompressed, 617956 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_fastrand/fastrand0.dll
 Comment: 
 
 Filename: sqlite_fastrand/version.py
 Comment: 
 
-Filename: sqlite_fastrand-0.2.1a7.dist-info/METADATA
+Filename: sqlite_fastrand-0.2.1a8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_fastrand-0.2.1a7.dist-info/WHEEL
+Filename: sqlite_fastrand-0.2.1a8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_fastrand-0.2.1a7.dist-info/top_level.txt
+Filename: sqlite_fastrand-0.2.1a8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_fastrand-0.2.1a7.dist-info/RECORD
+Filename: sqlite_fastrand-0.2.1a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_fastrand/fastrand0.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800e7114
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jun  7 18:17:38 2023
+Time/Date		Sat Jun 10 20:47:37 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	36
 SizeOfCode		00000000000e7a00
 SizeOfInitializedData	0000000000031600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000e7114
@@ -249,17 +249,17 @@
 	[   0] +base[   1] 67d0 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] sqlite3_fastrand_init
 
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
- 0000000180111000:	0000000180001000 0000000180001137 00000001800fc5d0
- 000000018011100c:	0000000180001140 0000000180001169 00000001800fc5e8
- 0000000180111018:	0000000180001170 00000001800012b6 00000001800fc63c
+ 0000000180111000:	0000000180001000 0000000180001146 00000001800fc5d0
+ 000000018011100c:	0000000180001150 0000000180001179 00000001800fc5e8
+ 0000000180111018:	0000000180001180 00000001800012b7 00000001800fc63c
  0000000180111024:	00000001800012c0 00000001800012e9 00000001800fc654
  0000000180111030:	00000001800012f0 00000001800013df 00000001800fc6a8
  000000018011103c:	00000001800013e0 000000018000140b 00000001800fc6c4
  0000000180111048:	0000000180001410 00000001800014ff 00000001800fc71c
  0000000180111054:	0000000180001500 000000018000152b 00000001800fc738
  0000000180111060:	0000000180001530 000000018000161f 00000001800fc790
  000000018011106c:	0000000180001620 0000000180001648 00000001800fc7a8
@@ -3580,43 +3580,43 @@
  000000018011abd0:	00000001800e8845 00000001800e885c 000000018010a4fc
  000000018011abdc:	00000001800e885c 00000001800e8875 000000018010a4fc
  000000018011abe8:	00000001800e8875 00000001800e8889 000000018010a4fc
  000000018011abf4:	00000001800e8889 00000001800e88bf 00000001800fe880
  000000018011ac00:	00000001800e88bf 00000001800e88d7 000000018010a5c8
 
 Dump of .rdata
- 00000001800fc5d0 (rva: 000fc5d0): 0000000180001000 - 0000000180001137
+ 00000001800fc5d0 (rva: 000fc5d0): 0000000180001000 - 0000000180001146
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x12: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x0a: alloc large area: rsp = rsp - 0x90
+	  pc+0x0a: alloc large area: rsp = rsp - 0xa0
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001800e7cf0.
 	User data:
 	  000: f4 c5 0f 00
- 00000001800fc5e8 (rva: 000fc5e8): 0000000180001140 - 0000000180001169
+ 00000001800fc5e8 (rva: 000fc5e8): 0000000180001150 - 0000000180001179
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: alloc small area: rsp = rsp - 0x20
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 1c c6 0f 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 24 c6 0f 00 88 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 40 11 00 00
-	  030: 00 10 00 00 ff ff ff ff 9c 10 00 00 00 00 00 00
-	  040: a8 10 00 00 ff ff ff ff
- 00000001800fc63c (rva: 000fc63c): 0000000180001170 - 00000001800012b6
+	  010: 00 00 00 00 03 00 00 00 24 c6 0f 00 98 00 00 00
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 50 11 00 00
+	  030: 00 10 00 00 ff ff ff ff ab 10 00 00 00 00 00 00
+	  040: b7 10 00 00 ff ff ff ff
+ 00000001800fc63c (rva: 000fc63c): 0000000180001180 - 00000001800012b7
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x12: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x0a: alloc large area: rsp = rsp - 0xa0
+	  pc+0x0a: alloc large area: rsp = rsp - 0x90
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001800e7cf0.
 	User data:
 	  000: 60 c6 0f 00
  00000001800fc654 (rva: 000fc654): 00000001800012c0 - 00000001800012e9
@@ -3624,18 +3624,18 @@
 	Nbr codes: 4, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: alloc small area: rsp = rsp - 0x20
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 88 c6 0f 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 90 c6 0f 00 98 00 00 00
+	  010: 00 00 00 00 03 00 00 00 90 c6 0f 00 88 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff c0 12 00 00
-	  030: 70 11 00 00 ff ff ff ff 1b 12 00 00 00 00 00 00
-	  040: 27 12 00 00 ff ff ff ff
+	  030: 80 11 00 00 ff ff ff ff 1c 12 00 00 00 00 00 00
+	  040: 28 12 00 00 ff ff ff ff
  00000001800fc6a8 (rva: 000fc6a8): 00000001800012f0 - 00000001800013df
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x15, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x15: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rdi
@@ -27322,16 +27322,16 @@
 	reloc   29 offset  7d8 [e97d8] DIR64
 	reloc   30 offset  838 [e9838] DIR64
 	reloc   31 offset  980 [e9980] DIR64
 	reloc   32 offset  a90 [e9a90] DIR64
 	reloc   33 offset  aa8 [e9aa8] DIR64
 	reloc   34 offset  ab0 [e9ab0] DIR64
 	reloc   35 offset  ab8 [e9ab8] DIR64
-	reloc   36 offset  ad8 [e9ad8] DIR64
-	reloc   37 offset  af0 [e9af0] DIR64
+	reloc   36 offset  ae0 [e9ae0] DIR64
+	reloc   37 offset  af8 [e9af8] DIR64
 	reloc   38 offset  b00 [e9b00] DIR64
 	reloc   39 offset  b18 [e9b18] DIR64
 	reloc   40 offset  b20 [e9b20] DIR64
 	reloc   41 offset  b38 [e9b38] DIR64
 	reloc   42 offset  b70 [e9b70] DIR64
 	reloc   43 offset  c30 [e9c30] DIR64
 	reloc   44 offset  d00 [e9d00] DIR64
@@ -29175,15 +29175,15 @@
 	reloc   32 offset  3d0 [10f3d0] DIR64
 	reloc   33 offset  418 [10f418] DIR64
 
 There is a debug directory in .rdata at 0x1800fbee0
 
 Type                Size     Rva      Offset
   2        CodeView 00000065 000fc1a0 000fafa0
-(format RSDS signature a4e0ec8b9dc14338af0c6960330b4a1f age 1 pdb D:\a\sqlite-fastrand\sqlite-fastrand\target\release\deps\sqlite_fastrand.pdb)
+(format RSDS signature 3cf7f874cd4445d2845fc9947355a98d age 1 pdb D:\a\sqlite-fastrand\sqlite-fastrand\target\release\deps\sqlite_fastrand.pdb)
  12         Feature 00000014 000fc208 000fb008
  13         CoffGrp 00000318 000fc21c 000fb01c
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         000e78d7  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
@@ -29202,206 +29202,206 @@
 
 Disassembly of section .text:
 
 0000000180001000 <.text>:
    180001000:	push   %rbp
    180001001:	push   %rsi
    180001002:	push   %rdi
-   180001003:	sub    $0x90,%rsp
+   180001003:	sub    $0xa0,%rsp
    18000100a:	lea    0x80(%rsp),%rbp
-   180001012:	movq   $0xfffffffffffffffe,0x8(%rbp)
+   180001012:	movq   $0xfffffffffffffffe,0x18(%rbp)
    18000101a:	mov    %rcx,%rsi
    18000101d:	call   0x180022cf0
    180001022:	lea    0xe86af(%rip),%rax        # 0x1800e96d8
    180001029:	mov    %rax,-0x40(%rbp)
    18000102d:	lea    0x5cdc(%rip),%rax        # 0x180006d10
    180001034:	mov    %rax,-0x38(%rbp)
-   180001038:	lea    0xe8679(%rip),%rax        # 0x1800e96b8
-   18000103f:	mov    %rax,-0x20(%rbp)
-   180001043:	movq   $0x1,-0x18(%rbp)
-   18000104b:	movq   $0x0,-0x30(%rbp)
-   180001053:	lea    -0x40(%rbp),%rax
-   180001057:	mov    %rax,-0x10(%rbp)
-   18000105b:	movq   $0x1,-0x8(%rbp)
-   180001063:	lea    -0x58(%rbp),%rdi
-   180001067:	lea    -0x30(%rbp),%rdx
-   18000106b:	mov    %rdi,%rcx
-   18000106e:	call   0x18001a360
-   180001073:	mov    %rsi,%rcx
-   180001076:	mov    %rdi,%rdx
-   180001079:	call   0x180006870
-   18000107e:	test   %rax,%rax
-   180001081:	je     0x18000111d
-   180001087:	lea    -0x30(%rbp),%rcx
-   18000108b:	mov    %rax,%rdx
-   18000108e:	call   0x180007a20
-   180001093:	mov    -0x28(%rbp),%rdx
-   180001097:	mov    -0x20(%rbp),%r8
-   18000109b:	mov    %rsi,%rcx
-   18000109e:	mov    %rdx,0x0(%rbp)
-   1800010a2:	call   0x180008020
-   1800010a7:	mov    %rax,%rdi
-   1800010aa:	test   %rax,%rax
-   1800010ad:	je     0x1800010f3
-   1800010af:	mov    (%rdi),%eax
-   1800010b1:	lea    -0x2(%rax),%rcx
-   1800010b5:	cmp    $0x2,%rcx
-   1800010b9:	jb     0x1800010e0
-   1800010bb:	test   %rax,%rax
-   1800010be:	je     0x1800010e0
-   1800010c0:	cmp    $0x1,%eax
-   1800010c3:	jne    0x180001129
-   1800010c5:	lea    0x10(%rdi),%rax
-   1800010c9:	mov    (%rax),%rdx
-   1800010cc:	test   %rdx,%rdx
-   1800010cf:	je     0x1800010e0
-   1800010d1:	mov    0x8(%rax),%rcx
-   1800010d5:	mov    $0x1,%r8d
-   1800010db:	call   0x180007720
-   1800010e0:	mov    $0x28,%edx
-   1800010e5:	mov    $0x8,%r8d
-   1800010eb:	mov    %rdi,%rcx
-   1800010ee:	call   0x180007720
-   1800010f3:	mov    -0x30(%rbp),%rdx
-   1800010f7:	test   %rdx,%rdx
-   1800010fa:	je     0x18000110b
-   1800010fc:	mov    $0x1,%r8d
-   180001102:	mov    0x0(%rbp),%rcx
-   180001106:	call   0x180007720
-   18000110b:	test   %rdi,%rdi
-   18000110e:	je     0x18000111d
-   180001110:	mov    %rsi,%rcx
-   180001113:	mov    $0x2,%edx
-   180001118:	call   0x180008140
-   18000111d:	nop
-   18000111e:	add    $0x90,%rsp
-   180001125:	pop    %rdi
-   180001126:	pop    %rsi
-   180001127:	pop    %rbp
-   180001128:	ret
-   180001129:	lea    0x8(%rdi),%rax
-   18000112d:	mov    (%rax),%rdx
-   180001130:	test   %rdx,%rdx
-   180001133:	jne    0x1800010d1
-   180001135:	jmp    0x1800010e0
-   180001137:	nopw   0x0(%rax,%rax,1)
-   180001140:	mov    %rdx,0x10(%rsp)
-   180001145:	push   %rbp
-   180001146:	push   %rsi
-   180001147:	push   %rdi
-   180001148:	sub    $0x20,%rsp
-   18000114c:	lea    0x80(%rdx),%rbp
-   180001153:	mov    -0x30(%rbp),%rcx
-   180001157:	mov    0x0(%rbp),%rdx
-   18000115b:	call   0x180003c80
-   180001160:	nop
-   180001161:	add    $0x20,%rsp
-   180001165:	pop    %rdi
-   180001166:	pop    %rsi
-   180001167:	pop    %rbp
-   180001168:	ret
-   180001169:	int3
-   18000116a:	int3
-   18000116b:	int3
-   18000116c:	int3
-   18000116d:	int3
-   18000116e:	int3
-   18000116f:	int3
-   180001170:	push   %rbp
-   180001171:	push   %rsi
-   180001172:	push   %rdi
-   180001173:	sub    $0xa0,%rsp
-   18000117a:	lea    0x80(%rsp),%rbp
-   180001182:	movq   $0xfffffffffffffffe,0x18(%rbp)
-   18000118a:	mov    %rcx,%rsi
-   18000118d:	call   0x180022cf0
-   180001192:	lea    0xe853f(%rip),%rax        # 0x1800e96d8
-   180001199:	mov    %rax,-0x40(%rbp)
-   18000119d:	lea    0x5b6c(%rip),%rax        # 0x180006d10
-   1800011a4:	mov    %rax,-0x38(%rbp)
-   1800011a8:	lea    0xe85a9(%rip),%rcx        # 0x1800e9758
-   1800011af:	mov    %rcx,-0x30(%rbp)
-   1800011b3:	mov    %rax,-0x28(%rbp)
-   1800011b7:	lea    0xe8542(%rip),%rax        # 0x1800e9700
-   1800011be:	mov    %rax,-0x10(%rbp)
-   1800011c2:	movq   $0x3,-0x8(%rbp)
-   1800011ca:	movq   $0x0,-0x20(%rbp)
-   1800011d2:	lea    -0x40(%rbp),%rax
-   1800011d6:	mov    %rax,0x0(%rbp)
-   1800011da:	movq   $0x2,0x8(%rbp)
-   1800011e2:	lea    -0x58(%rbp),%rdi
-   1800011e6:	lea    -0x20(%rbp),%rdx
-   1800011ea:	mov    %rdi,%rcx
-   1800011ed:	call   0x18001a360
-   1800011f2:	mov    %rsi,%rcx
-   1800011f5:	mov    %rdi,%rdx
-   1800011f8:	call   0x180006870
-   1800011fd:	test   %rax,%rax
-   180001200:	je     0x18000129c
-   180001206:	lea    -0x20(%rbp),%rcx
-   18000120a:	mov    %rax,%rdx
-   18000120d:	call   0x180007a20
-   180001212:	mov    -0x18(%rbp),%rdx
-   180001216:	mov    -0x10(%rbp),%r8
-   18000121a:	mov    %rsi,%rcx
-   18000121d:	mov    %rdx,0x10(%rbp)
-   180001221:	call   0x180008020
-   180001226:	mov    %rax,%rdi
-   180001229:	test   %rax,%rax
-   18000122c:	je     0x180001272
-   18000122e:	mov    (%rdi),%eax
-   180001230:	lea    -0x2(%rax),%rcx
-   180001234:	cmp    $0x2,%rcx
-   180001238:	jb     0x18000125f
-   18000123a:	test   %rax,%rax
-   18000123d:	je     0x18000125f
-   18000123f:	cmp    $0x1,%eax
-   180001242:	jne    0x1800012a8
-   180001244:	lea    0x10(%rdi),%rax
-   180001248:	mov    (%rax),%rdx
-   18000124b:	test   %rdx,%rdx
-   18000124e:	je     0x18000125f
-   180001250:	mov    0x8(%rax),%rcx
-   180001254:	mov    $0x1,%r8d
-   18000125a:	call   0x180007720
-   18000125f:	mov    $0x28,%edx
-   180001264:	mov    $0x8,%r8d
-   18000126a:	mov    %rdi,%rcx
-   18000126d:	call   0x180007720
-   180001272:	mov    -0x20(%rbp),%rdx
-   180001276:	test   %rdx,%rdx
-   180001279:	je     0x18000128a
-   18000127b:	mov    $0x1,%r8d
-   180001281:	mov    0x10(%rbp),%rcx
-   180001285:	call   0x180007720
-   18000128a:	test   %rdi,%rdi
-   18000128d:	je     0x18000129c
-   18000128f:	mov    %rsi,%rcx
-   180001292:	mov    $0x2,%edx
-   180001297:	call   0x180008140
-   18000129c:	nop
-   18000129d:	add    $0xa0,%rsp
-   1800012a4:	pop    %rdi
-   1800012a5:	pop    %rsi
-   1800012a6:	pop    %rbp
-   1800012a7:	ret
-   1800012a8:	lea    0x8(%rdi),%rax
-   1800012ac:	mov    (%rax),%rdx
-   1800012af:	test   %rdx,%rdx
-   1800012b2:	jne    0x180001250
-   1800012b4:	jmp    0x18000125f
-   1800012b6:	cs nopw 0x0(%rax,%rax,1)
+   180001038:	lea    0xe8719(%rip),%rcx        # 0x1800e9758
+   18000103f:	mov    %rcx,-0x30(%rbp)
+   180001043:	mov    %rax,-0x28(%rbp)
+   180001047:	lea    0xe86b2(%rip),%rax        # 0x1800e9700
+   18000104e:	mov    %rax,-0x10(%rbp)
+   180001052:	movq   $0x3,-0x8(%rbp)
+   18000105a:	movq   $0x0,-0x20(%rbp)
+   180001062:	lea    -0x40(%rbp),%rax
+   180001066:	mov    %rax,0x0(%rbp)
+   18000106a:	movq   $0x2,0x8(%rbp)
+   180001072:	lea    -0x58(%rbp),%rdi
+   180001076:	lea    -0x20(%rbp),%rdx
+   18000107a:	mov    %rdi,%rcx
+   18000107d:	call   0x18001a360
+   180001082:	mov    %rsi,%rcx
+   180001085:	mov    %rdi,%rdx
+   180001088:	call   0x180006870
+   18000108d:	test   %rax,%rax
+   180001090:	je     0x18000112c
+   180001096:	lea    -0x20(%rbp),%rcx
+   18000109a:	mov    %rax,%rdx
+   18000109d:	call   0x180007a20
+   1800010a2:	mov    -0x18(%rbp),%rdx
+   1800010a6:	mov    -0x10(%rbp),%r8
+   1800010aa:	mov    %rsi,%rcx
+   1800010ad:	mov    %rdx,0x10(%rbp)
+   1800010b1:	call   0x180008020
+   1800010b6:	mov    %rax,%rdi
+   1800010b9:	test   %rax,%rax
+   1800010bc:	je     0x180001102
+   1800010be:	mov    (%rdi),%eax
+   1800010c0:	lea    -0x2(%rax),%rcx
+   1800010c4:	cmp    $0x2,%rcx
+   1800010c8:	jb     0x1800010ef
+   1800010ca:	test   %rax,%rax
+   1800010cd:	je     0x1800010ef
+   1800010cf:	cmp    $0x1,%eax
+   1800010d2:	jne    0x180001138
+   1800010d4:	lea    0x10(%rdi),%rax
+   1800010d8:	mov    (%rax),%rdx
+   1800010db:	test   %rdx,%rdx
+   1800010de:	je     0x1800010ef
+   1800010e0:	mov    0x8(%rax),%rcx
+   1800010e4:	mov    $0x1,%r8d
+   1800010ea:	call   0x180007720
+   1800010ef:	mov    $0x28,%edx
+   1800010f4:	mov    $0x8,%r8d
+   1800010fa:	mov    %rdi,%rcx
+   1800010fd:	call   0x180007720
+   180001102:	mov    -0x20(%rbp),%rdx
+   180001106:	test   %rdx,%rdx
+   180001109:	je     0x18000111a
+   18000110b:	mov    $0x1,%r8d
+   180001111:	mov    0x10(%rbp),%rcx
+   180001115:	call   0x180007720
+   18000111a:	test   %rdi,%rdi
+   18000111d:	je     0x18000112c
+   18000111f:	mov    %rsi,%rcx
+   180001122:	mov    $0x2,%edx
+   180001127:	call   0x180008140
+   18000112c:	nop
+   18000112d:	add    $0xa0,%rsp
+   180001134:	pop    %rdi
+   180001135:	pop    %rsi
+   180001136:	pop    %rbp
+   180001137:	ret
+   180001138:	lea    0x8(%rdi),%rax
+   18000113c:	mov    (%rax),%rdx
+   18000113f:	test   %rdx,%rdx
+   180001142:	jne    0x1800010e0
+   180001144:	jmp    0x1800010ef
+   180001146:	cs nopw 0x0(%rax,%rax,1)
+   180001150:	mov    %rdx,0x10(%rsp)
+   180001155:	push   %rbp
+   180001156:	push   %rsi
+   180001157:	push   %rdi
+   180001158:	sub    $0x20,%rsp
+   18000115c:	lea    0x80(%rdx),%rbp
+   180001163:	mov    -0x20(%rbp),%rcx
+   180001167:	mov    0x10(%rbp),%rdx
+   18000116b:	call   0x180003c80
+   180001170:	nop
+   180001171:	add    $0x20,%rsp
+   180001175:	pop    %rdi
+   180001176:	pop    %rsi
+   180001177:	pop    %rbp
+   180001178:	ret
+   180001179:	int3
+   18000117a:	int3
+   18000117b:	int3
+   18000117c:	int3
+   18000117d:	int3
+   18000117e:	int3
+   18000117f:	int3
+   180001180:	push   %rbp
+   180001181:	push   %rsi
+   180001182:	push   %rdi
+   180001183:	sub    $0x90,%rsp
+   18000118a:	lea    0x80(%rsp),%rbp
+   180001192:	movq   $0xfffffffffffffffe,0x8(%rbp)
+   18000119a:	mov    %rcx,%rsi
+   18000119d:	call   0x180022cf0
+   1800011a2:	lea    0xe852f(%rip),%rax        # 0x1800e96d8
+   1800011a9:	mov    %rax,-0x40(%rbp)
+   1800011ad:	lea    0x5b5c(%rip),%rax        # 0x180006d10
+   1800011b4:	mov    %rax,-0x38(%rbp)
+   1800011b8:	lea    0xe84f9(%rip),%rax        # 0x1800e96b8
+   1800011bf:	mov    %rax,-0x20(%rbp)
+   1800011c3:	movq   $0x1,-0x18(%rbp)
+   1800011cb:	movq   $0x0,-0x30(%rbp)
+   1800011d3:	lea    -0x40(%rbp),%rax
+   1800011d7:	mov    %rax,-0x10(%rbp)
+   1800011db:	movq   $0x1,-0x8(%rbp)
+   1800011e3:	lea    -0x58(%rbp),%rdi
+   1800011e7:	lea    -0x30(%rbp),%rdx
+   1800011eb:	mov    %rdi,%rcx
+   1800011ee:	call   0x18001a360
+   1800011f3:	mov    %rsi,%rcx
+   1800011f6:	mov    %rdi,%rdx
+   1800011f9:	call   0x180006870
+   1800011fe:	test   %rax,%rax
+   180001201:	je     0x18000129d
+   180001207:	lea    -0x30(%rbp),%rcx
+   18000120b:	mov    %rax,%rdx
+   18000120e:	call   0x180007a20
+   180001213:	mov    -0x28(%rbp),%rdx
+   180001217:	mov    -0x20(%rbp),%r8
+   18000121b:	mov    %rsi,%rcx
+   18000121e:	mov    %rdx,0x0(%rbp)
+   180001222:	call   0x180008020
+   180001227:	mov    %rax,%rdi
+   18000122a:	test   %rax,%rax
+   18000122d:	je     0x180001273
+   18000122f:	mov    (%rdi),%eax
+   180001231:	lea    -0x2(%rax),%rcx
+   180001235:	cmp    $0x2,%rcx
+   180001239:	jb     0x180001260
+   18000123b:	test   %rax,%rax
+   18000123e:	je     0x180001260
+   180001240:	cmp    $0x1,%eax
+   180001243:	jne    0x1800012a9
+   180001245:	lea    0x10(%rdi),%rax
+   180001249:	mov    (%rax),%rdx
+   18000124c:	test   %rdx,%rdx
+   18000124f:	je     0x180001260
+   180001251:	mov    0x8(%rax),%rcx
+   180001255:	mov    $0x1,%r8d
+   18000125b:	call   0x180007720
+   180001260:	mov    $0x28,%edx
+   180001265:	mov    $0x8,%r8d
+   18000126b:	mov    %rdi,%rcx
+   18000126e:	call   0x180007720
+   180001273:	mov    -0x30(%rbp),%rdx
+   180001277:	test   %rdx,%rdx
+   18000127a:	je     0x18000128b
+   18000127c:	mov    $0x1,%r8d
+   180001282:	mov    0x0(%rbp),%rcx
+   180001286:	call   0x180007720
+   18000128b:	test   %rdi,%rdi
+   18000128e:	je     0x18000129d
+   180001290:	mov    %rsi,%rcx
+   180001293:	mov    $0x2,%edx
+   180001298:	call   0x180008140
+   18000129d:	nop
+   18000129e:	add    $0x90,%rsp
+   1800012a5:	pop    %rdi
+   1800012a6:	pop    %rsi
+   1800012a7:	pop    %rbp
+   1800012a8:	ret
+   1800012a9:	lea    0x8(%rdi),%rax
+   1800012ad:	mov    (%rax),%rdx
+   1800012b0:	test   %rdx,%rdx
+   1800012b3:	jne    0x180001251
+   1800012b5:	jmp    0x180001260
+   1800012b7:	nopw   0x0(%rax,%rax,1)
    1800012c0:	mov    %rdx,0x10(%rsp)
    1800012c5:	push   %rbp
    1800012c6:	push   %rsi
    1800012c7:	push   %rdi
    1800012c8:	sub    $0x20,%rsp
    1800012cc:	lea    0x80(%rdx),%rbp
-   1800012d3:	mov    -0x20(%rbp),%rcx
-   1800012d7:	mov    0x10(%rbp),%rdx
+   1800012d3:	mov    -0x30(%rbp),%rcx
+   1800012d7:	mov    0x0(%rbp),%rdx
    1800012db:	call   0x180003c80
    1800012e0:	nop
    1800012e1:	add    $0x20,%rsp
    1800012e5:	pop    %rdi
    1800012e6:	pop    %rsi
    1800012e7:	pop    %rbp
    1800012e8:	ret
@@ -29439,15 +29439,15 @@
    18000134a:	mov    %rax,%rbx
    18000134d:	jmp    0x1800013c2
    18000134f:	mov    0x60(%rbp),%r9d
    180001353:	mov    %rdi,-0x30(%rbp)
    180001357:	mov    %rsi,-0x28(%rbp)
    18000135b:	xorps  %xmm0,%xmm0
    18000135e:	movups %xmm0,0x30(%rsp)
-   180001363:	lea    -0x1fa(%rip),%rax        # 0x180001170
+   180001363:	lea    -0x36a(%rip),%rax        # 0x180001000
    18000136a:	mov    %rax,0x28(%rsp)
    18000136f:	movq   $0x0,0x40(%rsp)
    180001378:	movq   $0x1,0x20(%rsp)
    180001381:	mov    %r14,%rcx
    180001384:	mov    %rdi,%rdx
    180001387:	mov    %ebx,%r8d
    18000138a:	call   0x180008240
@@ -29529,15 +29529,15 @@
    18000146a:	mov    %rax,%rbx
    18000146d:	jmp    0x1800014e2
    18000146f:	mov    0x60(%rbp),%r9d
    180001473:	mov    %rdi,-0x30(%rbp)
    180001477:	mov    %rsi,-0x28(%rbp)
    18000147b:	xorps  %xmm0,%xmm0
    18000147e:	movups %xmm0,0x30(%rsp)
-   180001483:	lea    -0x48a(%rip),%rax        # 0x180001000
+   180001483:	lea    -0x30a(%rip),%rax        # 0x180001180
    18000148a:	mov    %rax,0x28(%rsp)
    18000148f:	movq   $0x0,0x40(%rsp)
    180001498:	movq   $0x1,0x20(%rsp)
    1800014a1:	mov    %r14,%rcx
    1800014a4:	mov    %rdi,%rdx
    1800014a7:	mov    %ebx,%r8d
    1800014aa:	call   0x180008240
@@ -29604,15 +29604,15 @@
    18000154a:	mov    %rcx,%rsi
    18000154d:	call   0x180022cf0
    180001552:	mov    0x8(%rax),%r9
    180001556:	movslq %ebx,%r8
    180001559:	mov    %r9,-0x10(%rbp)
    18000155d:	mov    %rsi,%rcx
    180001560:	mov    %rdi,%rdx
-   180001563:	call   0x180005100
+   180001563:	call   0x180004960
    180001568:	test   %rax,%rax
    18000156b:	je     0x180001607
    180001571:	lea    -0x28(%rbp),%rcx
    180001575:	mov    %rax,%rdx
    180001578:	call   0x180007a20
    18000157d:	mov    -0x20(%rbp),%rdx
    180001581:	mov    -0x18(%rbp),%r8
@@ -29842,15 +29842,15 @@
    1800017ea:	mov    %rcx,%rsi
    1800017ed:	call   0x180022cf0
    1800017f2:	mov    0x8(%rax),%r9
    1800017f6:	movslq %ebx,%r8
    1800017f9:	mov    %r9,-0x10(%rbp)
    1800017fd:	mov    %rsi,%rcx
    180001800:	mov    %rdi,%rdx
-   180001803:	call   0x180005590
+   180001803:	call   0x180005430
    180001808:	test   %rax,%rax
    18000180b:	je     0x1800018a7
    180001811:	lea    -0x28(%rbp),%rcx
    180001815:	mov    %rax,%rdx
    180001818:	call   0x180007a20
    18000181d:	mov    -0x20(%rbp),%rdx
    180001821:	mov    -0x18(%rbp),%r8
@@ -29961,15 +29961,15 @@
    18000193a:	mov    %rcx,%rsi
    18000193d:	call   0x180022cf0
    180001942:	mov    0x8(%rax),%r9
    180001946:	movslq %ebx,%r8
    180001949:	mov    %r9,-0x10(%rbp)
    18000194d:	mov    %rsi,%rcx
    180001950:	mov    %rdi,%rdx
-   180001953:	call   0x180005c50
+   180001953:	call   0x180005100
    180001958:	test   %rax,%rax
    18000195b:	je     0x1800019f7
    180001961:	lea    -0x28(%rbp),%rcx
    180001965:	mov    %rax,%rdx
    180001968:	call   0x180007a20
    18000196d:	mov    -0x20(%rbp),%rdx
    180001971:	mov    -0x18(%rbp),%r8
@@ -30080,15 +30080,15 @@
    180001a8a:	mov    %rcx,%rsi
    180001a8d:	call   0x180022cf0
    180001a92:	mov    0x8(%rax),%r9
    180001a96:	movslq %ebx,%r8
    180001a99:	mov    %r9,-0x10(%rbp)
    180001a9d:	mov    %rsi,%rcx
    180001aa0:	mov    %rdi,%rdx
-   180001aa3:	call   0x180005e90
+   180001aa3:	call   0x180005c50
    180001aa8:	test   %rax,%rax
    180001aab:	je     0x180001b47
    180001ab1:	lea    -0x28(%rbp),%rcx
    180001ab5:	mov    %rax,%rdx
    180001ab8:	call   0x180007a20
    180001abd:	mov    -0x20(%rbp),%rdx
    180001ac1:	mov    -0x18(%rbp),%r8
@@ -30199,15 +30199,15 @@
    180001bda:	mov    %rcx,%rsi
    180001bdd:	call   0x180022cf0
    180001be2:	mov    0x8(%rax),%r9
    180001be6:	movslq %ebx,%r8
    180001be9:	mov    %r9,-0x10(%rbp)
    180001bed:	mov    %rsi,%rcx
    180001bf0:	mov    %rdi,%rdx
-   180001bf3:	call   0x180005430
+   180001bf3:	call   0x180004020
    180001bf8:	test   %rax,%rax
    180001bfb:	je     0x180001c97
    180001c01:	lea    -0x28(%rbp),%rcx
    180001c05:	mov    %rax,%rdx
    180001c08:	call   0x180007a20
    180001c0d:	mov    -0x20(%rbp),%rdx
    180001c11:	mov    -0x18(%rbp),%r8
@@ -30318,15 +30318,15 @@
    180001d2a:	mov    %rcx,%rsi
    180001d2d:	call   0x180022cf0
    180001d32:	mov    0x8(%rax),%r9
    180001d36:	movslq %ebx,%r8
    180001d39:	mov    %r9,-0x10(%rbp)
    180001d3d:	mov    %rsi,%rcx
    180001d40:	mov    %rdi,%rdx
-   180001d43:	call   0x180003ec0
+   180001d43:	call   0x180005250
    180001d48:	test   %rax,%rax
    180001d4b:	je     0x180001de7
    180001d51:	lea    -0x28(%rbp),%rcx
    180001d55:	mov    %rax,%rdx
    180001d58:	call   0x180007a20
    180001d5d:	mov    -0x20(%rbp),%rdx
    180001d61:	mov    -0x18(%rbp),%r8
@@ -30437,15 +30437,15 @@
    180001e7a:	mov    %rcx,%rsi
    180001e7d:	call   0x180022cf0
    180001e82:	mov    0x8(%rax),%r9
    180001e86:	movslq %ebx,%r8
    180001e89:	mov    %r9,-0x10(%rbp)
    180001e8d:	mov    %rsi,%rcx
    180001e90:	mov    %rdi,%rdx
-   180001e93:	call   0x1800057c0
+   180001e93:	call   0x180005a10
    180001e98:	test   %rax,%rax
    180001e9b:	je     0x180001f37
    180001ea1:	lea    -0x28(%rbp),%rcx
    180001ea5:	mov    %rax,%rdx
    180001ea8:	call   0x180007a20
    180001ead:	mov    -0x20(%rbp),%rdx
    180001eb1:	mov    -0x18(%rbp),%r8
@@ -30556,15 +30556,15 @@
    180001fca:	mov    %rcx,%rsi
    180001fcd:	call   0x180022cf0
    180001fd2:	mov    0x8(%rax),%r9
    180001fd6:	movslq %ebx,%r8
    180001fd9:	mov    %r9,-0x10(%rbp)
    180001fdd:	mov    %rsi,%rcx
    180001fe0:	mov    %rdi,%rdx
-   180001fe3:	call   0x180004020
+   180001fe3:	call   0x1800057c0
    180001fe8:	test   %rax,%rax
    180001feb:	je     0x180002087
    180001ff1:	lea    -0x28(%rbp),%rcx
    180001ff5:	mov    %rax,%rdx
    180001ff8:	call   0x180007a20
    180001ffd:	mov    -0x20(%rbp),%rdx
    180002001:	mov    -0x18(%rbp),%r8
@@ -30675,15 +30675,15 @@
    18000211a:	mov    %rcx,%rsi
    18000211d:	call   0x180022cf0
    180002122:	mov    0x8(%rax),%r9
    180002126:	movslq %ebx,%r8
    180002129:	mov    %r9,-0x10(%rbp)
    18000212d:	mov    %rsi,%rcx
    180002130:	mov    %rdi,%rdx
-   180002133:	call   0x180005a10
+   180002133:	call   0x180003ec0
    180002138:	test   %rax,%rax
    18000213b:	je     0x1800021d7
    180002141:	lea    -0x28(%rbp),%rcx
    180002145:	mov    %rax,%rdx
    180002148:	call   0x180007a20
    18000214d:	mov    -0x20(%rbp),%rdx
    180002151:	mov    -0x18(%rbp),%r8
@@ -30794,15 +30794,15 @@
    18000226a:	mov    %rcx,%rsi
    18000226d:	call   0x180022cf0
    180002272:	mov    0x8(%rax),%r9
    180002276:	movslq %ebx,%r8
    180002279:	mov    %r9,-0x10(%rbp)
    18000227d:	mov    %rsi,%rcx
    180002280:	mov    %rdi,%rdx
-   180002283:	call   0x180005250
+   180002283:	call   0x180005590
    180002288:	test   %rax,%rax
    18000228b:	je     0x180002327
    180002291:	lea    -0x28(%rbp),%rcx
    180002295:	mov    %rax,%rdx
    180002298:	call   0x180007a20
    18000229d:	mov    -0x20(%rbp),%rdx
    1800022a1:	mov    -0x18(%rbp),%r8
@@ -30913,15 +30913,15 @@
    1800023ba:	mov    %rcx,%rsi
    1800023bd:	call   0x180022cf0
    1800023c2:	mov    0x8(%rax),%r9
    1800023c6:	movslq %ebx,%r8
    1800023c9:	mov    %r9,-0x10(%rbp)
    1800023cd:	mov    %rsi,%rcx
    1800023d0:	mov    %rdi,%rdx
-   1800023d3:	call   0x180004960
+   1800023d3:	call   0x180005e90
    1800023d8:	test   %rax,%rax
    1800023db:	je     0x180002477
    1800023e1:	lea    -0x28(%rbp),%rcx
    1800023e5:	mov    %rax,%rdx
    1800023e8:	call   0x180007a20
    1800023ed:	mov    -0x20(%rbp),%rdx
    1800023f1:	mov    -0x18(%rbp),%r8
@@ -31070,15 +31070,15 @@
    1800025a6:	mov    %rax,%rbx
    1800025a9:	jmp    0x18000261a
    1800025ab:	mov    0x70(%rbp),%r9d
    1800025af:	mov    %rdi,-0x30(%rbp)
    1800025b3:	mov    %rsi,-0x28(%rbp)
    1800025b7:	xorps  %xmm0,%xmm0
    1800025ba:	movups %xmm0,0x30(%rsp)
-   1800025bf:	lea    -0xf46(%rip),%rax        # 0x180001680
+   1800025bf:	lea    -0xdf6(%rip),%rax        # 0x1800017d0
    1800025c6:	mov    %rax,0x28(%rsp)
    1800025cb:	mov    %r15,0x20(%rsp)
    1800025d0:	movq   $0x0,0x40(%rsp)
    1800025d9:	mov    %r14,%rcx
    1800025dc:	mov    %rdi,%rdx
    1800025df:	mov    %ebx,%r8d
    1800025e2:	call   0x180008240
@@ -31228,15 +31228,15 @@
    180002796:	mov    %rax,%rbx
    180002799:	jmp    0x18000280a
    18000279b:	mov    0x70(%rbp),%r9d
    18000279f:	mov    %rdi,-0x30(%rbp)
    1800027a3:	mov    %rsi,-0x28(%rbp)
    1800027a7:	xorps  %xmm0,%xmm0
    1800027aa:	movups %xmm0,0x30(%rsp)
-   1800027af:	lea    -0x416(%rip),%rax        # 0x1800023a0
+   1800027af:	lea    -0x566(%rip),%rax        # 0x180002250
    1800027b6:	mov    %rax,0x28(%rsp)
    1800027bb:	mov    %r15,0x20(%rsp)
    1800027c0:	movq   $0x0,0x40(%rsp)
    1800027c9:	mov    %r14,%rcx
    1800027cc:	mov    %rdi,%rdx
    1800027cf:	mov    %ebx,%r8d
    1800027d2:	call   0x180008240
@@ -31386,15 +31386,15 @@
    180002986:	mov    %rax,%rbx
    180002989:	jmp    0x1800029fa
    18000298b:	mov    0x70(%rbp),%r9d
    18000298f:	mov    %rdi,-0x30(%rbp)
    180002993:	mov    %rsi,-0x28(%rbp)
    180002997:	xorps  %xmm0,%xmm0
    18000299a:	movups %xmm0,0x30(%rsp)
-   18000299f:	lea    -0xb46(%rip),%rax        # 0x180001e60
+   18000299f:	lea    -0xf36(%rip),%rax        # 0x180001a70
    1800029a6:	mov    %rax,0x28(%rsp)
    1800029ab:	mov    %r15,0x20(%rsp)
    1800029b0:	movq   $0x0,0x40(%rsp)
    1800029b9:	mov    %r14,%rcx
    1800029bc:	mov    %rdi,%rdx
    1800029bf:	mov    %ebx,%r8d
    1800029c2:	call   0x180008240
@@ -31544,15 +31544,15 @@
    180002b76:	mov    %rax,%rbx
    180002b79:	jmp    0x180002bea
    180002b7b:	mov    0x70(%rbp),%r9d
    180002b7f:	mov    %rdi,-0x30(%rbp)
    180002b83:	mov    %rsi,-0x28(%rbp)
    180002b87:	xorps  %xmm0,%xmm0
    180002b8a:	movups %xmm0,0x30(%rsp)
-   180002b8f:	lea    -0xbe6(%rip),%rax        # 0x180001fb0
+   180002b8f:	lea    -0x7f6(%rip),%rax        # 0x1800023a0
    180002b96:	mov    %rax,0x28(%rsp)
    180002b9b:	mov    %r15,0x20(%rsp)
    180002ba0:	movq   $0x0,0x40(%rsp)
    180002ba9:	mov    %r14,%rcx
    180002bac:	mov    %rdi,%rdx
    180002baf:	mov    %ebx,%r8d
    180002bb2:	call   0x180008240
@@ -31702,15 +31702,15 @@
    180002d66:	mov    %rax,%rbx
    180002d69:	jmp    0x180002dda
    180002d6b:	mov    0x70(%rbp),%r9d
    180002d6f:	mov    %rdi,-0x30(%rbp)
    180002d73:	mov    %rsi,-0x28(%rbp)
    180002d77:	xorps  %xmm0,%xmm0
    180002d7a:	movups %xmm0,0x30(%rsp)
-   180002d7f:	lea    -0x15b6(%rip),%rax        # 0x1800017d0
+   180002d7f:	lea    -0x1076(%rip),%rax        # 0x180001d10
    180002d86:	mov    %rax,0x28(%rsp)
    180002d8b:	mov    %r15,0x20(%rsp)
    180002d90:	movq   $0x0,0x40(%rsp)
    180002d99:	mov    %r14,%rcx
    180002d9c:	mov    %rdi,%rdx
    180002d9f:	mov    %ebx,%r8d
    180002da2:	call   0x180008240
@@ -31860,15 +31860,15 @@
    180002f56:	mov    %rax,%rbx
    180002f59:	jmp    0x180002fca
    180002f5b:	mov    0x70(%rbp),%r9d
    180002f5f:	mov    %rdi,-0x30(%rbp)
    180002f63:	mov    %rsi,-0x28(%rbp)
    180002f67:	xorps  %xmm0,%xmm0
    180002f6a:	movups %xmm0,0x30(%rsp)
-   180002f6f:	lea    -0x1266(%rip),%rax        # 0x180001d10
+   180002f6f:	lea    -0xfc6(%rip),%rax        # 0x180001fb0
    180002f76:	mov    %rax,0x28(%rsp)
    180002f7b:	mov    %r15,0x20(%rsp)
    180002f80:	movq   $0x0,0x40(%rsp)
    180002f89:	mov    %r14,%rcx
    180002f8c:	mov    %rdi,%rdx
    180002f8f:	mov    %ebx,%r8d
    180002f92:	call   0x180008240
@@ -32018,15 +32018,15 @@
    180003146:	mov    %rax,%rbx
    180003149:	jmp    0x1800031ba
    18000314b:	mov    0x70(%rbp),%r9d
    18000314f:	mov    %rdi,-0x30(%rbp)
    180003153:	mov    %rsi,-0x28(%rbp)
    180003157:	xorps  %xmm0,%xmm0
    18000315a:	movups %xmm0,0x30(%rsp)
-   18000315f:	lea    -0x1846(%rip),%rax        # 0x180001920
+   18000315f:	lea    -0x1c36(%rip),%rax        # 0x180001530
    180003166:	mov    %rax,0x28(%rsp)
    18000316b:	mov    %r15,0x20(%rsp)
    180003170:	movq   $0x0,0x40(%rsp)
    180003179:	mov    %r14,%rcx
    18000317c:	mov    %rdi,%rdx
    18000317f:	mov    %ebx,%r8d
    180003182:	call   0x180008240
@@ -32334,15 +32334,15 @@
    180003526:	mov    %rax,%rbx
    180003529:	jmp    0x18000359a
    18000352b:	mov    0x70(%rbp),%r9d
    18000352f:	mov    %rdi,-0x30(%rbp)
    180003533:	mov    %rsi,-0x28(%rbp)
    180003537:	xorps  %xmm0,%xmm0
    18000353a:	movups %xmm0,0x30(%rsp)
-   18000353f:	lea    -0x12f6(%rip),%rax        # 0x180002250
+   18000353f:	lea    -0x1986(%rip),%rax        # 0x180001bc0
    180003546:	mov    %rax,0x28(%rsp)
    18000354b:	mov    %r15,0x20(%rsp)
    180003550:	movq   $0x0,0x40(%rsp)
    180003559:	mov    %r14,%rcx
    18000355c:	mov    %rdi,%rdx
    18000355f:	mov    %ebx,%r8d
    180003562:	call   0x180008240
@@ -32492,15 +32492,15 @@
    180003716:	mov    %rax,%rbx
    180003719:	jmp    0x18000378a
    18000371b:	mov    0x70(%rbp),%r9d
    18000371f:	mov    %rdi,-0x30(%rbp)
    180003723:	mov    %rsi,-0x28(%rbp)
    180003727:	xorps  %xmm0,%xmm0
    18000372a:	movups %xmm0,0x30(%rsp)
-   18000372f:	lea    -0x2206(%rip),%rax        # 0x180001530
+   18000372f:	lea    -0x20b6(%rip),%rax        # 0x180001680
    180003736:	mov    %rax,0x28(%rsp)
    18000373b:	mov    %r15,0x20(%rsp)
    180003740:	movq   $0x0,0x40(%rsp)
    180003749:	mov    %r14,%rcx
    18000374c:	mov    %rdi,%rdx
    18000374f:	mov    %ebx,%r8d
    180003752:	call   0x180008240
@@ -32650,15 +32650,15 @@
    180003906:	mov    %rax,%rbx
    180003909:	jmp    0x18000397a
    18000390b:	mov    0x70(%rbp),%r9d
    18000390f:	mov    %rdi,-0x30(%rbp)
    180003913:	mov    %rsi,-0x28(%rbp)
    180003917:	xorps  %xmm0,%xmm0
    18000391a:	movups %xmm0,0x30(%rsp)
-   18000391f:	lea    -0x1eb6(%rip),%rax        # 0x180001a70
+   18000391f:	lea    -0x2006(%rip),%rax        # 0x180001920
    180003926:	mov    %rax,0x28(%rsp)
    18000392b:	mov    %r15,0x20(%rsp)
    180003930:	movq   $0x0,0x40(%rsp)
    180003939:	mov    %r14,%rcx
    18000393c:	mov    %rdi,%rdx
    18000393f:	mov    %ebx,%r8d
    180003942:	call   0x180008240
@@ -32808,15 +32808,15 @@
    180003af6:	mov    %rax,%rbx
    180003af9:	jmp    0x180003b6a
    180003afb:	mov    0x70(%rbp),%r9d
    180003aff:	mov    %rdi,-0x30(%rbp)
    180003b03:	mov    %rsi,-0x28(%rbp)
    180003b07:	xorps  %xmm0,%xmm0
    180003b0a:	movups %xmm0,0x30(%rsp)
-   180003b0f:	lea    -0x1f56(%rip),%rax        # 0x180001bc0
+   180003b0f:	lea    -0x1cb6(%rip),%rax        # 0x180001e60
    180003b16:	mov    %rax,0x28(%rsp)
    180003b1b:	mov    %r15,0x20(%rsp)
    180003b20:	movq   $0x0,0x40(%rsp)
    180003b29:	mov    %r14,%rcx
    180003b2c:	mov    %rdi,%rdx
    180003b2f:	mov    %ebx,%r8d
    180003b32:	call   0x180008240
@@ -33237,15 +33237,15 @@
    180003fb6:	pop    %rdi
    180003fb7:	pop    %rsi
    180003fb8:	pop    %rbp
    180003fb9:	ret
    180003fba:	lea    0xe5817(%rip),%rax        # 0x1800e97d8
    180003fc1:	mov    %rax,0x20(%rsp)
    180003fc6:	lea    0xe57eb(%rip),%rcx        # 0x1800e97b8
-   180003fcd:	lea    0xe55dc(%rip),%r9        # 0x1800e95b0
+   180003fcd:	lea    0xe55bc(%rip),%r9        # 0x1800e9590
    180003fd4:	mov    %rbp,%r8
    180003fd7:	mov    $0x10,%edx
    180003fdc:	call   0x1800e8710
    180003fe1:	ud2
    180003fe3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
    180003ff0:	mov    %rdx,0x10(%rsp)
    180003ff5:	push   %rbp
@@ -33342,15 +33342,15 @@
    180004148:	pop    %rdi
    180004149:	pop    %rsi
    18000414a:	pop    %rbp
    18000414b:	ret
    18000414c:	lea    0xe5425(%rip),%rax        # 0x1800e9578
    180004153:	mov    %rax,0x20(%rsp)
    180004158:	lea    0xe5391(%rip),%rcx        # 0x1800e94f0
-   18000415f:	lea    0xe542a(%rip),%r9        # 0x1800e9590
+   18000415f:	lea    0xe544a(%rip),%r9        # 0x1800e95b0
    180004166:	lea    0x40(%rbp),%r8
    18000416a:	mov    $0x37,%edx
    18000416f:	call   0x1800e8710
    180004174:	ud2
    180004176:	cs nopw 0x0(%rax,%rax,1)
    180004180:	mov    %rdx,0x10(%rsp)
    180004185:	push   %rbp
@@ -33758,15 +33758,15 @@
    180004799:	mov    %r13,-0x48(%rbp)
    18000479d:	movq   $0x2,-0x60(%rbp)
    1800047a5:	movq   $0x1,0x10(%rbp)
    1800047ad:	lea    -0x4c(%rbp),%rax
    1800047b1:	mov    %rax,0x18(%rbp)
    1800047b5:	lea    -0x60(%rbp),%rax
    1800047b9:	mov    %rax,-0x10(%rbp)
-   1800047bd:	lea    0x2b4c(%rip),%rax        # 0x180007310
+   1800047bd:	lea    0x2bcc(%rip),%rax        # 0x180007390
    1800047c4:	mov    %rax,-0x8(%rbp)
    1800047c8:	lea    0x10(%rbp),%rcx
    1800047cc:	mov    %rcx,0x0(%rbp)
    1800047d0:	mov    %rax,0x8(%rbp)
    1800047d4:	lea    0xe4e6d(%rip),%rax        # 0x1800e9648
    1800047db:	mov    %rax,-0x30(%rbp)
    1800047df:	movq   $0x2,-0x28(%rbp)
@@ -35604,15 +35604,15 @@
    180006147:	ret
    180006148:	movq   $0x2,-0x58(%rbp)
    180006150:	movq   $0x1,-0x30(%rbp)
    180006158:	lea    0x3f(%rbp),%rax
    18000615c:	mov    %rax,-0x28(%rbp)
    180006160:	lea    -0x58(%rbp),%rax
    180006164:	mov    %rax,0x18(%rbp)
-   180006168:	lea    0x1221(%rip),%rax        # 0x180007390
+   180006168:	lea    0x11a1(%rip),%rax        # 0x180007310
    18000616f:	mov    %rax,0x20(%rbp)
    180006173:	lea    -0x30(%rbp),%rcx
    180006177:	mov    %rcx,0x28(%rbp)
    18000617b:	mov    %rax,0x30(%rbp)
    18000617f:	lea    0xe34c2(%rip),%rax        # 0x1800e9648
    180006186:	mov    %rax,-0x8(%rbp)
    18000618a:	movq   $0x2,0x0(%rbp)
@@ -35749,218 +35749,218 @@
    180006352:	je     0x18000678b
    180006358:	mov    %rax,0x28(%rsp)
    18000635d:	movl   $0x0,0x20(%rsp)
    180006365:	lea    0xe3642(%rip),%rdx        # 0x1800e99ae
    18000636c:	mov    $0x11,%r8d
    180006372:	mov    %rsi,%rcx
    180006375:	xor    %r9d,%r9d
-   180006378:	call   0x180002ac0
+   180006378:	call   0x180003470
    18000637d:	mov    %rax,%rdi
    180006380:	test   %rax,%rax
    180006383:	jne    0x180006750
    180006389:	mov    -0x10(%rbp),%rax
    18000638d:	incq   (%rax)
    180006390:	je     0x18000678b
    180006396:	mov    %rax,0x28(%rsp)
    18000639b:	movl   $0x0,0x20(%rsp)
    1800063a3:	lea    0xe3615(%rip),%rdx        # 0x1800e99bf
    1800063aa:	mov    $0x11,%r8d
    1800063b0:	mov    %rsi,%rcx
    1800063b3:	mov    $0x1,%r9d
-   1800063b9:	call   0x180002ea0
+   1800063b9:	call   0x180003280
    1800063be:	mov    %rax,%rdi
    1800063c1:	test   %rax,%rax
    1800063c4:	jne    0x180006750
    1800063ca:	mov    -0x10(%rbp),%rax
    1800063ce:	incq   (%rax)
    1800063d1:	je     0x18000678b
    1800063d7:	mov    %rax,0x28(%rsp)
    1800063dc:	movl   $0x0,0x20(%rsp)
    1800063e4:	lea    0xe35e5(%rip),%rdx        # 0x1800e99d0
    1800063eb:	mov    $0xc,%r8d
    1800063f1:	mov    %rsi,%rcx
    1800063f4:	xor    %r9d,%r9d
-   1800063f7:	call   0x1800024f0
+   1800063f7:	call   0x180003660
    1800063fc:	mov    %rax,%rdi
    1800063ff:	test   %rax,%rax
    180006402:	jne    0x180006750
    180006408:	mov    -0x10(%rbp),%rax
    18000640c:	incq   (%rax)
    18000640f:	je     0x18000678b
    180006415:	mov    %rax,0x28(%rsp)
    18000641a:	movl   $0x0,0x20(%rsp)
    180006422:	lea    0xe35a7(%rip),%rdx        # 0x1800e99d0
    180006429:	mov    $0xc,%r8d
    18000642f:	mov    %rsi,%rcx
    180006432:	mov    $0x1,%r9d
-   180006438:	call   0x1800024f0
+   180006438:	call   0x180003660
    18000643d:	mov    %rax,%rdi
    180006440:	test   %rax,%rax
    180006443:	jne    0x180006750
    180006449:	mov    -0x10(%rbp),%rax
    18000644d:	incq   (%rax)
    180006450:	je     0x18000678b
    180006456:	mov    %rax,0x28(%rsp)
    18000645b:	movl   $0x0,0x20(%rsp)
    180006463:	lea    0xe3566(%rip),%rdx        # 0x1800e99d0
    18000646a:	mov    $0xc,%r8d
    180006470:	mov    %rsi,%rcx
    180006473:	mov    $0x2,%r9d
-   180006479:	call   0x1800024f0
+   180006479:	call   0x180003660
    18000647e:	mov    %rax,%rdi
    180006481:	test   %rax,%rax
    180006484:	jne    0x180006750
    18000648a:	mov    -0x10(%rbp),%rax
    18000648e:	incq   (%rax)
    180006491:	je     0x18000678b
    180006497:	mov    %rax,0x28(%rsp)
    18000649c:	movl   $0x0,0x20(%rsp)
    1800064a4:	lea    0xe3531(%rip),%rdx        # 0x1800e99dc
    1800064ab:	mov    $0xe,%r8d
    1800064b1:	mov    %rsi,%rcx
    1800064b4:	xor    %r9d,%r9d
-   1800064b7:	call   0x1800026e0
+   1800064b7:	call   0x180003090
    1800064bc:	mov    %rax,%rdi
    1800064bf:	test   %rax,%rax
    1800064c2:	jne    0x180006750
    1800064c8:	mov    -0x10(%rbp),%rax
    1800064cc:	incq   (%rax)
    1800064cf:	je     0x18000678b
    1800064d5:	mov    %rax,0x28(%rsp)
    1800064da:	movl   $0x0,0x20(%rsp)
    1800064e2:	lea    0xe34f3(%rip),%rdx        # 0x1800e99dc
    1800064e9:	mov    $0xe,%r8d
    1800064ef:	mov    %rsi,%rcx
    1800064f2:	mov    $0x1,%r9d
-   1800064f8:	call   0x1800026e0
+   1800064f8:	call   0x180003090
    1800064fd:	mov    %rax,%rdi
    180006500:	test   %rax,%rax
    180006503:	jne    0x180006750
    180006509:	mov    -0x10(%rbp),%rax
    18000650d:	incq   (%rax)
    180006510:	je     0x18000678b
    180006516:	mov    %rax,0x28(%rsp)
    18000651b:	movl   $0x0,0x20(%rsp)
    180006523:	lea    0xe34b2(%rip),%rdx        # 0x1800e99dc
    18000652a:	mov    $0xe,%r8d
    180006530:	mov    %rsi,%rcx
    180006533:	mov    $0x2,%r9d
-   180006539:	call   0x1800026e0
+   180006539:	call   0x180003090
    18000653e:	mov    %rax,%rdi
    180006541:	test   %rax,%rax
    180006544:	jne    0x180006750
    18000654a:	mov    -0x10(%rbp),%rax
    18000654e:	incq   (%rax)
    180006551:	je     0x18000678b
    180006557:	mov    -0x10(%rbp),%rax
    18000655b:	mov    %rax,0x28(%rsp)
    180006560:	movl   $0x0,0x20(%rsp)
    180006568:	lea    0xe347b(%rip),%rdx        # 0x1800e99ea
    18000656f:	mov    $0xf,%r8d
    180006575:	mov    %rsi,%rcx
    180006578:	xor    %r9d,%r9d
-   18000657b:	call   0x180003660
+   18000657b:	call   0x180003850
    180006580:	mov    %rax,%rdi
    180006583:	test   %rax,%rax
    180006586:	jne    0x180006750
    18000658c:	mov    -0x10(%rbp),%rax
    180006590:	incq   (%rax)
    180006593:	je     0x18000678b
    180006599:	mov    -0x10(%rbp),%rax
    18000659d:	mov    %rax,0x28(%rsp)
    1800065a2:	movl   $0x0,0x20(%rsp)
    1800065aa:	lea    0xe3448(%rip),%rdx        # 0x1800e99f9
    1800065b1:	mov    $0xd,%r8d
    1800065b7:	mov    %rsi,%rcx
    1800065ba:	mov    $0x1,%r9d
-   1800065c0:	call   0x180003470
+   1800065c0:	call   0x180002cb0
    1800065c5:	mov    %rax,%rdi
    1800065c8:	test   %rax,%rax
    1800065cb:	jne    0x180006750
    1800065d1:	mov    -0x10(%rbp),%rax
    1800065d5:	incq   (%rax)
    1800065d8:	je     0x18000678b
    1800065de:	mov    -0x10(%rbp),%rax
    1800065e2:	mov    %rax,0x28(%rsp)
    1800065e7:	movl   $0x0,0x20(%rsp)
    1800065ef:	lea    0xe3410(%rip),%rdx        # 0x1800e9a06
    1800065f6:	mov    $0xd,%r8d
    1800065fc:	mov    %rsi,%rcx
    1800065ff:	xor    %r9d,%r9d
-   180006602:	call   0x180003a40
+   180006602:	call   0x1800024f0
    180006607:	mov    %rax,%rdi
    18000660a:	test   %rax,%rax
    18000660d:	jne    0x180006750
    180006613:	mov    -0x10(%rbp),%rax
    180006617:	incq   (%rax)
    18000661a:	je     0x18000678b
    180006620:	mov    -0x10(%rbp),%rax
    180006624:	mov    %rax,0x28(%rsp)
    180006629:	movl   $0x0,0x20(%rsp)
    180006631:	lea    0xe33db(%rip),%rdx        # 0x1800e9a13
    180006638:	mov    $0x13,%r8d
    18000663e:	mov    %rsi,%rcx
    180006641:	xor    %r9d,%r9d
-   180006644:	call   0x180002cb0
+   180006644:	call   0x1800026e0
    180006649:	mov    %rax,%rdi
    18000664c:	test   %rax,%rax
    18000664f:	jne    0x180006750
    180006655:	mov    -0x10(%rbp),%rax
    180006659:	incq   (%rax)
    18000665c:	je     0x18000678b
    180006662:	mov    -0x10(%rbp),%rax
    180006666:	mov    %rax,0x28(%rsp)
    18000666b:	movl   $0x0,0x20(%rsp)
    180006673:	lea    0xe33ac(%rip),%rdx        # 0x1800e9a26
    18000667a:	mov    $0x15,%r8d
    180006680:	mov    %rsi,%rcx
    180006683:	xor    %r9d,%r9d
-   180006686:	call   0x1800028d0
+   180006686:	call   0x180002ea0
    18000668b:	mov    %rax,%rdi
    18000668e:	test   %rax,%rax
    180006691:	jne    0x180006750
    180006697:	mov    -0x10(%rbp),%rax
    18000669b:	incq   (%rax)
    18000669e:	je     0x18000678b
    1800066a4:	mov    -0x10(%rbp),%rax
    1800066a8:	mov    %rax,0x28(%rsp)
    1800066ad:	movl   $0x0,0x20(%rsp)
    1800066b5:	lea    0xe337f(%rip),%rdx        # 0x1800e9a3b
    1800066bc:	mov    $0x12,%r8d
    1800066c2:	mov    %rsi,%rcx
    1800066c5:	xor    %r9d,%r9d
-   1800066c8:	call   0x180003090
+   1800066c8:	call   0x1800028d0
    1800066cd:	mov    %rax,%rdi
    1800066d0:	test   %rax,%rax
    1800066d3:	jne    0x180006750
    1800066d5:	mov    -0x10(%rbp),%rax
    1800066d9:	incq   (%rax)
    1800066dc:	je     0x18000678b
    1800066e2:	mov    -0x10(%rbp),%rax
    1800066e6:	mov    %rax,0x28(%rsp)
    1800066eb:	movl   $0x0,0x20(%rsp)
    1800066f3:	lea    0xe3353(%rip),%rdx        # 0x1800e9a4d
    1800066fa:	mov    $0x12,%r8d
    180006700:	mov    %rsi,%rcx
    180006703:	xor    %r9d,%r9d
-   180006706:	call   0x180003280
+   180006706:	call   0x180003a40
    18000670b:	mov    %rax,%rdi
    18000670e:	test   %rax,%rax
    180006711:	jne    0x180006750
    180006713:	mov    -0x10(%rbp),%rax
    180006717:	incq   (%rax)
    18000671a:	je     0x18000678b
    18000671c:	mov    -0x10(%rbp),%rax
    180006720:	mov    %rax,0x28(%rsp)
    180006725:	movl   $0x0,0x20(%rsp)
    18000672d:	lea    0xe332b(%rip),%rdx        # 0x1800e9a5f
    180006734:	mov    $0xe,%r8d
    18000673a:	mov    %rsi,%rcx
    18000673d:	mov    $0x1,%r9d
-   180006743:	call   0x180003850
+   180006743:	call   0x180002ac0
    180006748:	mov    %rax,%rdi
    18000674b:	test   %rax,%rax
    18000674e:	je     0x18000678f
    180006750:	mov    -0x10(%rbp),%rcx
    180006754:	decq   (%rcx)
    180006757:	jne    0x18000676f
    180006759:	decq   0x8(%rcx)
@@ -36372,30 +36372,30 @@
    180006c07:	test   %al,%al
    180006c09:	je     0x180006c1c
    180006c0b:	mov    %rdi,%rcx
    180006c0e:	mov    %rsi,%rdx
    180006c11:	add    $0x28,%rsp
    180006c15:	pop    %rdi
    180006c16:	pop    %rsi
-   180006c17:	jmp    0x18001e910
+   180006c17:	jmp    0x18001ea50
    180006c1c:	mov    %rsi,%rcx
    180006c1f:	call   0x18001c210
    180006c24:	mov    %rdi,%rcx
    180006c27:	mov    %rsi,%rdx
    180006c2a:	test   %al,%al
    180006c2c:	je     0x180006c39
    180006c2e:	add    $0x28,%rsp
    180006c32:	pop    %rdi
    180006c33:	pop    %rsi
-   180006c34:	jmp    0x18001e9b0
+   180006c34:	jmp    0x18001eaf0
    180006c39:	nop
    180006c3a:	add    $0x28,%rsp
    180006c3e:	pop    %rdi
    180006c3f:	pop    %rsi
-   180006c40:	jmp    0x18001f000
+   180006c40:	jmp    0x18001f260
    180006c45:	int3
    180006c46:	int3
    180006c47:	int3
    180006c48:	int3
    180006c49:	int3
    180006c4a:	int3
    180006c4b:	int3
@@ -36414,30 +36414,30 @@
    180006c67:	test   %al,%al
    180006c69:	je     0x180006c7c
    180006c6b:	mov    %rdi,%rcx
    180006c6e:	mov    %rsi,%rdx
    180006c71:	add    $0x28,%rsp
    180006c75:	pop    %rdi
    180006c76:	pop    %rsi
-   180006c77:	jmp    0x18001e7d0
+   180006c77:	jmp    0x18001e910
    180006c7c:	mov    %rsi,%rcx
    180006c7f:	call   0x18001c210
    180006c84:	mov    %rdi,%rcx
    180006c87:	mov    %rsi,%rdx
    180006c8a:	test   %al,%al
    180006c8c:	je     0x180006c99
    180006c8e:	add    $0x28,%rsp
    180006c92:	pop    %rdi
    180006c93:	pop    %rsi
-   180006c94:	jmp    0x18001e870
+   180006c94:	jmp    0x18001e9b0
    180006c99:	nop
    180006c9a:	add    $0x28,%rsp
    180006c9e:	pop    %rdi
    180006c9f:	pop    %rsi
-   180006ca0:	jmp    0x18001ef60
+   180006ca0:	jmp    0x18001f000
    180006ca5:	int3
    180006ca6:	int3
    180006ca7:	int3
    180006ca8:	int3
    180006ca9:	int3
    180006caa:	int3
    180006cab:	int3
@@ -36456,30 +36456,30 @@
    180006cc7:	test   %al,%al
    180006cc9:	je     0x180006cdc
    180006ccb:	mov    %rdi,%rcx
    180006cce:	mov    %rsi,%rdx
    180006cd1:	add    $0x28,%rsp
    180006cd5:	pop    %rdi
    180006cd6:	pop    %rsi
-   180006cd7:	jmp    0x18001ea50
+   180006cd7:	jmp    0x18001e7d0
    180006cdc:	mov    %rsi,%rcx
    180006cdf:	call   0x18001c210
    180006ce4:	mov    %rdi,%rcx
    180006ce7:	mov    %rsi,%rdx
    180006cea:	test   %al,%al
    180006cec:	je     0x180006cf9
    180006cee:	add    $0x28,%rsp
    180006cf2:	pop    %rdi
    180006cf3:	pop    %rsi
-   180006cf4:	jmp    0x18001eaf0
+   180006cf4:	jmp    0x18001e870
    180006cf9:	nop
    180006cfa:	add    $0x28,%rsp
    180006cfe:	pop    %rdi
    180006cff:	pop    %rsi
-   180006d00:	jmp    0x18001f260
+   180006d00:	jmp    0x18001ef60
    180006d05:	int3
    180006d06:	int3
    180006d07:	int3
    180006d08:	int3
    180006d09:	int3
    180006d0a:	int3
    180006d0b:	int3
@@ -36971,23 +36971,23 @@
    180007297:	mov    (%rcx),%rdx
    18000729a:	test   %rdx,%rdx
    18000729d:	je     0x1800072c2
    18000729f:	cmp    $0x1,%edx
    1800072a2:	jne    0x1800072f7
    1800072a4:	add    $0x8,%rcx
    1800072a8:	mov    %rcx,0x30(%rsp)
-   1800072ad:	lea    0xe2824(%rip),%rcx        # 0x1800e9ad8
+   1800072ad:	lea    0xe282c(%rip),%rcx        # 0x1800e9ae0
    1800072b4:	mov    %rcx,0x20(%rsp)
    1800072b9:	lea    0xe2809(%rip),%rdx        # 0x1800e9ac9
    1800072c0:	jmp    0x1800072de
    1800072c2:	add    $0x8,%rcx
    1800072c6:	mov    %rcx,0x30(%rsp)
-   1800072cb:	lea    0xe2806(%rip),%rcx        # 0x1800e9ad8
+   1800072cb:	lea    0xe280e(%rip),%rcx        # 0x1800e9ae0
    1800072d2:	mov    %rcx,0x20(%rsp)
-   1800072d7:	lea    0xe281a(%rip),%rdx        # 0x1800e9af8
+   1800072d7:	lea    0xe27f3(%rip),%rdx        # 0x1800e9ad1
    1800072de:	lea    0x30(%rsp),%r9
    1800072e3:	mov    $0x8,%r8d
    1800072e9:	mov    %rax,%rcx
    1800072ec:	call   0x18001c390
    1800072f1:	nop
    1800072f2:	add    $0x38,%rsp
    1800072f6:	ret
@@ -37009,15 +37009,15 @@
    180007334:	mov    %rcx,0x20(%rsp)
    180007339:	lea    0xe2789(%rip),%rdx        # 0x1800e9ac9
    180007340:	jmp    0x18000735e
    180007342:	add    $0x8,%rcx
    180007346:	mov    %rcx,0x30(%rsp)
    18000734b:	lea    0xe27ae(%rip),%rcx        # 0x1800e9b00
    180007352:	mov    %rcx,0x20(%rsp)
-   180007357:	lea    0xe279a(%rip),%rdx        # 0x1800e9af8
+   180007357:	lea    0xe2773(%rip),%rdx        # 0x1800e9ad1
    18000735e:	lea    0x30(%rsp),%r9
    180007363:	mov    $0x8,%r8d
    180007369:	mov    %rax,%rcx
    18000736c:	call   0x18001c390
    180007371:	nop
    180007372:	add    $0x38,%rsp
    180007376:	ret
@@ -37039,15 +37039,15 @@
    1800073b4:	mov    %rcx,0x20(%rsp)
    1800073b9:	lea    0xe2709(%rip),%rdx        # 0x1800e9ac9
    1800073c0:	jmp    0x1800073de
    1800073c2:	add    $0x8,%rcx
    1800073c6:	mov    %rcx,0x30(%rsp)
    1800073cb:	lea    0xe274e(%rip),%rcx        # 0x1800e9b20
    1800073d2:	mov    %rcx,0x20(%rsp)
-   1800073d7:	lea    0xe271a(%rip),%rdx        # 0x1800e9af8
+   1800073d7:	lea    0xe26f3(%rip),%rdx        # 0x1800e9ad1
    1800073de:	lea    0x30(%rsp),%r9
    1800073e3:	mov    $0x8,%r8d
    1800073e9:	mov    %rax,%rcx
    1800073ec:	call   0x18001c390
    1800073f1:	nop
    1800073f2:	add    $0x38,%rsp
    1800073f6:	ret
@@ -292907,29 +292907,28 @@
    1800e9593:	addb   $0x0,(%rcx)
 	...
    1800e959e:	add    %al,(%rax)
    1800e95a0:	add    %eax,(%rax)
    1800e95a2:	add    %al,(%rax)
    1800e95a4:	add    %al,(%rax)
    1800e95a6:	add    %al,(%rax)
-   1800e95a8:	mov    $0xf4,%al
-   1800e95aa:	add    %eax,0x1(%rax)
-   1800e95b0:	loopne 0x1800e95ee
-   1800e95b2:	add    %al,0x1(%rax)
+   1800e95a8:	subb   $0x0,0x18001(%rbx)
+   1800e95af:	add    %ah,%al
+   1800e95b1:	cmp    $0x0,%al
+   1800e95b3:	addb   $0x0,(%rcx)
 	...
+   1800e95be:	add    %al,(%rax)
    1800e95c0:	add    %eax,(%rax)
    1800e95c2:	add    %al,(%rax)
    1800e95c4:	add    %al,(%rax)
    1800e95c6:	add    %al,(%rax)
-   1800e95c8:	subb   $0x0,0x18001(%rbx)
-   1800e95cf:	add    %al,0x3a(%rbx)
-   1800e95d2:	pop    %rsp
-   1800e95d3:	push   %rbp
-   1800e95d4:	jae    0x1800e963b
-   1800e95d6:	jb     0x1800e964b
+   1800e95c8:	mov    $0xf4,%al
+   1800e95ca:	add    %eax,0x1(%rax)
+   1800e95d0:	cmp    0x73(%r13,%r10,2),%bl
+   1800e95d5:	gs jb  0x1800e964b
    1800e95d8:	pop    %rsp
    1800e95d9:	jb     0x1800e9650
    1800e95db:	outsb  %ds:(%rsi),(%dx)
    1800e95dc:	outsb  %ds:(%rsi),(%dx)
    1800e95dd:	gs jb  0x1800e9641
    1800e95e0:	fs insl (%dx),%es:(%rdi)
    1800e95e2:	imul   $0x7261632e,0x5c(%rsi),%ebp
@@ -293019,20 +293018,18 @@
    1800e96c1:	add    %al,(%rax)
    1800e96c3:	add    %al,(%rax)
    1800e96c5:	add    %al,(%rax)
    1800e96c7:	add    %dh,(%rax)
    1800e96c9:	cs xor (%rsi),%ch
    1800e96cc:	xor    %ebp,0x68706c61(%rip)        # 0x1e87f0333
    1800e96d2:	(bad)
-   1800e96d3:	cs (bad)
-   1800e96d5:	add    %al,(%rax)
-   1800e96d7:	add    %cl,%al
-   1800e96d9:	xchg   %eax,%esi
-   1800e96da:	(bad)
-   1800e96db:	addb   $0x0,(%rcx)
+   1800e96d3:	cs cmp %al,(%rax)
+   1800e96d6:	add    %al,(%rax)
+   1800e96d8:	enter  $0xe96,$0x80
+   1800e96dc:	add    %eax,(%rax)
    1800e96de:	add    %al,(%rax)
    1800e96e0:	or     $0x0,%eax
    1800e96e5:	add    %al,(%rax)
    1800e96e7:	add    %dl,0x65(%rsi)
    1800e96ea:	jb     0x1800e975f
    1800e96ec:	imul   $0xa76203a,0x6e(%rdi),%ebp
    1800e96f3:	push   %rbx
@@ -293063,26 +293060,30 @@
    1800e9723:	addb   $0x0,(%rcx)
    1800e9726:	add    %al,(%rax)
    1800e9728:	add    %eax,(%rax)
    1800e972a:	add    %al,(%rax)
    1800e972c:	add    %al,(%rax)
    1800e972e:	add    %al,(%rax)
    1800e9730:	(bad)
-   1800e9731:	xor    $0x36,%al
-   1800e9733:	(bad)
-   1800e9734:	xor    $0x33323432,%eax
-   1800e9739:	movsxd (%rbx),%esi
-   1800e973b:	xor    %ah,0x31(%rsi,%rsi,1)
-   1800e973f:	movsxd 0x61(%rsi),%esp
-   1800e9742:	gs cmp %esi,%gs:(%rdx)
-   1800e9746:	xor    %bh,(%rax)
-   1800e9748:	xor    %ah,0x36(%rbp)
-   1800e974b:	xor    $0x31333661,%eax
-   1800e9750:	cmp    %ah,0x61(%rdx,%riz,2)
-   1800e9754:	movsxd 0x61(%rbx),%sp
+   1800e9731:	cmp    %esp,0x34(%rsi)
+   1800e9734:	xor    %bh,%fs:(%rax)
+   1800e9737:	cmp    %esp,0x64(%rcx)
+   1800e973a:	cmp    %dh,(%rdx)
+   1800e973c:	(bad)
+   1800e9742:	(bad)
+   1800e9744:	(bad)
+   1800e9745:	cmp    %esp,0x33(%rdx)
+   1800e9748:	(bad)
+   1800e9749:	xor    %ah,0x64(%rbx)
+   1800e974c:	data16 xor (%rax),%bh
+   1800e974f:	(bad)
+   1800e9750:	(bad)
+   1800e9751:	cmp    %si,(%rdx,%riz,2)
+   1800e9755:	(bad)
+   1800e9756:	xor    %esi,(%rcx)
    1800e9758:	xor    %dl,0x1800e(%rdi)
    1800e975e:	add    %al,(%rax)
    1800e9760:	sub    %al,(%rax)
    1800e9762:	add    %al,(%rax)
    1800e9764:	add    %al,(%rax)
    1800e9766:	add    %al,(%rax)
    1800e9768:	imul   $0x616e7265,0x74(%rsi),%ebp
@@ -293493,46 +293494,46 @@
    1800e9ac1:	outsb  %ds:(%rsi),(%dx)
    1800e9ac2:	(bad)
    1800e9ac3:	outsl  %ds:(%rsi),(%dx)
    1800e9ac4:	jne    0x1800e9b34
    1800e9ac6:	fs gs fs rex.RB js 0x1800e9b2f
    1800e9acc:	insb   (%dx),%es:(%rdi)
    1800e9acd:	jne    0x1800e9b33
-   1800e9acf:	gs add %al,%fs:(%rax)
-   1800e9ad3:	add    %al,(%rax)
-   1800e9ad5:	add    %al,(%rax)
-   1800e9ad7:	add    %ah,%al
-   1800e9ad9:	cmp    $0x0,%al
-   1800e9adb:	addb   $0x0,(%rcx)
-   1800e9ade:	add    %al,(%rax)
-   1800e9ae0:	or     %al,(%rax)
-   1800e9ae2:	add    %al,(%rax)
-   1800e9ae4:	add    %al,(%rax)
+   1800e9acf:	gs rex.WB outsb %fs:(%rsi),(%dx)
+   1800e9ad3:	movsxd 0x64(%rbp,%rsi,2),%ebp
+   1800e9ad7:	gs add %al,%fs:(%rax)
+   1800e9adb:	add    %al,(%rax)
+   1800e9add:	add    %al,(%rax)
+   1800e9adf:	add    %ah,%al
+   1800e9ae1:	cmp    $0x0,%al
+   1800e9ae3:	addb   $0x0,(%rcx)
    1800e9ae6:	add    %al,(%rax)
    1800e9ae8:	or     %al,(%rax)
    1800e9aea:	add    %al,(%rax)
    1800e9aec:	add    %al,(%rax)
    1800e9aee:	add    %al,(%rax)
-   1800e9af0:	mov    $0x6c,%al
-   1800e9af2:	add    %al,0x1(%rax)
-   1800e9af8:	rex.WB outsb %ds:(%rsi),(%dx)
-   1800e9afa:	movsxd 0x64(%rbp,%rsi,2),%ebp
-   1800e9afe:	gs fs loopne 0x1800e9b3e
+   1800e9af0:	or     %al,(%rax)
+   1800e9af2:	add    %al,(%rax)
+   1800e9af4:	add    %al,(%rax)
+   1800e9af6:	add    %al,(%rax)
+   1800e9af8:	lock imul $0xffffff80,(%rax),%eax
+   1800e9afc:	add    %eax,(%rax)
+   1800e9afe:	add    %al,(%rax)
+   1800e9b00:	loopne 0x1800e9b3e
    1800e9b02:	add    %al,0x1(%rax)
    1800e9b08:	or     %al,(%rax)
    1800e9b0a:	add    %al,(%rax)
    1800e9b0c:	add    %al,(%rax)
    1800e9b0e:	add    %al,(%rax)
    1800e9b10:	or     %al,(%rax)
    1800e9b12:	add    %al,(%rax)
    1800e9b14:	add    %al,(%rax)
    1800e9b16:	add    %al,(%rax)
-   1800e9b18:	lock imul $0xffffff80,(%rax),%eax
-   1800e9b1c:	add    %eax,(%rax)
-   1800e9b1e:	add    %al,(%rax)
+   1800e9b18:	mov    $0x6c,%al
+   1800e9b1a:	add    %al,0x1(%rax)
    1800e9b20:	loopne 0x1800e9b5e
    1800e9b22:	add    %al,0x1(%rax)
    1800e9b28:	or     %al,(%rax)
    1800e9b2a:	add    %al,(%rax)
    1800e9b2c:	add    %al,(%rax)
    1800e9b2e:	add    %al,(%rax)
    1800e9b30:	or     %al,(%rax)
@@ -322643,40 +322644,39 @@
    1800fbed8:	pop    %rax
    1800fbed9:	xchg   %eax,%esp
    1800fbeda:	(bad)
    1800fbedb:	addb   $0x0,(%rcx)
    1800fbede:	add    %al,(%rax)
    1800fbee0:	add    %al,(%rax)
    1800fbee2:	add    %al,(%rax)
-   1800fbee4:	ret    $0x80c9
-   1800fbee7:	add    %al,%fs:(%rax)
+   1800fbee4:	imul   $0x6484,%ecx,%esp
    1800fbeea:	add    %al,(%rax)
    1800fbeec:	add    (%rax),%al
    1800fbeee:	add    %al,(%rax)
    1800fbef0:	add    %al,%gs:(%rax)
    1800fbef3:	add    %ah,-0x5ffff03f(%rax)
    1800fbef9:	scas   %es:(%rdi),%eax
    1800fbefa:	sldt   (%rax)
    1800fbefd:	add    %al,(%rax)
-   1800fbeff:	add    %al,%dl
-   1800fbf01:	leave
-   1800fbf02:	andb   $0x0,0x0(%rax,%rax,1)
-   1800fbf07:	add    %cl,(%rax,%rax,1)
+   1800fbeff:	add    %ch,-0x1f(%rcx)
+   1800fbf02:	test   %ah,0x0(%rax,%rax,1)
+   1800fbf06:	add    %al,(%rax)
+   1800fbf08:	or     $0x0,%al
    1800fbf0a:	add    %al,(%rax)
    1800fbf0c:	adc    $0x0,%al
    1800fbf0e:	add    %al,(%rax)
    1800fbf10:	or     %al,%dl
    1800fbf12:	str    (%rax)
    1800fbf15:	mov    $0xf,%al
    1800fbf17:	add    %al,(%rax)
    1800fbf19:	add    %al,(%rax)
-   1800fbf1b:	add    %al,%dl
-   1800fbf1d:	leave
-   1800fbf1e:	andb   $0x0,0x0(%rax,%rax,1)
-   1800fbf23:	add    %cl,0x18000000(%rip)        # 0x1980fbf29
+   1800fbf1b:	add    %ch,-0x1f(%rcx)
+   1800fbf1e:	test   %ah,0x0(%rax,%rax,1)
+   1800fbf22:	add    %al,(%rax)
+   1800fbf24:	or     $0x18000000,%eax
    1800fbf29:	add    (%rax),%eax
    1800fbf2b:	add    %bl,(%rdx,%rax,8)
    1800fbf2e:	ltr    (%rax,%rsi,4)
    1800fbf32:	sldt   (%rax)
 	...
    1800fbf7d:	add    %al,(%rax)
    1800fbf7f:	add    %bl,-0x3b(%rax)
@@ -322863,23 +322863,24 @@
    1800fc190:	push   $0x8000e7d
    1800fc195:	add    %al,(%rax)
    1800fc197:	add    %al,-0x78(%rbp)
    1800fc19a:	(bad)
    1800fc19b:	add    %dl,0x52000000(%rdx)
    1800fc1a1:	push   %rbx
    1800fc1a2:	rex.R push %rbx
-   1800fc1a4:	mov    %esp,%ebp
-   1800fc1a6:	loopne 0x1800fc14c
-   1800fc1a8:	rcrl   $0x69,0xcaf4338(%rbp)
-   1800fc1af:	(bad)
-   1800fc1b0:	xor    (%rbx),%ecx
-   1800fc1b2:	rex.WX (bad)
-   1800fc1b4:	add    %eax,(%rax)
-   1800fc1b6:	add    %al,(%rax)
-   1800fc1b8:	cmp    0x5c(%rcx,%riz,2),%r11b
+   1800fc1a4:	je     0x1800fc19e
+   1800fc1a6:	idivl  (%rsp,%rax,2)
+   1800fc1a9:	int    $0xd2
+   1800fc1ab:	test   %r11b,-0x37(%r15)
+   1800fc1af:	xchg   %eax,%esp
+   1800fc1b0:	jae    0x1800fc207
+   1800fc1b2:	test   $0x18d,%eax
+   1800fc1b7:	add    %al,0x5c(%rdx,%rdi,1)
+   1800fc1bb:	(bad)
+   1800fc1bc:	pop    %rsp
    1800fc1bd:	jae    0x1800fc230
    1800fc1bf:	insb   (%dx),%es:(%rdi)
    1800fc1c0:	imul   $0x74736166,0x2d(%rbp,%riz,2),%esi
    1800fc1c8:	jb     0x1800fc22b
    1800fc1ca:	outsb  %ds:(%rsi),(%dx)
    1800fc1cb:	fs pop %rsp
    1800fc1cd:	jae    0x1800fc240
@@ -323273,17 +323274,16 @@
    1800fc598:	or     %al,(%rax)
 	...
    1800fc5ce:	add    %al,(%rax)
    1800fc5d0:	sbb    %edx,(%rdx)
    1800fc5d2:	(bad)
    1800fc5d3:	test   %edx,(%rdx)
    1800fc5d5:	add    (%rdx),%ecx
-   1800fc5d7:	add    %edx,(%rdx)
-   1800fc5d9:	add    %al,(%rbx)
-   1800fc5db:	jo     0x1800fc5df
+   1800fc5d7:	add    %edx,(%rax,%rax,1)
+   1800fc5da:	add    0x2(%rax),%esi
    1800fc5dd:	(bad)
    1800fc5de:	add    %edx,-0x10(%rax)
    1800fc5e1:	jl     0x1800fc5f1
    1800fc5e3:	add    %dh,%ah
    1800fc5e5:	(bad)
    1800fc5e8:	add    %edx,(%rbx)
    1800fc5ea:	add    $0x0,%al
@@ -323298,41 +323298,40 @@
    1800fc5fe:	sldt   (%rax)
    1800fc601:	add    %al,(%rax)
    1800fc603:	add    %al,(%rax)
    1800fc605:	add    %al,(%rax)
    1800fc607:	add    %al,(%rbx)
    1800fc609:	add    %al,(%rax)
    1800fc60b:	add    %ah,(%rsi,%rax,8)
-   1800fc60e:	str    0x0(%rax)
+   1800fc60e:	ltr    0x0(%rax)
    1800fc615:	add    %al,(%rax)
    1800fc617:	add    %al,(%rcx)
    1800fc619:	add    %al,(%rax)
    1800fc61b:	add    %bh,%bh
    1800fc61d:	(bad)
    1800fc61e:	(bad)
-   1800fc61f:	incl   0x11(%rax)
+   1800fc61f:	call   *0x11(%rax)
    1800fc622:	add    %al,(%rax)
    1800fc624:	add    %dl,(%rax)
    1800fc626:	add    %al,(%rax)
    1800fc628:	(bad)
    1800fc629:	(bad)
    1800fc62a:	(bad)
-   1800fc62b:	lcall  *0x0(%rax,%rdx,1)
-   1800fc632:	add    %al,(%rax)
-   1800fc634:	test   $0x10,%al
-   1800fc636:	add    %al,(%rax)
-   1800fc638:	(bad)
+   1800fc62b:	ljmp   *0x10(%rbx)
+   1800fc631:	add    %al,(%rax)
+   1800fc633:	add    %dh,-0xfffff0(%rdi)
    1800fc639:	(bad)
    1800fc63a:	(bad)
    1800fc63b:	lcall  *(%rcx)
    1800fc63d:	adc    (%rsi),%al
    1800fc63f:	test   %edx,(%rdx)
    1800fc641:	add    (%rdx),%ecx
-   1800fc643:	add    %edx,(%rax,%rax,1)
-   1800fc646:	add    0x2(%rax),%esi
+   1800fc643:	add    %edx,(%rdx)
+   1800fc645:	add    %al,(%rbx)
+   1800fc647:	jo     0x1800fc64b
    1800fc649:	(bad)
    1800fc64a:	add    %edx,-0x10(%rax)
    1800fc64d:	jl     0x1800fc65d
    1800fc64f:	add    %ah,-0x3a(%rax)
    1800fc652:	sldt   (%rcx)
    1800fc655:	adc    (%rax,%rax,1),%eax
    1800fc658:	or     $0x32,%al
@@ -323345,37 +323344,35 @@
    1800fc668:	mov    %al,%dh
    1800fc66a:	sldt   (%rax)
    1800fc66d:	add    %al,(%rax)
    1800fc66f:	add    %al,(%rax)
    1800fc671:	add    %al,(%rax)
    1800fc673:	add    %al,(%rbx)
    1800fc675:	add    %al,(%rax)
-   1800fc677:	add    %dl,-0x67fff03a(%rax)
+   1800fc677:	add    %dl,-0x77fff03a(%rax)
    1800fc67d:	add    %al,(%rax)
    1800fc67f:	add    %al,(%rax)
    1800fc681:	add    %al,(%rax)
    1800fc683:	add    %al,(%rcx)
    1800fc685:	add    %al,(%rax)
    1800fc687:	add    %bh,%bh
    1800fc689:	(bad)
    1800fc68a:	(bad)
    1800fc68b:	inc    %eax
    1800fc68d:	adc    (%rax),%al
-   1800fc68f:	add    %dh,0x11(%rax)
-   1800fc692:	add    %al,(%rax)
-   1800fc694:	(bad)
+   1800fc68f:	add    %al,-0xffffef(%rax)
    1800fc695:	(bad)
    1800fc696:	(bad)
-   1800fc697:	lcall  *(%rbx)
-   1800fc699:	adc    (%rax),%al
-   1800fc69b:	add    %al,(%rax)
-   1800fc69d:	add    %al,(%rax)
-   1800fc69f:	add    %ah,(%rdi)
-   1800fc6a1:	adc    (%rax),%al
-   1800fc6a3:	add    %bh,%bh
+   1800fc697:	lcall  *(%rdx,%rdx,1)
+   1800fc69a:	add    %al,(%rax)
+   1800fc69c:	add    %al,(%rax)
+   1800fc69e:	add    %al,(%rax)
+   1800fc6a0:	sub    %dl,(%rdx)
+   1800fc6a2:	add    %al,(%rax)
+   1800fc6a4:	(bad)
    1800fc6a5:	(bad)
    1800fc6a6:	(bad)
    1800fc6a7:	lcall  *(%rcx)
    1800fc6a9:	adc    $0x3158508,%eax
    1800fc6ae:	or     $0x6001201,%eax
    1800fc6b3:	xor    %al,0x3600470(%rip)        # 0x1836fcb29
    1800fc6b9:	loopne 0x1800fc6bc
@@ -351312,24 +351309,24 @@
 	...
 
 Disassembly of section .pdata:
 
 0000000180111000 <.pdata>:
    180111000:	add    %dl,(%rax)
    180111002:	add    %al,(%rax)
-   180111004:	(bad)
-   180111005:	adc    %eax,(%rax)
+   180111004:	rex.RX adc %r8d,(%rax)
    180111007:	add    %dl,%al
    180111009:	(bad)
-   18011100c:	rex adc %eax,(%rax)
-   18011100f:	add    %ch,0x11(%rcx)
+   18011100c:	push   %rax
+   18011100d:	adc    %eax,(%rax)
+   18011100f:	add    %bh,0x11(%rcx)
    180111012:	add    %al,(%rax)
-   180111014:	call   0x1f0111fde
+   180111014:	call   0x100111fde
    180111019:	adc    %eax,(%rax)
-   18011101b:	add    %dh,0x3c000012(%rsi)
+   18011101b:	add    %dh,0x3c000012(%rdi)
    180111021:	(bad)
    180111022:	sldt   %eax
    180111025:	adc    (%rax),%al
    180111027:	add    %ch,%cl
    180111029:	adc    (%rax),%al
    18011102b:	add    %dl,0xf(%rsi,%rax,8)
    18011102f:	add    %dh,%al
@@ -366574,15 +366571,15 @@
    18011b03a:	adc    %ah,-0x58a758e0(%rdi)
    18011b040:	test   $0xa7,%al
    18011b042:	fsubs  -0x567f57c8(%rdi)
    18011b048:	nop
    18011b049:	stos   %al,%es:(%rdi)
    18011b04a:	test   $0xaa,%al
    18011b04c:	mov    $0xaa,%al
-   18011b04e:	mov    $0xf0aad8aa,%eax
+   18011b04e:	mov    $0xf8aae0aa,%eax
    18011b053:	stos   %al,%es:(%rdi)
    18011b054:	add    %ch,-0x54df54e8(%rbx)
    18011b05a:	cmp    %ch,-0x53cf5490(%rbx)
    18011b060:	add    %ch,-0x52cf52e8(%rbp)
    18011b066:	lods   %ds:(%rsi),%rax
    18011b068:	(bad)
    18011b069:	lods   %ds:(%rsi),%eax
```

## sqlite_fastrand/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.7"
+__version__ = "0.2.1-alpha.8"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_fastrand-0.2.1a7.dist-info/METADATA` & `sqlite_fastrand-0.2.1a8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-fastrand
-Version: 0.2.1a7
+Version: 0.2.1a8
 Home-page: https://github.com/asg017/sqlite-fastrand
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-fastrand/issues
 Project-URL: CI, https://github.com/asg017/sqlite-fastrand/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-fastrand/releases
 Requires-Python: >=3.7
```

