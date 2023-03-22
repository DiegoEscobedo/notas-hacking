# Level 9
## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.
## Datos de Acceso
bandit9
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
## Solucion
bandit9@bandit:~$ Strings data.txt | greep"==
Command 'Strings' not found, did you mean:
  command 'strings' from deb binutils (2.38-4ubuntu2.1)
Try: apt install 
greep==: command not found
bandit9@bandit:~$ strings data.txt | greep==
greep==: command not found
bandit9@bandit:~$ strings data.txt | greep ==
Command 'greep' not found, did you mean:
  command 'greed' from deb greed (4.2-1)
  command 'grep' from deb grep (3.7-1build1)
Try: apt install 
bandit9@bandit:~$ strings data.txt | grep "=="
c========== the
h;========== password
========== isT
n.E========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
bandit9@bandit:~$
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|string|regresa solo las cadenas|
## Referencias