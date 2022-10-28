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

| INF-012 | Producto |
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| Agregar productos |
| Descripción:| El comprador selecciona un producto y lo agrega al carrito |
| Datos especificos:| -Nombre del producto <br> -Imagen del producto <br> -Tipo de producto <br > -Precio del producto <br> -Especificaciones del producto <br> -Disponibilidad del producto |
| Importancia:| Muy importante |
| Estado:| Aceptado |
| Comentar:| - |

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


