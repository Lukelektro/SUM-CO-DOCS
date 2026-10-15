# Glosario y mapa de navegación

Este mapa conecta los temas del compendio y define términos usados en la documentación de Sumatoria.

## Navegación

- [Informe académico](informe-academico.docx) · [PDF](informe-academico.pdf)
- [Visión y alcance](proyecto/vision-y-alcance.md)
- [Módulos y madurez](proyecto/modulos-y-madurez.md)
- [Arquitectura actual](arquitectura/estado-actual.md)
- [Decisiones y pendientes](arquitectura/decisiones-y-pendientes.md)
- [Hitos](planificacion-y-avances/hitos.md)
- [Estado agregado](planificacion-y-avances/estado-agregado.md)
- [Pruebas](pruebas-y-validacion/resultados.md)
- [Anexos y procedencia](anexos/README.md)
- [Modelo de datos conceptual](anexos/modelo-conceptual.svg)

## Términos

| Término | Significado | Distinción de estado |
|---|---|---|
| SumatoriaCO | Empresa vinculada al sistema. | No es el equipo de desarrollo ni el nombre del producto. |
| EFFIXI | Equipo que desarrolla Sumatoria. | No se usa como nombre de empresa cliente. |
| Sumatoria | Sistema y proyecto descrito en este compendio. | Sus módulos tienen estados distintos. |
| APT | Proyecto académico aplicado usado para organizar la entrega formativa. | Los requisitos curriculares oficiales deben confirmarse con la institución. |
| ADR | Registro de una decisión de arquitectura. | Un ADR puede estar propuesto, activo, aceptado o reemplazado; se respeta el estado escrito en la fuente. |
| Backlog | Lista priorizada o registrada de trabajo por realizar. | Una tarea en el backlog no prueba que se haya ejecutado. |
| Scrum | Marco de trabajo iterativo descrito en la planificación del proyecto. | La fuente menciona ciclos de dos semanas; no se encontraron evidencias completas de todas las ceremonias. |
| Kanban | Método visual para gestionar el flujo de tareas. | La presencia de una vista Kanban no demuestra por sí sola persistencia ni operación completa. |
| Definition of Done | Criterios acordados para considerar terminado un elemento. | Se requiere evidencia de criterios aplicados; una plantilla no demuestra cumplimiento. |
| STAGING | Ambiente de validación separado de producción. | Un registro histórico de despliegue no confirma su estado actual. |
| E2E | Prueba de extremo a extremo entre varios componentes. | El caso documentado cubre una lectura acotada de proyecto. |
| PostgreSQL 16.15 | Versión del motor indicada en los registros de validación local. | No equivale a una inspección actual de una instancia remota. |
| U0–U7 | Unidades de la migración arquitectónica MIG-ARCH-001. | El gate de migración se reportó cerrado; el backlog posterior conserva trabajo pendiente. |
| main | Rama principal integrada observada en cada repositorio. | El 15-10-2026 se consultó y actualizó `main` de PC y DOCS; los SHAs se indican en el estado agregado. No se obtuvo un inventario completo de ramas remotas. |
| Rama no integrada | Cambio que solo aparece en una referencia separada de main local. | Puede aportar evidencia o código, pero no se atribuye a main. |
| Fast-forward | Actualización de una rama cuando su historial remoto desciende del commit local. | En esta actualización se usó para avanzar ambos `main` sin crear merge commit. |
| Database 2.2.3 | Candidato de evolución del modelo relacional que incorpora creación delegada de proyectos. | Validado localmente según los registros y presente en `main`; no consta desplegado en STAGING o producción. |
| PASS | Resultado positivo para un criterio y entorno definidos. | No se extrapola a funciones fuera del gate probado. |
| PARTIAL | Evidencia o implementación cubre solo una parte del flujo. | No significa necesariamente fallo. |
| PENDING | Trabajo o criterio abierto en el snapshot citado. | Debe leerse con su fecha y alcance. |
| IMPLEMENTADO | El código observado contiene la capacidad nombrada. | No afirma despliegue ni validación completa. |
| PARCIAL | Hay componentes, pero falta una parte del flujo o evidencia de cierre. | Se aplica a una capacidad concreta. |
| PROTOTIPO | Interfaz o prueba de concepto sin operación integral demostrada. | No equivale a una función disponible a usuarios. |
| PROPUESTO | Requisito o alcance en planificación. | No implica que exista en el producto. |
| HISTÓRICO | Evidencia de un corte previo. | Se conserva para explicar evolución, no como estado actual. |
