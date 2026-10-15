# Glosario y mapa de navegación

Este archivo ofrece definiciones breves y lleva a las síntesis principales. No reemplaza los documentos fuente.

## Navegación

- [Visión y alcance](proyecto/vision-y-alcance.md)
- [Módulos y madurez](proyecto/modulos-y-madurez.md)
- [Arquitectura actual](arquitectura/estado-actual.md)
- [Decisiones y pendientes](arquitectura/decisiones-y-pendientes.md)
- [Hitos](planificacion-y-avances/hitos.md)
- [Estado agregado](planificacion-y-avances/estado-agregado.md)
- [Pruebas y validaciones](pruebas-y-validacion/resultados.md)

## Términos

| Término | Significado en este compendio | Estado o distinción relevante |
|---|---|---|
| SumatoriaCO | Empresa asociada al producto. | No es el nombre del equipo de desarrollo. |
| EFFIXI | Equipo que desarrolla Sumatoria. | No confundir con la empresa cliente ni con el sistema. |
| Sumatoria | Sistema/proyecto descrito en estos documentos. | Algunas funciones están implementadas y otras son parciales o propuestas. |
| ADR | Registro de una decisión de arquitectura. | La existencia de un ADR no implica aprobación; revisar su estado explícito. |
| Backlog | Conjunto de tareas registradas para trabajo futuro o en curso. | Una tarea escrita no demuestra que se haya ejecutado. |
| Kanban | Vista o flujo visual para organizar trabajo. | Hay interfaz en el código; el flujo completo conectado no se considera validado aquí. |
| STAGING | Entorno de validación distinto de producción. | El registro citado describe validaciones concretas; no confirma el estado actual de los recursos. |
| E2E | Prueba de extremo a extremo que recorre varios componentes. | La evidencia descrita aquí cubre una lectura de proyecto, no todo el backend. |
| U0–U7 | Unidades numeradas en la migración arquitectónica documentada. | La documentación marca el ciclo MIG-ARCH-001 como cerrado; esto no cierra todo el producto. |
| `main` | Rama integrada observada en cada clon local. | La consulta en vivo a GitHub no estuvo disponible en la fecha de corte. |
| Rama no integrada | Rama cuyo tip local no está contenido en `main` local. | Puede contener evidencia o cambios útiles; no equivale a integración ni a cierre. |
| PASS | Resultado positivo de una validación con alcance definido. | No es un porcentaje global ni se extiende a funciones fuera del gate. |
| PARTIAL | Cobertura incompleta en una matriz o gate específico. | No significa automáticamente fallo ni representa por sí sola todo el producto. |
| PENDING | Tarea o criterio aún no cerrado según el registro citado. | Debe acompañarse de la fecha y fuente del snapshot. |
| IMPLEMENTADO | Código actual contiene la capacidad descrita. | No implica despliegue ni validación funcional completa. |
| PARCIAL | Existe una parte del flujo, pero falta integración o evidencia de cierre. | Aplicado por capacidad, no como puntuación total del producto. |
| PROTOTIPO | Interfaz o prueba de concepto sin flujo operativo completo demostrado. | No debe describirse como función productiva. |
| PROPUESTO | Diseño o alcance planteado. | No implica implementación. |
| HISTÓRICO | Evidencia de una etapa anterior. | No describe automáticamente el estado actual. |
