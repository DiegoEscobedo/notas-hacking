# Level 7
## Objetivo
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.
## Pistas
The `str_xor` function does not need to be reverse engineered for this challenge.
## Solucion
┌──(diego㉿kali)-[~]
└─$ python level1.py 
Please enter correct password for flag: xxx
That password is incorrect
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ nano level1.flag.txt.enc 
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ nano level1.py 
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ python level1.py                                           
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_fa343060}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias