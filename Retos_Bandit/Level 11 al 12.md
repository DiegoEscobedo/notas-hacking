# Level 11
## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
## Datos de Acceso
bandit11
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
## Solucion
bandit11@bandit:~$ cat data.txtx
cat: data.txtx: No such file or directory
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z][n-za-mN-ZA-M]
tr: missing operand after ‘[a-zA-Z][n-za-mN-ZA-M]’
Two strings must be given when translating.
Try 'tr --help' for more information.
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M]
The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
bandit11@bandit:~$ python
Command 'python' not found, did you mean:
  command 'python3' from deb python3
  command 'python' from deb python-is-python3
bandit11@bandit:~$ python3
Python 3.10.6 (main, Nov 14 2022, 16:10:14) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import codecs
>>> cadena=open("data.txt").read()
>>> codecs.decode(cadena, "rot13")
'The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv\n'
>>>
## Notas Adicionales
|comando|descripcion|
|tr|transforma textos|
## Referencias
https://en.wikipedia.org/wiki/ROT13