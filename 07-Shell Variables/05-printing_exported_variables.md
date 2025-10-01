# Printing Exported Variables

### Try the env command: it'll print out every exported variable set in your shell, and you can look through that output to find the FLAG variable!

**Flag:** `pwn.college{saauyW5l8r3Z1nTQMvgGFCmL5Jr.QX4UTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=5f6d33d72644106b87b8f0dbd4a8daee65b61472a562e59897cd9461e365367f
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{saauyW5l8r3Z1nTQMvgGFCmL5Jr.QX4UTN0wSO4gjNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## What I learned

I learnt to print every exported variables using the 'env' command

## References

NA
