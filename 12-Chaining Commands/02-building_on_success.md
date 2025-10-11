# Building on Success

### In this challenge, you need to chain the programs /challenge/first-success and /challenge/second using the && operator. Try running each command separately first to see what happens (which is that you will not get the flag). But if you chain them with &&, the flag will appear!

**Flag:** `pwn.college{k6qB_GEWtNgq2XDdVJh9swdDfrm.0lM0MDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@chaining~building-on-success:~$ /challenge/first-success
hacker@chaining~building-on-success:~$ /challenge/second
Error: /challenge/first-success must be successfully chained with
/challenge/second using &&
hacker@chaining~building-on-success:~$ /challenge/first-success && /challenge/second
Nice chaining! Flag: pwn.college{k6qB_GEWtNgq2XDdVJh9swdDfrm.0lM0MDOxwSO4gjNzEzW}
```

## What I learned

I learnt to chain commands using && where second command runs only if the first one succeeds

## References

NA
