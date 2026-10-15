# Procedencia y alcance de la evidencia pública

## Fuentes consultadas

| Fuente | Uso en el compendio | Tratamiento |
|---|---|---|
| Guías DUOC APT de avance, informe final y apoyo | Estructura académica y ruta Scrum/Kanban. | Citadas como fuentes institucionales de estructura; no adjuntas ni reproducidas. |
| Informe grupal APT versionado en DOCS y eliminado del working tree | Contexto y snapshot histórico con corte 30-09-2026. | Leído directamente desde Git sin restaurarlo. Se descartaron nombres, asignaciones, rutas internas y estados superados por evidencia posterior. No se copia el documento. |
| Código de PR-SUM-CO-PC `main`, actualizado desde GitHub el 15-10-2026, SHA `ceb973b` | Contraste de módulos, backend, identidad, persistencia, Tauri y rutas de proyectos. | Se describen capacidades de forma agregada; no se copia código. |
| PR-SUM-CO-DOCS, gate MIG-ARCH-001 del 01-10-2026 | Estado documentado de cierre de migración y suites incluidas. | Se resume con su alcance; no se adjunta el log completo. |
| PR-SUM-CO-DOCS, release DB V2.2.0 y registros de validación local | Baseline y pruebas locales de base de datos. | Se resumen resultados sin SQL, controles detallados ni configuración. |
| PR-SUM-CO-DOCS `main`, actualizado desde GitHub el 15-10-2026, SHA `cd46933` | Backlog global, trazabilidad, validación local de Database 2.2.3 y estado de integración. | Se usan conteos agregados y registros pertinentes. Se excluyen nombres, asignaciones personales, prompts y reglas de agentes. |
| PR-SUM-CO-DOCS, logs de runtime e identidad del 02–04-10-2026 | Evolución posterior, flujo de escritorio y E2E de lectura en STAGING. | La lectura HTTP 200 se mantiene acotada y documentada; se omiten cuentas, nombres de proyecto, configuración e identificadores. |
| Referencias remotas consultadas el 15-10-2026 | Confirmación del SHA actual de `main` en ambos repositorios fuente. | Solo se consultó `main`; no se validó el conjunto de ramas remotas ni el estado actual de ramas archivadas. |

## Material no incorporado

- Guías DUOC completas: material de terceros; uso limitado a estructura y cita.
- Diarios individuales y datos de autoría personal: excluidos.
- Informe APT anterior: no se publica por contener datos personales y un estado fechado que quedó superado. La copia eliminada del checkout fuente permanece intacta.
- Plantillas DUOC con nombres, asignaciones, identificadores y campos pendientes: no se publican; se usaron únicamente para identificar requisitos académicos.
- SQL, scripts de pruebas, permisos, runbooks, configuración de cloud y detalles de seguridad: excluidos por su carácter técnico-operacional.
- Evidencia de clientes y archivos generados: no incorporados.

## Limitaciones

La fecha de corte de fuentes es 15-10-2026. Se consultó GitHub y ambos `main` se actualizaron por fast-forward. Los logs de STAGING y las validaciones locales son evidencia documental de sus autores; no se reejecutaron. GCP no se inspeccionó. No se encontró evidencia completa de retrospectivas, métricas de impacto, competencias curriculares oficiales ni todos los artefactos académicos de Scrum/Kanban.
