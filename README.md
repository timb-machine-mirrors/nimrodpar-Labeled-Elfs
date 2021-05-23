# Labeled-Elfs
A collection of well labeled ELF binaries compiled from benign and malicious code in various ways (various archs, compilers and opt levels). Great for exploring similarity in executables and training various ML models.

Here's an example of one of the filenames, containing detailed labeling:

`x86__64__lsb__unix-system-v__gcc-5.5.0__O0__no-obf__unstripped__coreutils-8.30__nice`

The structure is: 

`{Architecture}__{Bit width}__{Endianess}__{ABI}__{Compiler used to compile the exe}__{Optimization level}__{Whether obfuscation was applied}__{Is the file stripped of debug symbols}__{Package name}__{Program name}`

There are some obfuscated files which will by labeled by compilers named `llvm-obfuscator-3.6.1` etc. with the specific obfuscation applied e.g., `mllvmsub_mllvmbcf`. See https://github.com/obfuscator-llvm/obfuscator/wiki for more details on that.

The Malware is labeled with the following Package names:
1. Mirai-vanilla
2. BASHLITE-1.0
3. BASHLITE-lizkebab
4. lightaidra-1.0

The following are what you call "Hackware" meaning they are not Malware per say, but will be flagged by most AV engines:

5. pnscan  
  
Hope this is useful. 
