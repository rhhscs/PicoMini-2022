# Serpentine
Tags: General Skills, Python  
Author: LT 'syreal' Jones
## Description
Find the flag in the Python script!  
[Download Python script](./serpentine.py)
## Hints
1. Try running the script and see what happens
1. In the webshell, try examining the script with a text editor like `nano`
1. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
If we try running it and printing the flag from there, the program says "Oops! I must have misplaced the print_flag function! Check my source code!". On line 20, we see a function called `print_flag`, line 35 a function called `main` and line 79 and 80, 
```python
if __name__ == "__main__":
  main()
```
Essentially what this does is tell other readers that this code is meant to be run and that it runs the `main` function upon being run. What we want to do is print the flag so we can replace `main()` with `print_flag()`
```python
if __name__ == "__main__":
  print_flag()
```
## Flag
picoCTF{7h3_r04d_l355_7r4v3l3d_ae743140}