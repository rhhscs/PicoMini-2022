# fixme1.py
Tags: General Skills, Python  
Author: LT 'syreal' Jones
## Description
Fix the syntax error in this Python script to print the flag.  
[Download Python script](./fixme1.py)
## Hints
1. Indentation is very meaningful in Python
1. To view the file in the webshell, do: `$ nano fixme1.py`
1. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
If we look at [`fixme1.py`](./fixme1.py) we'll see there's an indent on line 20. Python cares about whitespace (spaces, tabs, newlines) and this extra tab is against Python syntax (rules). If we delete the tab we should get the same code as [this](./fixedme1.py). After running that, we can get the flag.
## Flag
picoCTF{1nd3nt1ty_cr1515_05a3c38c}