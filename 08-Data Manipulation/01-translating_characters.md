# Translating Characters

### In this level, /challenge/run will print the flag but will swap the casing of all characters (e.g., A will become a and vice-versa). Can you undo it with tr and get the flag?

**Flag:** `pwn.college{YlMed6a5KucY0eMZ1LlB_luwdNT.01MxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@data~translating-characters:~$ /challenge/run | tr abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz
yOUR CASE-SWAPPED FLAG:
pwn.college{YlMed6a5KucY0eMZ1LlB_luwdNT.01MxEzNxwSO4gjNzEzW}
```

## What I learned

I learnt the translate 'tr' command

## References

NA
