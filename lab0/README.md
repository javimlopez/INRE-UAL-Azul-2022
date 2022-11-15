# :large_blue_circle: LAB0 :large_blue_circle: EQUIPO AZUL :large_blue_circle:

## Supuesto 1

### Enunciado

En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

<br><img src=./svgs/supuesto1.svg>
<br>

## Supuesto 2

### Enunciado

En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.

<br><img src=./svgs/supuesto2.svg>
<br>

## Supuesto 3

### Enunciado

En una compañía hotelera, el administrador y el comercial pueden consultar reservas. El comercial realiza ofertas y gestiona nuevas reservas. El administrador gestiona nuevas peticiones y también realiza ofertas. La realización de ofertas por parte del comercial conlleva un recálculo de precios. Además, dicha realización de ofertas conlleva opcionalmente el bloqueo temporal de una reserva. Los clientes, los administradores y los comerciales pueden consultar disponibilidades y visualizar ofertas. La consulta de disponibilidades y la consulta de reservas tienen la funcionalidad común de buscar elementos. Por su parte, la consulta de disponibilidades conlleva una funcionalidad que muestra un calendario.

<br><img src=./svgs/supuesto3.svg>
<br>

## Supuesto 4

### Enunciado

En una aplicación de fotografía online, los clientes pueden visualizar las fotos, donde de forma excepcional se puede realizar una denuncia sobre la foto. Al denunciar una foto, se ha de introducir una explicación sobre la denuncia. Los clientes también pueden llevar a cabo consultas sobre las fotos, operación que es un caso particular de visualizar las fotos. Los controladores de fotos pueden indicar que una foto debe ser revisada. Esta funcionalidad es un caso general de la funcionalidad de denunciar foto. Además, los controladores también pueden editar la información de las fotos. En esta aplicación también participan usuarios de tipo vendedor. Los vendedores pueden escribir a los clientes para hacerles ofertas sobre los productos de la aplicación. De forma excepcional, al hacer una oferta pueden reducir el precio de un producto. Los vendedores también pueden buscar detalles en las fotos, operación que es un caso particular de visualizar fotos. Pero esa búsqueda conlleva la verificación de los datos introducidos. Por otro lado, los gestores de la aplicación pueden ver ofertas, bloquear ofertas, emitir facturas y editar facturas. La emisión de facturas requiere la participación de un software de facturación. El administrador de la tienda puede ver ofertas, emitir facturas, editar facturas, bloquear ofertas, crear usuarios y editar usuarios. Esta funcionalidad de ver ofertas también la pueden realizar los clientes. Editar usuarios tiene características en común con editar facturas. Crear usuarios conlleva el envío de un email en el que es necesario el uso de un gestor de correo.

<br><img src=./svgs/supuesto4.svg>
<br>

## Supuesto 5

### Enunciado

En un sistema de gestión de incidencias, los técnicos y los operadores pueden dar de alta incidencias, para lo cual, de forma excepcional se enviará un correo (en esta operación participa un sistema de gestión de correo). Los técnicos también atienden llamadas telefónicas y realizan informes sobre las incidencias. Por su parte, los operadores atienden llamadas telefónicas, marcan incidencias como duplicadas y ordenan incidencias. La forma de atender llamadas de los técnicos y los operadores no es exactamente igual, pero tiene similitudes. De forma específica, cuando los técnicos atienden llamadas, comprueban datos de la incidencia en el sistema. Cuando los operadores atienden llamadas, introducen nuevos datos de la incidencia. Los administradores del sistema gestionan categorías de incidencias, consultan incidencias y ordenan incidencias. La ordenación por parte de los administradores conlleva la adición de un comentario. Los técnicos y los operadores también pueden consultar incidencias. La consulta de incidencias por parte técnicos, operadores y administradores puede conllevar, de forma excepcional, la edición de los datos de la incidencia. Los usuarios invitados también pueden consultar incidencias, pero sin la posible edición de los datos. Además, los invitados informan sobre posibles incidencias, se pueden registrar para ver notificaciones y pueden acceder a un listado del histórico de notificaciones. El informe de posibles incidencias conlleva el dar de alta la localización en un mapa, la incorporación de una explicación completa en formato textual y la subida de una foto.

<br><img src=./svgs/supuesto5.svg>
<br>

## Supuesto GD

### Enunciado

El usuario puede elegir hacer la matrícula de nuevo ingreso, continuación de estudios o finalización de estudios. La automatrícula le pide al estudiante que inicie sesión (usuario y contraseña)
La automatrícula de la ual accede a los datos que tiene guardados sobre la persona que inicia sesión en la plataforma, en el caso de que no tenga ningún dato sobre el usuario que accede, los pide. Dentro de la plataforma, la automatrícula ofrece las posibilidades a las que el usuario puede matricularse. El usuario selecciona las opciones en las que quiere matricularse, excepto si es el primer año, ya que el primer año está obligado a matricularse en las asignaturas asociadas al primer curso del grado seleccionado por el alumno. La matriculación ofrece tres posibilidades al principio, a tiempo completo, a tiempo parcial y finalización de estudios. Cuando el usuario/alumno ha seleccionado las opciones en la que se va a matricular (la matrícula se divide en el número de cursos al que pertenece cada asignatura, en cada asignatura se indica el número de plazas disponibles para cada grupo docente, el número de convocatoria y matrícula , muestra un formulario preguntando por datos personales del usuario como son familia numerosa, opción a becas, cuenta bancaria, etc. Al terminar este formulario, esta plataforma realiza los cálculos del coste de la matrícula asociada a lo seleccionado por el usuario. Para finalizar, la plataforma muestra un calendario con el horario provisional de las asignaturas seleccionadas por el alumno.
-Datos personales y familiares (discapacidades, empleos, residencia, víctima de violencia de género…).
-Encuesta de satisfacción con la Universidad de Almería.
-Review de horarios (dependiendo de las asignaturas escogidas, el calendario muestra un mensaje de solapamiento si existen conflictos entre las asignaturas y muestra qué asignaturas son las que se solapan y donde y el número de matriculación y convocatoria usada hasta ahora)
-Selección de asignaturas y horarios divididos por cursos (notificación del cuatrimestre donde se cursa dicha asignatura, disponibilidad de plazas y división en grupos / elección de grupos docentes)
-Datos de becas (Selección de beca MEC si se dispone de ella y en caso de no superar las asignaturas mínimas aprobadas el año pasado salta un mensaje de error donde no permite seleccionarla, en su defecto se puede seleccionar la bonificación 99% de la junta de Andalucía)

<br><img src=./svgs/supuestoGD.svg>
<br>

## Autores

:large_blue_diamond: FRANCISCO DE BORJA JOSE GUTIERREZ CARRASCO<br>
:large_blue_diamond: FRANCISCO JAVIER MOTA LOPEZ<br>
:large_blue_diamond: JUAN RAUL MELLADO GARCIA<br>
:large_blue_diamond: ANGEL NIETO BURGOS
