[HU01][Inicio de Sesión]

`Como` usuario registrado
`Quiero` ingresar mis credenciales
`Para` acceder al panel principal de OrangeHRM

*Criterios de Aceptación*
1. 
    `Dado` que el usuario se encuentra en la página de inicio de sesión
    `Cuando` ingrese las credenciales válidas y haga clic en "log in"
    `Entonces` será redirigido al panel principal de OrganHRM
2. 
    `Dado` que el usuario se encuentra en la página de inicio de sesión
    `Cuando` ingrese las credenciales NO válidas y haga clic en "log in"
    `Entonces` Se mostrará un mensaje de error y permanecerá en la misma página

[HU02][Cierre de Sesión]

`Como` usuario autenticado
`Quiero` poder cerrar mi sesión
`Para` garantizar la seguridad de mi cuenta y mis datos

*Criterios de Aceptación*
1. 
    `Dado` que el usuario se encuentra en el panel principal
    `Cuando` haga clic en "log out"
    `Entonces` será redirigido a la página de inicio de sesión
2. 
    `Dado` que el usuario se encuentra en el panel principal
    `Cuando` cierre el navegador y lo vuelva a abrir
    `Entonces` la sesión se invalidará y deberá cerrarse correctamente