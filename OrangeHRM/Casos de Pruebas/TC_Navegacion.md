*Navegación: Acceso al Panel de Control*
- ID: TC09
- Título: Acceso al Panel de Control
- Descripción: Verificar que el usuario pueda acceder al panel principal luego del Log In
- Datos de Entrada:
    * Usuario: Admin
    * Contraseña: admin123
- Resultado Esperado: El panel principal carga correctamente y sin errores
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-17.png)
    [Evidencia: Navegación](https://jam.dev/c/a13ae700-9701-4339-b7f5-17a8bc49dd31)

*Navegación: Acceso al Módulo PIM*
- ID: TC10
- Título: Acceso al Módulo PIM
- Descripción: Validar que se pueda navegar al módulo PIM
- Datos de Entrada:
    * Usuario: -
    * Contraseña: -
- Resultado Esperado: Se carga la pantalla de búsqueda de empleados
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-18.png)
    [Evidencia: Navegación al Módulo PIM](https://jam.dev/c/3698fff0-6469-45b4-9f1e-92b6bed409fd)
    

*Navegación Fallida: Acceso Fallido por tiempo de expiración de Sesión*
- ID: TC11
- Título: Acceso fallido por tiempo de expiración de sesión
- Descripción: Validar que tras expirar la sesión, no se puede navegar entre módulos
- Datos de Entrada:
    * Usuario: -
    * Contraseña: -
- Resultado Esperado: Se redirige al logiun o se muestra un mensaje de sesión expirada
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-19.png)
    [Evidencia: Navegación Fallida](https://jam.dev/c/7fd1acd9-26be-4914-b5ab-9027c4d294b0)