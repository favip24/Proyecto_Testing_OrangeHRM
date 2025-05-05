*Navegación Fallida: Acceso Fallido por tiempo de expiración de Sesión*
- ID: B-02
- Título: Sesión NO invalidada tras tiempo de expiración por inactividad
- Descripción: El sistema no invalidad la sesión tras el tiempo de inactividad esperado, permitiendo el acceso continuo sin reautenticación
- Pasos para Reproducción:
    1. Iniciar sesión con usuario válido
    2. Permanecer inactivo por al menos 5 minutos (timeout estimado)
    3. Intentar navegar por las secciones nuevamente
- Prioridad: Alta
- Severidad: Media
- Resultado Actual: El sistema no invalida la sesión y permite la libre navegación sin solicitar reautenticación aún pasado el tiempo de expiración
- Resultado Esperado: El sistema debería invalidar la sesión y requerir reautenticación pasado el tiempo de expiración de sesión
- Evidencias:
    [Reporte del Defecto](../Imagenes/image-20.png)
    [Evidencia Bug: Navegación Fallida](https://jam.dev/c/7fd1acd9-26be-4914-b5ab-9027c4d294b0)

# Mi conclusion: 
Se está validando una funcionalidad relacionada con la seguridad, si el sistema no invalida la sesión luego del tiempo estipulado está ocurriendo un comportamiento inesperado.
El sistema debería cerrar la sesión luego de 5 minutos de inactividad.