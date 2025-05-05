*Inicio de Sesión Exitoso*
- ID: TC01
- Título: Inicio de Sesión Exitoso
- Descripción: El usuario accede al sistema correctamente con credenciales válidas
- Datos de Entrada:
    * Usuario: Admin
    * Contraseña: admin123
- Resultado Esperado: Se redirige al panel principal sin errores
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-0.png)
    [Evidencia: Entrada de Datos](../Imagenes/image-1.png)
    [Evidencia: Ingreso al sistema exitoso](../Imagenes/image-2.png)

*Inicio de Sesión Fallido*
- ID: TC02
- Título: Inicio Sesión Fallido 1
- Descripción: Se intenta acceder al sistema con un usuario inexistente
- Datos de Entrada:
    * Usuario: Admin321
    * Contraseña: admin123
- Resultado Esperado: Mensaje de error: "Invalid credentials"
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-3.png)
    [Evidencia: Entrada de Datos](../Imagenes/image-4.png)
    [Evidencia: Mensaje de Error](../Imagenes/image-5.png)

- ID: TC03
- Título: Inicio de Sesión Fallido 1.1
- Descripción: Se intenta acceder al sistema con una contraseña inválida para el usuario ya existente
- Datos de Entrada:
    * Usuario: Admin
    * Contraseña: failpass
- Resultado Esperado: Mensaje de error: "Invalid credentials"
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-6.png)
    [Evidencia: Entrada de Datos](../Imagenes/image-7.png)
    [Evidencia: Mensaje de Error](../Imagenes/image-8.png)

- ID: TC04
- Título: Inicio de Sesión Fallido 1.2
- Descripción: Se intenta acceder al sistema sin completar 'Username' y 'Password' dejando ambos espacios vacíos
- Datos de Entrada:
    * Usuario: *campo vacío*
    * Contraseña: *campo vacío*
- Resultado Esperado: Mensaje: "Required" en ambos espacios
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-9.png)
    [Evidencia: Mensaje de Error](../Imagenes/image-10.png)

- ID: TC05
- Título: Inicio de Sesión Fallido 1.3
- Descripción: Se intenta acceder al sistema completando 'Username' y 'Password' con espacios en blanco
- Datos de Entrada:
    * Usuario: *espacio en blanco*
    * Contraseña: *espacio en blanco*
- Resultado Esperado: Esperado: Mensaje: "Required" en ambos espacios
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-11.png)
    [Evidencia: Mensaje de Error](../Imagenes/image-12.png)