| UC-01               |   |
| :----------------- | - |
| Nombre:            | Enviar alarma  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la creación y envio de alarmas del sistema|
| Actores:           | Sistema  |
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
| Actores:           | Sistema  |
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
| Actores:           | Sistema, Administrador  |
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
| Actores:           | Sistema  |
| Precondiciones:    | Un cliente realiza un pago  |
| Flujo Normal:      | 1. El sistema comprueba que el pago se ha realizado correctamente <br> 2. El sistema busca en la base de datos al cliente <br> 3. El sistema añade el articulo asociado al pago realizado  |
| Flujo Alternativo: | 1A. El pago no se ha realizado correctamente <br> 1.1A. El sistema muestra el mensaje "El pago no se ha realizado correctamente" <br> 2A. El sistema no encuentra al cliente <br> 2.1A. El sistema muestra el mensaje "cliente no encontrado" <br> 2.2A. El sistema realiza la devolucion del importe pagado |
| Poscondiciones:    | Articulo añadido en la base del cliente que ha realizado el pago  |

| UC-05                |   |
| :----------------- | - |
| Nombre:            | Visualizar Mapa (Admin)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad del administrador de ver el mapa |
| Actores:           | Administrador  |
| Precondiciones:    | Usuario administrador registrado en el sistema. Mapa creado en el sistema. Información sobre el mapa  |
| Flujo Normal:      | 1. El sistema organiza la informacion del mapa <br> 2. El sistema crea el mapa con la informacion que se le ha añadido <br> 3. El usuario clicka en el boton que lleva al mapa <br> 4. El sistema muestra el mapa con la iformacion asociada |
| Flujo Alternativo: | 2A. El sistema puede no localizar algo en el mapa por un error al introducir los datos <br> 2.1A El sistema muestra que hay un error en la informacion introducida <br> 5A. El administrador recibe el aviso de una situacion inusual/puntual <br> 5A.1. El administrador añade dicha situacion a la informacion del mapa <br> 5A.2. El sistema modifica la informacion que se muestra en el mapa <br> 5B. Un administrador accede al mapa <br> 5.1B. Clicka el boton de grabacion <br> 5.2B. El sistema registra toda la informacion de lo que va pasando <br> 5.2B.1. El sistema no tiene espacio para realizar el registro de la informacion. <br> 5.2B.2. El sistema muestra el mensaje "No hay espacio suficiente" <br> 5.3B. Clicka el boton de detener grabacion <br> 5.4B. El sistema guarda la informacion registrada  |
| Poscondiciones:    |   |

| UC-06                |   |
| :----------------- | - |
| Nombre:            | Registrar periodos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad de registrar un periodo concreto  |
| Actores:           | Administrador  |
| Precondiciones:    | Usuario administrador registrado en el sistema  |
| Flujo Normal:      | 1. Un administrador accede al mapa <br> 2. Clicka el boton de grabacion <br> 3. El sistema registra toda la informacion de lo que va pasando <br> 4. Clicka el boton de detener grabacion <br> 5. El sistema guarda la informacion registrada |
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
| Flujo Normal:      | 1. El administrador accede al sistema <br> 2. El administrador accede al aparatado de creacion de eventos <br> 3. El administrador guarda el evento <br> 4. Se cumplen las condiciones del evento <br> 5. Se genera la alarma del aviso <br> 6. Se envia la alarma al sistema |
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
| Actores:           | Sistema  |
| Precondiciones:    | El cliente ha seleccionado sms como metodo de aviso. Apliacion cerrada  |
| Flujo Normal:      | 1. Se envia un sms al cliente  |
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
| Actores:           | Sistema |
| Precondiciones:    | El cliente ha seleccionado aviso sonoro como metodo de aviso. Apliacion cerrada  |
| Flujo Normal:      | 1. Se envia un aviso sonoro al cliente  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-13                |   |
| :----------------- | - |
| Nombre:            |Ayuda en linea (SMET)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |Operadores de transporte , Clientes, Administradores  |
| Precondiciones:    | Informacion de ayuda añadida a la base de datos  |
| Flujo Normal:      | 1. El usuario accede a la aplicacion <br> 2. El usuario accede al apartado de ayuda en linea <br> 3. El usuario consulta la informacion correspondiente a sus necesidades  |
| Flujo Alternativo: | 3A. El usuario no encuentra la informacion que necesita <br> 3.1A. El usuario se pone en contacto con AUTGC para indicar su duda <br> 3.2A. Se añade un apartado nuevo  |
| Poscondiciones:    | -  |

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
| Flujo Normal:      | 1. El cliente acciona el boton de mostrar itinerario <br> 2. El itinerario se muestra en el mapa <br> 3. El cliente cierra el mapa   |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-16                |   |
| :----------------- | - |
| Nombre:            | Previsualizacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-17                |   |
| :----------------- | - |
| Nombre:            | Definir itinerario  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion por la que el cliente introduce los datos de itinerario para que el sistema calcule el itinerario mas recomendable |
| Actores:           | Cliente  |
| Precondiciones:    | Itinerarios calculados por el sistema  |
| Flujo Normal:      | 1. El cliente define inicio <br> 2. El cliente define fin  <br> 3. El cliente guarda los datos <br> 4. El cliente selecciona calcular itinerario <br> 5. Se muestra una representacion sencilla del itinerario |
| Flujo Alternativo: | 5A. El cliente acciona el boton de mostrar itinerario <br> 5A.1. El itinerario se muestra en el mapa <br> 5A.2. El cliente cierra el mapa   |
| Poscondiciones:    | -  |

<!---| UC-18                |   |
| :----------------- | - |
| Nombre:            | Añadir pagina  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |-->

| UC-19                |   |
| :----------------- | - |
| Nombre:            | Mostrar paradas general  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-20                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa general  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-21                |   |
| :----------------- | - |
| Nombre:            | Definir transbordo  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-22                |   |
| :----------------- | - |
| Nombre:            | Calcular distancia entre paradas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-23                |   |
| :----------------- | - |
| Nombre:            | Calculo de itinerarios recomendados tiempo real  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-24                |   |
| :----------------- | - |
| Nombre:            | Mostrar parada inicio y fin  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-25                |   |
| :----------------- | - |
| Nombre:            | Calcular tiempos de recorrido  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-26                |   |
| :----------------- | - |
| Nombre:            | Ayuda en linea (SIT)  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |Operadores de transporte , Clientes, Administradores  |
| Precondiciones:    | Informacion de ayuda añadida a la base de datos  |
| Flujo Normal:      | 1. El usuario accede a la aplicacion <br> 2. El usuario accede al apartado de ayuda en linea <br> 3. El usuario consulta la informacion correspondiente a sus necesidades  |
| Flujo Alternativo: | 3A. El usuario no encuentra la informacion que necesita <br> 3.1A. El usuario se pone en contacto con AUTGC para indicar su duda <br> 3.2A. Se añade un apartado nuevo  |
| Poscondiciones:    | -  |

| UC-27                |   |
| :----------------- | - |
| Nombre:            | Localizacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-28                |   |
| :----------------- | - |
| Nombre:            | Consulta  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-29                |   |
| :----------------- | - |
| Nombre:            | Gestion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-30                |   |
| :----------------- | - |
| Nombre:            | Herramienta de analisis  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-31                |   |
| :----------------- | - |
| Nombre:            | Definir inicio y fin  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Funcion para introducir el inicio y fin de un itinerario  |
| Actores:           | Cliente  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El cliente define inicio <br> 2. El cliente define fin  <br> 3. El cliente guarda los datos  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-32                |   |
| :----------------- | - |
| Nombre:            | Ubicar zonas de interes  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Funcion para introducir zonas marcadas como zonas de interes para el calculo de itinerarios |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador accede a la opcion de ubicar zonas de interes <br> 2. El administrador introduce los datos de la zona de interes <br> 3. El administrador guarda los datos  |
| Flujo Alternativo: | - |
| Poscondiciones:    | Los datos de la ubicacion de interes se introducen en la base de datos  |

| UC-33                |   |
| :----------------- | - |
| Nombre:            | Consultar de forma dinamica  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

<!--| UC-34                |   |
| :----------------- | - |
| Nombre:            | Mostrar itinerario de mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |-->

| UC-35                |   |
| :----------------- | - |
| Nombre:            | Definir zonas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-36                |   |
| :----------------- | - |
| Nombre:            | Introduccion manual de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Metodo para la introduccion de datos necesarios para el calculo de itinerarios en el sistema  |
| Actores:           | Administrador  |
| Precondiciones:    | -  |
| Flujo Normal:      | 1. El administrador accede a la opcion de introduccion de datos manual <br> 2. El administrador introduce los datos <br> 3. El administrador guarda los datos  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Los datos introducidos se guardan en la base de datos  |

| UC-37                |   |
| :----------------- | - |
| Nombre:            | Control y edicion de la informacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Desarrollo de los procesos de control, edicion de la informacion, carga inicial y mantenimiento de datos  |
| Actores:           | Administrador  |
| Precondiciones:    |   |
| Flujo Normal:      | 1. El administrador accede al menu de control y edicion de la informacion <br> 2. Se selecciona una opcion <br> 3. Se cierra el menu  |
| Flujo Alternativo: | 2A. Se selecciona la opcion de listado de datos <br> 2A.1. Se visualizan los horarios y servicios disponibles <br> 2B. El administrador accede a la opcion de introduccion de datos manual <br> 2B.1. El administrador introduce los datos <br> 2B.2. El administrador guarda los datos <br> 2C. El administrador accede al menu de modificacion de datos <br> 2C.1. El administrador modifica datos <br> 2C.2. El administrador guarda los datos <br> 2D. El administrador accede a la opcion de ubicar zonas de interes <br> 2D.1. El administrador introduce los datos de la zona de interes <br> 2D.2. El administrador guarda los datos|
| Poscondiciones:    |   |

| UC-38                |   |
| :----------------- | - |
| Nombre:            | Modificacion de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Funcion para modificar los datos necesarios para el calculo de itinerarios  |
| Actores:           | Adminstrador  |
| Precondiciones:    | Realizacion de introduccion manual de datos  |
| Flujo Normal:      | 1. El administrador accede al menu de modificacion de datos <br> 2. El administrador modifica datos <br> 3. El administrador guarda los datos  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | Datos se han modificado en la base de datos  |

| UC-39                |   |
| :----------------- | - |
| Nombre:            | Datos asociados  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-40                |   |
| :----------------- | - |
| Nombre:            | Mostrar paradas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-41                |   |
| :----------------- | - |
| Nombre:            | Listados de datos  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Parte del flujo alternativo de CU-37. Proceso para visualizar listados de horarios y servicios necesarios para el calculo de itinerarios |
| Actores:           | Administrador  |
| Precondiciones:    | Horarios y servicios introducidos en el sistema  |
| Flujo Normal:      | 1. Se selecciona la opcion de listado de datos <br> 2. Se visualizan los horarios y servicios disponibles  |
| Flujo Alternativo: | -  |
| Poscondiciones:    | -  |

| UC-42                |   |
| :----------------- | - |
| Nombre:            | Identificar zonas no transitables  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-43                |   |
| :----------------- | - |
| Nombre:            | Recoger informacion no recogida  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-44                |   |
| :----------------- | - |
| Nombre:            | Centrar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-45                |   |
| :----------------- | - |
| Nombre:            | Mostrar informacion linea  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-46                |   |
| :----------------- | - |
| Nombre:            | Presentar recorrido cierta linea  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-47                |   |
| :----------------- | - |
| Nombre:            | Acercar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-48                |   |
| :----------------- | - |
| Nombre:            | Ir a mapa base  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-49                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-50                |   |
| :----------------- | - |
| Nombre:            | Desplazar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-51                |   |
| :----------------- | - |
| Nombre:            | Alejar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-52                |   |
| :----------------- | - |
| Nombre:            | Editor WYSYWYG  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-53                |   |
| :----------------- | - |
| Nombre:            | Modificar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-54                |   |
| :----------------- | - |
| Nombre:            | Buscador  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-55                |   |
| :----------------- | - |
| Nombre:            | Mostrar estadisticas  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-56                |   |
| :----------------- | - |
| Nombre:            | Retirar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-57                |   |
| :----------------- | - |
| Nombre:            | Publicar  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-58                |   |
| :----------------- | - |
| Nombre:            | Acceso web  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-59                |   |
| :----------------- | - |
| Nombre:            | Creacion de pagina sencilla  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-60                |   |
| :----------------- | - |
| Nombre:            | Modificacion general  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-61               |   |
| :----------------- | - |
| Nombre:            | Previsualizacion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-62                |   |
| :----------------- | - |
| Nombre:            | Entorno de colaboracion cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-63                |   |
| :----------------- | - |
| Nombre:            | Blog  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-64                |   |
| :----------------- | - |
| Nombre:            | CloudTag  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-65                |   |
| :----------------- | - |
| Nombre:            | Entorno de colaboracion  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-66                |   |
| :----------------- | - |
| Nombre:            | Foro  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-67                |   |
| :----------------- | - |
| Nombre:            | Acceso web cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-68                |   |
| :----------------- | - |
| Nombre:            | Buscador cliente  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |
