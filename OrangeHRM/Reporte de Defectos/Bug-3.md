*Carga de Datos Fallida: Agregar Empleados Completando Campos Incorrectos*
- ID: B-03
- Título: Cargar empleados con campos con datos incorrectos
- Descripción: El sistema no validó correctamente los datos ingresados, permitiendo la carga de un empleado con números en el campo "First Name" y "Last Name", y letras en el campo "Employee ID"
- Pasos para Reproducción:
    1. Navegar a la sección PIM
    2. Click en el botón "+ Add"
    3. Completar los campos obligatorios con datos incorrectos
    4. Verificar que el nuevo empleado con datos incorrectos fue creado
- Prioridad: Media
- Severidad: Media/Alta
- Resultado Actual: El sistema acepta los datos incorrectos y guarda el nuevo empleado
- Resultado Esperado: El sistema debe impedir la carga del nuevo empleado y mostrar un mensajes de que los datos ingresados no son correctos
- Evidencias:
    [Reporte del Defecto](../Imagenes/image-26.png)
    [Evidencia Bug: Carga de Empleados con Campos Incorrectos](https://jam.dev/c/78efd12f-307c-4621-81aa-05dcd3d24ba8)

# Mi conclusion: 
Tengo ciertas dudas a la hora de asignarle un Severidad clara a este bug, ya que pone en peligro la integridad en la base de datos y es un riegso para la calidad del sistema ya que se estarían registrando datos inválidos.
Por otro lado Le asigno una prioridad Media ya que no es Alta porque no bloquea el sistema pero debería corregirse antes de liberar la versión a producción.