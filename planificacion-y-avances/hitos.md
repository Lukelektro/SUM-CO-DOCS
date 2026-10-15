# Hitos documentados

Las fechas se distinguen por origen. Una fecha de commit es un registro de Git, no la hora de trabajo de una persona. Una fecha escrita en un log no garantiza que los hechos se hayan repetido durante esta auditoría.

| Fecha | Tipo | Hito y estado | Evidencia y límite |
|---|---|---|---|
| 2026-08-15 | Fecha de documento | Se emitió una propuesta de módulos y alcance. PROPUESTO. | Documento de planificación de módulos; no demuestra implementación. |
| 2026-09-26 | Fecha de documento | Se congeló la baseline PostgreSQL V2.2.0 para instalaciones nuevas. | Release y documentación de DB; validaciones locales documentadas. |
| 2026-09-30 | Corte de informe | El informe APT versionado describía MIG-ARCH-001 en curso. HISTÓRICO. | Leído desde Git tras encontrar una eliminación local; no se restauró. El estado fue superado por el gate del día siguiente. |
| 2026-10-01 | Fecha de documento | El gate formal MIG-ARCH-001 se reportó PASS/CLOSED e incluyó pruebas y reconciliación de preservación. | PASS del gate con su alcance; no cierra todo el producto ni tareas posteriores. |
| 2026-10-01 | Fecha de commit | El historial de PC main registra integración frontend con endpoints Fastify y validación de base de datos para U4. | Commits integrados localmente; el mensaje de commit no sustituye resultados de pruebas. |
| 2026-10-02 | Fecha de commit | Se registró retiro del runtime Express legado y cierre de la unidad U7 en el historial integrado. | Hito técnico de migración, no de finalización de módulos de negocio. |
| 2026-10-03 | Fecha de documento y commit | Se documentó resolución OIDC y lectura de un proyecto en STAGING con HTTP 200 reportado. | Evidencia de un camino real acotado; no reproducida durante esta preparación. |
| 2026-10-03 | Fecha de snapshot | El checklist de main registró 39 unidades: 33 PENDING y 6 IN_PROGRESS. | Conteo de backlog; no es porcentaje de avance del sistema. |
| 2026-10-04 | Fecha de referencia cacheada | Se observó una rama local no integrada con reconciliación de backend/tareas. | Solo evidencia local cacheada; no confirma actividad remota actual. |

## Procedencia

Hitos derivados de documentos de planificación, logs de ejecución y commits integrados en los checkouts locales. Las diferencias temporales se conservan explícitas; no se convierten en horas trabajadas.
