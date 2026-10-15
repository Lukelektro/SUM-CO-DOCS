# Decisiones y pendientes

Esta síntesis conserva el estado que indican las fuentes. Un diseño, un ADR o código presente no convierten por sí solos una decisión en aprobada ni cierran la funcionalidad.

## Decisiones y baselines documentadas

| Tema | Estado documentado | Síntesis pública |
|---|---|---|
| Stack de cliente | Baseline observada en código | React/Vite para la interfaz y Tauri para escritorio. La presencia del stack no acredita empaquetado vigente. |
| Backend | Implementación integrada en el checkout local de main | La migración hacia Node.js/Fastify reemplazó el runtime Express legado para el alcance integrado. No implica que todas las features estén migradas. |
| Modelo relacional | V2.2.0 FINAL para bootstrap nuevo según release del 26-09-2026 | Los cambios posteriores se registran mediante migraciones forward. No se publica SQL ni detalles de permisos. |
| Creación de proyectos | Database 2.2.3 CANDIDATE; main integra la ruta de creación delegada y el contrato de datos. | La validación se documenta para laboratorio local; no consta despliegue ni autorización productiva para la nueva capacidad. La capacidad de crear se mantiene separada de la lectura global. |
| Freeze de migración | Aprobado en registro de octubre | Fijó un baseline y criterios de preservación para MIG-ARCH-001. El gate formal se reportó cerrado el 01-10. |
| Resolución de identidad externa | ADR relacionado aparece como ACTIVE | El código integrado y la lectura E2E documentada aportan evidencia, pero el estado del ADR no se presenta como cerrado si la fuente no lo marca así. |
| Inicio de sesión de escritorio | Integrado en PC `main` el 04-10 según el historial y el log de ejecución | El flujo nativo usa Google OAuth con PKCE e Identity Platform. Código integrado y validación documentada no equivalen a distribución de una aplicación firmada. |

## Pendientes y límites

- El snapshot integrado de tareas del 03-10 conserva 33 pendientes y 6 en curso de 39 unidades. La nueva estructura de backlog enlaza 39 fichas con 21 frentes globales, pero no reemplaza los estados por sí sola ni cierra el trabajo.
- Falta evidencia de ciclos Scrum completos, retrospectivas y Definition of Done aplicado por incremento.
- No se encontraron mediciones de rendimiento, impacto, satisfacción ni objetivos de negocio cuantificados.
- No se verificó el estado actual de GCP, producción, backups ni recuperación.
- La documentación no aporta la malla académica oficial para asignar competencias curriculares; debe cotejarse con la guía institucional.
- La consulta remota del 15-10 confirmó `main` en ambos repositorios fuente; no se consultó el listado completo de otras ramas. La relación de ramas archivadas se atribuye solo a los logs documentales.

## Fuentes y tratamiento

Se consultaron registros ADR, release y checkpoint de base de datos, gate de migración, backlog global, logs de ejecución y código de PC `main` después del fast-forward del 15-10-2026. Los textos originales de arquitectura, operación, gestión interna y seguridad no se copian en este repositorio público.
