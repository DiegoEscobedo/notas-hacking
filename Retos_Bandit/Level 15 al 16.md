# Level 15
## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL encryption.

**Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…**
## Datos de Acceso
bandit15
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
## Solucion
bandit15@bandit:~$ openssl s_client -connect localhost:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
Certificate chain
 0 s:CN = localhost
   i:CN = localhost
   a:PKEY: rsaEncryption, 2048 (bit); sigalg: RSA-SHA1
   v:NotBefore: Feb 21 06:19:29 2023 GMT; NotAfter: Feb 21 06:20:29 2023 GMT
Server certificate
-----BEGIN CERTIFICATE-----
MIIDCzCCAfOgAwIBAgIEA7qUdzANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMjMwMjIxMDYxOTI5WhcNMjMwMjIxMDYyMDI5WjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDL
vM0gZzAHdXTeD5t4ruUJo/kRs4UAodA9XcqDhNtW464W0c55RqKLp921syy3Lvjr
8Q9WkqvCFX+efShMd8XnzbT/dyRrD+cZQnSiPJ3bwDdpwqfkl9h3mb609Kb5HI6R
JgogEyuRLJI+HKtr/wXHwo1vBZ0+yaPMX6sdkd6Hu5Ra0L5Q5+E5+3F/8QgvCeVE
hDRIOrh2a7jxykb8G6+xVC6jIZY0YfrZz6LrESyQau256pqyaQPqQoUWTlitxIql
Ym2Baw7vYDxmFZrvj0FkumC6NokX6K2G9bZ0DaKR/DspPdAC4oT81SawJvsBibdN
51VI6dxBn412ZS8bS155AgMBAAGjZTBjMBQGA1UdEQQNMAuCCWxvY2FsaG9zdDBL
BglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0ZWQgYnkgTmNhdC4g
U2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3DQEBBQUAA4IBAQA9
skxWNwZbedjaVTa5yMPUZQ4Nf5/LAAMtS5Q7mzGH5tdQsTGR0Z4n4eA4hzrmzHBF
MVRL5mR9n+sM5pIrKDa6f4zIc5ObxDyN19ie+3SFASCPz9tihK8Js2V8qsR6LHV1
pfD8DSG0hZPtUuK3Mfi+nWqQUFiiTGj30mb9vlS1sSWv5PGznou1gQ3ZfrDs7B4K
ZKZrllPIVV1CrlDw2Bv8Dc432LQuZAmKAjBd6FG0OAboU/WJMTwAfVjlKMtvC8tg
DZ3djSTprq6PrXlI0utw/MsMIh69b61BRXUuDvRxhU11SNmSI8aegjVL8KuK+Euh
sSLPTocV29SY1YXOwEQi
-----END CERTIFICATE-----
subject=CN = localhost
issuer=CN = localhost
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
SSL handshake has read 1339 bytes and written 373 bytes
Verification error: certificate has expired
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 2048 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 10 (certificate has expired)
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 8A5C1F6F8F9D54A992404743D607998B1B6094E39D1BDCEAF2A00A9FC3E4BA39
    Session-ID-ctx:
    Resumption PSK: 35F3387CFDA20AD324C0ED10F6FE08C6939059D7128171E5A36CD0E39FEB739A34BF7397B23F86ADD47F1CBFF0459A5D
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - 08 30 1f c7 c9 1f f7 7e-10 eb f2 7d b1 cf a6 d0   .0.....~...}....
    0020 - 80 70 c6 b6 76 a9 d6 1f-52 63 61 d8 3e 8f 16 21   .p..v...Rca.>..!
    0030 - b8 4e 22 71 c6 65 d2 1d-f1 24 8d d1 b1 65 62 b8   .N"q.e...$...eb.
    0040 - b3 01 ff aa 53 3a 28 9c-19 36 4d 28 e1 45 80 fd   ....S:(..6M(.E..
    0050 - 77 37 ee 03 61 a5 79 1a-9a da 42 be 7f 77 78 23   w7..a.y...B..wx#
    0060 - d1 0f ef e4 26 e2 4b 87-7e 2f fb 12 a2 ec 2f 4f   ....&.K.~/..../O
    0070 - 8c dd 43 6f 44 4f 4f bd-aa 54 14 a1 c9 a3 f7 a2   ..CoDOO..T......
    0080 - c9 a2 cf fb b5 92 f4 57-2c 3d 4a 14 1d 6e 7a 65   .......W,=J..nze
    0090 - ad 1b d5 eb 98 09 13 7e-e5 10 50 66 ed c3 44 5c   .......~..Pf..D\
    00a0 - c6 ba 21 9d 23 da 54 fd-41 6e 51 0c 1b e4 f4 5f   ..!.#.T.AnQ...._
    00b0 - c5 12 b4 d6 ef 75 07 d0-f1 08 18 2b bd 2d f9 71   .....u.....+.-.q
    00c0 - 5d 06 20 8e c6 10 47 5c-23 c5 12 98 38 00 39 d5   ]. ...G\#...8.9.

    Start Time: 1677007658
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: F94AE701D7ADC393F736E9244DBAD0062EB41FEC83F771DCED0000A18A4345B3
    Session-ID-ctx:
    Resumption PSK: 38C7DBCB26819F5D3D907A4E84FAD1139CF49F6A15F35E14A1B7CDF614622A52A2AF92D30BAA7E2DC797E3C6FD892EB0
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - 1e 56 97 25 67 23 2a a3-5a 05 d4 06 5b bd 58 ac   .V.%g#*.Z...[.X.
    0020 - fa 4e a0 89 c5 c6 4d 72-4b 6e f5 af 57 e7 40 14   .N....MrKn..W.@.
    0030 - ad 60 87 d4 a4 27 66 0d-6f ae 71 a0 11 27 03 0c   .`...'f.o.q..'..
    0040 - b1 03 98 84 bf 24 53 7b-cc 50 0d 35 56 89 31 67   .....$S{.P.5V.1g
    0050 - df 47 ed 7d 2d 5b cf 83-18 01 2a 4c 83 58 69 7b   .G.}-[....*L.Xi{
    0060 - 4a 90 4b 74 50 c4 27 ca-4d ca 6b 46 d7 b2 ae 18   J.KtP.'.M.kF....
    0070 - d8 88 31 18 82 a4 de 1c-31 89 3a ec ed d0 3e 49   ..1.....1.:...>I
    0080 - cc e4 28 41 ba 1c b7 20-65 20 b0 1b fb 6d 35 a1   ..(A... e ...m5.
    0090 - 70 8a cb 37 58 f8 da 13-0b c2 68 ce 89 e8 8c 8d   p..7X.....h.....
    00a0 - 96 10 05 a6 da e2 97 9f-93 77 e3 63 fa a1 79 4f   .........w.c..yO
    00b0 - ca 41 ba 00 0f b1 a6 bd-9b 71 82 d5 d3 ca ef de   .A.......q......
    00c0 - 38 e8 3f 87 f5 f3 b4 82-3f 35 bb 7f 28 cc 60 09   8.?.....?5..(.`.

    Start Time: 1677007658
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
Correct!
JQttfApK4SeyHwDlI9SXGR50qclOAil1

closed
bandit15@bandit:~$
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias