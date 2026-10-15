# Compendio académico de Sumatoria

Este repositorio reúne un informe académico y síntesis públicas sobre el desarrollo de Sumatoria. El documento principal es el [informe académico en DOCX](informe-academico.docx); también está disponible en [PDF](informe-academico.pdf). La documentación Markdown facilita la navegación y mantiene la procedencia de las afirmaciones.

**Fecha de corte documental:** 15 de octubre de 2026.

## Identidad

- **SumatoriaCO** es la empresa.
- **EFFIXI** es el equipo que desarrolla Sumatoria.
- **Sumatoria** es el sistema y proyecto descrito.

## Navegación

- [Informe académico](informe-academico.docx) · [PDF de lectura](informe-academico.pdf)
- [Glosario y mapa](glosario.md)
- [Visión y alcance](proyecto/vision-y-alcance.md)
- [Módulos y madurez](proyecto/modulos-y-madurez.md)
- [Arquitectura actual](arquitectura/estado-actual.md)
- [Decisiones y pendientes](arquitectura/decisiones-y-pendientes.md)
- [Hitos](planificacion-y-avances/hitos.md)
- [Estado agregado](planificacion-y-avances/estado-agregado.md)
- [Pruebas y validaciones](pruebas-y-validacion/resultados.md)
- [Anexos y procedencia](anexos/README.md)
- [Modelo de datos conceptual](anexos/modelo-conceptual.svg)

## Fuentes y límites

La síntesis se preparó contrastando el código de PR-SUM-CO-PC con la documentación de PR-SUM-CO-DOCS. Los checkouts locales consultados tenían PC y DOCS en main. La rama de continuación parte de la primera edición publicada del compendio.

Las referencias a ramas remotas de los repositorios fuente eran referencias cacheadas localmente. El 15 de octubre de 2026, GitHub no respondió a una consulta de solo lectura desde este equipo. Por eso, este compendio no afirma cuál es el estado remoto actual de esas ramas. Esta limitación no afecta la identificación de los commits que ya estaban integrados en los checkouts locales de main.

Las guías DUOC se usaron para organizar los apartados académicos y definir los entregables de la ruta Scrum/Kanban. No se adjuntan ni se reproducen. El informe grupal versionado eliminado en el checkout fuente se leyó desde Git como antecedente histórico fechado el 30 de septiembre de 2026; no se restauró ni se incorporó. Los diarios individuales, nombres y asignaciones personales se excluyeron.

El compendio no incluye código, SQL, permisos, credenciales, configuración operativa, identificadores de infraestructura, hallazgos internos de seguridad ni documentos completos de terceros. Las referencias de procedencia describen repositorio y documento, no exponen rutas privadas del equipo.

## Estados de madurez

- **IMPLEMENTADO:** el código observado contiene la capacidad descrita. No implica despliegue ni validación integral.
- **PARCIAL:** se observan componentes, pero falta parte del flujo o su validación.
- **PROTOTIPO:** interfaz o prueba de concepto sin flujo operativo completo demostrado.
- **PROPUESTO:** alcance descrito en planificación o diseño, sin evidencia suficiente de implementación.
- **PENDIENTE:** la fuente de seguimiento lo mantiene abierto o falta evidencia para resolverlo.
- **HISTÓRICO:** refleja un corte anterior y no representa automáticamente el estado actual.

## Cómo usarlo

Cada resultado conserva su alcance y fuente. Los PASS citados corresponden a gates documentados, no a una calificación global. El registro de lectura en staging es un caso acotado; no certifica todas las rutas, usuarios, permisos, escritura ni producción. No se repitieron pruebas ni se inspeccionó GCP durante la preparación de esta edición.

Este compendio complementa y no reemplaza los repositorios oficiales del sistema y de su documentación.
