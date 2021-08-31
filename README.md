# LABORATORIO-PROGRAMACION-

Taller Grupal 

Integrantes: Quilumbaquín Lenin

             Robalino Johanna
             
             Jiménez Iván
             
             Vallejo Keily
             
             Mosquera William 
             
NRC: 3725

Carrera: Electrónica y Automatización

Asignatura: Programación Orientada a Objetos 

Docente: Ing. Cesar Osorio

Tema: 


OBJETIVOS.-

MARCO TEÓRICO.-

PROCEDIMEINTO.-

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

CONCLUSIONES.-

1.	En conclusión, podemos decir que las bases de datos es una colección de información organizada de forma que un programa de ordenador puede seleccionar rápidamente los fragmentos de datos que necesite.

2.	Se puede concluir que la base de datos tradicionales se organiza por campos, registros y archivos.

3.	Finalmente podemos concluir que la base de datos puede clasificarse de varias maneras, de acuerdo al contexto que se este manejando, o la utilidad de la misma.

RECOMENDACIONES.-

1.	Verificar el código para no obtener errores ni filtración de datos durante la ejecución.  

2. Revisar cada uno de los comandos propuestos en clases para poder verificar que el trabajo este yendo de una manera ordenada y adecuada.

3. Para realizar la busqueda debemos tener en cuento lo que se dispone en en cada tabla creada para con ello poder realizar una busqueda mas exitosa asi como tambien si se dispone de una infromacion abundante realizar las condiciones para que se obtenga la informacion mas relevante e importante.

REFERENCIAS

