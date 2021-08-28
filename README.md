# r2sheets
radare2 cheat sheet

install [radare2](https://github.com/radareorg/radare2):
```
git clone https://github.com/radareorg/radare2
radare2/sys/install.sh
```

install plugins:
```
r2pm init
r2pm update               # initialize and update the package database
r2pm install [pkg]        # installs the package
r2pm search name          # search for packages
```
for example:
> r2pm install r2ghidra     #[r2ghidra](https://github.com/radareorg/r2ghidra) the native ghidra decompiler plugin: `pdg` command

## quick start

run:<br>
~$: r2 ./file.bin

> Append '?' to any char command to get detailed help


Help or evaluate math expression:<br>
\[0x08048890\]> ? 0x16+6

Show info of current file:<br>
\[0x08048890\]> i

find Entrypoint:<br>
\[0x08048890\]> ie

Show main address:<br>
\[0x08048890\]> iM

Strings in data sections:<br>
\[0x08048890\]> iz

search for string 'foo':<br>
\[0x08048890\]> / foo

grep output of commands for search 'foo':<br>
\[0x08048890\]> i ~ foo

analysis:<br>
\[0x08048890\]> aaa

perform additional experimental analysis:<br>
\[0x08048890\]> aaaa

list functions:<br>
\[0x08048890\]> afl

Seek to address:<br>
\[0x08048890\]> s addr

disassemble N instructions:<br>
\[0x08048890\]> pd N

disassemble function:<br>
\[0x08048890\]> pdf

quit program:<br>
\[0x08048890\]> q

### debugging<br>
soon...<br>
### patching<br>
soon...<br>
### virtual mode<br>
soon...
