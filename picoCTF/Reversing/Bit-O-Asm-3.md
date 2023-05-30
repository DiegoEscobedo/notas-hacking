# Level 4
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.
## Pistas
Not everything in this disassembly listing is optimal.
## Solucion
Calculamos la bandera haciendo las operaciones correspondientes al lenguaje ensamblador 
1. Se carga `654874` en el registro `eax`.
2. Se multiplica `eax` por `4`, lo que resulta en `2619496`.
3. Se suma `0x1f5` (`501` en decimal) al resultado de la multiplicación, lo que da un valor final de `2619997`.
La bandera es picoCTF{`2619997`}
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
