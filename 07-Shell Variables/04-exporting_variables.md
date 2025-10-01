# Exporting Variables

### In this challenge, you must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported (e.g., not inherited by /challenge/run). Good luck!

**Flag:** `pwn.college{EWJA3l4YOw0lql9yZ7jJ9-gVRsY.QXyYTN0wSO4gjNzEzW}`

```
#!/bin/bash

hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{EWJA3l4YOw0lql9yZ7jJ9-gVRsY.QXyYTN0wSO4gjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## What I learned

I learnt to export variables

## References

NA
