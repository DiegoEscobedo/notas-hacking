# Level 16
## Objetivo
## Datos de Acceso
bandit16
JQttfApK4SeyHwDlI9SXGR50qclOAil1
## Solucion
bandit16@bandit:~$ nmap -p 31000-32000 localhost Starting Nmap 7.40 ( https://nmap.org ) at 2020-09-22 16:06 CEST Nmap scan report for localhost (127.0.0.1) Host is up (0.00030s latency). Not shown: 996 closed ports PORT STATE SERVICE 31046/tcp open unknown 31518/tcp open unknown 31691/tcp open unknown 31790/tcp open unknown 31960/tcp open unknown Nmap done: 1 IP address (1 host up) scanned in 0.09 seconds bandit16@bandit:~$ openssl s_client -connect localhost:31790 CONNECTED(00000003) depth=0 CN = localhost verify error:num=18:self signed certificate verify return:1 depth=0 CN = localhost verify return:1 --- Certificate chain 0 s:/CN=localhost i:/CN=localhost --- Server certificate -----BEGIN CERTIFICATE----- MIICBjCCAW+gAwIBAgIEYXGqnDANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls ... ... 6nrC3qIegoiRUO0Uj9WUo83AjlWJ//Se7WW0R5SVwwG9ld490NeQFcgL -----END CERTIFICATE----- --- JQttfApK4S
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
