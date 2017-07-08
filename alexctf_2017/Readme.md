# AlexCTF: SC2: Cutie cat

**Category:** Scripting
**Points:** 150
**Solves:** 132
**Description:**

> yeah steganography challenges are the worst... that's why we got only ~~one
> ~~ two steganography challenges 
> Hint: It scripting because we need a python library to solve the challenge, one that is made in japan

## Write-up

We have this image :

![](https://github.com/medbenali/Write-up-Hacking-Challenges/blob/master/alexctf_2017/cat_with_secrets.png)

After reading the hint given we  search the python librairies made in [japan](https://pypi.python.org/pypi?%3Aaction=search&term=japanese)

We search the seteganography library in the page and we find this [library](https://pypi.python.org/pypi/steganography/0.1.1)

And we install it with the command `pip install steganography`

Now you should write a small script python : 

```python
from steganography.steganography import Steganography
print Steganography.decode("cat_with_secrets.png")
```

After running this [script](https://github.com/medbenali/Write-up-Hacking-Challenges/blob/master/alexctf_2017/script.py) we get the flag :

![](https://github.com/medbenali/Write-up-Hacking-Challenges/blob/master/alexctf_2017/flag.png)

 





