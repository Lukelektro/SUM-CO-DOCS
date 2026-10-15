# Decisiones y pendientes

Este resumen conserva el estado indicado por cada fuente. La existencia de un ADR o de código no transforma una propuesta en decisión aprobada.

## Decisiones documentadas

| Tema | Estado que declara la fuente | Síntesis divulgable | Fuente y límite |
|---|---|---|---|
| Reglas centrales de dominio | D1–D9 se presentan como cerradas | Se registran reglas para abastecimiento, planificación, membresía por proyecto, trazabilidad y operación principalmente en línea. | `PR-SUM-CO-DOCS/03-Modelo-de-datos/modelo-v2/02-Documentacion/DECISIONES-D1-D9.md`. La síntesis omite políticas financieras y detalles de permisos. |
| Freeze de arquitectura de migración | Aprobado según el registro asociado a ADR-0009 | Se congeló un baseline para ejecutar la migración priorizando preservar capacidades existentes. | `PR-SUM-CO-DOCS/09-Trazabilidad/decisiones/ADR-0009-architecture-freeze-approved.md`. El alcance es el freeze de migración, no el cierre del producto. |
| Gestión de identidad externa previa al contexto | `ACTIVE` en el encabezado de ADR-0013 | Se documenta una decisión en curso sobre resolución controlada de identidad externa. | `PR-SUM-CO-DOCS/09-Trazabilidad/decisiones/ADR-0013-controlled-pre-context-external-identity-resolution.md`. No se presenta como decisión cerrada. |

Los ADR 0001–0012 no comparten en sus encabezados un campo normalizado de estado. Por ello, este compendio no los clasifica en bloque como aprobados; cada decisión requeriría revisar su resolución explícita antes de divulgarla como cerrada.

## Pendientes de seguimiento

- El checklist integrado de DOCS conserva tareas pendientes y en curso. Su snapshot y limitaciones están en [estado agregado](../planificacion-y-avances/estado-agregado.md).
- Los registros de migración describen una etapa cerrada; ese cierre no reemplaza la validación independiente de recorridos funcionales pendientes.
- La validación STAGING citada es específica de una lectura. No constituye aprobación general de autenticación, escritura, producción o de todo el backend.
- Las ramas no integradas contienen propuestas de reconciliación y evidencia adicional. Se describen por separado y no cambian el estado de `main`.

## Cómo interpretar esta página

Las decisiones funcionales se resumen sin replicar manuales ni SQL. Los diseños objetivo se mantienen como **PROPUESTO** hasta tener aprobación explícita; los asuntos que las fuentes no resuelven permanecen **PENDIENTE** o **REVISAR**.
