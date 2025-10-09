# Extracting Specific Sections of Text

### In this challenge, the /challenge/run program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use cut to extract the flag characters, then pipe them to tr -d "\n" (like the previous level!) to join them together into a single line. Your solution will look something like /challenge/run | cut ??? | tr ???, with the ??? filled out.

**Flag:** `pwn.college{4UdZ68gxEq3xPeTVpl7LOcQmtuK.01NxEzNxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{4UdZ68gxEq3xPeTVpl7LOcQmtuK.01NxEzNxwSO4gjNzEzW}
```

## What I learned

I learnt the cut command to extract specific columns of output

## References

NA
