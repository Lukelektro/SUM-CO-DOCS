# Pruebas y validaciones documentadas

Los registros siguientes describen resultados escritos en las fuentes y contrastados con el estado integrado en `main`. No se reejecutaron pruebas, builds, migraciones ni consultas a STAGING para esta edición.

| Fecha | Prueba y procedimiento documentado | Resultado reportado | Alcance y límite |
|---|---|---|---|
| 2026-09-26 | Dos instalaciones limpias de la baseline de base de datos en PostgreSQL 16.15; verificaciones de catálogo y generación/contraste de la proyección. | PASS; el release también reporta 37 verificaciones estáticas sin fallos. | Resultado local documentado para DB V2.2.0. No prueba despliegue remoto, backup/restore cloud ni integración total del producto. |
| 2026-09-26 | Gates de seguridad y concurrencia de la baseline de base de datos; el registro indica tres ejecuciones del gate de concurrencia. | PASS según el release documentado. | El informe no reproduce los casos sensibles ni scripts internos; aplica al modelo y entorno indicados. No constituye certificación de todos los servicios. |
| 2026-10-01 | Gate de integración física de base de datos U4 sobre PostgreSQL 16.15, con suite específica del gate. | 21/21 pruebas PASS en el reporte formal. | Evidencia del gate U4 y su harness. No es el total de pruebas de Sumatoria ni prueba todos los dominios. |
| 2026-10-01 | Suite backend foundation y suite frontend de estado/dominio, registradas en el gate final. | 182 tests backend y 165 frontend reportados PASS; ocho suites backend. | Resultado documentado en el gate final. No se reejecutó en esta preparación y no mide el avance global. |
| 2026-10-01 | Flujo browser FLOW-008 en Chromium/Puppeteer. | PASS reportado; se registró generación de dos documentos PDF sin errores observados en el gate. | Solo el flujo de render identificado por el gate; no demuestra calidad de todo el frontend ni se adjuntan artefactos generados. |
| 2026-10-03 | Autenticación de identidad real y lectura de un proyecto en STAGING; token válido, resolución a usuario interno y consulta de lectura. | El log reporta HTTP 200 y respuesta exitosa. | Resultado operacional entregado por el owner y documentado. Cubre una lectura específica; no se probaron por HTTP todos los casos negativos, escrituras, rutas, usuarios o producción. |
| 2026-10-04 | Flujo de Google OAuth de escritorio con PKCE e intercambio con Identity Platform; el código se integró después en `main`. | El log de ejecución reporta validación del flujo y la integración está presente en PC `main`. | Evidencia documentada, no reejecutada en esta actualización. No acredita firma, distribución, estado actual de configuración o una sesión completa de API. |
| 2026-10-12 | Regresión post-migración de frontend, contratos de API/sesión y recorridos funcionales. | Los registros y README de PC informan 251 pruebas, además de validaciones de build, lint, typecheck y flujo PDF; el gate mantiene revisión final pendiente. | Conteos y resultados documentados, no reejecutados aquí. No se interpretan como pruebas de STAGING ni como porcentaje de producto terminado. |
| 2026-10-15 | Gate local Database 2.2.3 y regresión de Project Routes con PostgreSQL 16.15 y fixtures sintéticos. | El checkpoint informa T01–T16 PASS, regresión HTTP de lectura 6/6, rutas POST/LIST/GET, `test:foundation` 208/208, typecheck y build PASS. | Candidato local. El log indica que no se desplegó a STAGING/Cloud SQL/producción ni se asignó el permiso de creación a roles productivos. Resultados documentados; no reejecutados aquí. |

## Interpretación

Cada PASS se conserva unido a su fecha, entorno y criterio. El gate final del 01-10 describe cierre de MIG-ARCH-001; el backlog integrado del 03-10 conserva tareas PENDING e IN_PROGRESS. Ambos registros tienen alcances distintos.

Los resultados de STAGING no se presentan como certificación actual de GCP. La documentación de la baseline DB V2.2.0 incluye estados antiguos de infraestructura; registros posteriores describen V2.2.2 en STAGING y V2.2.3 en pruebas locales. No se consultaron recursos cloud en esta preparación.

## Reejecución de auditoría

**AUDIT_REEXECUTION:** no realizada. Esta edición revisó documentación y código integrado en `main`, sin iniciar suites, instalaciones de base de datos, builds ni llamadas a servicios externos.
