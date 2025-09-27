# An Epic Filesystem Quest

### In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it! Here's how it'll work:

Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!

**Flag:** `pwn.college{EvSR2EHwMZxBm98-bZ2WoN_s5cO.QX5IDO0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SPOILER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat SPOILER
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/sphinx/texinputs_win

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/lib/python3/dist-packages/sphinx/texinputs_win
Makefile_t
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/lib/python3/dist-packages/sphinx/texinputs_win -a
.  ..  .DOSSIER  Makefile_t
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/sphinx/texinputs_win/.DOSSIER
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/logread

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/busybox/busybox-1.33.2/include/config/feature/logread
cat: /opt/busybox/busybox-1.33.2/include/config/feature/logread: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/busybox/busybox-1.33.2/include/config/feature/logread
WHISPER  reduced
hacker@commands~an-epic-filesystem-quest:/$ /opt/busybox/busybox-1.33.2/include/config/feature/logread/WHISPER
bash: /opt/busybox/busybox-1.33.2/include/config/feature/logread/WHISPER: Permission denied
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/busybox/busybox-1.33.2/include/config/feature/logread/WHISPER
cat: /opt/busybox/busybox-1.33.2/include/config/feature/logread/WHISPER: Permission denied
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/busybox/busybox-1.33.2/include/config/feature/logread
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ cat WHISPER
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/mips/lib

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ ls /opt/linux/linux-5.4/arch/mips/lib -a
.         Makefile   bswapsi.c       dump_tlb.c    libgcc.h  mips-atomic.c   strncpy_user.S
..        bitops.c   csum_partial.S  iomap-pci.c   memcpy.S  multi3.c        strnlen_user.S
.POINTER  bswapdi.c  delay.c         iomap_copy.c  memset.S  r3k_dump_tlb.c  uncached.c
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ cat /opt/linux/linux-5.4/arch/mips/lib/.POINTER
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/tools/arch/ia64

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ la /opt/linux/linux-5.4/tools/arch/ia64 -a
bash: la: command not found
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ ls /opt/linux/linux-5.4/tools/arch/ia64 -a
.  ..  .ALERT  include
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ cat /opt/linux/linux-5.4/tools/arch/ia64/.ALERT
Lucky listing!
The next clue is in: /usr/share/gap/pkg/AtlasRep

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread$ cd /usr/share/gap/pkg/AtlasRep
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ ls
INFO  PackageInfo.g  bibl  datagens  dataword  doc  etc  gap  init.g  read.g
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ cat INFO
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/net/ethernet/atheros/alx

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ ls /opt/linux/linux-5.4/drivers/net/ethernet/atheros/alx
LEAD-TRAPPED  Makefile  alx.h  ethtool.c  hw.c  hw.h  main.c  reg.h
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ cat /opt/linux/linux-5.4/drivers/net/ethernet/atheros/alx/LEAD-TRAPPED
Tubular find!
The next clue is in: /opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/protocols

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ ls /opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/protocols -a
.  ..  NOTE-TRAPPED  __init__.py  __pycache__  adb
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ cat /opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/protocols/NOTE-TRAPPED
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/Documentation/firmware-guide/acpi/dsd
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ ls /opt/linux/linux-5.4/Documentation/firmware-guide/acpi/dsd
MEMO  data-node-references.rst  graph.rst  leds.rst
hacker@commands~an-epic-filesystem-quest:/usr/share/gap/pkg/AtlasRep$ cat /opt/linux/linux-5.4/Documentation/firmware-guide/acpi/dsd/MEMO
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{EvSR2EHwMZxBm98-bZ2WoN_s5cO.QX5IDO0wSO4gjNzEzW}
```

## What I learned

I practiced cd, ls, cat commands to get the flag

## References

NA
