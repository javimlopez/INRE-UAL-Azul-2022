En una universidad, el **personal del PDI**, el **personal del PAS** y los **estudiantes** pueden *consultar horarios*. Por su parte, el **personal del PAS** puede *modificar horarios* y *dar de alta estudiantes*. El **personal de PDI** puede *proponer cambios en los horarios* y *dar de alta estudiantes*. La funcionalidad de *dar de alta estudiantes* **del PAS** realiza una *verificación de los datos del estudiante*. Sin embargo, la funcionalidad de *dar de alta estudiantes* **del PDI**, además de *verificar los datos* también permite de forma excepcional *realizar la búsqueda en las listas de clase de sus asignaturas*.


- Actores:
    - Personal del PDI:
        - Casos de uso:
            1. Consultar horarios
            2. Proponer cambios en los horarios
            3. Dar de alta estudiantes --> Verificar datos del estudiante y except Realizar búsqueda en las listas de clase de sus asignaturas
    - Personal del PAS:
        - Casos de uso:
            1. Consultar horarios
            2. Modificar horarios
            3. Dar de alta estudiantes --> Verificar datos de estudiante
    
    - Estudiante:

        - Casos de uso:
            1. Consultar horarios


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

|INF-003 | DatosHorario |
| ----------- | ----------- |
| Nombre |  Horarios |  
|Referencia| consultar horarios,proponer cambios en los horarios, modificar horarios|
|Informacion|Los datos que son necesarios para el funcionamiento de los horarios  |
|Datos especificos|<ul> <li>Fecha y Hora</li> <li>  Asignaturas </li> <li>Aula </li></ul> |
|Importancia|Muy Importante|
|Estado| Aceptado|
|Comentarios| - |

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

