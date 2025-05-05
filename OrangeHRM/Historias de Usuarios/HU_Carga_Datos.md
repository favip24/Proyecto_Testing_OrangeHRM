[HU05][Carga de Datos]

`Como` usuario registrado
`Quiero` poder cargar datos nuevos al sistema
`Para` mantener la información actualizada

*Criterios de Aceptación*
1. 
    `Dado` que el usuario se encuentra en el formulario de carga de datos
    `Cuando` se completan los campos obligatorios correctamente y se hace clic en "enviar"
    `Entonces` el sistema debe guardar los datos y mostrar un mensaje de éxito
2. 
    `Dado` que el usuario se encuentra en el formulario de carga de datos
    `Cuando` deja los campos obligatorios vacíos y hace clic en "enviar"
    `Entonces` el sistema debe mostrar un mensaje indicando que falta completar campos obligatorios y no se guardaran datos