# Level 3
## Objetivo
Run the Python script `code.py` in the same directory as `codebook.txt`.
-   [Download code.py](https://artifacts.picoctf.net/c/1/code.py)
-   [Download codebook.txt](https://artifacts.picoctf.net/c/1/codebook.txt)
## Pistas
On the webshell, use `ls` to see if both files are in the directory you are in
## Solucion
┌──(diego㉿kali)-[~]
└─$ wget https://artifacts.picoctf.net/c/1/codebook.txt
--2023-03-22 12:21:39--  https://artifacts.picoctf.net/c/1/codebook.txt
Resolviendo artifacts.picoctf.net (artifacts.picoctf.net)... 13.249.74.56, 13.249.74.22, 13.249.74.69, ...
Conectando con artifacts.picoctf.net (artifacts.picoctf.net)[13.249.74.56]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 27 [application/octet-stream]
Grabando a: «codebook.txt»

codebook.txt              100%[====================================>]      27  --.-KB/s    en 0s      

2023-03-22 12:21:40 (22.9 MB/s) - «codebook.txt» guardado [27/27]

                                                                                                       
┌──(diego㉿kali)-[~]
└─$ python code.py 
picoCTF{c0d3b00k_455157_d9aa2df2}
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias