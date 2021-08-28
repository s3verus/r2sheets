# r2sheets
radare2 cheat sheet

install [radare2](https://github.com/radareorg/radare2):
> git clone https://github.com/radareorg/radare2
> radare2/sys/install.sh

install plugins:
> r2pm update               # initialize and update the package database
> r2pm install [pkg]        # installs the package

for example:
> r2pm install r2ghidra     #[r2ghidra](https://github.com/radareorg/r2ghidra) the native ghidra decompiler plugin: `pdg` command
