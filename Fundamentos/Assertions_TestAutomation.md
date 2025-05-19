# Assertions con Javascript en Postman #

`¿Qué son?`
- Validaciones automáticas que se ejecutan solamente dentro del entorno de Postman.
- Usa Javascript básico (con funciones propias de la librería 'pm' de Postman).
- No se integran fácilmente con pipelines CI/CD, no permiten flujos complejos, ni lógica avanzada de automatización.

`Objetivos`
- Asegurar que la API devuelve lo esperado, se consideran parte del _testing automatizado ligero o semiautomatico_.

`javascript`
pm.test("Status code is 200", function () {
  pm.response.to.have.status(200);
});

# Pruebas Automatizadas #

`¿Qué son?`
- Scripts que automatizan flujos de pruebas, con lógica compleja, múltiples pasos, validaciones, reportes, etc.
- Pueden correr en entornos como CI/CD (Jenkins, GitHub, etc) o locales.

`Objetivos`
- Automatizar pruebas regresivas, integrarlas al desarrollo continuo, escalar testing.

`Lenguajes y Frameworks`
- Java + RestAssured
- JavaScript + Cypress / Jest / Mocha
- Python + Pytest / Requests
- Postman + Newman (para CI/CD con colecciones)

*Conclusión*
- Las Assertions de Postman son un excelenter primer paso hacia la automatización, pero las pruebas automatizadas completas son más potentes, escalables y integrables.