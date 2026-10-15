# Estado agregado y evolución por ramas

## Snapshot integrado en `main`

Fecha de corte de este compendio: **2026-10-15**. El snapshot de tareas disponible en `PR-SUM-CO-DOCS/main` fue revisado por última vez el **2026-10-03** y registra 39 unidades: **33 PENDING, 6 IN_PROGRESS, 0 BLOCKED, 0 FAIL y 0 PASS**. Es un conteo de ese backlog; no una medida global de avance del sistema.

Los clones locales observados estaban en:

- `PR-SUM-CO-PC/main`, HEAD `62d80ccdad9ebb703c88ba7a507dd913182cb14c`.
- `PR-SUM-CO-DOCS/main`, HEAD `4b4aea4290bd90aa2ff3bb4508516e7b70044064`.

Las fechas anteriores describen los clones locales en el corte. No se confirmó si `main` remoto cambió después.

## Hitos integrados en `main`

- El historial local de PC contiene el tip de `migration/architecture-v1` (`cc38c56`) y de `feat/backend-runtime-identity` (`2418eba`) como ancestros de `main`.
- DOCS `main` contiene el cierre documental de la lectura de proyecto en STAGING.
- Las ramas locales de documentación de handoff/runtime observadas tienen sus tips contenidos en `main` local.

La relación de ancestro demuestra integración de esos commits en el historial local observado; no prueba que cada capacidad funcione de forma completa.

## Cambios que solo aparecían en referencias no integradas

Estas referencias existían en los clones al corte anterior; sus nombres `origin/*` corresponden a referencias remotas cacheadas, no a una consulta actual de GitHub.

| Repositorio | Referencia cacheada | Diferencia local respecto de `main` | Interpretación |
|---|---|---|---|
| PC | Rama cacheada de validación backend | Un commit exclusivo (`3405a82`), con cambios en validación de entradas de rutas y una prueba. | Cambio no integrado en `main` local; no asumir finalización. |
| DOCS | Rama cacheada de reconciliación de tareas | Siete commits exclusivos; agrega logs/evidencia y cambia el checklist. Su snapshot indica 25 PENDING, 12 IN_PROGRESS, 2 BLOCKED, 0 PASS. | Reconciliación no integrada en `main` local. No sustituir el snapshot de `main`. |
| DOCS | Rama cacheada de handoff OIDC | Un commit exclusivo que agrega un log de adaptación OIDC. | Log no integrado según el grafo local; no usar como estado oficial de `main`. |
| DOCS | `origin/archive/post-migration-validation-draft` | Tres commits exclusivos con planificación y asignaciones preliminares. | Referencia etiquetada como archivo, no integrada; evidencia de borrador, no de trabajo terminado. |
| PC | `origin/archive/pre-migration-main` | Rama histórica divergente con commits previos a la migración. | Referencia histórica; no describe el producto actual en `main`. |

Otras referencias de migración y handoff observadas tenían sus tips contenidos en `main` local. La etiqueta `archive/` describe el nombre de la referencia local, no confirma su estado actual en GitHub.

## Estado remoto no verificable

El 2026-10-15, `git ls-remote --heads origin` falló para `PR-SUM-CO-PC`, `PR-SUM-CO-DOCS` y el repositorio destino porque no se pudo resolver `github.com`. No se hizo `fetch`, no se actualizaron referencias y no se clonó ningún repositorio. Por tanto, no se puede asegurar si desde la última actualización local surgieron ramas, se eliminaron ramas o cambiaron los commits remotos.
