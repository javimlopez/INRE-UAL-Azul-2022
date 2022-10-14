| UC-XX ||
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


| IR-XX ||
|:------------|:----------------|
| Nombre: | Finalizar compra |
| Autor: | Juanra |
| Version: | 1.0 |
| Descripcion:| Un usuario finaliza la compra |
| Datos específicos:| <ul><li>Usuario</li><li>Lista de objetos a pagar</li><li>Precio total</li></ul> |
| Importancia:| Importante |
| Estado:| Aceptado |
| Comentarios:| - |