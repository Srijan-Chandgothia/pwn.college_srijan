# Deleting Characters

### I'll intersperse some decoy characters (specifically: ^ and %) among the flag characters. Use tr -d to remove them!
**Flag:** `pwn.college{wZMvVKj12nMfY7DGMn8X7_TJZoB.0FNxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{wZMvVKj12nMfY7DGMn8X7_TJZoB.0FNxEzNxwSO4gjNzEzW}
```

## What I learned

I learnt to delete characters using tr command with -d flag

## References

NA
