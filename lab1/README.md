# A1E1

| INF-001: | PAS |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Se validan los datos insertados por el estudiante |
| Datos especificos:| <ul><li>Usuario PAS</li><li>DNI estudiante</li><li>Nombre y apellidos estudiante</li><li>Fecha de nacimiento estudiante</li><li>Sexo</li><li>Dirección</li><li>Telefono</li><li>Correo electronico</li></ul>  |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

| UC-02|  |
| :---------- | ------------------------------------ |
| Nombre: | Modificar horarios |
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 30-09-22|
| Descripción:  | Permite modificar los horarios de las asignaturas |
| Actores: Personal PAS|
| Precondiciones: | El usuario tiene que estar autentificado en el sistema |
| Flujo Normal: | 1. El actor pulsa el botón de modificar horario <br> 2. El sistema muestra el horario y herramientas para el cambio <br> 3. El actor hace los cambios pertinentes  |
| Flujo Alternativo: | |
| Poscondiciones: | El horario queda correctamente modificado|

<br>

| INF-002: | PDI |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Dar de alta estudiantes, Buscar estudiantes en la lista de clase, Proponer cambios en los horarios |
| Descripción:| Se validan los datos insertados por el estudiante |
| Datos especificos:| <ul><li>DNI Usuario PDI</li><li>Contraseña</li><li>Nombre y apellidos</li><li>Fecha de nacimiento </li><li>Sexo</li><li>Dirección</li><li>Telefono</li><li>Correo electronico</li></ul>  |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

|UC-03||
| ----------- | ----------- |
| Nombre | Consultar horarios |
| Autor |   Angel Nieto Burgos |
| Fecha |30/09/2022   |
| Descripcion | En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. 
| actores |   El personal del PDI, el personal del PAS y los estudiantes   |
| precondicion |   Inicio sesion    |
| flujo normal   |  1 seleccionar boton <br>  2 consultar horarios <br> 3 Devolver horario <br> |
| flujo alternativo | 
| poscondiciones |

<br>

|INF-003 | DatosHorario |
| ----------- | ----------- |
| Nombre |  Horarios |  
|Referencia| consultar horarios,proponer cambios en los horarios, modificar horarios|
|Informacion|Los datos que son necesarios para el funcionamiento de los horarios  |
|Datos especificos|<ul> <li>Fecha y Hora</li> <li>  Asignaturas </li> <li>Aula </li></ul> |
|Importancia|Muy Importante|
|Estado| Aceptado|
|Comentarios| - |

<br>

| UC-04 ||
|:------------|:----------------|
| Nombre: | Dar de alta estudiante |
| Autor: | Juanra |
| Fecha: | 30/09/2022 |
|Descripcion:| Un actor puede dar de alta a un usuario|
| Actores:| PAS |
| Precondiciones:| Usuario registrado como usuario PAS |
| Flujo Normal:| 1. Se introducen los datos del usuario a dar de alta <br>2. Se validan los datos del usuario<br>3. Se guarda el usuario en la base de datos dandole de alta en este proceso |
| Flujo Alternativo:| 2A. Si los datos no son validos, se muestra el mensaje: "Datos invalidos" <br>3A. Si no se ha podido acceder a la base de datos, se muestra el mensaje: "No se ha podido acceder a la base de datos" |
| Poscondiciones:| El usuario se ha dado de alta y se ha notificado |

<br>

| INF-004 ||
|:------------|:----------------|
| Nombre: | Dar de alta estudiante |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un usuario verificado como PAS da de alta un usuario estudiante |
| Datos específicos:| <ul><li>Usuario PAS</li><li>DNI estudiante</li><li>Nombre y apellidos estudiante</li><li>Fecha de nacimiento estudiante</li><li>Sexo</li><li>Dirección</li><li>Telefono</li><li>Correo electronico</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |

<br>

| UC-05 ||
|:------------|:----------------|
| Nombre: | Dar de alta estudiante (PDI)|
| Autor: | Francisco Javier Mota López |
| Fecha: | 28/10/2022 |
|Descripcion:| Un actor puede dar de alta a un usuario|
| Actores:| PDI |
| Precondiciones:| Usuario registrado como usuario PAS |
| Flujo Normal:| 1a. Se introducen los datos del usuario a dar de alta <br>2. Se validan los datos del usuario<br>3. Se guarda el usuario en la base de datos dandole de alta en este proceso |
| Flujo Alternativo:| 1b. Se busca en la lista de la clase al estudiante <br> 2A. Si los datos no son validos, se muestra el mensaje: "Datos invalidos" <br>3A. Si no se ha podido acceder a la base de datos, se muestra el mensaje: "No se ha podido acceder a la base de datos" |
| Poscondiciones:| El usuario se ha dado de alta y se ha notificado |

<br>

| UC-6|  |
| :---------- | ------------------------------------ |
| Nombre: | Buscar estudiantes en la lista de clase|
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  | Permite buscar estudiantes en la lista de la clase por asignatura|
| Actores: Personal PDI|
| Precondiciones: | El usuario tiene que estar autentificado en el sistema |
| Flujo Normal: | 1. El actor accede a la asignatura específica <br> 2. El actor accede al listado de la clase <br> 3. El actor busca en la clase el estudiante específico   |
| Flujo Alternativo: | |
| Poscondiciones: | Estudiante encontrado|

<br>

|UC-7||
| ----------- | ----------- |
| Nombre | Proponer cambios en los horarios |
| Autor |   Angel Nieto Burgos |
| Fecha |30/09/2022   |
| Descripcion | En una universidad, el personal del PDI pueden proponer cambios en los horarios. 
| Actores |   El personal del PDI  |
| precondicion |   Inicio sesion  y datos verificados  |
| flujo normal   |  1  introducir cambios<br>  2  seleccionar boton  <br>  3 proponer cambios en los horarios <br> 4 verificación de los datos del estudiante <br>|
| flujo alternativo | |
| poscondiciones |   Se ha realizado la propuesta correctamente


<br>

# A1E2

| UC-01 ||
|:------------|:----------------|
| Nombre: | Acordar precio |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
|Descripcion:| Negociación del precio que tendrá el procucto |
| Actores:| Vendedor y Comprador |
| Precondiciones:| realizar venta |
| Flujo Normal:| 1. Se acuerda el precio entre ambos actores <br> 2. Se realiza venta del producto |
| Flujo Alternativo:| 1A. En caso de no llegar a un acuerdo entre actores no se realizará la venta |
| Poscondiciones:| 1. Se realiza la venta <br> 2. Se guarda en la base de datos |

| INF-001: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Negociación del precio que tendrá el procucto |
| Datos especificos:|  <ul><li>Comprador</li><li>Nombre articulo</li><li>Vendedor</li><li>Precio default</li><li>Stock</li><li>Disponibilidad</li></ul>  |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-02 ||
|:------------|:----------------|
| Nombre: | Eliminar oferta |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
|Descripcion:| Proceso por el cual se cancela una oferta de un producto dado por el proovedor |
| Actores:| Provedor |
| Precondiciones:| avisar fin de la oferta |
| Flujo Normal:| 1. Se avisa del final de la oferta <br> 2. Se elimina la oferta del producto |
| Flujo Alternativo:| - |
| Poscondiciones:| La oferta quedará eliminada de la lista de ofertas |

| INF-002: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual se cancela una oferta de un producto dado por el proovedor |
| Datos especificos:| <ul><li>Descripción oferta</li><li>Fecha oferta</li><li>Estado oferta</li><li>Identificador oferta</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-03 ||
|:------------|:----------------|
| Nombre: | Eliminar productos |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
|Descripcion:| Proceso por el cual el administrador elimina productos existentes |
| Actores:| Administrador |
| Precondiciones:| La existencia de un producto |
| Flujo Normal:| 1.Se elimina producto existente |
| Flujo Alternativo:|  |
| Poscondiciones:| El producto que teniamos ha sido borrado |

| INF-003: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual el administrador elimina productos existentes |
| Datos especificos:| <ul><li>Datos producto</li><li>Identificador producto</li><li>Estado producto</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-04 ||
|:------------|:----------------|
| Nombre: | Incoporar oferta |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
|Descripcion:| Consiste en tras un aviso incorporar una oferta a la lista de ofertas |
| Actores:| Proveedor |
| Precondiciones:| Avisar de nuevos productos |
| Flujo Normal:| 1.Avisar de oferta <br> 2.Incorporar oferta |
| Flujo Alternativo:| 1A. No hay aviso de oferta |
| Poscondiciones:| La oferta queda incorporada |


| INF-004: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Consiste en tras un aviso incorporar una oferta a la lista de ofertas |
| Datos especificos:| <ul><li>Descripción oferta</li><li>Fecha oferta</li><li>Estado oferta</li><li>Identificador oferta</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-05 ||
|:------------|:----------------|
| Nombre: | Validar disponibilidad |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
| Descripcion:| Proceso por el cual el producto consultado muestra su estado de disponibilidad |
| Actores:| Comprador |
| Precondiciones:| Consultar producto |
| Flujo Normal:| 1. Consultar producto <br> 2. Verificar disponibilidad |
| Flujo Alternativo:| 1A. Producto no encontrado |
| Poscondiciones:| El producto consultado muestra su disponibildad en el momento de la consulta |


| INF-005: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual el producto consultado muestra su estado de disponibilidad |
| Datos especificos:| <ul><li>Datos productos</li><li>Fecha producto</li><li>Estado producto</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

|UC-06||
| ----------- | ----------- |
| Nombre | Enviar Notificación |
| Autor |   Angel Nieto Burgos |
| Fecha |14/10/2022   |
| Descripcion | Notificación de proveedores cuando se termina una ofeta o cuando se avisa  que le queda poco. 
| actores |   proveedores.|
| precondicion |  Tener que realizar un aviso  |
| flujo normal   |  1 seleccionar tipo de notificacion  <br>  2 preparar notificacion de fin de oferta   <br> 3 enviarla <br> |
| flujo alternativo | 2b preparar notificacion elminacion de oferta 
| poscondiciones |


| INF-006: |  |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual el producto consultado muestra su estado de disponibilidad |
| Datos especificos:| <ul><li>Datos productos</li><li>Fecha producto</li><li>Estado producto</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

|UC-7||
| ----------- | ----------- |
| Nombre | Consultar ofertas |
| Autor |   Angel Nieto Burgos |
| Fecha |21/10/2022   |
| Descripcion | En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. 
| actores |   El comprador, el vendedor, los proveedores  y los administradores   |
| precondicion ||
| flujo normal   |  1 seleccionar boton <br>  2 recopilar ofertas <br> 3 Devolver horario <br> |
| flujo alternativo | 
| poscondiciones |

|UC-8||
| ----------- | ----------- |
| Nombre | consultar Productos |
| Autor |   Angel Nieto Burgos |
| Fecha |07/10/2022   |
| Descripcion | comprador y administrador pueden ver ofertas. 
| actores |   comprador y administrador.|
| precondicion |   inicio sesion y consultar precios   |
| flujo normal   |  1 seleccionar boton <br>  2 consultar productos <br> 3 mostrar datos productos <br> |
| flujo alternativo || 
| poscondiciones ||


| UC-10|  |
| :---------- | ------------------------------------ |
| Nombre: |  Buscar productos|
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  |Buscar productos en la página de compras |
| Actores: | Proveedor, Comprador, Vendedor, Administrador|
| Precondiciones: |  El usuario debe estar identificado |
| Flujo Normal: |1. Acceder al buscador <br> 2. Escribir el producto que se busca <br> 3. El sistema despliega una lista de coincidencias con los productos |
| Flujo Alternativo: | 3. El sistema no encuentra ningún producto que coincida con el criterio de búsqueda y permite al usuario volver a realizar una búsqueda|
| Poscondiciones: |La búsqueda ofrece productos que coinciden con la búsqueda con mucha certeza |

| INF-010| Buscar productos|
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Buscar productos |
| Descripción:| El sistema deberá mostrar una lista de productos que coincidan con la búsqueda realizada y las especificaciones de cada uno |
| Datos especificos:| -Nombre del producto <br> -Precio del producto <br> -Imagen del producto <br> -Tipo de producto <br> -Especificaciones del producto <br> -Disponibilidad del producto |
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-11|  |
| :---------- | ------------------------------------ |
| Nombre: | Avisar de fin de oferta |
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  |Se avisa de que una oferta ha finalizado |
| Actores: |Proveedor |
| Precondiciones: |Oferta terminada |
| Flujo Normal: |1. Se elimina la oferta <br> 2. Se manda una notificación con el aviso de oferta terminada |
| Flujo Alternativo: | |
| Poscondiciones: | La oferta se ha eliminado correctamente y se ha avisado correctamente de ello|

| INF-011 | Fin de ofertas |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Avisar de fin de oferta |
| Descripción:| El proveedor deberá informar sobre la oferta que ha finalizado |
| Datos especificos:| -Nombre de oferta <br> -Fecha de inicio de oferta <br> -Fecha de fin de oferta <br> -Productos afectados por la oferta <br > -Porcentaje de descuento <br> -Precio antiguo de los productos <br> -Precio de los productos en oferta |
| Importancia:|  |
| Estado:| Aceptado |
| Comentar:| - |

| UC-12|  |
| :---------- | ------------------------------------ |
| Nombre: | Agregar productos|
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  |Agrega productos al carrito de la compra |
| Actores: |Comprador |
| Precondiciones: |El usuario debe estar autenticado en el sistema |
| Flujo Normal: | 1. Se marca el producto como bloqueado <br> 2. Una vez que está bloqueado, se agrega el producto al carrito|
| Flujo Alternativo: | |
| Poscondiciones: | El producto ha sido añadido correctamente al carrito|



| UC-13|  |
| :---------- | ------------------------------------ |
| Nombre: | Consultar histórico de ventas |
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 14-10-22|
| Descripción:  | Permite consultar las ventas pasadas durante la realización de una venta |
| Actores: | Vendedor, Comprador |
| Precondiciones: | Se está dando una venta entre un vendedor y un comprador |
| Flujo Normal: | 1. Se accede al histórico de ventas <br> 2. El sistema muestra una lista de las ventas pasadas <br> 3. Consultar ventas|
| Flujo Alternativo: | |
| Poscondiciones: | El sistema muestra correctamente todas las ventas pasadas|

| INF-013 | Histórico de ventas |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Consultar histórico de ventas |
| Descripción:| Permite consultar el histórico de ventas durante la realización de una|
| Datos especificos:| <ul><li>ID venta actual</li> <li>Identificador de venta</li><li>Productos vendidos</li><li>Nombre productos</li><li>Cantidad del producto</li><li>Precio de cada producto</li><li>Precio total de la venta</li></ul> |
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| UC-14 ||
|:------------|:----------------|
| Nombre: | Avisar de nuevos productos |
| Autor: | Juanra |
| Fecha: | 30/09/2022 |
|Descripcion:| Un usuario puede agregar nuevos productos |
| Actores:| Proveedor |
| Precondiciones:| Articulos no registrados |
| Flujo Normal:| 1. Se indica que existen nuevos objetos para añadir |
| Flujo Alternativo:| 1A. Los objetos se ponen de oferta |
| Poscondiciones:| Se añaden los objetos al listado |


| IR-014 ||
|:------------|:----------------|
| Nombre: | Avisar de nuevos productos |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un proveedor indica que tiene nuevos articulos |
| Datos específicos:| <ul><li>Proveedor</li><li>Lista de nuevos articulos</li><li>Precio de cada articulo</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |

| UC-15 ||
|:------------|:----------------|
| Nombre: | Bloquear productos |
| Autor: | Juanra |
| Fecha: | 30/09/2022 |
|Descripcion:| Un usuario puede bloquear un producto |
| Actores:| Comprador |
| Precondiciones:| Existencia del articulo a bloquear |
| Flujo Normal:| 1. Se busca el articulo a bloquear <br> 2. Se selecciona el articulo a bloquear <br> 3. Se marca el articulo como bloqueado |
| Flujo Alternativo:| - |
| Poscondiciones:| El articulo bloqueado no aparece en la lista de articulos disponibles |


| INF-015 ||
|:------------|:----------------|
| Nombre: | Bloquear productos |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un comprador bloquea un articulo |
| Datos específicos:| <ul><li>Comprador</li><li>articulo</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |

| UC-16 ||
|:------------|:----------------|
| Nombre: | Consultar precio |
| Autor: | Juanra |
| Fecha: | 30/09/2022 |
|Descripcion:| Un usuario puede visualizar el precio de un producto |
| Actores:| Comprador, Vendedor, Administrador, Proveedor |
| Precondiciones:| Articulos existente |
| Flujo Normal:| 1. Se busca el producto a consultar <br> 2. Se selecciona el producto <br> 3. Se muestra el precio del producto |
| Flujo Alternativo:| - |
| Poscondiciones:| - |


| IR-016 ||
|:------------|:----------------|
| Nombre: | Consultar precio |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un usuario consulta el precio de un articulo |
| Datos específicos:| <ul><li>Usuario</li><li>Articulo a consultar</li><li>Precio del articulo</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |

| UC-17 ||
|:------------|:----------------|
| Nombre: | Finalizar compra |
| Autor: | Juanra |
| Fecha: | 30/09/2022 |
|Descripcion:| Un usuario puede finalizar la compra |
| Actores:| Comprador, Vendedor, Administrador, Proveedor |
| Precondiciones:| Ha de tener articulos en la cesta de la compra |
| Flujo Normal:| 1. Se pulsa el boton de pagos <br>2. Se accede a la pasarela de pagos<br>3. Se rellenan los datos de la pasarela de pagos<br>4. Se pulsa el boton para pagar<br>5. Se verifica el pago<br>6. Se crea el pedido |
| Flujo Alternativo:| 1A. Si la cesta esta vacia, se muestra el mensaje: "Cesta vacia" <br>5A. Si no se ha verificado la compra, se muestra el mensaje: "No se ha podido verificar la compra" |
| Poscondiciones:| Se registra la compra en la base de datos |


| IR-017 ||
|:------------|:----------------|
| Nombre: | Finalizar compra |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un usuario finaliza la compra |
| Datos específicos:| <ul><li>Usuario</li><li>Lista de objetos a pagar</li><li>Precio total</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |

**Requisitos de información**

| INF-001 | Producto |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Agregar productos, Buscar productos, Eliminar productos, Consultar precios, Avisar de nuevos productos, Bloquear productos, Consultar productos, Finalizar compra, Verificar disponibilidad, Realizar venta, Consultar histórico de ventas|
| Descripción:| Información importante de los productos |
| Datos especificos:| <ul> <li> ID producto </li> <li>Nombre del producto </li> <li> Imagen del producto </li>  <li>Tipo de producto </li> <li>Precio del producto </li> <li> Descripción del producto </li> <li>Disponibilidad del producto </li> <li> Valoración del producto</li> <li> ID de oferta </li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-002 | Vendedor |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Realizar venta, Acordar precio, Consultar histórico de ventas, Buscar productos, Consultar precios, Consultar ofertas|
| Descripción:| Datos del vendedor |
| Datos especificos:| <ul> <li> ID vendedor</li> <li> Nombre del vendedor</li> <li>Imagen del vendedor</li> <li>ID producto</li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-003 | Comprador |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Agregar productos, Bloquear productos, Consultar productos, Verificar disponibilidad, Finalizar compra, Realizar venta|
| Descripción:| Información importante del comprador|
| Datos especificos:| <ul> <li> ID comprador</li> <li> Nombre del comprador</li> <li>Imagen del comprador</li> <li>ID carrito</li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-004 | Proveedor |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Consultar precios, Consultar ofertas, Buscar productos, Avisar de nuevos productos, Incorporar oferta, Avisar, Avisar de fin de oferta, Eliminar oferta, Enviar notificación |
| Descripción:| |
| Datos especificos:| <ul> <li> ID proveedor</li> <li> Nombre del proveedor</li> <li>Imagen del proveedor</li> <li>Lista productos</li> <li>ID oferta</li> <li>ID notificación</li></ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-005 | Administrador |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Eliminar productos |
| Descripción:| Datos importantes del administrador |
| Datos especificos:| <ul> <li> ID Administrador</li> <li> Nombre administrador</li> <li>Imagen del administrador</li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-006 | Oferta |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Incorporar oferta, Eliminar oferta, Avisar de fin de oferta, Avisar de nuevos productos, Consultar productos, Buscar productos, Realizar venta, Consultar ofertas |
| Descripción:| Información importante que tiene cada oferta|
| Datos especificos:| <ul> <li> ID Oferta</li> <li> Nombre de la oferta</li> <li>Lista de productos con la oferta</li> <li> Descuento aplicado </li> <li> Fecha de inicio de oferta </li> <li> Fecha final de la oferta </li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-007 | Notificación |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Enviar notificación, Avisar, Avisar de fin de oferta, Avisar de nuevos productos |
| Descripción:| Información importante sobre el contenido de una notificación|
| Datos especificos:| <ul> <li> ID Notificación</li> <li> Asunto de la notificación</li> <li>Contenido notificación</li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-008 | Ventas |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Realizar venta, Acordar precio, Consultar histórico de ventas |
| Descripción:| Información esencial sobre las ventas |
| Datos especificos:| <ul> <li> ID Venta</li> <li> Lista productos</li> <li>Coste total de la venta</li> <li>ID Comprador</li> <li> ID Vendedor</li></ul> |
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

| INF-009 | Carrito |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Agregar productos, Bloquear productos |
| Descripción:| Datos necesarios para el carrito |
| Datos especificos:| <ul> <li> ID Carrito</li> <li> Lista productos</li> <li>Coste total del carrito</li> <li>ID Comprador</li> </ul>|
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |