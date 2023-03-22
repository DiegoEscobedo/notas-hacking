# Level 9
## Objetivo
There is a secure website running at `https://2019shell1.picoctf.com/problem/4161/` ([link](https://2019shell1.picoctf.com/problem/4161/)) or [http://2019shell1.picoctf.com:4161](http://2019shell1.picoctf.com:4161/). Try to see if you can login as admin!
## Pistas
> Seems like the password is encrypted
## Solucion
Esta vez, cuando inyectamos la misma inyección ' o 1=1--, obtenemos nuestra consulta cifrada:

contraseña: ' o 1=1--
Consulta SQL: SELECT * FROM admin where contraseña = '' be 1=1--'
Vemos que los caracteres alfabéticos 'o' y 'r' se han cambiado a 'b' y 'e'. Curioso. Intentemos poner cada letra del alfabeto después del comentario para ver exactamente qué tipo de encriptación es mientras configuramos la entrada oculta en 1 todavía.

contraseña: ' o 1=1--abcdefghijklmnopqrstuvwxyz
Consulta SQL: SELECCIONE * DESDE el administrador donde la contraseña = '' sea 1 = 1--nopqrstuvwxyzabcdefghijklm'
Ahora podemos confirmar que se trata de algún tipo de cifrado César. Los caracteres de la palabra OR se sustituyen por BE. Intentamos nuestra consulta de nuevo, esta vez siguiendo el cifrado, así: ' be 1=1--. El portal nos deja pasar y finalmente vemos nuestra bandera.

picoCTF{3v3n_m0r3_SQL_4424e7af}
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias