# LABORATORIO-PROGRAMACION-

**Taller Grupal** 

Integrantes: Quilumbaquín Lenin

             Robalino Johanna
             
             Jiménez Iván
             
             Vallejo Keily
             
             Mosquera William 
             
NRC: 3725

Carrera: Electrónica y Automatización

Asignatura: Programación Orientada a Objetos 

Docente: Ing. Cesar Osorio

Tema: BASE DE DATOS 


**OBJETIVOS**

Objetivo General 

Analizar la realización, generación y acceso a una Base de Datos en SQL.

Objetivos específicos

•	Interpretar el funcionamiento de una baso de datos mediante el uso del lenguaje desarrollado en SQL.
•	Identificar los comandos necesarios para el desarrollo del ejercicio planteado.
•	Identificar la organización de las bases de datos, así como también, la clasificación de estas mediante investigación y análisis.
•	Entender y aplicar las sentencias para obtener una correcta filtración de los resultados obtenidos.

**MARCO TEÓRICO**

Una base de datos es una colección organizada de información estructurada, o datos, típicamente almacenados electrónicamente en un sistema de computadora. Una base de datos es usualmente controlada por un sistema de gestión de base de datos (DBMS). En conjunto, los datos y el DBMS, junto con las aplicaciones que están asociados con ellos, se conocen como un sistema de base de datos, que a menudo se reducen a solo base de datos.

Los datos dentro de los tipos más comunes de bases de datos en funcionamiento hoy en día se modelan típicamente en filas y columnas en una serie de tablas para que el procesamiento y la consulta de datos sean eficientes. Luego se puede acceder, administrar, modificar, actualizar, controlar y organizar fácilmente los datos. La mayoría de las bases de datos utilizan lenguaje de consulta estructurado (SQL) para escribir y consultar datos.

¿Qué es el lenguaje de consulta estructurado (SQL)?

SQL es un lenguaje de programación usado por casi todas las bases de datos relacionales para consultar, manipular y definir datos, y para proporcionar control de acceso.

SQL se desarrolló por primera vez en IBM en la década de 1970 con Oracle como uno de los principales contribuyentes, lo que llevó a la implementación del estándar ANSI de SQL. 

SQL ha generado muchas extensiones por parte de compañías como IBM, Oracle y Microsoft. Aunque SQL todavía se usa ampliamente en la actualidad, comienzan a aparecer nuevos lenguajes de programación.

¿Qué es una base de datos de MySQL?

MySQL es un sistema de gestión de bases de datos relacionales de código abierto basado en SQL. Fue diseñado y optimizado para aplicaciones web y puede ejecutarse en cualquier plataforma. 

A medida que surgían nuevos y diferentes requisitos con Internet, MySQL se convirtió en la plataforma elegida por los desarrolladores web y las aplicaciones basadas en la web. Debido a que está diseñada para procesar millones de consultas y miles de transacciones, MySQL es una opción popular para las empresas de comercio electrónico que necesitan administrar múltiples transferencias de dinero. 

La flexibilidad bajo demanda es la característica principal de MySQL.

![image](https://user-images.githubusercontent.com/84789076/131421201-450314de-da2f-4a92-9494-d52e8c3244d4.png)

MySQL es el DBMS detrás de algunos de los mejores sitios web y aplicaciones basadas en la web del mundo, incluyendo Airbnb, Uber, LinkedIn, Facebook, Twitter y YouTube.

**PROCEDIMEINTO**

Con el script dado en clase para la creación de las diversas tablas de una base de
datos; genere las instrucciones necesarias para extraer datos según los siguientes
requerimientos:

- Consulta para extraer el nombre de los clientes con el porcentaje de
descuento obtenido en la compra y cual fue el vendedor que vendió o
atendió el pedido.

**Codigo**
SELECT ORDENID,NOMBRECONTACTO as Nomb_Cliente,ordenes.descuento,empleados.NOMBRE as Nomb_Vendedor
from clientes,ordenes,empleados
where clientes.CLIENTEID = ordenes.CLIENTEID and
empleados.empleadoID = ordenes.EMPLEADOID;

![image](https://user-images.githubusercontent.com/84586923/131421495-e194a2c3-e59d-4a08-bf67-96de2b7b78eb.png)

-	Consulta para extraer los productos con el nombre de proveedor y su contacto.

**Codigo**
SELECT DESCRIPCION as PRODUCTO,NOMBREPROV as NOMB_PROVEEDOR,CONTACTO
from proveedores,productos
where productos.PROVEEDORID=proveedores.PROVEEDORID;

![image](https://user-images.githubusercontent.com/84586923/131421632-4850d79d-726b-4a49-b722-9bf5b53d3c0c.png)

- Consulta para extraer de la tabla ordenes los clientes cuyo nombre empiecen con la letra s

**Codigo**
SELECT NOMBRECIA,NOMBRECONTACTO FROM clientes WHERE NOMBRECIA like 's%';

![image](https://user-images.githubusercontent.com/84586923/131421706-ff82916d-0809-4bfb-a8ef-a3eb78ef53fd.png)

- Consulta para mostrar los productos con sus categorías ordenado por categoría

**Codigo**
select DESCRIPCION ,categorias.NOMBRECAT FROM PRODUCTOS,CATEGORIAS
Where PRODUCTOS.categoriaID = CATEGORIAS.CATEGORIAID ;

![image](https://user-images.githubusercontent.com/84586923/131421791-61a4ce36-ef0b-4208-8d8a-e113000cda0a.png)

**CONCLUSIONES**

1.	En conclusión, podemos decir que las bases de datos es una colección de información organizada de forma que un programa de ordenador puede seleccionar rápidamente los fragmentos de datos que necesite.

2.	Se puede concluir que la base de datos tradicionales se organiza por campos, registros y archivos.

3.	Finalmente podemos concluir que la base de datos puede clasificarse de varias maneras, de acuerdo al contexto que se este manejando, o la utilidad de la misma.

**RECOMENDACIONES**

1.	Verificar el código para no obtener errores ni filtración de datos durante la ejecución.  

2. Revisar cada uno de los comandos propuestos en clases para poder verificar que el trabajo este yendo de una manera ordenada y adecuada.

3. Para realizar la busqueda debemos tener en cuento lo que se dispone en en cada tabla creada para con ello poder realizar una busqueda mas exitosa asi como tambien si se dispone de una infromacion abundante realizar las condiciones para que se obtenga la informacion mas relevante e importante.

**REFERENCIAS**

Escuel De Ingenieria Industrial. (2 de Febrero de 2015). Obtenido de https://www.slideshare.net/JessicaParra15/base-de-datos-programacion-64593256

Oracle. (22 de Junio de 2014). Obtenido de https://www.oracle.com/mx/database/what-is-database/

