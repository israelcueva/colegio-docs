# 5-Secundaria - Unidad 5

## 3BS01: Genero mi entorno de desarrollo

> <i class="bi bi-calendar"></i> **Fecha:** 12 al 16 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** HeidiSQL / Xampp<br><i class="bi bi-clipboard-check"></i> **Tarea:** Prepara tu entorno de desarrollo en casa<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/MySQL/default.asp<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=NRPAur8m7M0 / https://www.youtube.com/watch?v=ydgRu2X5nHA<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1g8v-4EJPwj1QgNCqxrMytty-gGLZ3s2n?usp=sharing

MySQL es uno de los sistemas de gestión de bases de datos relacionales más populares y ampliamente utilizados en el mundo. Desarrollado inicialmente por MySQL AB y ahora mantenido por Oracle Corporation, MySQL es conocido por su rendimiento, fiabilidad y facilidad de uso. En el contexto del desarrollo de aplicaciones, trabajar con bases de datos MySQL de manera eficiente requiere un entorno de desarrollo adecuado que facilite la creación, gestión y optimización de bases de datos.

**¿Qué es un Entorno de Desarrollo para MySQL?**

Un entorno de desarrollo para MySQL es un conjunto de herramientas y aplicaciones que permiten a los desarrolladores interactuar con bases de datos MySQL de manera eficiente. Estos entornos proporcionan interfaces gráficas, herramientas de línea de comandos, y características avanzadas para la gestión de esquemas, ejecución de consultas, análisis de rendimiento y depuración. Los entornos de desarrollo adecuados pueden acelerar significativamente el proceso de desarrollo y administración de bases de datos.

## 3BS02: Conozco la sintaxis básica de SQL

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** HeidiSQL<br><i class="bi bi-clipboard-check"></i> **Tarea:** <br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/MySQL/default.asp<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=NRPAur8m7M0 / https://www.youtube.com/watch?v=ydgRu2X5nHA<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1g8v-4EJPwj1QgNCqxrMytty-gGLZ3s2n?usp=sharing

SQL en MySQL se divide en varias categorías de comandos, cada una de las cuales sirve para un propósito específico en la gestión y manipulación de datos:

- Lenguaje de Definición de Datos (DDL): Incluye comandos que definen la estructura de la base de datos, como CREATE, ALTER y DROP. Estos comandos permiten crear, modificar y eliminar tablas y otros objetos de la base de datos.
- Lenguaje de Manipulación de Datos (DML): Incluye comandos que manipulan los datos dentro de las tablas, como INSERT, UPDATE, DELETE y SELECT. Estos comandos permiten añadir, actualizar, eliminar y consultar datos respectivamente.
- Lenguaje de Control de Datos (DCL): Incluye comandos como GRANT y REVOKE, que gestionan los permisos y accesos a la base de datos.
- Lenguaje de Control de Transacciones (TCL): Incluye comandos como COMMIT, ROLLBACK y SAVEPOINT, que controlan las transacciones dentro de la base de datos, asegurando la integridad de los datos.

## 3BS03: Modelando mi base de datos

> <i class="bi bi-calendar"></i> **Fecha:** 26 al 30 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** HeidiSQL<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/MySQL/default.asp<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=J1kqPtuvdJM<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1g8v-4EJPwj1QgNCqxrMytty-gGLZ3s2n?usp=sharing


En MySQL, las bases de datos relacionales se organizan en tablas que contienen datos estructurados. Uno de los aspectos más importantes en este tipo de bases de datos son las relaciones entre las tablas, que permiten vincular datos de manera eficiente y lógica. Estas relaciones ayudan a mantener la integridad de los datos y facilitan las consultas complejas al conectar diferentes tablas entre sí.

Existen tres tipos principales de relaciones en MySQL:

- **Relación Uno a Uno (1:1)**: Esta relación implica que un registro en una tabla está asociado con un solo registro en otra tabla. Se utiliza cuando ambos conjuntos de datos están estrechamente relacionados pero deben almacenarse en tablas separadas por motivos de diseño o seguridad.
- **Relación Uno a Muchos (1)**: En este tipo de relación, un registro en una tabla puede estar relacionado con múltiples registros en otra tabla. Es una de las relaciones más comunes y se utiliza, por ejemplo, cuando un cliente puede tener varios pedidos.
- **Relación Muchos a Muchos (N):** En esta relación, varios registros en una tabla pueden estar relacionados con múltiples registros en otra tabla. Para implementar este tipo de relación, generalmente se utiliza una tabla intermedia que contiene las claves foráneas de ambas tablas principales.

Cada uno de estos tipos de relaciones tiene su propio propósito y aplicación en la estructura de una base de datos, y entenderlos es fundamental para diseñar bases de datos eficientes y bien estructuradas.

<div class="currentTheme">

## 3BS04: Llaves primarias y foráneas

> <i class="bi bi-calendar"></i> **Fecha:** 02 al 06 de Setiembre<br><i class="bi bi-laptop"></i> **Programa:** HeidiSQL<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea, avanzar práctica<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/MySQL/default.asp<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=hFwHAt8nCQY<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1g8v-4EJPwj1QgNCqxrMytty-gGLZ3s2n?usp=sharing

En MySQL, el uso de llaves primarias y foráneas es esencial para la organización y gestión de datos en bases de datos relacionales. Estas llaves permiten establecer la integridad referencial, garantizando la consistencia y coherencia de los datos entre diferentes tablas.

**Llave Primaria (Primary Key)**

Una llave primaria es un identificador único para cada registro en una tabla. Se utiliza para asegurar que cada fila de la tabla sea única y fácilmente identificable. Las características principales de una llave primaria son:

- Unicidad: Ningún otro registro en la tabla puede tener el mismo valor de la llave primaria.
- No nulo: Los campos que componen la llave primaria no pueden contener valores nulos.
- Índice: MySQL crea automáticamente un índice sobre la columna o columnas que forman la llave primaria, lo que mejora la velocidad de las consultas.

Una tabla puede tener una sola llave primaria, y puede estar compuesta por una o varias columnas (llave primaria compuesta).

**Llave Foránea (Foreign Key)**

Una llave foránea es un campo (o conjunto de campos) en una tabla que crea un vínculo entre esa tabla y otra. Específicamente, la llave foránea hace referencia a la llave primaria de otra tabla, estableciendo una relación entre las dos. Esto asegura que los datos en la tabla de referencia (la tabla que contiene la llave primaria) están representados de manera consistente en la tabla que contiene la llave foránea.

Las llaves foráneas tienen varias funciones importantes:

- Mantener la integridad referencial: Impiden la inserción de valores en la tabla hija que no existan en la tabla padre, evitando así referencias inválidas.
- Propagación de cambios: Con el uso de opciones como ON UPDATE y ON DELETE, es posible controlar cómo se comportan las llaves foráneas cuando se actualizan o eliminan los registros en la tabla de referencia.

El uso adecuado de llaves primarias y foráneas es fundamental para garantizar la integridad y la coherencia de los datos, permitiendo al mismo tiempo la creación de estructuras de datos más complejas y eficientes.

</div>

## 3BS05: Práctica Calificada & Revisión de Folder

> <i class="bi bi-calendar"></i> **Fecha:** Domingo 15<br><i class="bi bi-laptop"></i> **Programa:** Cualquier editor de código.

Para esta semana deberás realizar tu práctica calificada que consiste en lo siguiente:

- Realiza una exposición en video de 3 ejemplos de base de datos en torno a Universidades con sus respectivos campos, además de sus llaves primarias y foráneas. [Ejemplo](https://lh3.googleusercontent.com/proxy/d1CIAQds82H9aQtYKuh2-LtsKd5IqsmItG8LzNKW2YrGpq0Kbrk6b61J9SDujNrDqTpoNL1HVt8zMbU1lyUGcbtRn_wE6dKPV2wYvEZk4tIfRACYy1rf01HBczrqqSCY4rjFqKi3Kirv2_dXFg),
- En dicho video deberás aparecer explicando tus ejemplos, el porqué los modelaste de esa manera.

El video de tu exposición deberás subirlo a través del enlace siguiente:

https://mariareinista-my.sharepoint.com/:f:/g/personal/admin_mrc_edu_pe/EpTznbUqBtVAqyogtW6MnLgBzhMjJ4AqQ7S_l9CU6ZLv1Q

> No habrá extensión de fecha para la práctica.