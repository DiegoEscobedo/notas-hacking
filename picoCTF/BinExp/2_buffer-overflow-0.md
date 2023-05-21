# Level 2
## Objetivo
Smash the stackLet's start off simple, can you overflow the correct buffer? The program is available [here](https://artifacts.picoctf.net/c/172/vuln). You can view source [here](https://artifacts.picoctf.net/c/172/vuln.c). And connect with it using:`nc saturn.picoctf.net 63397`
## Pistas
How can you trigger the flag to print?
If you try to do the math by hand, maybe try and add a few more characters. Sometimes there are things you aren't expecting.
Run `man gets` and read the BUGS section. How many characters can the program really read?
## Solucion
┌──(diego㉿kali)-[~]
└─$ nc saturn.picoctf.net 63397

Input: tf66gyygftfgyhujhgtfgyhu7y6tfgyhu7y6gyhu87ygyu98y78yhuij8u978yhu
picoCTF{ov3rfl0ws_ar3nt_that_bad_8446a0c3}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias