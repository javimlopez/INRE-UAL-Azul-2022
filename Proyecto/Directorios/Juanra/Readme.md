| UC-01               |   |
| :----------------- | - |
| Nombre:            | Enviar alarma  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la creación y envio de alarmas del sistema|
| Actores:           | Sistema de monitorizacion |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. El sistema recibe un evento a avisar <br> 2. El sistema crea una alarma <br> 3. El sistema envia una alarma a los destinatarios  |
| Flujo Alternativo: |  - |
| Poscondiciones:    |  - |

| UC-02                |   |
| :----------------- | - |
| Nombre:            | Recabar informacion en tiempo real Operadores  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad del sistema para conocer los datos en tiempo real de los operadores de transporte  |
| Actores:           | Sistema de monitorizacion |
| Precondiciones:    | Operador de transporte habilitado en el sistema  |
| Flujo Normal:      | 1. El operador de transporte activa el dispositivo de seguimiento <br> 2. El dispositivo envia constantemente los datos del operador de transporte y su posición <br> 3. El sistema recibe estos datos |
| Flujo Alternativo: | 3A. El sistema deja de recibir la informacion <br> 3.1A. El sistema muestra el mensaje "operador de transporte deslocalizado"  |
| Poscondiciones:    | -  |

| UC-03                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad del sistema de mostrar el mapa  |
| Actores:           | Sistema de monitorizacion  |
| Precondiciones:    | Usuario administrador registrado en el sistema. Mapa creado en el sistema. Información sobre el mapa |
| Flujo Normal:      | 1. El sistema organiza la informacion del mapa <br> 2. El sistema crea el mapa con la informacion de los operadores de transporte que se le ha añadido |
| Flujo Alternativo: | 2A. El sistema puede no localizar algo en el mapa por un error al introducir los datos <br> 2.1A El sistema muestra que hay un error en la informacion introducida  |
| Poscondiciones:    |   |

| UC-04                |   |
| :----------------- | - |
| Nombre:            | Gestion de pagos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la gestion que realiza el sistema al recibir un pago  |
| Actores:           | Sistema de monitorizacion |
| Precondiciones:    | Un cliente realiza un pago  |
| Flujo Normal:      | 1. El sistema comprueba que el pago se ha realizado correctamente <br> 2. El sistema busca en la base de datos al cliente <br> 3. El sistema añade el articulo asociado al pago realizado  |
| Flujo Alternativo: | 1A. El pago no se ha realizado correctamente <br> 1.1A. El sistema muestra el mensaje "El pago no se ha realizado correctamente" <br> 2A. El sistema no encuentra al cliente <br> 2.1A. El sistema muestra el mensaje "cliente no encontrado" <br> 2.2A. El sistema realiza la devolucion del importe pagado |
| Poscondiciones:    | Articulo añadido en la base del cliente que ha realizado el pago  |

| UC-05                |   |
| :----------------- | - |
| Nombre:            | Visualizar Mapa (Admin)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad del administrador de ver el mapa con los datos de los operadores sobre el |
| Actores:           | Administrador  |
| Precondiciones:    | Usuario administrador registrado en el sistema. Mapa creado en el sistema. Información sobre el mapa  |
| Flujo Normal:      | 1. El sistema organiza la informacion del mapa <br> 2. El sistema crea el mapa con la informacion de los operadores de transporte que se le ha añadido  <br> 3. El sistema muestra el mapa con la iformacion asociada |
| Flujo Alternativo: | 2A. El sistema puede no localizar algo en el mapa por un error al introducir los datos <br> 2.1A El sistema muestra que hay un error en la informacion introducida <br> 3A. El administrador recibe el aviso de una situacion inusual/puntual <br> 3A.1. El administrador añade dicha situacion a la informacion del mapa <br> 3A.2. El sistema modifica la informacion que se muestra en el mapa <br> 3B. Un administrador accede al mapa <br> 3.1B. El sistema registra toda la informacion de lo que va pasando <br> 3.1B.1. El sistema no tiene espacio para realizar el registro de la informacion. <br> 3.1B.2. El sistema muestra el mensaje "No hay espacio suficiente" <br>  |
| Poscondiciones:    | El sistema guarda la informacion registrada, Se cambia la informacion del mapa|

| UC-06                |   |
| :----------------- | - |
| Nombre:            | Registrar periodos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad de registrar un periodo concreto  |
| Actores:           | Administrador  |
| Precondiciones:    | Usuario administrador registrado en el sistema  |
| Flujo Normal:      | 1. Un administrador accede al mapa <br> 2. El sistema registra toda la informacion de lo que va pasando |
| Flujo Alternativo: | 3A. El sistema no tiene espacio para realizar el registro de la informacion. <br> 3.1A. El sistema muestra el mensaje "No hay espacio suficiente"  |
| Poscondiciones:    | El sistema guarda todo lo transcurrido en el periodo de tiempo grabado  |

| UC-07                |   |
| :----------------- | - |
| Nombre:            | Registrar situaciones  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Flujo alternativo de UC-05. Registra situaciones inusuales/puntuales comunicadas al administrador   |
| Actores:           | Administrador  |
| Precondiciones:    | Sucesión de una situacion inusual/puntual y comunicada dicha situacion  |
| Flujo Normal:      | 1. El administrador recibe el aviso de una situacion inusual/puntual <br> 2. El administrador añade dicha situacion a la informacion del mapa <br> 3. El sistema modifica la informacion que se muestra en el mapa  |
| Flujo Alternativo: | - |
| Poscondiciones:    | Se cambia la informacion del mapa  |

| UC-08                |   |
| :----------------- | - |
| Nombre:            | Definir evento  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Añade un evento al sistema  |
| Actores:           | Administrador  |
| Precondiciones:    | Evento existente  |
| Flujo Normal:      | 1. El administrador accede al sistema <br> 2. El administrador accede al aparatado de creacion de eventos <br> 3. Se cumplen las condiciones del evento <br> 4. Se genera la alarma del aviso <br> 5. Se envia la alarma al sistema |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Se añade el evento a la base de datos  |

| UC-09                |   |
| :----------------- | - |
| Nombre:            | Generar aviso  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que genera una alarma especifica de un evento  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se cumplen las condiciones del evento <br> 2. Se genera la alarma del aviso <br> 3. Se envia la alarma al sistema  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | - |

| UC-10                |   |
| :----------------- | - |
| Nombre:            | SMS  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Si la apliacion se encuentra cerrada, se envia un sms al cliente  |
| Actores:           | Operador de transporte, Cliente, Administrador |
| Precondiciones:    | El cliente ha seleccionado sms como metodo de aviso. Apliacion cerrada  |
| Flujo Normal:      | 1. La aplicacion esta cerrada <br> 2. Se envia un sms al cliente  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-11                |   |
| :----------------- | - |
| Nombre:            | Visualizar alarma  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Visualiza una alarma recibida  |
| Actores:           | Operador de transporte, Cliente, Administrador  |
| Precondiciones:    | Alarma enviada por el sistema  |
| Flujo Normal:      | 1. Se comprueba que la aplicacion se encuetra abierta <br> 2. Se muestra por pantalla una notificacion visual  |
| Flujo Alternativo: | 1A. La aplicacion esta cerrada <br> 1A.1. Se envia un aviso sonoro al cliente <br> 1B. La aplicacion esta cerrada <br> 1B.1. Se envia un sms al cliente  |
| Poscondiciones:    |  - |

| UC-12                |   |
| :----------------- | - |
| Nombre:            | Aviso sonoro  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Si la apliacion se encuentra cerrada, se envia un aviso sonoro al cliente  |
| Actores:           | Operador de transporte, Cliente, Administrador |
| Precondiciones:    | El cliente ha seleccionado aviso sonoro como metodo de aviso. Apliacion cerrada  |
| Flujo Normal:      | 1. La aplicacion esta cerrada <br> 2. Se envia un aviso sonoro al cliente  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-13                |   |
| :----------------- | - |
| Nombre:            |Ayuda en linea (SMET)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion de ayuda en linea de uso general |
| Actores:           |Operadores de transporte , Clientes, Administradores  |
| Precondiciones:    | Informacion de ayuda añadida a la base de datos  |
| Flujo Normal:      | 1. El usuario consulta la informacion correspondiente a sus necesidades  |
| Flujo Alternativo: | 1A. El usuario no encuentra la informacion que necesita <br> 1.1A. El usuario se pone en contacto con AUTGC para indicar su duda <br> 1.1A.1 Se añade un apartado nuevo  |
| Poscondiciones:    | Se almacenan los nuevos apartados |

| UC-14                |   |
| :----------------- | - |
| Nombre:            | Realizar pagos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Se realiza el pago de un billete  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se selecciona el tipo de billete a comprar <br> 2. Se accede al portal de pagos <br> 3. Se introducen los datos de pago <br> 4. Se realiza el pago <br> 5. Se verifica que el pago se ha realizado correctamente  |
| Flujo Alternativo: | 5A. No se realiza el pago correctamente <br> 5A.1. Se muestra el mensaje "No se ha realizado el pago correctamente"  |
| Poscondiciones:    | Se asocia el billete al cliente  |

| UC-15                |   |
| :----------------- | - |
| Nombre:            | Mostrar itinerarios en mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Una opcion de visualizacion del itinerario ya definido por el cliente  |
| Actores:           | Cliente  |
| Precondiciones:    | itinerario definido por el cliente  |
| Flujo Normal:      | 1. El itinerario se muestra en el mapa  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-16               |   |
| :----------------- | - |
| Nombre:            | Definir itinerario  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el cliente introduce los datos de itinerario para que el sistema calcule el itinerario mas recomendable |
| Actores:           | Cliente  |
| Precondiciones:    | Itinerarios calculados por el sistema  |
| Flujo Normal:      | 1. El cliente define inicio <br> 2. El cliente define fin  <br> 3. El cliente selecciona calcular itinerario <br> 4. Se muestra una representacion sencilla del itinerario |
| Flujo Alternativo: | 4A. El itinerario se muestra en el mapa|
| Poscondiciones:    | Se guardan los datos  |

| UC-17              |   |
| :----------------- | - |
| Nombre:            | Ver paradas |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que se pueden ver las paradas y lineas ya organizadas por el sistema  |
| Actores:           | Cliente, Operador de transporte, Administrador  |
| Precondiciones:    | El sistema ha de tener organizadas las paradas y lineas  |
| Flujo Normal:      | 1. Se muestran las lineas y paradas |
| Flujo Alternativo: | 1A. Se selecciona una linea <br> 1A.1. Se muestra la informacion de esa linea  |
| Poscondiciones:    | -  |

| UC-18                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa general  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que los usuario pueden interactuar con el mapa interactivo renderizado por el sistema  |
| Actores:           | Operador de transporte, Cliente, Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El sistema crea el mapa en base a los datos cartograficos <br> 2. El sistema renderiza el mapa|
| Flujo Alternativo: | 2A. Se centra el mapa <br> 2B. Se acerca el mapa <br> 2C. Se aleja el mapa  <br> 2D. Se desplaza el mapa en cualquier direccion <br> 2E. Se vuelve a colocar como el mapa en su estado inicial |
| Poscondiciones:    | -  |

| UC-19                |   |
| :----------------- | - |
| Nombre:            | Definir transbordo  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la cual el sistema, mediante los datos de las lineas, calcula los transbordos incluyendo entre vehiculos diferentes  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | Datos de la linea presentados  |
| Flujo Normal:      | 1. El sistema obtiene los datos <br> 2. El sistema organiza los transbordos|
| Flujo Alternativo: | -  |
| Poscondiciones:    | Los transbordos se guardan en la base de datos  |

| UC-20                |   |
| :----------------- | - |
| Nombre:            | Calcular distancia entre paradas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | El sistema calcula la distancia entre las paradas  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | Datos de las paradas introducidos manualmente  |
| Flujo Normal:      | 1. El sistema obtiene los datos <br> 2. Se calcula la distancia |
| Flujo Alternativo: | 2A. Se identifica que no se puede transitar de una parada a otra <br> 2B. Se ofrece una parada cercana sustituta  |
| Poscondiciones:    | Se guardan las distancias en la base de datos  |

| UC-21                |   |
| :----------------- | - |
| Nombre:            | Calculo de itinerarios recomendados tiempo real  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | El sistema calcula los tiempos de recorrido segun los datos  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | Datos introducidos manualmente  |
| Flujo Normal:      | 1. El sistema define el recorrido <br> 2. El sistema calcula el recorrido |
| Flujo Alternativo: | 2A. El sistema encuentra que el recorrido no es transitable <br> 2A.1. Se ofrece un recorrido sustituto  |
| Poscondiciones:    | -  |

| UC-22               |   |
| :----------------- | - |
| Nombre:            |Ayuda en linea (SMET)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion de ayuda en linea de uso general |
| Actores:           | Operadores de transporte , Clientes, Administradores  |
| Precondiciones:    | Informacion de ayuda añadida a la base de datos  |
| Flujo Normal:      | 1. El usuario consulta la informacion correspondiente a sus necesidades  |
| Flujo Alternativo: | 1A. El usuario no encuentra la informacion que necesita <br> 1.1A. El usuario se pone en contacto con AUTGC para indicar su duda <br> 1.1A.1 Se añade un apartado nuevo  |
| Poscondiciones:    | Se almacenan los nuevos apartados |

| UC-23                |   |
| :----------------- | - |
| Nombre:            | Localizacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |  Funcion por la que el administrador localiza operadores de transporte en el sistema |
| Actores:           | Administrador  |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. El administrador localiza operadores de transporte |
| Flujo Alternativo: |  - |
| Poscondiciones:    |  - |

| UC-24                |   |
| :----------------- | - |
| Nombre:            | Consulta  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el administrador consulta datos del servicio  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador consulta datos de servicio  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-25                |   |
| :----------------- | - |
| Nombre:            | Gestion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que se gestiona la informacion del servicio |
| Actores:           | Administrador  |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. El administrador gestiona la informacion del servicio   |
| Flujo Alternativo: |  - |
| Poscondiciones:    |  - |

| UC-26                |   |
| :----------------- | - |
| Nombre:            | Herramienta de analisis  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que permite al administrador gestionar la informacion del servicio de forma dinamica  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador decide las herramientas a usar |
| Flujo Alternativo: | 2A. El administrador consulta datos del servicio <br> 2B. El administrador localiza operadores de transporte <br> 2C. El administrador gestiona la informacion del servicio  |
| Poscondiciones:    | -  |

| UC-27                |   |
| :----------------- | - |
| Nombre:            | Definir inicio y fin  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion para introducir el inicio y fin de un itinerario  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El cliente define inicio <br> 2. El cliente define fin |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Se guardan los datos  |

| UC-28                |   |
| :----------------- | - |
| Nombre:            | Ubicar zonas de interes  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Funcion para introducir zonas marcadas como zonas de interes para el calculo de itinerarios |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador introduce los datos de la zona de interes |
| Flujo Alternativo: | - |
| Poscondiciones:    | Los datos de la ubicacion de interes se introducen en la base de datos  |

| UC-29                |   |
| :----------------- | - |
| Nombre:            | Consultar de forma dinamica  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el cliente puede consultar la informacion del servicio de forma dinamica  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Constantemente consulta la informacion del servicio actualizando la informacion que muestra  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-30                |   |
| :----------------- | - |
| Nombre:            | Definir zonas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | El sistema usa los datos cartograficos para delimitar zonas, municipios y barrios  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El sistema obtiene los datos cartograficos <br> 2. El sistema delimita las zonas <br> 3. El sistema delimita municipios <br> 4. El sistema delimita barrios |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Se añaden los datos de las zonas, municipios y barrios a la base de datos |

| UC-31                |   |
| :----------------- | - |
| Nombre:            | Introduccion manual de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Metodo para la introduccion de datos necesarios para el calculo de itinerarios en el sistema  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador introduce los datos <br>  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Los datos introducidos se guardan en la base de datos  |

| UC-32                |   |
| :----------------- | - |
| Nombre:            | Control y edicion de la informacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Desarrollo de los procesos de control, edicion de la informacion, carga inicial y mantenimiento de datos  |
| Actores:           | Administrador |
| Precondiciones:    |   |
| Flujo Normal:      | 1. Se selecciona una opcion |
| Flujo Alternativo: | 1A. Se visualizan los horarios y servicios disponibles <br> 1B. El administrador modifica datos <br> 1C. El administrador introduce los datos <br> 1D. El administrador introduce los datos de la zona de interes|
| Poscondiciones:    | Los datos introducidos se guardan en la base de datos, Los datos introducidos se guardan en la base de datos, Los datos de la ubicacion de interes se introducen en la base de datos |

| UC-33                |   |
| :----------------- | - |
| Nombre:            | Modificacion de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Funcion para modificar los datos necesarios para el calculo de itinerarios  |
| Actores:           | Adminstrador  |
| Precondiciones:    | Realizacion de introduccion manual de datos  |
| Flujo Normal:      | 1. El administrador modifica datos |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Datos se han modificado en la base de datos  |

| UC-34                |   |
| :----------------- | - |
| Nombre:            | Datos asociados  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el sistema comprueba los datos de paradas y lineas introducidos por el administrador  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | Datos introducidos manualmente  |
| Flujo Normal:      | 1. El sistema compureba los datos asociados a las paradas y lineas  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-35                |   |
| :----------------- | - |
| Nombre:            | Organizar paradas y lineas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la cual el sistema organiza las paradas y lineas segun los datos que le ha dado el administrador  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | Datos introducidos manualmente  |
| Flujo Normal:      | 1. El sistema comprueba los datos asociados a las paradas y lineas <br> 2. Las paradas y lineas se organizan segun los datos asociados|
| Flujo Alternativo: | -  |
| Poscondiciones:    | Las paradas junto a las lineas se modifican y se guardan |

| UC-36                |   |
| :----------------- | - |
| Nombre:            | Listados de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Proceso para visualizar listados de horarios y servicios necesarios para el calculo de itinerarios |
| Actores:           | Administrador  |
| Precondiciones:    | Horarios y servicios introducidos en el sistema  |
| Flujo Normal:      | 1. Se visualizan los horarios y servicios disponibles  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-37                |   |
| :----------------- | - |
| Nombre:            | Centrar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que centra el mapa  |
| Actores:           | Sistema  |
| Precondiciones:    | Mostrar mapa  |
| Flujo Normal:      | 1. Se centra el mapa  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-38                |   |
| :----------------- | - |
| Nombre:            | Mostrar informacion linea  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que muestra la informacion de una linea  |
| Actores:           | Operador de transporte, Cliente, Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1.Se selecciona una linea <br> 2. Se muestra la informacion de esa linea  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-39                |   |
| :----------------- | - |
| Nombre:            | Acercar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que acerca el mapa |
| Actores:           | Sistema  |
| Precondiciones:    | Mostrar mapa  |
| Flujo Normal:      | 1. Se acerca el mapa  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-40                |   |
| :----------------- | - |
| Nombre:            | Ir a mapa base  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que desplaza el mapa  |
| Actores:           | Sistema  |
| Precondiciones:    | Mostrar mapa  |
| Flujo Normal:      | 1. Se vuelve a colocar como el mapa en su estado inicial  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-41                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion encargada de mostrar el mapa interactivo de la aplicacion  |
| Actores:           | Sistema de informacion |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El sistema crea el mapa en base a los datos cartograficos <br> 2. El sistema renderiza el mapa|
| Flujo Alternativo: | 2A. Se centra el mapa <br> 2B. Se acerca el mapa <br> 2C. Se aleja el mapa  <br> 2D. Se desplaza el mapa en cualquier direccion <br> 2E. Se vuelve a colocar como el mapa en su estado inicial |
| Poscondiciones:    | - |

| UC-42                |   |
| :----------------- | - |
| Nombre:            | Desplazar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que desplaza el mapa  |
| Actores:           | Sistema  |
| Precondiciones:    | Mostrar mapa  |
| Flujo Normal:      | 1. Se desplaza el mapa en cualquier direccion  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-43                |   |
| :----------------- | - |
| Nombre:            | Alejar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que aleja el mapa  |
| Actores:           | Sistema  |
| Precondiciones:    | Mostrar mapa  |
| Flujo Normal:      | 1. Se aleja el mapa  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-44                |   |
| :----------------- | - |
| Nombre:            | Editor WYSYWYG  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Editor para el desarrollo de paginas web con previsualizador que usan los administradores |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se modifica la pagina con el editor <br> 2. Se previsualizan los cambios realizados en la pagina  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Se guardan los cambios  |

| UC-45                |   |
| :---------------- | - |
| Nombre:            | Modificar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |  Funcion por la cual el administrador puede modificar contenidos del portal |
| Actores:           | Administrador  |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. Se modifican contenidos  |
| Flujo Alternativo: |  - |
| Poscondiciones:    | Se guardan los cambios |

| UC-46                |   |
| :----------------- | - |
| Nombre:            | Buscador  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que permite buscar informacion tanto en el foro como en la pagina  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se introducen los terminos a buscar <br> 2. Se localizan los terminos  |
| Flujo Alternativo: | 2A. No se localizan los terminos  |
| Poscondiciones:    | -  |

| UC-47                |   |
| :----------------- | - |
| Nombre:            | Mostrar estadisticas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la cual el administrador es capaz de visualizar las estadisticas del sitio  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se obtienen los datos <br> 2. Se calculan las estadisticas en base a los datos  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-48                |   |
| :----------------- | - |
| Nombre:            | Retirar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el administrador puede retirar contenido del portal  |
| Actores:           |  Administrador |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. Se retira contenido  |
| Flujo Alternativo: |  - |
| Poscondiciones:    | Se guardan los cambios realizados  |

| UC-49                |   |
| :----------------- | - |
| Nombre:            | Publicar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el administrador puede publicar contenidos en el portal  |
| Actores:           | Administrador  |
| Precondiciones:    |  - |
| Flujo Normal:      | 1. Se publica contenido  |
| Flujo Alternativo: |  - |
| Poscondiciones:    |  Se guardan los cambios realizados |

| UC-50                |   |
| :----------------- | - |
| Nombre:            | Acceso web  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso web a la informacion de interes tanto turistica como del transporte  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El usuario se conecta al portal de informacion  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-51                |   |
| :----------------- | - |
| Nombre:            | Creacion de pagina sencilla  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Interfaz por la que los administradores mas novatos en html pueden editar la pagina de forma sencilla  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se modifica la pagina <br> 2. Se previsualiza la pagina  |
| Flujo Alternativo: | 1A. Se modifican varias paginas  |
| Poscondiciones:    | Se guardan los cambios  |

| UC-52                |   |
| :----------------- | - |
| Nombre:            | Modificacion general  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que permite modificar contenido en varias paginas o todas en general  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se modifican varias paginas  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Se guardan los cambios  |

| UC-53               |   |
| :----------------- | - |
| Nombre:            | Previsualizacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Previsualizacion de los cambios realizados durante la edicion de una pagina  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se previsualiza la pagina  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-54                |   |
| :----------------- | - |
| Nombre:            | Entorno de colaboracion cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Entorno de colaboracion donde se pueden acceder a varias funcionalidades  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se concede acceso al entorno de colaboracion  |
| Flujo Alternativo: | 1A. Accede al blog <br> 1B. Acceso al cloudtag de la pagina principal del foro <br> 1C. Acceso al foro |
| Poscondiciones:    | -  |

| UC-55                |   |
| :----------------- | - |
| Nombre:            | Blog  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso al Blog   |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Accede al blog  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-56                |   |
| :----------------- | - |
| Nombre:            | CloudTag  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso al cloudtag  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Acceso al cloudtag de la pagina principal del foro  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-57                |   |
| :----------------- | - |
| Nombre:            | Entorno de colaboracion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Entorno de colaboracion donde se pueden acceder a varias funcionalidades y el administrador puede moderar |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se concede acceso al entorno de colaboracion  |
| Flujo Alternativo: | 1A. Accede al blog <br> 1B. Acceso al cloudtag de la pagina principal del foro <br> 1C. Acceso al foro |
| Poscondiciones:    | -  |

| UC-58                |   |
| :----------------- | - |
| Nombre:            | Foro  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso al foro  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Acceso al foro  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-59                |   |
| :----------------- | - |
| Nombre:            | Acceso web cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso web a la informacion de interes tanto turistica como del transporte  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El usuario se conecta al portal de informacion |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-60                |   |
| :----------------- | - |
| Nombre:            | Buscador cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion que permite buscar informacion tanto en el foro como en la pagina  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. Se introducen los terminos a buscar <br> 2. Se localizan los terminos  |
| Flujo Alternativo: | 2A. No se localizan los terminos  |
| Poscondiciones:    | -  |

| UC-61                |   |
| :----------------- | - |
| Nombre:            | Acceso web sin registro  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Acceso web a la informacion de interes tanto turistica como del transporte usuarios no registrados  |
| Actores:           | Usuario anonimo  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El usuario se conecta al portal de informacion  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-62                |   |
| :----------------- | - |
| Nombre:            | Gestor de contenido  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Gestor por el cual el administrador puede controlar contenidos del portal  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador escoge una opcion  |
| Flujo Alternativo: | 1A. Se modifican contenidos <br> 1B. Se retira contenido <br> 1C. Se publica contenido  |
| Poscondiciones:    | Se guardan los cambios realizados  |
