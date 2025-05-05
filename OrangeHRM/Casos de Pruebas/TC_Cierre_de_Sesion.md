*Cierre de Sesión Exitoso*
- ID: TC06
- Título: Cierre de Sesión Exitoso
- Descripción: El usuario cierra sesión y sale del sistema correctamente
- Pasos:
    1. Hacer clic en el ícono de usuario
    2. Hacer clic en en "Log out"
- Resultado Esperado: El sistema redirige al usuario a la pantalla de inicio de sesión, y la sesión se termina correctamente
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-13.png)
    [Evidencia: Cierre de Sesión](https://jam.dev/c/653faf02-770b-40e3-9466-c94a6022fbc9)

*Cierre de Sesión Fallido*
- ID: TC07
- Título: Cierre de Sesión Fallido 1
- Descripción: Se intenta cerrar sesión y el proceso es interrumpido
- Pasos:
    1. Hacer clic en el ícono de usuario
    2. Hacer clic en en "Log out"
    3. Interrumpir el proceso cerrando rápidamente el navegador
    4. Abrir el navegador
- Resultado Esperado: El sistema no finaliza correctamente la sesión y el usuario puede continuar accediendo sin necesidad de login
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-14.png)
    [Evidencia: Cierre de Sesión Interrumpido](https://jam.dev/c/653faf02-770b-40e3-9466-c94a6022fbc9)

- ID: TC08
- Título: Cierre de Sesión Fallido 1.1
- Descripción: Se intenta cerrar sesión cerrando directamente el navegador
- Pasos:
    1. Cerrar el navegador sin cerrar sesión
    2. Abrir el navegador 
- Resultado Esperado: El sistema debería haber invalidado la sesión y requerir login nuevamente
- Evidencias:
    [Caso de Prueba Ejecutado](../Imagenes/image-15.png)
    [Evidencia: Cierre del Navegador](https://jam.dev/c/8e41bbc7-4c71-48ee-8c10-4da98480f678)