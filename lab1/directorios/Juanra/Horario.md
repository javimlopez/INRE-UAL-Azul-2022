| UC-03 ||
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


|UC-1 DatosUsuario||
| ----------- | ----------- |
| Nombre |  Horarios |  
|Referencia| consultar horarios,proponer cambios en los horarios,Dar de alta datos,validar datos.|
|Informacion|Los datos que son necesarios para el funcionamiento de los inicios de sesion  |
|Datos especificos|1 nombre y apelllidos <br>  ID <br> Asignatiras<br> fecha matriculacion <br> cargo<br> DNI estudiante<br> Fecha de nacimiento<br> correo electrico<br> Direccion<br> telefono<br> sexo<br>|
|Importancia|Muy Importantes|
|Estado||
|Comentarios||
