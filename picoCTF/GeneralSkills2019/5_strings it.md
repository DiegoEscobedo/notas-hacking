# Level 5
## Objetivo
Can you find the flag in [file](https://github.com/kevinjycui/picoCTF-2019-writeup/blob/master/General%20Skills/strings%20it/strings) without running it? You can also find the file in /problems/strings-it_5_1fd17da9526a76a4fffce289dee10fbb on the shell server.
## Pistas
strings
## Solucion
The title and tutorial in the hint seems to point towards using the `strings` command like `strings strings` to get the flag. However, we are met with a lot of plain-text upon doing so, which would be quite the hassle to sort through manually. Instead, we can use the `grep` command which filters for specifc expressions in plain-text. Since we know the format of picoCTF flags is picoCTF{...}, we can grep for picoCTF. The command would then be `strings strings | grep picoCTF` 
picoCTF{5tRIng5_1T_d66c7bb7} 
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|strings|lee archivos de cadenas|
## Referencias
https://linux.die.net/man/1/strings