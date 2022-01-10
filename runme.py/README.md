# runme.py
Category: General Skills, Python  
Author: Sujeet Kumar
## Description
Run the `runme.py` script to get the flag. Download the script with your browser or with `wget` in the webshell.
## Hints
1. If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
1. To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
1. Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
1. Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 runme.py` You should have the flag now!  
[Download runme.py Python script](./runme.py)
## Approach
### Method 1
Read and follow the hints
### Method 2
If you open [runme.py](./runme.py) you'll see the code:
```python
#!/usr/bin/python3
################################################################################
# Python script which just prints the flag
################################################################################

flag ='picoCTF{run_s4n1ty_run}'
print(flag)
```
The first few lines are [comments](https://en.wikipedia.org/wiki/Comment_(computer_programming)) meaning the computer doesn't look at it. The lines the computer will look at are here:
```python
flag ='picoCTF{run_s4n1ty_run}'
print(flag)
```
`flag ='picoCTF{run_s4n1ty_run}'` will define a variable `flag` with the value "picoCTF{run_s4n1ty_run}". The next line `print(flag)` will print the value contained in flag, so "picoCTF{run_s4n1ty_run}".
## Flag
picoCTF{run_s4n1ty_run}