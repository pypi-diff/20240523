# Comparing `tmp/systrack-0.4rc3.tar.gz` & `tmp/systrack-0.5rc1.tar.gz`

## Comparing `systrack-0.4rc3.tar` & `systrack-0.5rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 systrack-0.4rc3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/__init__.py
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/__main__.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/elf.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/kconfig.py
--rw-r--r--   0        0        0    27501 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/kconfig_options.py
--rw-r--r--   0        0        0    22002 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/kernel.py
--rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/location.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/output.py
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/signature.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/syscall.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/type_hints.py
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/utils.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/version.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/all.py
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/arch_base.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/arm.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/arm64.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/mips.py
--rw-r--r--   0        0        0    13556 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/powerpc.py
--rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/arch/x86.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/templates/syscall_table.css
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/templates/syscall_table.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.4rc3/src/systrack/templates/syscall_table.js
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 systrack-0.4rc3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.4rc3/LICENSE
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 systrack-0.4rc3/README.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 systrack-0.4rc3/pyproject.toml
--rw-r--r--   0        0        0    47677 2020-02-02 00:00:00.000000 systrack-0.4rc3/PKG-INFO
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 systrack-0.5rc1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/__init__.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/__main__.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/elf.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kconfig.py
+-rw-r--r--   0        0        0    27501 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kconfig_options.py
+-rw-r--r--   0        0        0    23039 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/kernel.py
+-rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/location.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/output.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/signature.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/syscall.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/type_hints.py
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/utils.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/version.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/all.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arch_base.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arm.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/arm64.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/mips.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/powerpc.py
+-rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/arch/x86.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.css
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.5rc1/src/systrack/templates/syscall_table.js
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 systrack-0.5rc1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.5rc1/LICENSE
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 systrack-0.5rc1/README.md
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 systrack-0.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 systrack-0.5rc1/PKG-INFO
```

### Comparing `systrack-0.4rc3/src/systrack/__main__.py` & `systrack-0.5rc1/src/systrack/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	return '\n'.join(tx.fill(line) for line in body.splitlines() if line.strip())
 
 def parse_args() -> argparse.Namespace:
 	'''Parse and partially validate command line arguments through argparse.
 	'''
 	ap = argparse.ArgumentParser(
 		prog='systrack',
-		usage=f'systrack [OPTIONS...] [VMLINUX]',
+		usage='systrack [OPTIONS...] [VMLINUX]',
 		description='Analyze a Linux kernel image and extract information about implemented syscalls',
 		formatter_class=argparse.RawTextHelpFormatter
 	)
 
 	ap.add_argument('vmlinux', metavar='VMLINUX', nargs='?',
 		help=wrap_help('path to vmlinux, if not inside KDIR or no KDIR supplied'))
 	ap.add_argument('-k', '--kdir', metavar='KDIR',
@@ -261,15 +261,15 @@
 
 	if not vmlinux.is_file():
 		eprint(f'Unable to find vmlinux at "{vmlinux}".')
 		eprint('Build the kernel or provide a valid path.')
 		return 1
 
 	if not command_available('readelf'):
-		eprint(f'Command "readelf" unavailable, can\'t do much without it!')
+		eprint('Command "readelf" unavailable, can\'t do much without it!')
 		return 127
 
 	kernel = instantiate_kernel(arch_name, vmlinux, kdir, outdir, rdir)
 	eprint('Detected kernel version:', kernel.version_str)
 
 	if args.checkout == 'auto':
 		assert kernel.version_source == 'vmlinux'
```

### Comparing `systrack-0.4rc3/src/systrack/elf.py` & `systrack-0.5rc1/src/systrack/elf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import re
 import sys
 
 from enum import IntEnum
+from functools import lru_cache
 from pathlib import Path
 from struct import unpack
 from operator import attrgetter
 from collections import namedtuple
 from typing import Union, Dict, Optional
 
 from .utils import ensure_command
@@ -167,15 +168,18 @@
 
 	def read_symbol(self, sym: Union[str,Symbol]) -> bytes:
 		if not isinstance(sym, Symbol):
 			sym = self.symbols[sym]
 
 		return self.vaddr_read(sym.real_vaddr, sym.size)
 
+	@lru_cache(maxsize=128)
 	def next_symbol(self, sym: Symbol) -> Optional[Symbol]:
-		'''Find and return the first symbol whose .vaddr is higher than sym.'''
-		candidates = filter(lambda s: s.vaddr > sym.vaddr, self.symbols.values())
+		'''Find and return the symbol (if any) with the lowest real virtual
+		address higher than the one of sym.
+		'''
+		candidates = filter(lambda s: s.real_vaddr > sym.real_vaddr, self.symbols.values())
 
 		try:
 			return min(candidates, key=attrgetter('vaddr'))
 		except ValueError:
 			return None
```

### Comparing `systrack-0.4rc3/src/systrack/kconfig.py` & `systrack-0.5rc1/src/systrack/kconfig.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/kconfig_options.py` & `systrack-0.5rc1/src/systrack/kconfig_options.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/kernel.py` & `systrack-0.5rc1/src/systrack/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import struct
 import atexit
 from pathlib import Path
 from time import monotonic
 from os import sched_getaffinity
 from operator import itemgetter, attrgetter
 from collections import defaultdict, Counter
-from typing import Tuple, List, Iterator, Union, Any
+from typing import Tuple, List, Dict, Iterator, Union, Any
 
 from .arch import arch_from_name, arch_from_vmlinux
 from .elf import ELF, Symbol, Section
 from .kconfig import edit_config, edit_config_check_deps
 from .kconfig import kconfig_more_syscalls, kconfig_debugging
 from .kconfig import kconfig_compatibility, kconfig_syscall_deps
 from .location import extract_syscall_locations
@@ -231,39 +231,29 @@
 				cur_idx_vaddr += self.__long_size
 
 			logging.info('Syscall table seems to be %d bytes, %d entries',
 				cur_idx_vaddr - tbl.vaddr, len(vaddrs))
 
 		return vaddrs
 
-	def __extract_syscalls(self) -> List[Syscall]:
-		if self.arch.bits32 != self.vmlinux.bits32:
-			a, b = (32, 64) if self.arch.bits32 else (64, 32)
-			logging.critical('Selected arch is %d-bit, but kernel is %d-bit', a, b)
-			return []
-
-		self.arch.adjust_abi(self.vmlinux)
-		logging.debug('Arch: %r', self.arch)
-
-		syscall_table_name = self.arch.syscall_table_name
-		tbl = self.vmlinux.symbols.get(syscall_table_name)
-		ni_syscalls = set()
-
+	def __syscall_vaddrs_from_syscall_table(self) -> Dict[int,int]:
+		tbl = self.vmlinux.symbols.get(self.arch.syscall_table_name)
 		if not tbl:
-			logging.critical('Unable to find %s symbol!', syscall_table_name)
-			return []
+			logging.critical('Unable to find %s symbol!',
+				self.arch.syscall_table_name)
+			return {}
 
 		logging.debug('Syscall table: %r', tbl)
 
 		# Read and parse the syscall table unpacking all virtual addresses it
 		# contains. Depending on arch, we might need to parse function
 		# descriptors for the function pointers in the syscall table.
 
 		text   = self.vmlinux.sections['.text']
-		vaddrs = []
+		vaddrs = {}
 
 		if self.arch.uses_function_descriptors:
 			text_vstart = text.vaddr
 			text_vend   = text_vstart + text.size
 
 			# Even if this arch uses function descriptors, we don't know if they
 			# are effectively used for function pointers in the syscall table.
@@ -272,53 +262,80 @@
 			if not (text_vstart <= self.__unpack_long(tbl.vaddr) < text_vend):
 				logging.debug('Syscall table uses function descriptors')
 
 				opd = self.vmlinux.sections.get('.opd')
 				if not opd:
 					logging.critical('Arch uses function descriptors, but '
 						'vmlinux has no .opd section!')
-					return []
+					return {}
 
 				descriptors = self.__unpack_syscall_table(tbl, opd)
 
 				# Translate function descriptors (one more level of indirection)
-				for desc_vaddr in descriptors:
+				for i, desc_vaddr in enumerate(descriptors):
 					vaddr = self.vmlinux.vaddr_read(desc_vaddr, self.__long_size)
 					vaddr = struct.unpack(self.__long_pack_fmt, vaddr)[0]
 
 					if not (text_vstart <= vaddr < text_vend):
 						logging.warn('Function descriptor at 0x%x points '
 							'outside .text: something is off!', desc_vaddr)
 
-					vaddrs.append(vaddr)
+					vaddrs[i] = vaddr
 			else:
 				logging.debug('Syscall table does NOT use function descriptors')
 
 		if not vaddrs:
-			vaddrs = self.__unpack_syscall_table(tbl, text)
+			vaddrs = dict(enumerate(self.__unpack_syscall_table(tbl, text)))
 
 		if not vaddrs:
 			logging.critical('Could not extract any valid function pointer '
-				'from %s, giving up!', syscall_table_name)
+				'from %s, giving up!', self.arch.syscall_table_name)
 			logging.critical('Is the kernel relocatable? Relocation entries '
 				'for the syscall table are not supported.')
+			return {}
+
+		return vaddrs
+
+	def __extract_syscalls(self) -> List[Syscall]:
+		if self.arch.bits32 != self.vmlinux.bits32:
+			a, b = (32, 64) if self.arch.bits32 else (64, 32)
+			logging.critical('Selected arch is %d-bit, but kernel is %d-bit', a, b)
+			return []
+
+		self.arch.adjust_abi(self.vmlinux)
+		logging.debug('Arch: %r', self.arch)
+
+		have_syscall_table = self.arch.syscall_table_name is not None
+
+		if have_syscall_table:
+			vaddrs = self.__syscall_vaddrs_from_syscall_table()
+		else:
+			logging.warn('No syscall table available! Trying my best...')
+			vaddrs = self.arch.extract_syscall_vaddrs(self.vmlinux)
+
+		if not vaddrs:
+			logging.critical('Unable to extract any syscall vaddr, giving up!')
 			return []
 
 		# Find all ni_syscall symbols (there might be multiple) and keep track
 		# of them for later in order to detect non-implemented syscalls.
+		ni_syscalls = set()
+
 		for sym in self.vmlinux.functions.values():
 			if self.arch.symbol_is_ni_syscall(sym):
 				ni_syscalls.add(sym)
-				logging.debug('Found ni_syscall: %r', sym)
+
+		for sym in sorted(ni_syscalls, key=attrgetter('name')):
+			logging.debug('Found ni_syscall: %r', sym)
 
 		if not ni_syscalls:
 			logging.critical('No ni_syscall found!')
 			return []
 
-		seen = set(vaddrs)
+		seen = set(vaddrs.values())
 		symbols_by_vaddr = {sym.vaddr: sym for sym in ni_syscalls}
 		discarded_logs = []
 		preferred_logs = []
 
 		# Create a mapping vaddr -> symbol for every vaddr in the syscall table
 		# for convenience. Sort symbols by name to generate reproducible results
 		# and logs.
@@ -360,43 +377,56 @@
 			logging.critical('Unable to find any symbol in the syscall table, giving up!')
 			logging.critical('Is "%s" the correct arch/ABI combination for '
 				'this kernel?', self.arch_name)
 			return []
 
 		# Sanity check: the only repeated vaddrs in the syscall table should be
 		# the ones for *_ni_syscall. Warn in case there are others.
-		counts = sorted(Counter(vaddrs).items(), key=itemgetter(1), reverse=True)
-		best = symbols_by_vaddr[counts[0][0]]
-
-		if best not in ni_syscalls:
-			logging.error('Interesting! I was expecting *_ni_syscall to be the '
-				'most frequent symbol in the syscall table, but %s is ('
-				'appearing %d times).', best.name, counts[0][1])
-
-		for va, n in counts[1:]:
-			if n == 1:
-				break
-
-			logging.warn('Interesting! Vaddr 0x%x (%s) found %d times in %s',
-				va, symbols_by_vaddr.get(va, '<unknown>'), n, syscall_table_name)
+		counts = Counter(vaddrs.values()).items()
+		counts = filter(lambda c: c[1] > 1, counts)
+		counts = sorted(counts, key=itemgetter(1), reverse=True)
+
+		if counts:
+			# In case of no syscall table, ni_syscalls may have already been
+			# filtered by arch-specific extraction code, so don't sweat it.
+			if any(sym in ni_syscalls for sym in vaddrs.values()):
+				best = symbols_by_vaddr[counts[0][0]]
+
+				if best not in ni_syscalls:
+					logging.error('Interesting! I was expecting *_ni_syscall to be the '
+						'most frequent symbol in the syscall table, but %s is ('
+						'appearing %d times).', best.name, counts[0][1])
+
+		for va, n in counts:
+			sym = symbols_by_vaddr.get(va, f'{va:#x} <unknown symbol!>')
+			if sym not in ni_syscalls:
+				logging.warn('Interesting! Vaddr found %d times: %s', n, sym)
 
 		symbols      = []
 		symbol_names = []
 		ni_count     = defaultdict(int)
 
 		# Filter out only defined syscalls
-		for idx, vaddr in enumerate(vaddrs):
+		for idx, vaddr in sorted(vaddrs.items()):
 			sym = symbols_by_vaddr.get(vaddr)
 			if sym is None:
-				logging.error('Unable to find symbol for %s[%d]: 0x%x',
-					syscall_table_name, idx, vaddr)
+				if have_syscall_table:
+					logging.error('Unable to find symbol for %s[%d]: 0x%x',
+						self.arch.syscall_table_name, idx, vaddr)
+				else:
+					logging.error('Unable to find symbol for #%d 0x%x', idx,
+						vaddr)
 				continue
 
 			if high_verbosity():
-				logging.debug('%s[%d]: %s', syscall_table_name, idx, sym)
+				if have_syscall_table:
+					logging.debug('%s[%d]: %s', self.arch.syscall_table_name,
+						idx, sym)
+				else:
+					logging.debug('#%d: %s', idx, sym)
 
 			if sym in ni_syscalls:
 				ni_count[sym.name] += 1
 				continue
 
 			symbols.append((idx, sym))
 			symbol_names.append(sym.name)
@@ -431,15 +461,15 @@
 				n_skipped += 1
 				continue
 
 			syscalls.append(sc)
 
 		ni_total = 0
 		for name, n in sorted(ni_count.items(), key=itemgetter(1), reverse=True):
-			logging.info('%d syscall table entries point to %s', n, name)
+			logging.info('%d entries point to %s', n, name)
 			ni_total += n
 
 		# Add esoteric syscalls to the list, if any. These do not need any name
 		# translation or signature search. Some may need tailored static binary
 		# analysis. Very fun.
 		esoteric   = self.arch.extract_esoteric_syscalls(self.vmlinux)
 		n_esoteric = len(esoteric)
@@ -453,15 +483,15 @@
 			sym = self.vmlinux.symbols[sym_name]
 			syscalls.append(Syscall(None, num, name, name, sym, kconf, signature=sig, esoteric=True))
 
 		assert len(syscalls) == len(vaddrs) - ni_total - n_skipped + n_esoteric
 
 		# Some syscalls are just a dummy function that does `return -ENOSYS` or
 		# some other error, meaning that the syscall is not actually
-		# implemented, even if present inthe syscall table. We can filter those
+		# implemented, even if present in the syscall table. We can filter those
 		# out on archs for which we have .is_dummy_syscall() implemented, but
 		# we're not guaranteed to catch everything. For example,
 		# .is_dummy_syscall() may be useless if the symbol has bad/zero size or
 		# if the compiler does something funny and uses weird instructions.
 		# Unless we check sources, we can always have false positives even after
 		# this step.
 		#
```

### Comparing `systrack-0.4rc3/src/systrack/location.py` & `systrack-0.5rc1/src/systrack/location.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/output.py` & `systrack-0.5rc1/src/systrack/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	table    = [(
 		'INDEX', 'NUMBER', 'NAME', 'ORIG NAME', 'SYMBOL', 'LOCATION', 'KCONFIG',
 		'SIGNATURE'
 	)]
 
 	for sc in syscalls:
 		if sc.number - prevnum > 1:
-			# Blank line to separate groups of congiguous syscall numbers
+			# Blank line to separate groups of contiguous syscall numbers
 			table.append(None)
 
 		prevnum = sc.number
 
 		if sc.file and sc.line:
 			loc = f'{sc.file}:{sc.line}'
 		elif sc.file:
```

### Comparing `systrack-0.4rc3/src/systrack/signature.py` & `systrack-0.5rc1/src/systrack/signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,57 +64,62 @@
 		nargs = int(sig[0])
 		assert nargs <= 6, f'SYSCALL_DEFINE{nargs}? {file}:{line}'
 
 		if start == 0:
 			assert nargs == 0, f'Expected {nargs} arguments, but found 0: {file}:{line}'
 			return () # no arguments
 
-		sig = sig[start:sig.rfind(')')].replace(' __user', '')
+		sig = sig[start:sig.rfind(')')]
+		# Remove __user annotation, collapse multiple spaces into one and remove
+		# spaces between double pointers
+		sig = ' '.join(sig.replace(' __user', '').split()).replace('* *', '**')
 		sig = parse_signature(sig, big_endian)
 
 		assert len(sig) % 2 == 0 and len(sig) // 2 == nargs, f'Bad signature after parsing: {file}:{line}'
 		sig = tuple(f'{t}{" " * (t[-1] != "*")}{n}' for t, n in zip(sig[::2], sig[1::2]))
 	elif sig.startswith('asmlinkage'):
 		start = sig.find('(') + 1
-		sig = sig[start:sig.rfind(')')].replace(' __user', '').strip()
+		sig = sig[start:sig.rfind(')')].strip()
 		if not sig or sig == 'void':
 			return () # no arguments
 
+		# Remove __user annotation, collapse multiple spaces into one and remove
+		# spaces between asterisks of pointers
+		sig = ' '.join(sig.replace(' __user', '').split()).replace('* *', '**')
+
 		# We are assuming macros like arg_u32p are only used for SYSCALL_DEFINEx
 		assert '(' not in sig and ')' not in sig, f'Unexpected parentheses in signature: {file}:{line}'
 		sig = tuple(map(str.strip, sig.split(',')))
 		assert len(sig) <= 7, f'Syscall with {len(sig)} arguments? {file}:{line}'
 	else:
 		logging.error("This doesn't look like a syscall signature: %s:%d", file, line)
 		return None
 
 	return sig
 
 def extract_syscall_signatures(syscalls: List[Syscall], vmlinux: ELF, have_source: bool):
-	res = []
-	meta = {}
 	have_syscall_metadata = '__start_syscalls_metadata' in vmlinux.symbols
-	all_from_ftrace = False
+	meta = {}
+	res = []
 
-	# TODO: we could also extract signatures from DWARF or BTF even if we have
-	# no ftrace metadata and no KDIR. How?
+	# TODO: could we also extract signatures from DWARF or BTF even if we have
+	# no ftrace metadata and no KDIR? How?
 
 	# First extract signatures from ftrace metadata. If the kernel was compiled
 	# with CONFIG_FTRACE_SYSCALLS=y we have signature information available in a
 	# bunch of `struct syscall_metadata` objects.
 	if have_syscall_metadata:
 		logging.info('Kernel has ftrace syscall metadata from FTRACE_SYSCALLS=y')
 
 		start    = vmlinux.symbols['__start_syscalls_metadata'].real_vaddr
 		stop     = vmlinux.symbols['__stop_syscalls_metadata'].real_vaddr
 		ptr_fmt  = '<>'[vmlinux.big_endian] + 'QL'[vmlinux.bits32]
 		meta_fmt = '<>'[vmlinux.big_endian] + ('QllQQ', 'LllLL')[vmlinux.bits32]
 		ptr_sz   = 4 if vmlinux.bits32 else 8
 		meta_sz  = 8 + 3 * ptr_sz
-		endian   = 'big' if vmlinux.big_endian else 'little'
 		ptrs     = map(itemgetter(0), iter_unpack(ptr_fmt, vmlinux.vaddr_read(start, stop - start)))
 
 		# Sanity check
 		open_meta = vmlinux.symbols.get('__syscall_meta__open')
 		if open_meta and open_meta.size:
 			assert open_meta.size >= meta_sz
 
@@ -129,14 +134,16 @@
 			sig = []
 
 			for i in range(nargs):
 				typ = unpack(ptr_fmt, vmlinux.vaddr_read(types + i * ptr_sz, ptr_sz))[0]
 				arg = unpack(ptr_fmt, vmlinux.vaddr_read(args + i * ptr_sz, ptr_sz))[0]
 				typ = vmlinux.vaddr_read_string(typ).strip()
 				arg = vmlinux.vaddr_read_string(arg).strip()
+				# Double pointers can have spaces between asterisks
+				typ = typ.replace('* *', '**')
 				sig.append(f'{typ}{" " * (typ[-1] != "*")}{arg}')
 
 			meta[name] = tuple(sig)
 	else:
 		logging.info('Kernel DOES NOT have ftrace syscall metadata')
 
 	# Now extract signatures from the source code based on the location info we
@@ -154,18 +161,16 @@
 			if sig is None:
 				sig = meta.get(sc.name)
 				if sig is None:
 					logging.debug('Signature NOT found in ftrace metadata: %s', sc.name)
 					continue
 
 			sc.signature = sig
-
-			if not have_source:
-				logging.debug('Signature extracted from ftrace metadata: %s', sc.name)
+			logging.debug('Signature extracted from ftrace metadata: %s', sc.name)
 		else:
-			# Weird/bad location, no FTRACE_SYSCALLS metadata :(
+			# Weird/bad location and no FTRACE_SYSCALLS metadata :(
 			if sc.file is not None and sc.line is not None:
 				logging.debug('Signature extraction skipped: %s at %s:%d',
 					sc.name, sc.file, sc.line)
 
 	return res
```

### Comparing `systrack-0.4rc3/src/systrack/syscall.py` & `systrack-0.5rc1/src/systrack/syscall.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/utils.py` & `systrack-0.5rc1/src/systrack/utils.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/arch/__init__.py` & `systrack-0.5rc1/src/systrack/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/arch/arch_base.py` & `systrack-0.5rc1/src/systrack/arch/arch_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from abc import ABC, abstractmethod
-from typing import Tuple, List, Type, Optional
+from typing import Tuple, List, Dict, Type, Optional
 
 from ..elf import Symbol, ELF
 from ..syscall import Syscall
 from ..type_hints import KernelVersion, EsotericSyscall
 from ..utils import VersionedDict, anysuffix, noprefix, nosuffix
 
 class Arch(ABC):
@@ -32,15 +32,15 @@
 	# Kernel version that we are intersted in analyzing
 	kernel_version: KernelVersion = None
 
 	# Make target to build for the base config
 	config_target: str = 'defconfig'
 
 	# Name of the syscall table symbol to look for
-	syscall_table_name: str = 'sys_call_table'
+	syscall_table_name: Optional[str] = 'sys_call_table'
 
 	# Base syscall number (actual syscall number is base + idx in syscall table)
 	# NOTE: easiest way to check this is to just compile a binary that makes a
 	# raw syscall for the right arch/ABI. The arch_syscall_addr() kernel
 	# function can also be useful to inspect.
 	syscall_num_base: int = 0
 
@@ -145,15 +145,19 @@
 		By default, also avoid ftrace-related _eil_addr_XXX symbols generated
 		with CONFIG_FTRACE_SYSCALLS=y.
 		'''
 		# This generic approach should be good enough
 		return (
 			sym.type == 'FUNC'
 			and anysuffix(sym.name, 'sys_ni_syscall', 'compat_ni_syscall')
+			# Avoid ftrace-related symbols
 			and not sym.name.startswith('_eil_addr_')
+			# Avoid KCFI-related symbols
+			and not sym.name.startswith('__cfi_')
+			and not sym.name.startswith('__pfx_')
 		)
 
 	def skip_syscall(self, sc: Syscall) -> bool:
 		'''Determine whether to skip this syscall.
 
 		Kernels compiled with support for multiple ABIs might share the same
 		syscall table between two or more ABIs, and in such case we want to
@@ -262,14 +266,22 @@
 	def adjust_syscall_number(self, number: int) -> int:
 		'''Adjust the number for the given syscall according to any
 		arch-specific quirk there might be (e.g. PowerPC with its interleaved
 		syscall numbers).
 		'''
 		return number
 
+	def extract_syscall_vaddrs(self, vmlinux: ELF) -> Dict[int,int]:
+		'''Extract virtual addresses of syscall functions. Implemented in case
+		this isn't just as simple as looking at the addresses in the syscall
+		table (e.g., there might not be one to begin with).
+		'''
+		logging.error("Sorry, don't know how to extract syscall vaddrs for this arch!")
+		return {}
+
 	def extract_esoteric_syscalls(self, vmlinux: ELF) -> EsotericSyscall:
 		'''Extract weird arch-specific syscalls not in the syscall table: there
 		isn't much else to do except either manually list these (if they are
 		always present) or perform static binary analysis.
 
 		The returned value is a list of tuples of the form: (number, name,
 		symbol_name, signature, kconfig_opts).
```

### Comparing `systrack-0.4rc3/src/systrack/arch/arm.py` & `systrack-0.5rc1/src/systrack/arch/arm.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/arch/arm64.py` & `systrack-0.5rc1/src/systrack/arch/arm64.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/arch/mips.py` & `systrack-0.5rc1/src/systrack/arch/mips.py`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/arch/powerpc.py` & `systrack-0.5rc1/src/systrack/arch/powerpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,15 @@
 
 			if 'spu_syscall_table' in vmlinux.symbols:
 				abis.append('spu')
 
 		return ArchPowerPC, vmlinux.bits32, abis
 
 	def matches(self, vmlinux: ELF) -> bool:
-		# Linux PPC 32-bit should be big-endian only, and  _dummy_syscall_code()
-		# below also relies on this
+		# Linux PPC 32-bit should be big-endian only
 		assert vmlinux.big_endian, 'Little-endian PowerPC 32-bit kernel? WAT'
 		return (
 			vmlinux.e_machine == (E_MACHINE.EM_PPC64, E_MACHINE.EM_PPC)[self.bits32]
 			and vmlinux.bits32 == self.bits32
 		)
 
 	def preferred_symbol(self, a: Symbol, b: Symbol) -> Symbol:
```

### Comparing `systrack-0.4rc3/src/systrack/templates/syscall_table.css` & `systrack-0.5rc1/src/systrack/templates/syscall_table.css`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/templates/syscall_table.html` & `systrack-0.5rc1/src/systrack/templates/syscall_table.html`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/src/systrack/templates/syscall_table.js` & `systrack-0.5rc1/src/systrack/templates/syscall_table.js`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/LICENSE` & `systrack-0.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `systrack-0.4rc3/README.md` & `systrack-0.5rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,45 +17,35 @@
 
 Systrack can configure and build kernels for all its supported architectures,
 and works best at analyzing kernels that it has configured and built by itself.
 
 Installation
 ------------
 
-Systrack is [available on PyPI][pypi-systrack], it requires Python 3.6+ and is
+Systrack is [available on PyPI][pypi-systrack], it requires Python 3.8+ and is
 installable through Pip:
 
 ```bash
-pip install systrack        # Base version with no dependencies
-pip install systrack[html]  # + HTML output support
+pip install systrack
 ```
 
 Building and installaing from source requires [`hatch`][pypi-hatch]:
 
 ```bash
 hatch build
-pip install dist/systrack-XXX.whl       # Base version with no dependencies
-pip install dist/systrack-XXX.whl[html] # + HTML output support
+pip install dist/systrack-XXX.whl
 ```
 
 Usage
 -----
 
 Systrack can mainly be used for two purposes: analyzing or building Linux
 kernels. For more detailed information, see `systrack --help`. For information
 about supported architecture/ABI combinations, see `systrack --arch help`.
 
-- **Building** can be done through the `--build` option. You will need to
-  provide a kernel source directory (`--kdir`) and an architecture/ABI
-  combination to build for (`--arch`).
-
-  ```none
-  systrack --build --kdir path/to/linux_git_repo --arch x86-64
-  ```
-
 - **Analyzing** a kernel image can be done given a `vmlinux` ELF with symbols,
   and optionally also a kernel source directory (`--kdir`). Systrack will
   extract information about implemented syscalls from the symbol table present
   in the given `vmlinux` ELF, and if debugging information is present, it will
   also extract file and line number information for syscall definitions.
   Supplying `--kdir` will help refine and/or correct the location of the
   definitions, pointing Systrack to the checked-out sources for the right kernel
@@ -64,34 +54,49 @@
   Systrack can guess the architecture and ABI to analyze, but if the given
   kernel was built for support for multiple ABIs, the right one can be selected
   through `--arch`.
 
   ```none
   systrack path/to/vmlinux
   systrack --format json path/to/vmlinux
+  systrack --format html path/to/vmlinux
   systrack --kdir path/to/linux_git_repo path/to/vmlinux
   systrack --kdir path/to/linux_git_repo --arch x86-64-ia32 path/to/vmlinux
   ```
 
+- **Building** can be done through the `--build` option. You will need to
+  provide a kernel source directory (`--kdir`) and an architecture/ABI
+  combination to build for (`--arch`).
+
+  ```none
+  systrack --build --kdir path/to/linux_git_repo --arch x86-64
+  ```
+
+  Cross-compilation is possible specifying the correct toolchain prefix with
+  the `--cross` option, which will set the `CROSS_COMPILE` variable for the
+  kernel's `Makefile`.
+
+  ```none
+  systrack --build --kdir path/to/linux_git_repo --arch arm64 --cross aarch64-linux-gnu-
+  ```
+
 Runtime dependencies
 --------------------
 
+External (non-Python) runtime dependencies are:
+
 - **Required**: `readelf` (from GNU binutils) is used to parse and extract ELF
   metadata such as symbols and sections. This is currently the only *compulsory*
   dependency for Systrack to work.
 - Optional: `addr2line` (from GNU binutils) is used to extract location
   information from DWARF debug info (if available). Without this program,
   Systrack will not output any information about syscall definition locations.
 - Optional: if available, the `rg` ([ripgrep][ripgrep]) command is used for much
   faster recursive grepping of syscall definition locations within kernel
   sources when needed. Otherwise, slower pure-Python code is used.
-- Optional: the `jinja2` Python package, which can be either installed
-  separately or automatically (`pip install systrack[html]`) is used to output
-  interactive HTML pages with a sortable table, links and more. This is the
-  richest output format (selectable with `--format html`).
 - Optional: a working compiler toolchain and
   [kernel build dependencies](https://www.kernel.org/doc/html/latest/process/changes.html)
   are obviously needed if you want Systrack to *build* kernels from source.
 
 Limitations
 -----------
 
@@ -102,15 +107,15 @@
   uncompress and unstrip kernel images, after which Systrack will be able to
   analyze them.
 - Old kernel versions: Systrack was mainly designed for and tested on modern
   kernels (>= v4.0) and has not been tested on older kernels. It should still
   *somewhat* work on older kernels, but without the same level of guarantee on
   the correctness of the output. Support for old kernels may come gradually in
   the future.
-- Relocatable kernel support: Systrack does not currently parse and apply ELF
+- Relocatable kernels: Systrack does not currently parse and apply ELF
   relocations. This means that Systrack does not support kernels using
   relocation entries for the syscall table. On some architectures (notably MIPS)
   if the kernel is relocatable the syscall table is relocated at startup and
   does not contain valid virtual addresses: Systrack will currently fail to
   analyze such kernels.
 
 ---
```

### Comparing `systrack-0.4rc3/pyproject.toml` & `systrack-0.5rc1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = 'systrack'
 description = 'Linux kernel syscall implementation tracker'
-authors = [{name = 'Marco Bonelli', email = 'marco@mebeim.net'}]
-maintainers = [{name = 'Marco Bonelli', email = 'marco@mebeim.net'}]
-license = {file = 'LICENSE'}
+authors = [{name = 'Marco Bonelli'}, {name = 'Marco Bonelli', email = 'marco@mebeim.net'}]
+maintainers = [{name = 'Marco Bonelli'}, {name = 'Marco Bonelli', email = 'marco@mebeim.net'}]
+license = {text = 'GNU General Public License v3 (GPLv3)'}
 readme = 'README.md'
 platforms = 'any'
-requires-python = '>=3.6'
+requires-python = '>=3.8'
 dynamic = ['version']
 keywords = ['systrack', 'linux', 'kernel', 'syscall', 'kconfig', 'elf', 'abi']
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'Environment :: Console',
 	'Intended Audience :: Developers',
 	'Intended Audience :: Science/Research',
@@ -21,26 +21,27 @@
 	'Programming Language :: Python :: 3',
 	'Topic :: Security',
 	'Topic :: Software Development :: Embedded Systems',
 	'Topic :: Software Development :: Testing',
 	'Topic :: System :: Operating System Kernels :: Linux',
 	'Topic :: Utilities',
 ]
+dependencies = [
+	'iced-x86~=1.21.0',
+	'jinja2~=3.1.2'
+]
 
 [project.urls]
-homepage = 'https://github.com/mebeim/systrack'
-repository = 'https://github.com/mebeim/systrack.git'
+Homepage = 'https://github.com/mebeim/systrack'
+Repository = 'https://github.com/mebeim/systrack.git'
+Changelog = 'https://github.com/mebeim/systrack.git/blob/master/CHANGELOG.md'
 
 [project.scripts]
 systrack = 'systrack.__main__:main'
 
-[project.optional-dependencies]
-full = ['jinja2']
-html = ['jinja2']
-
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [tool.hatch.version]
 path = 'src/systrack/version.py'
 
@@ -55,7 +56,16 @@
 include = ['src', 'CHANGELOG.md']
 
 [tool.hatch.envs.default]
 python = '3'
 
 [tool.hatch.envs.test]
 dependencies = ['pytest']
+
+[tool.ruff.lint]
+# Don't warn for multi-line statements
+ignore = ['E701']
+
+[tool.ruff.lint.per-file-ignores]
+# Don't warn for star imports in these files
+'arch/__init__.py' = ['E403']
+'tests/*' = ['E403']
```

