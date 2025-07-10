# Merge pwndbg and pwngdb

## Download pwndbg

space: ~/

$ https://github.com/pwndbg/pwndbg.git

$ cd ~/pwndbg

$ ./setup.sh

## Download pwngdb
$ https://github.com/scwuaptx/Pwngdb.git

$ cp ~/Pwngdb/.gdbinit ~/

then add source ~/pwndbg/gdbinit.py to .gdbinit
```
source ~/peda/peda.py
source ~/pwndbg/gdbinit.py
source ~/Pwngdb/pwngdb.py
source ~/Pwngdb/angelheap/gdbinit.py

define hook-run
python
import angelheap
angelheap.init_angelheap()
end
end
```


