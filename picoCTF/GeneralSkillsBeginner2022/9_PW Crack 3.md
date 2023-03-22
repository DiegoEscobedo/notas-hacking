# Level 9
## Objetivo
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
## Pistas
To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
## Solucion┌──(diego㉿kali)-[~]
└─$ bvi level3.hash.bin

bvi version 1.4.1 (C) GPL 1996-2019 by Gerhard Buergmann
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ python level3.py   
Please enter correct password for flag: .mU.]...R.>..W+{   
That password is incorrect
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ python level3.py
Please enter correct password for flag: .mU.]...R.>..W+{   
That password is incorrect
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ bvi level3.hash.bin 

bvi version 1.4.1 (C) GPL 1996-2019 by Gerhard Buergmann
                                                                                                        
┌──(diego㉿kali)-[~]
└─$ python level3.py   
Please enter correct password for flag: 87ab
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_cd6ed2eb}

transformamos el hashcode que habia en el archivo .bin pa usarlo como password
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|bvi|lee archivos .bin|
## Referencias
https://crackstation.net/