*Cierre de Sesión Fallido*
- ID: B-01
- Título: Sesión Invalidada Incorrectamente
- Descripción: La sesión del usuario persiste después de cerrar y volver a abrir el navegador
- Pasos para Reproducción:
    1. Iniciar sesión con usuario válido
    2. Cerrar navegador sin cerrar sesión manualmente
    3. Reabrir el navegador e ingresar a la misma página
- Prioridad: Media
- Severidad: Media
- Resultado Actual: El sistema no invalida la sesión correctamente y no requiere el login
- Resultado Esperado: El sistema debería invalidar la sesión y requerir login nuevamente
- Evidencias:
    [Reporte del Defecto](../Imagenes/image-16.png)
    [Evidencia Bug: Cierre del Navegador](https://jam.dev/c/8e41bbc7-4c71-48ee-8c10-4da98480f678)

# Mi conclusion: 
No impide el uso general del sistema ni afecta a una funcionalidad crítica directa, tampoco rompe la lógica principal del negocio. Por otro lado, se expone una vulnerabilidad de seguridad importante sobre todo en en entornos públicos o compartidos.
En entornos más exigentes, como por ejemplo bancaria o salud, podrían considerarse una severidad y prioridad Alta