| UC-01 ||
|:------------|:----------------|
| Nombre: | Validar datos |
| Autor: | Francisco de Borja Gutiérrez |
| Fecha: | 07/10/2022 |
|Descripcion:|Se validan los datos insertados por el estudiante|
| Actores:| PAS |
| Precondiciones:| Rellenar el alta de los estudiantes |
| Flujo Normal:| 1. Se introducen los datos del usuario a dar de alta <br>2. Se validan los datos del usuario |
| Flujo Alternativo:| 2A. Si los datos no son validos, se muestra el mensaje: "Datos invalidos" |
| Poscondiciones:| Validación de los datos anteriores |

| IR-01 ||
|:------------|:----------------|
| INF-010: | PAS |
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

| IR-01 ||
|:------------|:----------------|
| INF-010: |  |
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Negociación del precio que tendrá el procucto |
| Datos especificos:|  <ul><li>Comprador</li><li>Nombre articulo</li><li>Vendedor</li><li>Precio default</li><li>Stock</li><li>Disponibilidad</li></ul>  |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

| UC-01 ||
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

| IR-01 ||
|:------------|:----------------|
| INF-010: |  |
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual se cancela una oferta de un producto dado por el proovedor |
| Datos especificos:| <ul><li>Descripción oferta</li><li>Fecha oferta</li><li>Estado oferta</li><li>Identificador oferta</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

| UC-01 ||
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

| IR-01 ||
|:------------|:----------------|
| INF-010: |  |
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual el administrador elimina productos existentes |
| Datos especificos:| <ul><li>Datos producto</li><li>Identificador producto</li><li>Estado producto</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

| UC-01 ||
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

| IR-01 ||
|:------------|:----------------|
| INF-010: |  |
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Consiste en tras un aviso incorporar una oferta a la lista de ofertas |
| Datos especificos:| <ul><li>Descripción oferta</li><li>Fecha oferta</li><li>Estado oferta</li><li>Identificador oferta</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |

<br>

| UC-01 ||
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

| IR-01 ||
|:------------|:----------------|
| INF-010: |  |
| Versión: | 1.0 (Octubre-2022) |
| Autor: | Francisco de Borja Gutiérrez |
| Fuente:| - |
| Referencia:| - |
| Descripción:| Proceso por el cual el producto consultado muestra su estado de disponibilidad |
| Datos especificos:| <ul><li>Datos productos</li><li>Fecha producto</li><li>Estado producto</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentar:| - |
