# Level 4
## Objetivo
The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.
## Datos de Acceso
bandit4
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
## Solucion
bandit4@bandit:~$ ls 
inhere 
bandit4@bandit:~$ cd inhere/ 
bandit4@bandit:~/inhere$ ls 
-file00 -file02 -file04 -file06 -file08 
-file01 -file03 -file05 -file07 -file09 
bandit4@bandit:~/inhere$ cat ./-file00 
T     B    #6   Kt  3 
                             6X    t      )bandit4@bandit:~/inhere$ 
bandit4@bandit:~/inhere$ file ./-file00 
./-file00: data 
bandit4@bandit:~/inhere$ file ./* 
./-file00: data 
./-file01: data 
./-file02: data 
./-file03: data 
./-file04: data 
./-file05: data 
./-file06: data 
./-file07: ASCII text 
./-file08: data 
./-file09: data 
bandit4@bandit:~/inhere$ cat ./-file07 
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR 
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|file|indica el tipo de archivo|
|*|indica todos|

## Referencias
