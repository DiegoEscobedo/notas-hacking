# Level 4
## Objetivo
Attackers have hidden information in a very large mass of data in the past, maybe they are still doing it.Download the data [here](https://artifacts.picoctf.net/c/126/anthem.flag.txt).
## Pistas
Download the file and search for the flag based on the known prefix.
## Solucion
┌──(diego㉿kali)-[~]
└─$ wget https://artifacts.picoctf.net/c/126/anthem.flag.txt 
--2023-05-11 16:19:43--  https://artifacts.picoctf.net/c/126/anthem.flag.txt
Resolviendo artifacts.picoctf.net (artifacts.picoctf.net)... 18.160.124.119, 18.160.124.34, 18.160.124.108, ...
Conectando con artifacts.picoctf.net (artifacts.picoctf.net)[18.160.124.119]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 108668 (106K) [application/octet-stream]
Grabando a: «anthem.flag.txt»

anthem.flag.txt           100%[====================================>] 106.12K  --.-KB/s    en 0.07s   

2023-05-11 16:19:44 (1.57 MB/s) - «anthem.flag.txt» guardado [108668/108668]

                                                                                                       
┌──(diego㉿kali)-[~]
└─$ grep pico anthem.flag.txt 
      we think that the men of picoCTF{gr3p_15_@w3s0m3_2116b979}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias