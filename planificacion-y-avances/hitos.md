# Hitos documentados

Las fechas de commit son fechas registradas por Git. Las fechas de documentación describen lo que indica el documento; ninguna se interpreta automáticamente como jornada de trabajo.

| Fecha | Tipo de fecha | Hito y estado | Fuente / alcance |
|---|---|---|---|
| 2026-08-15 | DOCUMENTED_DATE | Se emitió una propuesta de módulos y alcance para Sumatoria. **PROPUESTO**. | `PR-SUM-CO-DOCS/01-Documentacion/SUMATORIA/Planteamiento/DESCRIPCION_MODULOS_PROYECTO_SUMATORIA_ERP.txt`; no acredita ejecución ni se reproducen sus cifras comerciales. |
| 2026-09-26 | DOCUMENTED_DATE | Se fijó la documentación de release de la baseline DB 2.2.0. **HISTÓRICO**. | `PR-SUM-CO-DOCS/03-Modelo-de-datos/modelo-v2/02-Documentacion/DATABASE-RELEASE-V2.2.md`; la documentación posterior trata migración/runtime 2.2.2. |
| 2026-10-01 | DOCUMENTED_DATE | El gate formal de migración se reportó cerrado; el informe registra pruebas y alcance de preservación. | `PR-SUM-CO-DOCS/10-Migracion-Arquitectura/05-Validacion/GATE-MIG-FINAL-2026-10-01.md`; PASS corresponde a ese gate. |
| 2026-10-01 | COMMIT_DATE | `7c7fa76` registra conexión de frontend con endpoints Fastify y cierre de U6 en el mensaje del commit. | `PR-SUM-CO-PC`, historial local de `main`; el mensaje no demuestra por sí solo validación integral. |
| 2026-10-02 | COMMIT_DATE | `14fd207` registra una suite de integración de base de datos para el gate U4; `cc38c56` registra retiro del runtime Express legado y cierre de U7. | `PR-SUM-CO-PC`, historial local de `main`; son hitos de migración, no de finalización del producto. |
| 2026-10-03 | COMMIT_DATE | En `main` se registran cambios de resolución de identidad OIDC y compatibilidad de rutas de salud. | `PR-SUM-CO-PC`, commits `74c182e`, `9d35df4` y `2418eba`; las capacidades se describen con alcance en [módulos](../proyecto/modulos-y-madurez.md). |
| 2026-10-03 | DOCUMENTED_EVENT_DATE | El log de ejecución reporta una lectura E2E de proyecto en STAGING con HTTP 200. | `PR-SUM-CO-DOCS/09-Trazabilidad/ejecuciones/2026/10/EXE-2026-10-03-STAGING-BACKEND-IDENTITY-PROJECT-READ-E2E.md`; resultado reportado por el owner, no reproducido en este compendio. |
| 2026-10-03 | COMMIT_DATE | `4b4aea4` registra en DOCS el cierre documental de esa lectura específica. | `PR-SUM-CO-DOCS`, `main`; no certifica todas las tareas ni el backend completo. |
| 2026-10-04 | COMMIT_DATE | Una referencia de reconciliación de backend/tareas, disponible en el clon local, registra avances y estado de tareas. | Rama no integrada en `main` local. El remoto actual no se pudo consultar; véase [estado agregado](estado-agregado.md). |

## Procedencia

Las fechas de commit se obtuvieron del historial local de ambos clones. Las fechas de los eventos STAGING provienen de los logs documentales. No se consultó GitHub en vivo ni se inspeccionó infraestructura cloud.
