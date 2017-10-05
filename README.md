Guía SQL 
=========

Crear una tabla
----------------

```sql
  create table nombre_tabla (
    nombre varchar(30),
    clave varchar(10),
    correo varchar(10),
    telefono integer
  );
```

Conocer estructura de la tabla 
----------------
```sql
SELECT table_name,column_name,udt_name,character_maximum_length 
  FROM information_schema.columns WHERE nomnre_tabla = 'campo'
```

Eliminar tabla  :x: :fire:
----------------
```sql
 drop table nombre_tabla;
 ```

Insertar elementos
---------------- 

```sql
 insert into usuarios(nombre, clave) values('Osman', 'Alexander');
  ```

Recuperar algunos campos de la tabla  :mag_right:
---------------- 

```sql
 select nombre, clave from usuarios
```
 
Operadores relacionales
---------------- 
```sql
 select * from nombre_table
  where nombre_campo<>'valor';


 select nombre_campo,nombre_campo..
  from nombre_tabla
  where precio>20;
```

Borrar registros
---------------- 
```sql
  delete from nombre_tabla
  where nombre_campo='valor';
```

Actualizar registros
---------------- 
```sql
  update nombre_tabla set nombre_campo ='campo'
  where nombre_campo_a_buscar='campo';
```

Comentarios
---------------- 
```sql
 select nombre_campo, nombre_campo 
 /*mostramos títulos y
 nombres de los autores*/
 from nombre_tabla;
 ```

 Valor NULL
 ---------------- 
 ```sql
  create table nombre_tabla(
  titulo varchar(30) not null,
  autor varchar(30) not null,
  editorial varchar(15) null,
  precio float
 );
```

Valor SERIAL
-------------
```sql
create table nombre_tabla(
  codigo serial,
  titulo varchar(30),
  autor varchar(30),
  editorial varchar(15),
  primary key (codigo)
 );
 ```

 Borrar todos los registros de una tabla :fire: :fire:
--------------------------------

```sql
truncate table libros;
```

Tipo de dato Numerico :one: :1234:
--------------------
almacenar un número de hasta 10 numeros con 2 decimales 
```sql
dígitos con 2 decimales
```





