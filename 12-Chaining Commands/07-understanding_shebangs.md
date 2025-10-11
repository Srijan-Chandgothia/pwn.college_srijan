# Understanding Shebangs

### For this challenge, create a script at /home/hacker/solve.sh that has a proper shebang and outputs "hack the planet". Remember to make it executable, then run /challenge/run to verify your script works correctly!

**Flag:** `pwn.college{QBrLIEpOBxRxhGDURCx6WeF-EKn.0VOzMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~understanding-shebangs:~$ cat > /home/hacker/solve.sh
#!/bin/bash
echo "hack the planet"
^C
hacker@chaining~understanding-shebangs:~$ chmod a+x /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{QBrLIEpOBxRxhGDURCx6WeF-EKn.0VOzMDOxwSO4gjNzEzW}
```

## What I learned

I learnt about shebangs

## References

NA
