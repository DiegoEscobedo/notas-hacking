# Level 27
## Objetivo
## Datos de Acceso
bandit27 - YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
## Solucion
bandit27@bandit:~$ mktemp -d
/tmp/tmp.wm1aW3K8Ho
bandit27@bandit:~$ cd /tmp/tmp.RH39ki24pd
-bash: cd: /tmp/tmp.RH39ki24pd: No such file or directory
bandit27@bandit:~$ cd /tmp/tmp.wm1aW3K8Ho
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho$ git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit27/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit27/.ssh/known_hosts).
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

bandit27-git@localhost's password:
Permission denied, please try again.
bandit27-git@localhost's password:
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho$ ls -la
total 124
drwx------    4 bandit27 bandit27   4096 Feb 28 19:26 .
drwxrwx-wt 3077 root     root     110592 Feb 28 19:27 ..
drwxrwxr-x    3 bandit27 bandit27   4096 Feb 28 19:26 git@localhost:2220
drwxrwxr-x    3 bandit27 bandit27   4096 Feb 28 19:27 repo
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho$ ls
git@localhost:2220  repo
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho$ cat README
cat: README: No such file or directory
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho$ cd repo
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho/repo$ cat README
The password to the next level is: AVanL161y9rsbcJIsFHuw35rjaOM19nR
bandit27@bandit:/tmp/tmp.wm1aW3K8Ho/repo$
## Notas Adicionales
|comando|descripcion|
|xxx|xxx|
## Referencias