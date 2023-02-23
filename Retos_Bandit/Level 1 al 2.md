# Level 1
## Objetivo
The password for the next level is stored in a file called **-** located in the home directory

## Datos de Acceso
bandit1

## Solucion
bandit1@bandit:~$ ls 
-
bandit1@bandit:~$ cat - 
^C 
bandit1@bandit:~$ cat ./- 
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi 
bandit1@bandit:~$ pwd 
/home/bandit1 
bandit1@bandit:~$ cat /home/bandit1/- 
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi 
bandit1@bandit:~$
## Notas Adicionales
|comando|descripcion|
|cat ./|para archivos que empiecen con guion|
## Referencias
https://www.google.com/search?q=dashed+filename
