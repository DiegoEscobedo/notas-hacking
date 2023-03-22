# Level 5
## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:
-   human-readable
-   1033 bytes in size
-   not executable
## Datos de Acceso
bandit5
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR 
## Solucion
bandit5@bandit:~$ ls
inhere
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ ls
maybehere00  maybehere03  maybehere06  maybehere09  maybehere12  maybehere15  maybehere18
maybehere01  maybehere04  maybehere07  maybehere10  maybehere13  maybehere16  maybehere19
maybehere02  maybehere05  maybehere08  maybehere11  maybehere14  maybehere17
bandit5@bandit:~/inhere$ find. -readable -type f -size 1033c
Command 'find.' not found, did you mean:
  command 'findg' from deb ncl-ncarg (6.6.2-10build2)
  command 'find' from deb findutils (4.8.0-1ubuntu3)
  command 'findv' from deb polylib-utils (5.22.5-4+dfsg)
bandit5@bandit:~/inhere$ find -readable -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
bandit5@bandit:~/inhere$
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|find|busca practicamente lo que sea|
|-readable|archivos leibles por humanos|
|-type|indica el tipo de archivo|
|f|tipo de archivo normal|
|size (tamaño)c|es el tamaño de caracteres|
## Referencias