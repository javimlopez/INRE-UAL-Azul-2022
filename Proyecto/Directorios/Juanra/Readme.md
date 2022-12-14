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
| Precondiciones:    | Operador habilitado en el sistema  |
| Flujo Normal:      | 1. El operador activa el dispositivo de seguimiento <br> 2. El dispositivo envia constantemente los datos del operador y su posición <br> 3. El sistema recibe estos datos |
| Flujo Alternativo: | 3A. El sistema deja de recibir la informacion <br> 3.1A. El sistema muestra el mensaje "operador deslocalizado"  |
| Poscondiciones:    | -  |

| UC-03                |   |
| :----------------- | - |
| Nombre:            | Mostrar mapa  |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       | Caso de uso referente a la funcionalidad del sistema de mostrar el mapa  |
| Actores:           | Sistema, Administrador  |
| Precondiciones:    | Usuario administrador registrado en el sistema. Mapa creado en el sistema. Información sobre el mapa |
| Flujo Normal:      | 1. El sistema organiza la informacion del mapa <br> 2. El sistema crea el mapa con la informacion de los operadores que se le ha añadido |
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
| Flujo Alternativo: | 2A. El sistema puede no localizar algo en el mapa por un error al introducir los datos <br> 2.1A El sistema muestra que hay un error en la informacion introducida <br> 5A. El usuario registra una situacion <br> 5B. Un administrador accede al mapa <br> 5.1B. Clicka el boton de grabacion <br> 5.2B. El sistema registra toda la informacion de lo que va pasando <br> 5.2B.1. El sistema no tiene espacio para realizar el registro de la informacion. <br> 5.2B.2. El sistema muestra el mensaje "No hay espacio suficiente" <br> 5.3B. Clicka el boton de detener grabacion <br> 5.4B. El sistema guarda la informacion registrada  |
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
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-                |   |
| :----------------- | - |
| Nombre:            |   |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |

| UC-                |   |
| :----------------- | - |
| Nombre:            |   |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:  |
| Fecha:             | 14/12/2022  |
| Descripción:       |   |
| Actores:           |   |
| Precondiciones:    |   |
| Flujo Normal:      |   |
| Flujo Alternativo: |   |
| Poscondiciones:    |   |
