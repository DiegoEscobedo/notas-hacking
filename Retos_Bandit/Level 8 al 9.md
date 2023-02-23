# Level X
## Objetivo
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once
## Datos de Acceso
bandit8
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
## Solucion
bandit8@bandit:~$ sort data.txt | uniq -u
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
bandit8@bandit:~$
## Notas Adicionales
|comando|descripcion|
|sort|ordena los datos|
|uniq -u|muestra el dato que es unico o sale 1 vez|
(|)--> le manda la salida de el comando anterior para que el sig comando la procese
## Referencias