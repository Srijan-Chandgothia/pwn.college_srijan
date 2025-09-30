# Process Substitution for Input

### Now for your challenge! Recall what you learned in the diff challenge from Comprehending Commands. In that challenge, you diffed two files. Now, you'll diff two sets of command outputs: /challenge/print_decoys, which will print a bunch of decoy flags, and /challenge/print_decoys_and_flag which will print those same decoys plus the real flag.

Use process substitution with diff to compare the outputs of these two programs and find your flag!

**Flag:** `pwn.college{MoKZTcDw69BFfgMWmDo1KR_nUwj.0lNwMDOxwSO4gjNzEzW}`

```
#!/bin/bash

hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
71a72
> pwn.college{MoKZTcDw69BFfgMWmDo1KR_nUwj.0lNwMDOxwSO4gjNzEzW}
```

## What I learned

I learnt process substitution for temporary files

## References

NA
