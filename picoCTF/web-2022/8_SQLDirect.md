# Level 8
## Objetivo
Connect to this PostgreSQL server and find the flag!`psql -h saturn.picoctf.net -p 49749 -U postgres pico`Password is `postgres`
## Pistas
What does a SQL database contain?
## Solucion
┌──(diego㉿kali)-[~]
└─$ psql -h saturn.picoctf.net -p 65391 -U postgres pico

Contraseña para usuario postgres: 
psql (14.4 (Debian 14.4-1+b1), servidor 15.2 (Debian 15.2-1.pgdg110+1))
ADVERTENCIA: psql versión mayor 14, servidor versión mayor 15.
          Algunas características de psql podrían no funcionar.
Digite «help» para obtener ayuda.

pico=# \?
pico=# \l
                               Listado de base de datos
  Nombre   |  Dueño   | Codificación |  Collate   |   Ctype    |      Privilegios      
-----------+----------+--------------+------------+------------+-----------------------
 pico      | postgres | UTF8         | en_US.utf8 | en_US.utf8 | 
 postgres  | postgres | UTF8         | en_US.utf8 | en_US.utf8 | 
 template0 | postgres | UTF8         | en_US.utf8 | en_US.utf8 | =c/postgres          +
           |          |              |            |            | postgres=CTc/postgres
 template1 | postgres | UTF8         | en_US.utf8 | en_US.utf8 | =c/postgres          +
           |          |              |            |            | postgres=CTc/postgres
(4 filas)

pico=# \c pico
psql (14.4 (Debian 14.4-1+b1), servidor 15.2 (Debian 15.2-1.pgdg110+1))
ADVERTENCIA: psql versión mayor 14, servidor versión mayor 15.
          Algunas características de psql podrían no funcionar.
Ahora está conectado a la base de datos «pico» con el usuario «postgres».
pico=# \dt
        Listado de relaciones
 Esquema | Nombre | Tipo  |  Dueño   
---------+--------+-------+----------
 public  | flags  | tabla | postgres
(1 fila)

pico=# SELECT * FROM flags;
 id | firstname | lastname  |                address                 
----+-----------+-----------+----------------------------------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 filas)

pico=# 

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias