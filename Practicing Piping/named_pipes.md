# Named Pipes

### This challenge will be a simple introduction to FIFOs. You'll need to create a /tmp/flag_fifo file and redirect the stdout of /challenge/run to it. If you're successful, /challenge/run will write the flag into the FIFO! Go do it!

**Flag:** `pwn.college{wYEcv85hPT-_kxk0NfGzb0KPdUV.01MzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!

hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{wYEcv85hPT-_kxk0NfGzb0KPdUV.01MzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt about FIFOs (First (byte) In, First (byte) Out.)

## References

NA
