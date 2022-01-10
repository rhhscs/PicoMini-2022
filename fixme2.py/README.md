# fixme2.py
Tags: General Skills, Python  
Author: LT 'syreal' Jones
## Description
Fix the syntax error in the Python script to print the flag.  
[Download Python script](./fixme2.py)
## Hints
1. Are equality and assignment the same symbol?
1. To view the file in the webshell, do: `$ nano fixme2.py`
1. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
The first hint gives us a good idea of what we're looking for. Equality checks in Python use `==` while assignments use `=`. After scanning the code, we see line 22 and the comment above it saying `# Check that flag is not empty`. `if flag = ""` will make the flag equal to "" thus making a tauntology. To fix this, we use `==` instead of `=` and the resulting code is [here](./fixedme2.py).
## Flag
picoCTF{3qu4l1ty_n0t_4551gnm3nt_b4d595d9}