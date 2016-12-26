# HW-Calc
Dr. Memory version 1.11.0 build 2 built on Aug 29 2016 02:42:07
Dr. Memory results for pid 6500: "exe.exe"
Application cmdline: "exe.exe"
Recorded 115 suppression(s) from default C:\Program Files (x86)\Dr. Memory\bin\suppress-default.txt

WARNING: application is missing line number information.
Re-compile with the -ggdb flag to include DWARF2 line numbers.

Error #1: LEAK 2 direct bytes 0x00be0c90-0x00be0c92 + 0 indirect bytes
# 0 replace_malloc                            [d:\drmemory_package\common\alloc_replace.c:2576]
# 1 msvcrt.dll!_strdup   
# 2 .text  
# 3 __mingw_glob
# 4 _setargv
# 5 .text  
# 6 ntdll.dll!RtlInitializeExceptionChain    +0x62     (0x778992b2 <ntdll.dll+0x392b2>)
# 7 ntdll.dll!RtlInitializeExceptionChain    +0x35     (0x77899285 <ntdll.dll+0x39285>)

Error #2: LEAK 12 direct bytes 0x00c10d08-0x00c10d14 + 40332 indirect bytes
# 0 replace_malloc               [d:\drmemory_package\common\alloc_replace.c:2576]
# 1 init   
# 2 getList
# 3 main   

Error #3: LEAK 12 direct bytes 0x00c38338-0x00c38344 + 8784 indirect bytes
# 0 replace_malloc               [d:\drmemory_package\common\alloc_replace.c:2576]
# 1 NLInit 
# 2 addFront
# 3 getList
# 4 main   

Error #4: LEAK 12 direct bytes 0x00c40d08-0x00c40d14 + 0 indirect bytes
# 0 replace_malloc               [d:\drmemory_package\common\alloc_replace.c:2576]
# 1 init   
# 2 man_oper
# 3 main   

===========================================================================
FINAL SUMMARY:

DUPLICATE ERROR COUNTS:

SUPPRESSIONS USED:

ERRORS FOUND:
      0 unique,     0 total unaddressable access(es)
      0 unique,     0 total uninitialized access(es)
      0 unique,     0 total invalid heap argument(s)
      0 unique,     0 total GDI usage error(s)
      0 unique,     0 total handle leak(s)
      0 unique,     0 total warning(s)
      4 unique,     4 total,  49154 byte(s) of leak(s)
      0 unique,     0 total,      0 byte(s) of possible leak(s)
ERRORS IGNORED:
      3 potential error(s) (suspected false positives)
         (details: C:\Users\1\AppData\Roaming\Dr. Memory\DrMemory-exe.exe.6500.000\potential_errors.txt)
     13 unique,  4105 total,  53552 byte(s) of still-reachable allocation(s)
         (re-run with "-show_reachable" for details)
Details: C:\Users\1\AppData\Roaming\Dr. Memory\DrMemory-exe.exe.6500.000\results.txt
