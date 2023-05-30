# Level 4
## Objetivo
Can you solve this?What two positive numbers can make this possible: `n1 > n1 + n2 OR n2 > n1 + n2`Enter them here `nc saturn.picoctf.net 56449`. [Source](https://artifacts.picoctf.net/c/456/flag.c)
## Pistas
Integer overflow
Not necessarily a math problem
## Solucion
EL macimo valor para un int es: 2147483647
Asi que se hace lo siguiente 
diego@kali:~$ nc saturn.picoctf.net 56449
n1 > n1 + n2 OR n2 > n1 + n2 
What two positive numbers can make this possible: 
2147483647 
1
You entered 2147483647 and 1
You have an integer overflow
YOUR FLAG IS: picoCTF{Tw0_Sum_Integer_Bu773R_0v3rfl0w_ccd078bd}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
