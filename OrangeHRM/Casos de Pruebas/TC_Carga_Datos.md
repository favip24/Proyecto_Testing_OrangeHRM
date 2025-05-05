*Carga: Búsqueda de Empleados*
- ID: TC12
- Título: Búsqueda de Empleados
- Descripción: Validar que al buscar empleados por nombre, apellido o ID, se muestren resultados correctos
- Datos de Entrada:
    * Apellido Empleado: Orion Harry
    * Nombre Empleado: McLary
    * ID Empleado: 0412
- Resultado Esperado: Se muestran resultados relacionados
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-21.png)
    [Evidencia: Búsqueda de Empleados](https://jam.dev/c/d1835d48-3294-4776-825d-8e26e0dd28cd)

*Carga: Agregar Nuevo Empleado*
- ID: TC13
- Título: Agregar un nuevo empleado
- Descripción: Validar que se pueda acceder a un formulario de carga de empleados
- Datos de Entrada:
    * Nombre: Favio
    * Palermo: Palermo 
    * ID: *sugerido por el sistema*
- Resultado Esperado: El empleado se agrega y se redirige a su ficha
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-22.png)
    [Evidencia: Agregar Nuevo Empleado](https://jam.dev/c/282b7d8c-0555-4806-a7fc-fcb7d56f363b)

*Carga de Datos Fallida: Agregar Empleados Sin Datos Obliatorios*
- ID: TC14
- Título: Cargar empleados sin datos obligatorios
- Descripción: Validar que el sistema impide cargar empleados si faltan datos requeridos obligatorios
- Datos de Entrada:
    * Nombre: *campo vacío*
    * Apellido: *campo vacío*
    * ID: *sugerido por el sistema*
- Resultado Esperado: Mensaje mostrando "campos requeridos" y no carga al empleado nuevo
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-23.png)
    [Evidencia: Carga de Empleados Fallida](https://jam.dev/c/264c4739-b5f6-4fd5-bae1-8b5d0e794ae2)

*Carga de Datos Fallida: Agregar Empleados Completando Campos Obligatorios con Espacios*
- ID: TC15
- Título: Cargar empleados completando campos con espacios
- Descripción: Validar que el sistema impide cargar empleados al completar campos obligatorios con espacios
- Datos de Entrada:
    * Nombre: *espacios en blanco*
    * Palermo: *espacios en blanco*
    * ID: *sugerido por el sistema*
- Resultado Esperado: Mensaje de error y no carga el empleado
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-24.png)
    [Evidencia: Carga de Empleados con Espacios Obligatorios Vacíos](https://jam.dev/c/3a34dab4-1401-4cfb-ae25-5c32a194dabc)

*Carga de Datos Fallida: Agregar Empleados Completando Campos Incorrectos*
- ID: TC16
- Título: Cargar empleados completando campos de forma incorrecta
- Descripción: Validar que el sistema impida cargar empleados nuevos si se completan de forma incorrecta los campos (números en los campos "First Name" y "Last Name", y letras en el campo "Employee Id")
- Datos de Entrada:
    * Nombre: 2025
    * Palermo: @27
    * ID: agjh
- Resultado Esperado: Mensaje de error y no carga el empleado
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-25.png)
    [Evidencia: Carga de Empleados con Campos Incorrectos](https://jam.dev/c/78efd12f-307c-4621-81aa-05dcd3d24ba8)