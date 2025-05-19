# Conceptos clave sobre APIs REST

*API (Application Programming Interface)*
* Es un intermediario que permite la comunicación entre dos aplicaciones a través de un conjunto de reglas.

*REST (Representational State Transfer)*
Un estilo arquitectónico para el diseño de APIs basado en recursos y operaciones HTTP.

*Métodos HTTP más comunes*
* GET: Obtener información de un recurso.
* POST: Crear un nuevo recurso.
* PUT: Actualizar  por completo un recurso existente.
* PATCH: Modificar parcialmente un recurso existente.
* DELETE: Eliminar un recurso del servidor.

*Códigos de estado HTTP*
`🔵 1xx: Códigos Informativos`
-  El servidor ha recibido la petición y procederá con ella

`🟢 2xx: Códigos de Éxito`
- El servidor ha sido recibido, entendido y procesado correctamente la petición.
    - 200 OK: Solicitud exitosa.
    - 201 Created: Recurso creado correctamente.
    - 204 No Content: La solicitud se procesó correctamente, pero no hay contenido en la respuesta

`🟡 3xx: Códigos de Redirección`
- El servidor ha recibido la solicitud, pero hay una redirección a alguna otra parte.
    - 301 Moved Permanently: La URL solicitada ha cambiado de manera permanente.
    - 302 Found: Redirección temporal a otra URL.
    - 304 Not Modified: Indica que el contenido no ha cambiado desde la última vez que se solicitó

`🔴 4xx: Códigos de Error de Cliente`
- El servidor no puede encontrar la página o web. Se trata de un error del lado de la Web.
    - 400 Bad Request: Error en la solicitud del cliente.
    - 401 Unauthorized: Falta autenticación.
    - 403 Forbidden: El servidor comprendió la solicitud, pero el usuario no tiene permisos para acceder al recurso.
    - 404 Not Found: El recurso no existe.
    - 409 Conflict: Ocurre cuando hay un conflicto en la solicitud, como un intento de crear un recurso que ya existe.

`🟠 5xx: Códigos de Error del Servidor`
- El cliente ha realizado una solicitud válida, pero el servidor ha fallado al completarla.
    - 500 Internal Server Error: Error interno en el servidor, generalmente causado por un fallo en el código backend.
    - 502 Bad Gateway: Un servidor intermedio (gateway) recibió una respuesta inválida del servidor upstream.
    - 503 Service Unavailable: El servidor está sobrecargado o en mantenimiento.
    - 504 Gateway Timeout: Un servidor intermedio no recibió respuesta a tiempo del servidor upstream.

*Inspeccionar Headers*
* Los Headers contienen metadatos de la respuesta HTTP, como el tipo de contenido, lngitud, servidor, etc:
    - Content-Type: Indica el formato de la respuesta
    - Content-Length: Tamaño del cuerpo de la respuesta
    - Server: Información del servidor
    - Authorization: Si requiere token o credenciales

*Inspeccionar Terminal*
* Statud Code: Escencial para verificar si la petición se fue exitosa o falló
* Time: Ayuda a detectar lentitud o problemas de rendimiento
* Size: Alertar si se recibe una respuesta vacía o demasiado grande

*Variables de Entorno*
* Son una característica que permite almacenar y reutilizar valores de parámetros en solicitudes y scripts de API.
* Estas variables pueden ser estáticas o dinámicas y se pueden acceder en la URL, parámetros, POST, código Javascript, entre otros.