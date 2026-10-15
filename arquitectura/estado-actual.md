# Arquitectura actual observada

## Componentes

| Capa | Estado observado en el corte | Alcance y cautela |
|---|---|---|
| Interfaz web | React con módulos de cartera, proyectos, planificación, tareas, compras, catálogo y otras vistas. | PARCIAL: hay interfaces y estado frontend; los recorridos no están todos conectados y validados contra backend. |
| Escritorio | El repositorio incluye una aplicación Tauri. | PARCIAL: la presencia del proyecto no demuestra empaquetado, firma o distribución vigente. |
| Backend | Node.js/Fastify con composición de rutas para proyectos, usuario, auditoría y almacenamiento. | IMPLEMENTADO en código para esas superficies; no implica cobertura funcional completa del sistema. |
| Autenticación | Proveedor OIDC y resolución de identidad externa conectados al contexto de autorización del backend. | IMPLEMENTADO en código; la validación real documentada tiene alcance limitado a una lectura en STAGING. |
| Persistencia | PostgreSQL, repositorios y transacciones aparecen en el backend; DOCS mantiene SQL canónico y migraciones. | PARCIAL a nivel de producto integrado. La evidencia de STAGING se limita a registros concretos. |
| Integraciones | Hay componentes de Dropbox y OCR en backend; la interfaz también contiene integraciones parciales. | PARCIAL. No se afirma que todos los flujos externos estén validados. |
| Infraestructura cloud | Los documentos registran despliegues de validación en STAGING. | DOCUMENTADO, no inspeccionado directamente en GCP en este corte. No se incluyen nombres ni configuración. |

## Camino de lectura respaldado

El código y los registros documentan una ruta que valida un token OIDC, resuelve una identidad externa a usuario interno, aplica autorización y contexto de actor y consulta un proyecto mediante PostgreSQL. Un log de 2026-10-03 reporta HTTP 200 para una lectura en STAGING. Esa evidencia no certifica otras rutas, operaciones de escritura, todos los roles, producción ni el producto completo. Véase [resultados](../pruebas-y-validacion/resultados.md).

## Evolución y fuentes

En `main` de PC, el historial registra el retiro del runtime Express legado y cambios de migración hacia Fastify durante octubre de 2026. El commit `cc38c56` está fechado 2026-10-02; commits posteriores del 2026-10-03 registran identidad OIDC y rutas de salud.

Fuentes de contraste: código de `PR-SUM-CO-PC` en `main`, en particular rutas bajo `backend/src/app/routes/`, seguridad bajo `backend/src/app/security/` e infraestructura de base de datos; documentación `PR-SUM-CO-DOCS/10-Migracion-Arquitectura/02-Arquitectura-Objetivo/TARGET-ARCHITECTURE.md` y logs fechados de ejecución. La arquitectura objetivo no se usa como evidencia de implementación.
