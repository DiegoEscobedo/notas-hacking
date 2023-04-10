# Level 1
## Objetivo
Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.
## Pistas
-How did pictures from the moon landing get sent back to Earth?
-What is the CMU mascot?, that might help select a RX option
## Solucion
┌──(diego㉿kali)-[~]
└─$ cat whitepages.txt                                        ----- codigo                                                                                                              
┌──(diego㉿kali)-[~]
└─$ xxd -l white pages
xxd: pages: No such file or directory
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ xxd -l whitepages.txt
                                                                                                       
┌──(diego㉿kali)-[~]
└─$ xxd -l 32 whitepages.txt
00000000: e280 83e2 8083 e280 83e2 8083 20e2 8083  ............ ...
00000010: 20e2 8083 e280 83e2 8083 e280 83e2 8083   ...............
                                                                                                       

resultado ya transformando el binario:
		picoCTF

		SEE PUBLIC RECORDS & BACKGROUND REPORT
		5000 Forbes Ave, Pittsburgh, PA 15213
		picoCTF{not_all_spaces_are_created_equal_3e2423081df9adab2a9d96afda4cfad6}
		ÿÿÿÿÿÿÿÿÿÿÿÿ
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
