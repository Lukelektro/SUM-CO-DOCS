# Estado agregado y evolución por ramas

## Estado integrado en main

Fecha de corte: **15-10-2026**. Ese día se consultaron las referencias actuales de GitHub y se hizo fast-forward de `main` en ambos repositorios fuente. PC quedó en `ceb973ba3c23aab3865b6bbc1073e403bc93cd61`; DOCS quedó en `cd46933f17e2071b4132894ee91903a782103279`. Ambos cambios están integrados en los checkouts locales y fueron observados en `origin/main` después de la consulta remota.

PC incorporó 13 commits desde el corte local anterior. El conjunto integra el flujo de autenticación Google para escritorio con PKCE e Identity Platform, ampliaciones de pruebas frontend y backend y la implementación de creación de proyectos sobre Database 2.2.3. La presencia en `main` prueba integración del código, no despliegue ni disponibilidad para usuarios.

DOCS incorporó 28 commits desde el corte local anterior. La estructura de seguimiento ahora incluye un backlog global con frentes y criterios de aceptación, vínculos entre registros de tareas y ese backlog, y logs de ejecución fechados. También incorpora la documentación del candidato Database 2.2.3 y de la sincronización del estado. Se omiten asignaciones personales, prompts, reglas de agentes y documentación operativa interna de este compendio público.

## Estado de trabajo y límites

El registro de sincronización del 15-10 describe 21 frentes globales y 39 fichas relacionadas, con criterios de aceptación y enlaces de trazabilidad. Es un esquema de seguimiento, no una medición porcentual del producto. Las fichas conservan estados y evidencias anteriores; su reorganización no equivale a cerrar tareas.

Database 2.2.3 figura como **CANDIDATE**: la documentación reporta validación local de la migración y de las rutas de creación, pero no despliegue en STAGING, Cloud SQL o producción ni asignación productiva del nuevo permiso de creación. El resultado anterior de lectura HTTP 200 en STAGING corresponde a Database 2.2.2 y a una lectura acotada; no se extiende a la nueva operación de escritura.

PC estaba limpio en `main` tras el fast-forward. DOCS conserva cambios locales previos del usuario en material DUOC (una eliminación y archivos/carpetas sin seguimiento); se dejaron intactos. El repositorio de este compendio sigue en `docs/academic-compendium-v2`, con el `.DS_Store` local sin seguimiento preservado.

## Ramas y relación con main

La actualización remota de esta auditoría consultó únicamente `main`; no obtuvo un listado completo actual de ramas. Los logs de DOCS documentan la integración en `main` de la autenticación de escritorio y del candidato Database 2.2.3, y mencionan ramas de trabajo preservadas bajo referencias de archivo. No se afirma que esas referencias sigan publicadas o activas. La evidencia de progreso incorporada aquí corresponde a commits integrados en `main`, no a nombres de ramas.

## Procedencia

Snapshot reproducible mediante los SHAs indicados, los commits integrados en PC y los registros fechados de DOCS del 15-10-2026. No se inspeccionó GCP ni se ejecutaron pruebas durante esta actualización del compendio. Para detalles de alcance de cada resultado, véanse [pruebas y validaciones](../pruebas-y-validacion/resultados.md) y [procedencia](../anexos/procedencia-y-alcance.md).
