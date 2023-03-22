# Level 6
## Objetivo
Our flag printing service has started glitching!`$ nc saturn.picoctf.net 50561`
## Pistas
ASCII is one of the most common encodings used in programming
## Solucion
┌──(diego㉿kali)-[~]
└─$ nc saturn.picoctf.net 50561
'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ python          
Python 3.10.5 (main, Jun  8 2022, 09:26:22) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> flag = 'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'
>>> print(flag)
picoCTF{gl17ch_m3_n07_9c42a45d}
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias