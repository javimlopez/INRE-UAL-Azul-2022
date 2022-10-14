



| UC-|  |
| :---------- | ------------------------------------ |
| Nombre: |  |
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  | |
| Actores: | |
| Precondiciones: |  |
| Flujo Normal: |   |
| Flujo Alternativo: | |
| Poscondiciones: | |

| UC-|  |
| :---------- | ------------------------------------ |
| Nombre: |  Buscar productos|
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 07-10-22|
| Descripción:  |Buscar productos en la página de compras |
| Actores: | Proveedor, Comprador, Vendedor, Administrador|
| Precondiciones: |  El usuario debe estar identificado |
| Flujo Normal: |1. Acceder al buscador <br> 2. Escribir el producto que se busca <br> 3. El sistema despliega una lista de coincidencias con los productos |
| Flujo Alternativo: | |
| Poscondiciones: |La búsqueda ofrece productos que coinciden con la búsqueda con mucha certeza |

| UC-|  |
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

| UC-|  |
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

| UC-|  |
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

**Requisitos de información**

| INF-010 ||
|:------------|:----------------|
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco Javier Mota López |
| Fuente:| - |
| Referencia:| - |
| Descripción:|  |
| Datos especificos:|  |
| Importancia:|  |
| Estado:| Aceptado |
| Comentar:| - |
