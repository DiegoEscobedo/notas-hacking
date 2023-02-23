# Level 2
## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory

## Datos de Acceso
bandit2
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi 
## Solucion
bandit2@bandit:~$ ls 
spaces in this filename 
bandit2@bandit:~$ cat spaces in this filename 
cat: spaces: No such file or directory 
cat: in: No such file or directory cat: this: No such file or directory 
cat: filename: No such file or directory 
bandit2@bandit:~$ cat spaces\ in\ this\ filename aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 
bandit2@bandit:~$ cat "spaces in this filename" aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 
bandit2@bandit:~$
## Notas Adicionales
|comando|descripcion|
|cat|lee un archivo y lo muestra|
## Referencias
