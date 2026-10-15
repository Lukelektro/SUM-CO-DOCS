# Decisiones y pendientes

Esta síntesis conserva el estado que indican las fuentes. Un diseño, un ADR o código presente no convierten por sí solos una decisión en aprobada ni cierran la funcionalidad.

## Decisiones y baselines documentadas

| Tema | Estado documentado | Síntesis pública |
|---|---|---|
| Stack de cliente | Baseline observada en código | React/Vite para la interfaz y Tauri para escritorio. La presencia del stack no acredita empaquetado vigente. |
| Backend | Implementación integrada en el checkout local de main | La migración hacia Node.js/Fastify reemplazó el runtime Express legado para el alcance integrado. No implica que todas las features estén migradas. |
| Modelo relacional | V2.2.0 FINAL para bootstrap nuevo según release del 26-09-2026 | Los cambios posteriores se registran mediante migraciones forward. No se publica SQL ni detalles de permisos. |
| Freeze de migración | Aprobado en registro de octubre | Fijó un baseline y criterios de preservación para MIG-ARCH-001. El gate formal se reportó cerrado el 01-10. |
| Resolución de identidad externa | ADR relacionado aparece como ACTIVE | El código integrado y la lectura E2E documentada aportan evidencia, pero el estado del ADR no se presenta como cerrado si la fuente no lo marca así. |

## Pendientes y límites

- El snapshot integrado de tareas del 03-10 conserva 33 pendientes y 6 en curso de 39 unidades. El cierre de MIG-ARCH-001 no cierra ese backlog posterior.
- Falta evidencia de ciclos Scrum completos, retrospectivas y Definition of Done aplicado por incremento.
- No se encontraron mediciones de rendimiento, impacto, satisfacción ni objetivos de negocio cuantificados.
- No se verificó el estado actual de GCP, producción, backups ni recuperación.
- La documentación no aporta la malla académica oficial para asignar competencias curriculares; debe cotejarse con la guía institucional.
- Las ramas fuente no integradas se basan en referencias cacheadas. No se afirma que sigan activas en GitHub.

## Fuentes y tratamiento

Se consultaron registros ADR, release de base de datos, gate de migración, checklist de tareas y el código local de PC main. Los textos originales de arquitectura, operación y seguridad no se copian en este repositorio público.
