[HU03][Navegación entre Secciones]

`Como` usuario registrado
`Quiero` poder navegar entre todas las secciones del menú
`Para` acceder a las distintas funcionalidades del sistema

*Criterios de Aceptación*
1. 
    `Dado` que el usuario se encuentra en el panel principal
    `Cuando` haga clic en la sección del menú (PIM, My info, Leave)
    `Entonces` será redirigido correctamente a dicha sección
2. 
    `Dado` que el usuario se encuentra en el panel principal
    `Cuando` intento acceder a una sección no disponible
    `Entonces` debo ver un mensaje de error o ser redirigido a una página válida

[HU04][Búsqueda]

`Como` usuario registrado
`Quiero` poder realizar búsquedas 
`Para` encontrar facilmente registros o información que me interese

*Criterios de Aceptación*
1. 
    `Dado` que el usuario se encuentra en una sección/barra de búsqueda
    `Cuando` ingrese un término válido y haga clic en "Buscar"
    `Entonces` se debe mostrar los resultados coincidentes
2. 
    `Dado` que el usuario se encuentra en una sección/barra de búsqueda
    `Cuando` ingrese un término inválido y haga clic en "Buscar"
    `Entonces` se debe mostrar un mensaje indicando que no se encontraron resultados