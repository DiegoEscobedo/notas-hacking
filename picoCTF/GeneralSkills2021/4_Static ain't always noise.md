# Level 4
## Objetivo
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/static)? This [BASH script](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/ltdis.sh) might help!
## Pistas
(none)
## Solucion
┌──(diego㉿kali)-[~]
└─$ chmod +x dis.sh     
┌──(diego㉿kali)-[~]
└─$ ./dis.sh static                        
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
┌──(diego㉿kali)-[~]
└─$ cat static.ltdis.x86_64.txt | grep pico
┌──(diego㉿kali)-[~]
└─$ cat static.ltdis.strings.txt | grep pico                        
   1020 picoCTF{d15a5m_t34s3r_ccb2b43e}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias