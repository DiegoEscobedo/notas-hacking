# Level 10
## Objetivo
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data
## Datos de Acceso
bandit10
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
## Solucion
bandit10@bandit:~$ la -la
total 24
drwxr-xr-x  2 root     root     4096 Jan 11 19:18 .
drwxr-xr-x 70 root     root     4096 Jan 11 19:19 ..
-rw-r--r--  1 root     root      220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root     root     3771 Jan  6  2022 .bashrc
-rw-r-----  1 bandit11 bandit10   69 Jan 11 19:18 data.txt
-rw-r--r--  1 root     root      807 Jan  6  2022 .profile
bandit10@bandit:~$ cat data.txt
VGhlIHBhc3N3b3JkIGlzIDZ6UGV6aUxkUjJSS05kTllGTmI2blZDS3pwaGxYSEJNCg==
bandit10@bandit:~$ echo "mensaje secreto" | base64
bWVuc2FqZSBzZWNyZXRvCg==
bandit10@bandit:~$ echo "bWVuc2FqZSBzZWNyZXRvCg" | base64 -d
mensaje secreto
base64: invalid input
bandit10@bandit:~$ base64 .d data.txt
base64: extra operand ‘data.txt’
Try 'base64 --help' for more information.
bandit10@bandit:~$ base64 -d data.txt
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
bandit10@bandit:~$
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|base64|desencripta los archivos que esten en base 64(rar,zip,etc.)|
## Referencias
https://en.wikipedia.org/wiki/Base64