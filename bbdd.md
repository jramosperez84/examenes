# Guia de estudio Bases de Datos

## UF1

---

### Sublenguajes SQL

|ENG|ESP|Explicación|Comandos|
| -- | -- | -- | -- |
|**DDL**: Data Definition Languaje|**LDD**: Lenguaje de Definición de Datos|Definicion y modificación de la estructura de y elementos|CREATE, RENAME, DROP, ALTER|
|**DML**: Data Manipulation Languaje|**LMD**: Lenguaje de Manipulación de Datos|Consulta y modificación de datos|INSERT, UPDATE, DELETE, SELECT|
|**DCL**: Data Control Languaje|**LCD**:Lenguaje de Control de Datos|
Controlar permisos de acceso a los datos|GRANT, REVOKE|

---

### Operaciones basicas

| |**BBDD**|**Tablas**|**Campos**|**Registros**|
| -- | -- | -- | -- | -- |
|**Crear**|CREATE DATABASE|CREATE TABLE|ALTER TABLE ADD|INSERT|
|**Modificar**||RENAME TABLE|ALTER TABLE CHANGE|UPDATE|
|**Borrar**|DROP DATABASE|DROP TABLE|ALTER TABLE DROP|DELETE|
|**Consultar**||||SELECT|

---

### El elemento DATABASE

#### **Creación de la Base de datos:**

~~~sql
CREATE DATABASE nombreBaseDatos;
~~~

Ejemplo:

~~~sql
CREATE DATABASE empresa;
~~~

#### **Crear una base de datos con la codificación adecuada:**

~~~sql
CREATE DATABASE empresa
DEFAULT CHARACTER SET UTF8
DEFAULT COLLATE utf8_general_ci;
~~~

#### **Borrar base de datos:**

~~~sql
DROP DATABASE nombreBaseDatos;
~~~

Ejemplo:

~~~sql
DROP DATABASE empresa;
~~~

---

### Nombres de los elementos

- Pueden contener letras, números o guiones bajos
- No pueden utilizarse comandos del lenguaje
- No deben comenzar con número
- No utilizar acentos, ni "ñ", ni otros signos
- No repetir nombres

#### CamelCase

NombreDeLosElementos

#### snake_case

nombre_de_los_elementos

---

### El lemento TABLE

~~~sql
CREATE TABLE nombreTabla (campo1, campo2, campo3, ...);
~~~

Indicar propiedades de campos:

~~~sql
CREATE TABLE nombreTabla (campo1 tipo (longitud), campo2 tipo (longitud), campo3 tipo (longitud), ...);
~~~

Ejemplo:

~~~sql
CREATE TABLE departamento (deptNum INT (4), deptNombre VARCHAR (50), deptLocalidad VARCHAR (50));
~~~
