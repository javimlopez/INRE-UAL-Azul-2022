# 🔵 ERS - Equipo - Azul - 2022 🔵

## Portal Web de Transporte de Gran Canaria

### Version 1.0

# Hoja de revisión

| Fecha      | Versión | Descripción                                                                | Autor                                        |
| :--------- | :------- | :-------------------------------------------------------------------------- | :------------------------------------------- |
| 08/11/2022 | 1.0      | Preparar preguntas para el entrevistador                                    | :large_blue_diamond: Equipo Azul :large_blue_diamond: |
| 11/11/2022 | 1.0      | Resaltado del pliego de condiciones, y revision de respuestas               | :large_blue_diamond: Equipo Azul :large_blue_diamond: |
| 15/11/2022 | 1.0      | Organigrama, glosario de datos, y especificación de los diagramas          | :large_blue_diamond: Equipo Azul :large_blue_diamond:                 |
| 18/11/2022 | 1.0      | Objetivos del negocio                                                       | :large_blue_diamond: Equipo Azul :large_blue_diamond: |
| 22/11/2022 | 1.0      | Toma de requisitos                                                          | :large_blue_diamond: Equipo Azul :large_blue_diamond:                 |
| 26/11/2022 | 1.0      | Aclaracion en casos de uso                                                  | :large_blue_diamond: Equipo Azul :large_blue_diamond:                     |
| 29/11/2022 | 1.1      | Revision de casos de uso                                                    | :large_blue_diamond: Equipo Azul :large_blue_diamond:                    |
| 2/12/2022  | 1.0      | Diagramas casos de uso + Diagrama ER                                        | :large_blue_diamond: Equipo Azul :large_blue_diamond:                          |
| 13/12/2022 | 1.0      | Defensa con Manel + Arreglo del ERS en el repo + Revision de lo que tenemos | :large_blue_diamond: Equipo Azul :large_blue_diamond:                |

# Introducción

En este documento se va a tratar la recopilación de toda la información necesaria para el uso y modificación del programa cuya implementación ha sido encargada por  la Autoridad Única del Transporte de Gran Canaria. Este proyecto se dividen en dos subproyectos, los cuales son:

* Portal web con el objetivo de disponer de un portal de servicios al usuario del transporte regular de viajeros, de carácter interactivo, de conformidad con las prescripciones técnicas definidas en el pliego de condiciones y en el de condiciones administrativas particulares.
* Sistema de monitorización de la explotación de transporte, es decir,  un sistema de información y monitorización que aglutina las informaciones procedentes de los sistemas de información embarcados en los vehículos de los operadores, que permita disponer de una visión global, instantánea e histórica del estado de la explotación del transporte regular de viajeros en la isla desarrollado por los distintos operadores.

# Información del Dominio del problema

#### Organigrama

<img src=./svgs/Organigrama.svg>

#### Glosario de terminos

|                    Término                    | Descripción                                                                                                                                                                   |
| :--------------------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|                     Guagua                     | Referido a autobús                                                                                                                                                            |
|                    Interfaz                    | Es la conexión funcional entre dos sistemas, programas, dispositivos o componentes que comunican de distintos niveles, permitiendo el intercambio de información             |
|                   CNPA-2002                   | Clasificación Nacional de Productos por Actividades 2002                                                                                                                      |
|                Libro de estilo                | Documento que ayuda a la comprensión de las partes de un proyecto                                                                                                             |
|                      CPV                      | Vocabulario Común de Contratos Públicos                                                                                                                                      |
|               Canales digitales               | Es un canal que sirve para dar servicio, comunicar o vender a través de un ordenador, una tablet o un móvil                                                                  |
|             Arquitectura software             | Pautas y criterios que se siguen en la elaboración abstracta a nivel de código dentro de un proyecto informático                                                            |
|                     AUTGC                     | Autoridad Única del Transporte de Gran Canaria                                                                                                                                |
|                   Licitante                   | Participar en una subasta pública ofreciendo la ejecución de un servicio a cambio de la obtención de dinero u otros beneficios.                                             |
|             Modificaciones comunes             | Modificación en conjunto de un elemento de múltiples páginas de forma simultánea                                                                                           |
|                 Editor WYSIWYG                 | Editor para el desarrollo de páginas web con previsualizador                                                                                                                  |
| Relación de cloud tag en la home del website. | Representación gráfica abstracta formada por múltiples palabras relacionadas con las funcionalidades de la página y con enlaces a ellas                                    |
|           Maquetación de contenido           | Utilización de una serie de recursos como las negritas, los sumarios y los títulos para favorecer la experiencia de usuario y facilitar la lectura de contenidos en internet |
|         Estructura de la base de datos         | Forma matemática mediante la cual se trabaja con los datos y las relaciones entre los mismos, de la manera más eficiente posible                                             |
|              Itinerario de línea              | Define, direcciona y describe el camino que va a ser recorrido o ruta.                                                                                                         |
|                     Tarifa                     | Cobro de servicios, durante un período determinado, por una cantidad fija y con independencia del tiempo y el tipo de su utilización.                                        |
|                   Transbordo                   | Trasladar efectos o personas de una embarcación a otra.                                                                                                                       |
|                  Tiempo Real                  | Un sistema que es capaz de responder y procesar la información al ritmo en que esta entra o se introduce                                                                      |
|       Consulta de programa informático       | Método que permite acceder a los datos guardados y realizar diversas acciones y operaciones                                                                                   |
|                Forma dinámica                | Método para reducir el tiempo de ejecución de un algoritmo mediante operaciones y estructuras óptimas                                                                       |
|                      SMET                      | Sistema de información y Monitorización de la Explotación del Transporte                                                                                                    |
|                      SIIT                      | Sistema Interactivo  Información Transport                                                                                                                                    |
|   HelpDesk para la atención de incidencias   | Hace referencia al conjunto de recursos humanos y tecnológicos que se dedican a la gestión de incidencias relacionadas con el soporte o la asistencia a usuarios.            |

# Necesidades del negocio

#### Objetivos del negocio

|    OBJ-1    |                                                                                                                                     SIIT                                                                                                                                     |
| :----------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Versión   |                                                                                                                                     1.0                                                                                                                                     |
| Descripción | Montar un sistema interactivo de información por el que los usuarios podrán conocer y disponer de las prestaciones que ofrece el servicio integrado de transporte público de viajeros de Gran Canaria relacionándolas con otras materias de ocio, turismo, cultura, etc. |
| Comentarios |                                                                                                    La información deberá ser accesible desde el portal web de la AUTGC.                                                                                                    |

|    OBJ-2    |                                                                                                                                               SMET                                                                                                                                               |
| :----------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Versión   |                                                                                                                                                1.0                                                                                                                                                |
| Descripción | Montar un sistema de información y monitorización de la explotación del transporte para la AUTGC que facilite reconocer, registrar y monitorizar en todo momento el grado de cumplimiento de las obligaciones de servicio de los operadores en base a una serie de condiciones parametrizables |
| Comentarios |                                                                                                                                              Ninguno                                                                                                                                              |

|    OBJ-3    |                                                                                                                                              Portal Web                                                                                                                                              |
| :----------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Versión   |                                                                                                                                                  1.0                                                                                                                                                  |
| Descripción | Se pide montar un portal web que abarque los aspectos de: identificar necesidades (contenidos, servicios, audiencias, etc), definir la estructura (arquitectura de la información, mapa web, etc) y organización del portal, detallar componentes organizativos, funcionales y técnicos del mismo. |
| Comentarios |                                                                            Forma parte del sistema SIIT, que se divide en dos partes: una el sistema de información y otra el portal web y ambos están interrelacionados                                                                            |

## Modelos de negocio

### Subprocesos

BPM diagramas

### Tareas

Enunciado del bpmn

# Requisitos del sistema a desarrollar

#### Requisitos

|Requisito|Descripción|Tipo|
|:--:|:--:|:--:|
|Edicion sencilla|Interfaz que facilite la introduccion de datos a los menos versados en html|Funcional|
|Mostrar paradas|Interfaz de usuario que muestra las paradas y sus datos asociados|Funcional|
|Definir itinerario|Se ha de poder definir el itinerario de inicio a fin con la posibilidad de mostrarlo en el mapa|Funcional|
|Ayuda en linea|Todo usuario ha de poder solicitar ayuda cuando sea necesario|Funcional|
|Mostrar Mapa|Se requiere un mapa cartografico interactivo|Funcional|
|Control y  edición de la informacion |Interfaz que nos permite ver una listados de datos ,introducir datos manualmente y modificar datos segun convenga |Funcional|
|Identificar zonas no transitables|El sistema de informacion ha de ser capaza de identificar zonas no transitables y alterar los itinerarios segun sea necesario|Funcional|
|calculo de itinerarios recomendados tiempo real|El sistema de informacion ha de ser capaz de calcular el mejor itinerario en tiempo real y una vez esta calculado lo muestra |Funcional|
|Calcular tiempos de recorrido|El sistema de informacion ha de ser capaz de calcular el tiempo de recorrido|Funcional|
|Calcular distancias entre paradas|El sistema de informacion ha de ser capaz de calcular distancias entre paradas|Funcional|
|Definir transbordo|El sistema de informacion ha de ser capaz de definir si es necesario un transbordo |Funcional|
|Ubicar zonas de interes|Los administradores han de ser capaces de ubicar zonas de interes |Funcional|
|Definir zonas|Los administradores han de ser capaces de crear zonas|Funcional|
|Presentar recorrido cierta linea|El sistema de informacion ha de poder mostrar el recorrido de una linea y si se quiere la informacion de la correspondiente linea|Funcional|
|Herramientas de analisis|herramientas de analisis, consulta, localizacion y gestion, con el objeto de que el usuario del transporte publico pueda consultar de forma dinamica la informacion del servicio permitiendole conocer y programar con antelacion su viaje. |Funcional|
||||
|Realizar Pagos|El cliente ha de ser capaz de pagar con tarjeta y  que el sistema de monitorizacion sea capaz de gestionarlo|Funcional|
|Recabar informacion en tiempo real Operadores|El sistema de monitorizacion se va a encargar de recabar informacion de los operadores de transporte |Funcional|
|Gestion de Alarmas|El sistema de monitorizacion debe poder enviar Alarmas y los todos los usuarios han de poder visualizar las Alarmas on en el caso de que la app este cerrada recibir un sms o una norificacion sonora|Funcional|
|Visualizar Mapa (Admin)|Los administradores han de poder visualizar en un mapa dado por el sistema de monitorizacion los datos de los conductores y de la explotacion donde tendran la opcion de registrar incidencias o periodos de tiempo|Funcional|
|Definir eventos|Se han de poder registrar eventos por parte de los administradores|Funcional|
||||
|Editor WYSYWYG|El portal  tiene que tener un editor de este tipo|Funcional|
|Mostrar estadisticas|El portal es capaz de mostrar la estadisticas de acceso a los administradores|Funcional|
|Gestor de contenidos|El administrador ha de ser capaza de modificar ,retirar y publicar contenido segun su juicio|Funcional|
|Creacion de pagina sencilla|En el portal se ha de poder modificar de forma sencilla una pagina o un conjunto de paginas siempre mostrando una previsualizacion antes de  aceptar la modificacion |Funcional|
|Etorno de colaboracion | El portal ha de poseer un entorno de colaboracion accesible por los administradores y los clientes formado por un blog, un foro y el cloid tag que siempre esta en la pagina principal|Funcional|
|Acceso Web|El portal ha de ser accesible por la web para administradores y clientes|Funcional|
|||Funcional|


#### Actores

| Código | Actor | Descripcion |
| :-------: | :----------: | :--: |
|ACT-01|Sistema||
|ACT-02|Cliente||
|ACT-03|Operadores||
|ACT-04|Administradores||
|ACT-05|Administrador(SIT)||
|ACT-06|Cliente(SIT)||
|ACT-07|Operador de transporte(SIT)||
|ACT-08|Auxiliar edicion||
|ACT-09|Sistema informacion||
|ACT-10|Cliente||
|ACT-11|Administrador||

#### Caso de uso

| Código |                      Casos de uso                      | Descripción |
| :-----: | :----------------------------------------------------: | :----------: |
|  UC-01  |                     Enviar alarma                     |              |
|  UC-02  |    Recabar informacion en tiempo real de operadores    |              |
|  UC-03  |                      Mostrar mapa                      |              |
|  UC-04  |                    Gestion de pagos                    |              |
|  UC-05  |                  mostrar Mapa (admin)                  |              |
|  UC-06  |                   Registrar periodos                   |              |
|  UC-07  |                 Registrar situaciones                 |              |
|  UC-08  |                     Definir evento                     |              |
|  UC-09  |                     Generar aviso                     |              |
|  UC-10  |                          sms                          |              |
|  UC-11  |                   Visualizar alarma                   |              |
|  UC-12  |                      Aviso sonoro                      |              |
|  UC-13  |                     Ayuda en linea                     |              |
|  UC-14  |                     Realizar pagos                     |              |
|  UC-15  |                 mostrar Mapa (cliente)                 |              |
|  UC-16  |                    Previsualizacion                    |              |
|  UC-17  |                    Edicion sencilla                    |              |
|  UC-18  |                    AÃ±adir pagina                    |              |
|  UC-19  |                Mostrar paradas general                |              |
|  UC-20  |                  Mostrar mapa general                  |              |
|  UC-21  |                   Definir transbordo                   |              |
|  UC-22  |            Calcular distancia entre paradas            |              |
|  UC-23  |    Calculo de itinerarios recomendados tiempo real    |              |
|  UC-24  |              Mostrar parada inicio y fin              |              |
|  UC-25  |             Calcular tiempos de recorrido             |              |
|  UC-26  |                  Ayuda en linea(SIT)                  |              |
|  UC-27  |                      Localizacion                      |              |
|  UC-28  |                        Consulta                        |              |
|  UC-29  |                        Gestion                        |              |
|  UC-30  |                Herramienta de analisis                |              |
|  UC-31  |                  Definir inicio y fin                  |              |
|  UC-32  |                Ubicar zonas de interes                |              |
|  UC-33  | Consultar de forma dinamica la informacion de servicio |              |
|  UC-34  |               Mostrar itinerario de mapa               |              |
|  UC-35  |                     Definir zonas                     |              |
|  UC-36  |              Introduccion manual de datos              |              |
|  UC-37  |          Control y edicion de la informacion          |              |
|  UC-38  |                 Modificacion de datos                 |              |
|  UC-39  |                    Datos asociados                    |              |
|  UC-40  |                    Mostrar paradas                    |              |
|  UC-41  |                     Lista de datos                     |              |
|  UC-42  |           Identificar zonas no transitables           |              |
|  UC-43  |            Recoger informacion no recogida            |              |
|  UC-44  |                        Centrar                        |              |
|  UC-45  |                Mostar informacion linea                |              |
|  UC-46  |            Presentar recorrido cierta linea            |              |
|  UC-47  |                         Acecar                         |              |
|  UC-48  |                     Ir a mapa base                     |              |
|  UC-49  |                      Mostrar mapa                      |              |
|  UC-50  |                       Desplazar                       |              |
|  UC-51  |                         Alejar                         |              |
|  UC-52  |                     Editor WYSYWYG                     |              |
|  UC-53  |                       Modificar                       |              |
|  UC-54  |                        Buscador                        |              |
|  UC-55  |                  Mostrar estadisticas                  |              |
|  UC-56  |                        Retirar                        |              |
|  UC-57  |                        Publicar                        |              |
|  UC-58  |                       Acceso Web                       |              |
|  UC-59  |              Creacion de pagina sencilla              |              |
|  UC-60  |                  Modificacion general                  |              |
|  UC-61  |                    Previsualizacion                    |              |
|  UC-62  |            Entorno de colaboracion cliente            |              |
|  UC-63  |                          Blog                          |              |
|  UC-64  |                        CloudTag                        |              |
|  UC-65  |                Entorno de colaboracion                |              |
|  UC-66  |                          Foro                          |              |
|  UC-67  |                   Acceso Web Cliente                   |              |
|  UC-68  |                    Buscador cliente                    |              |

#### Especificacion de Diagramas

# Lista de diagrama de casos de uso del modelo

# Diagramas de casos de uso

## Diagrama SMET

<img src="./svgs/DiagramaSmet.svg">
# Lista general de casos de uso y actores del proyecto

Diagrama SMET

| Detalles de los actores |              |
| :---------------------: | :----------: |
|          Actor          | Descripción |
|         Sistema         |              |
|      Administrador      |              |
|        Operador        |              |
|         Cliente         |              |

|:--:|:--:|
|Nombre: |Descripción|
|Autor: ||
|Fecha: ||
|Descripcion: ||
|Actores: ||
|Precondiciones: ||
|Flujo normal: ||
|Flujo alternativo: ||
|Post condiciones: ||

# Detalle de los casos de uso

# Diagramas de clases asociados a los requisitos de información

DIAGRAMAS DE CLASES

## Requisitos de información del portal

| INF-001:           | Administrador                                                                          |
| :----------------- | :------------------------------------------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                                                   |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                                                          |
| Fuente:            | Pliego de condiciones                                                                  |
| Referencia:        | -                                                                                      |
| Descripción:      | Información sobre el usuario Administrador                                            |
| Datos especificos: | <ul><li>Nombre</li><li>Teléfono</li><li>Correo Electrónico</li></ul> |
| Importancia:       | Muy Importante                                                                         |
| Estado:            | Aceptado                                                                               |
| Comentar:          | -                                                                                      |

| INF-002:           | Cliente                                              |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                        |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:       | Información sobre cliente |
| Datos especificos: | <ul><li>Nombre</li><li>Teléfono</li><li>Correo Electrónico</li><li>Número tarjeta</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-003:           | Estadísticas |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:       | Información sobre las estadísticas |
| Datos especificos: | <ul><li>Acceso página web</li><li>Origen más solicitado</li><li>Destino más solicitado</li><li>Información más requerida</li><li>Pungos de información más solicitados</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-004:           | Página |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:       | Plantillas de contenido |
| Datos especificos: |  |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-005:           | Blog                                                |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre el contenido de los blogs |
| Datos especificos: | <ul><li>Autor</li><li>Texto</li><li>Imagen</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-006:           | Foro                                               |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                        |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los foros |
| Datos especificos: | <ul><li>Autor</li><li>Mensaje</li><li>Hora</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-007:           | Cloud tag |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre Cloud tags |
| Datos especificos: | <ul><li>Enlace</li> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-008:           | Contenido                                               |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond: |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los contenidos de la página web |
| Datos especificos: | <ul><li>Información de texto</li><li>Contenidos visuales</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -   |

## Requisitos de información del sistema interactivo de información del transporte (SIIT)

| INF-001:           | Administrador (SIIT) |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      |                                                      |
| Datos especificos: | <ul><li>Nombre</li><li>Teléfono</li><li>Correo Electrónico</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-002:  | Cliente (SIIT) |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | - |
| Descripción:      |                                                      |
| Datos especificos: | <ul><li>Nombre</li><li>Teléfono</li><li>Correo Electrónico</li><li>Número tarjeta</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-003:           | Operador de transporte (SIIT) |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      |                                                      |
| Datos especificos: | <ul><li>Nombre</li><li>Teléfono</li><li>Correo Electrónico</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-004:           | Itinerario |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      |  Información relevante sobre itinerarios |
| Datos especificos: | <ul><li>Fecha inicio</li><li>Fecha fin</li><li>Líneas</li><li>Ubicaciones</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-005:           | Sistema Información |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre el sistema de información |
| Datos especificos: | <ul><li>Horario Servicio</li><li>Tipo servicio</li><li>Ubicaciones</li><li>Zonas no transitables</li><li>Rutas</li><li>barrios</li><li>municipios</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-006:           | Líneas |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información de líneas  |
| Datos especificos: | <ul><li>Vehículo</li><li>Ubicaciones</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-007:           | Ruta |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre rutas  |
| Datos especificos: | <ul><li>Información turística</li><li>Ubicaciones</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-008:           | Ubicaciones |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre ubicaciones  |
| Datos especificos: | <ul><li>Coordenadas</li><li>EsDeInteres</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-009:           | Horario |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre horario  |
| Datos especificos: | <ul><li>Fecha</li><li>Hora</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-010:           | Paradas |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre paradas  |
| Datos especificos: | <ul><li>Linea</li><li>Ubicacion</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-011:           | Datos cartográficos |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los datos cartográficos necesarios para generar el mapa  |
| Datos especificos: | <ul><li>Coordenadas</li><li>Ubicacion</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-012:           | Vehículo |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los datos cartográficos necesarios para generar el mapa  |
| Datos especificos: | <ul><li>Nombre Vehículo</li><li>Tipo Vehículo</li><li>Horario</li><li>Ubicación tiempo real </li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |
## Requisitos de información del sistema interactivo de información del transporte (SMET)

| INF-001:           | Sistema de monitorización  |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre el sistema de monitorización |
| Datos especificos: | <ul><li>Tipo de billete</li><li>SMS</li><li>Alarma</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-002:           | Administrador                                        |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información de los administradores |
| Datos especificos: | <ul><li>Nombre</li><li>Apellidos</li><li>Teléfono</li><li>Correo Electrónico</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-003:           | Operador de transporte|
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los operadores de transporte |
| Datos especificos: | <ul><li>Nombre</li><li>Apellidos</li><li>Teléfono</li><li>Correo Electrónico</li><li>Vehículo</li><li>Ruta asignada</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-004:           | Cliente |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond: |
| Fuente:            | Pliego de condiciones |
| Referencia:        | - |
| Descripción:      | Información de los clientes|
| Datos especificos: | <ul><li>Nombre</li><li>Apellidos</li><li>Teléfono</li><li>Correo Electrónico</li><li>Número tarjeta</li></ul> |
| Importancia:       | Muy Importante |
| Estado:            | Aceptado |
| Comentar:          | - |

| INF-005:           | Alarma |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre las alarmas |
| Datos especificos: | <ul><li>Nombre</li><li>Duración</li><li>Información</li>li>Tipo alarma</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-006:           | Dato |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre datos |
| Datos especificos: | `<ul><li>``</li><li>``</li><li>``</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-008:           | Pago |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los pagos |
| Datos especificos: | <ul><li>Número tarjeta</li><li>Hora transacción</li><li>Fecha Transacción</li><li>Importe</li></ul>` |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-009:           | Vehículo |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los Vehículos  |
| Datos especificos: | <ul><li>Nombre Vehículo</li><li>Tipo Vehículo</li><li>Horario</li><li>Ubicación tiempo real </li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-010:           | Evento |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los eventos  |
| Datos especificos: | <ul><li>Nombre evento</li><li>Fecha</li><li>Hora</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-011:           | Situación |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre las situaciones inesperadas  |
| Datos especificos: | <ul><li>Ubicacion</li><li>Fecha</li><li>Hora</li><li>InformaciónSituación</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-012:           | Período |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los operadores en un período de tiempo  |
| Datos especificos: | <ul><li>Ubicacion en tiempo real</li><li>Vehículo</li><li>Ruta</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |

| INF-013:           | Tipo Alarma |
| :----------------- | :--------------------------------------------------- |
| Versión:          | 1.0 (Diciembre-2022)                                 |
| Autor:             | :large_blue_diamond: Equipo Azul :large_blue_diamond:                         |
| Fuente:            | Pliego de condiciones                                |
| Referencia:        | -                                                    |
| Descripción:      | Información sobre los tipos de alarma  |
| Datos especificos: | <ul><li>Tipo de alarma</li></ul> |
| Importancia:       | Muy Importante                                       |
| Estado:            | Aceptado                                             |
| Comentar:          | -                                                    |
# Apéndices

## Detalles de entrevista

| Ficha entrevista |                                                |
| :--------------: | ---------------------------------------------- |
|   Entrevistado   | Juan Palomo (Conductor de autobuses)           |
|      Fecha      | 15 de noviembre de 2022                        |
|       Hora       | 9:10                                           |
|      Lugar      | Laboratorio de análisis y diseño de software |
|      Asunto      | Sistema de Transporte Público Canario         |

## Desarrollo de la entrevista

| Ficha entrevista |                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                |
| :--------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      Tiempo      |                                                                                            Preguntas                                                                                            |                                                                                                                                                                                                   Respuestas                                                                                                                                                                                                   |
|      1 min      |                                                        ¿Qué transportes se agrupan en la denominación de transporte público canario?                                                        |                                                                                                                                 Autobuses, barcos entre distintas islas, taxis públicos, carros turísticos tirados de caballos (forman parte del transporte publico canario)                                                                                                                                 |
|      1 min      |                                               ¿Qué tipos de datos se debería tener en cuenta por cada usuario interesado en usar el transporte?                                               |                                                                                                                                                                           Ninguno adicional al que viene en el pliego de condiciones.                                                                                                                                                                           |
|      2 min      |                                                         ¿Qué métodos de pago se pueden contemplar dentro de los servicios ofrecidos?                                                         |                                  Pago en efectivo, pago con tarjeta de transporte del gobierno de las islas canarias (cada persona empadronada en la isla puede sacarse esa tarjeta y sale con un descuento, recargable). Se recarga yendo al kiosco con tarjeta o efectivo y en los autobuses con dinero en efectivo. Uso exclusivo de la tarjeta para personas empadronadas.                                  |
|      1 min      |                                                        ¿Como enlazamos los aspectos de ocio, cultura y turismo dentro de la aplicación?                                                        |                                                                                                                                              En el portal por medio de noticias mientras que en las paradas y rutas se indicarán en el apartado de observaciones                                                                                                                                              |
|      30 seg      | ¿El sistema de información y monitorización de la explotación de transporte debe de ser trasparente y público, o por el contrario, exclusivo de la Autoridad Única del Transporte canario? |                                                                                                                                                                                            En principio es público.                                                                                                                                                                                            |
|      20 seg      |                                                              ¿El buscador tendría que funcionar con eventos, líneas y destginos?                                                              |                                                                                                                                                                                                       Sí                                                                                                                                                                                                       |
|      1 min      |                                                    ¿Tiene alguna preferencia de diseño, como por ejemplo en cuanto a la paleta de colores?                                                    |                                                                                                                                         La mayoría de las páginas del ayuntamiento de las islas canarias se hace con colores muy claros (azul muy claro por ejemplo).                                                                                                                                         |
|      2 min      |                                                             ¿Los itinerarios recomendados incluyen tanto ubicaciones como eventos?                                                             | La idea es que cuando alguien busque una ruta (Punto A a punto B) pueda tener la ruta más corta posible/ rápida, una ruta turística. Tener filtros. En principio no se informa sobre el turismo de las islas Canarias. Horario de autobuses subido en la página web con las paradas. Nosotros tendríamos que ajustar y definir bien las paradas, fotos a las paradas, mapa, por donde va el autobús, etc. |
|      1 min      |                                                            ¿Los usuarios que busquen información, deben tener la sesión iniciada?                                                            |                                                                                                                                                      No, accesible a todo el mundo porque es un engorro iniciar sesión para consultar como va un autobús                                                                                                                                                      |
|      1 min      |                           ¿La ubicación a tiempo real del transporte se hará en la aplicación, o por el contrario el propio transporte tendría un sistema propio?                           |                                                                                                                   Normalmente, las aplicaciones del móvil hacen que la batería dure poco, es preferente un dispositivo dentro del autobús o un móvil con una aplicación solo para ello.                                                                                                                   |
|      1 min      |                                                             ¿A qué se refiere con observaciones dentro del resultado de consultas?                                                             |                                                                                                                                  Cuando tú hagas el pedido de paradas o rutas, en observaciones pondrán cosas como lugares turísticos más cercanos, caminos cortados, etc.                                                                                                                                  |
# Miembros del grupo:
:large_blue_diamond: FRANCISCO DE BORJA JOSE GUTIERREZ CARRASCO<br>
:large_blue_diamond: FRANCISCO JAVIER MOTA LOPEZ<br>
:large_blue_diamond: JUAN RAUL MELLADO GARCIA<br>
:large_blue_diamond: ANGEL NIETO BURGOS
