*GET*
- ID: TC-01
- Título: Obtener un post.
- Descripción: Validar que el sistema devuelva correctamente los datos del post con ID 1.
- Datos de Entrada:
    * Request: `GET` _https://jsonplaceholder.typicode.com/posts/1_
    * Body: N/A
- Pasos:
    1. Ingresar a Postman.
    2. Enviar petición GET al EndPoint </post/1>.
    3. Validar respuestas.
- Resultado Esperado:
    1. Código de Estado: `200 OK`
- Evidencias:
    [Evidencia: Petición GET](Imagenes/image-0.png)
    [Caso de Prueba Ejecutado](Imagenes/image-1.png)


*POST*
- ID: TC-02
- Título: Crear un post.
- Descripción: Verificar que el sistema acepte un nuevo post y devuelve un ID generado.
- Datos de Entrada:
    * Request: `POST` _https://jsonplaceholder.typicode.com/posts_
    * Body: 
        {
            "title": "QA Tester",
            "body" : "Creación de post para testing en Postman",
            "userId": 1
        }
- Pasos:
    1. Ingresar a Postman.
    2. Enviar una petición POST al EndPoint </post> con el Body indicado.
    3. Verificiar respuestas y Body.
- Resultado Esperado:
    1. Código de Estado: `201 Created`
    2. Body:
        - Debe incluir un nuevo campo "id".
        - Los campos enviados deben reflejarse correctamente en la respuesta.
- Evidencias:
    [Evidencia: Petición POST](Imagenes/image-2.png)
    [Caso de Prueba Ejecutado](Imagenes/image-3.png)

*PUT*
- ID: TC-03
- Título: Editar un post existente.
- Descripción: Valdiar que se puede modificar un post con ID 1.
- Datos de Entrada:
    * Request: `PUT` _https://jsonplaceholder.typicode.com/post/1_
    * Body:
        {
            "id": 1,
            "title": "QA Editado",
            "body" : "Contenido actualizado para testing en Postman",
            "userId": 1
        }
- Pasos:
    1. Ingresar a Postman.
    2. Enviar una petición PUT al EndPoint  </post/1> con el nuevo Body.
    3. Verificar respuestas y Body modificado.
- Resultado Esperado:
    1. Código de Estado: `200 OK` 
    2. Body:
        - Datos actualizados correctamente
- Evidencias:
    [Evidencia: Petición PUT](Imagenes/image-4.png)
    [Caso de Prueba Ejecutado](Imagenes/image-5.png)

*DELETE*
- ID: TC-04
- Título: Eliminar un post existente.
- Descripción: Validar que el sistema acepte eliminar un post con ID 1.
- Datos de Entrada:
    * Request: `DELETE` _https://jsonplaceholder.typicode.com/post/1_
    * Body: N/A
- Pasos:
    1. Ingresar a Postman.
    2. Enviar una petición DELETE al EndPoint </post/1>.
    3. Validar respuesta y el body vacíos.
    4. Enviar una petición GET al EndPoint </post/1>.
    5. Validar respuesta.
- Resultado Esperado:
    1. Código de Estado:
        - `200 OK`
        - `204 No Content` 
    2. Body: 
        - Debe estar vacío o mostrar "{}"
- Evidencias:
    [Evidencia: Petición DELETE](Imagenes/image-6.png)
    [Caso de Prueba Ejecutado](Imagenes/image-7.png)

*GET*
- ID: TC-05
- Título: Obtener un post inexistente.
- Descripción: Verificar la respuesta del sistema al solicitar un post con un ID inexistente.
- Datos de Entrada:
    * Request: `GET` _https://jsonplaceholder.typicode.com/post/999_
    * Body: N/A
- Pasos:
    1. Ingresar a Postman.
    2. Eviar una petición GET al EndPoint </post/99>.
    3. Verificar respuesta.
- Resultado Esperado:
    1. Código de Estado: `404 Not Found`
    2. Body:
        - Sin información útil
- Evidencias:
    [Evidencia: Peticion GET Fallida](Imagenes/image-8.png)
    [Caso de Prueba Ejectuado](Imagenes/image-9.png)