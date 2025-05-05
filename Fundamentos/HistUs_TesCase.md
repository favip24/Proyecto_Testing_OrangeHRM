*Historias de Usuarios y Criterios de Aceptación*
* Las Historias de Usuarios son descripciones breves de una funcionalidad desde el punto de vista del usuario final. Por otro lado, los Criterisos de Aceptación son las condiciones que deben cumplirse para aceptar esa funcionalidad como correcta.

* El formato más común es:
[ID][Título]
`Como` = [Rol]
`Quiero` = [Funcionalidad]
`Para`= [Beneficio] o [Propósito]

[Criterios][Condiciones]
`Dado` = [Inicio]
`Cuando` = [Acción]
`Entonces` = [Concecuencia]

* Entonces quedaría algo así, por ejemplo:
    - Como usuario registrado
    - Quiero ingresar a mi cuenta de Super Mami
    - Para poder acceder a beneficios y descuentos

* Criterios de Aceptación:
    - Dado que ek usuario está en la página ed inicio de sesión
    - Cuando ingrese las credenciales válidas y haga clic en "Login"
    - Entonces debe ser redirigido al panel principal

* Este formato es muy útil ya que facilita la comunicación y establece claramente el `contexto`, la `acción` y la `respuesta esperada`.

*Casos de Pruebas*
* Son documentos detallados que se utiliazan para verificar que una funcionalidad funciona correectamente. Esta se crea a partir de requisitos, historias de usuarios, etc.
* El formato más común es:

`ID` = Identificador único del caso de prueba
`Título` = Aquello qué se va a probar
`Descripción`= Descripción breve de la funcionalidad
`Precondiciones`= Requisitos previos para realizar el caso de prueba
`Pasos`= Guía para ejecutar el caso de prueba
`Datos de Entrada`= Datos que ingresarán en el paso a paso
`Resultado Esperado`= Lo que se espera como resultado (un mensaje de error, etc)
`Resultado Obtenido`= El resultado real (una vez ejecutado)
`Estado`= Aprobado o Fallido (una vez ejecutado)