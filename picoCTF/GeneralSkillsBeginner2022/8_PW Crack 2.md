# Level 8
## Objetivo
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.v
## Pistas
Does that encoding look familiar?
## Solucion
┌──(diego㉿kali)-[~]
└─$ nano level2.flag.txt.enc 
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ nano level2.py 
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ python level2.py                                         
Please enter correct password for flag: asd
de76
That password is incorrect
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ python level2.py
Please enter correct password for flag: de76
de76
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}

(Agregue una linea que imprimiera el password)
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
