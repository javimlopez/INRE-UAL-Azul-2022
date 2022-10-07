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


| UC-02|  |
| :---------- | ------------------------------------: |
| Nombre: | Modificar horarios |
| Autor:  | Francisco Javier Mota López |
| Fecha:  | 30-09-22|
| Descripción:  | Permite modificar los horarios de las asignaturas |
| Actores: Personal PAS|
| Precondiciones: | El usuario tiene que estar autentificado en el sistema |
| Flujo Normal: | 1. El actor pulsa el botón de modificar horario <br> 2. El sistema muestra el horario y  |
| Flujo Alternativo: | |
| Poscondiciones: | |
