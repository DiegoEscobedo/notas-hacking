# Level 5
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.
## Pistas
Don't tell anyone I told you this, but you can solve this problem without understanding the compare/jump relationship.
Of course, if you're really good, you'll only need one attempt to solve this problem.
## Solucion
Analizando el código paso a paso:

1. Se inicializa `[rbp-0x4]` con el valor `0x9fe1a`.
2. Se compara el valor de `[rbp-0x4]` con `0x2710` (10000 en decimal).
3. Si `[rbp-0x4]` es menor o igual a `0x2710`, se salta a la dirección `0x55555555514e` (offset de `main+37`).
4. Si `[rbp-0x4]` es mayor que `0x2710`, se ejecuta la instrucción `sub` que resta `0x65` (101 en decimal) al valor de `[rbp-0x4]`.
5. Después de la resta, el valor de `[rbp-0x4]` es `0x9fdb5`.
6. Se carga el valor de `[rbp-0x4]` en el registro `eax`.

Por lo tanto, el valor correcto de `eax` en este caso es `0x9fdb5`
Bandera:
picoCTF{654773}
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias