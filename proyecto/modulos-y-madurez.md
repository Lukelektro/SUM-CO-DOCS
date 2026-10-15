# Módulos y madurez funcional

La tabla separa presencia de código de validación de un recorrido completo. “Interfaz observada” no equivale a integración funcional. Estados sujetos al corte y fuentes indicadas.

| Área | Evidencia en el código o registros | Estado | Límite de la afirmación |
|---|---|---|---|
| Cartera y ficha de proyectos | Vistas de cartera y rutas Fastify de proyectos en PC `main`. | PARCIAL | El código incluye lectura de proyectos; no se acredita aquí el ciclo completo de creación, edición y sincronización. |
| Planificación WBS, presupuesto y Gantt | Vistas y estado de planificación en el frontend. | PARCIAL | No hay validación documentada aquí del recorrido funcional completo contra una persistencia real. |
| Kanban y tareas | Componentes y vistas en el frontend. | PARCIAL | La existencia de la interfaz no demuestra integración completa, permisos ni comportamiento persistente. |
| Minutas y calidad | Vistas y componentes en el frontend. | PARCIAL | No se encontró evidencia suficiente en las fuentes consultadas para declarar el flujo completo validado. |
| Catálogo, solicitudes y órdenes de compra | Interfaces y estado de cliente en el frontend. | PROTOTIPO | No se presenta evidencia de un flujo completo de backend y persistencia de compras en `main`. |
| Documentos, Dropbox y OCR | Servicios y rutas de almacenamiento en backend, más integración de frontend en distintos estados. | PARCIAL | Los registros describen autorizaciones y flujos acotados; no certifican todas las operaciones de almacenamiento/OCR. |
| Autenticación OIDC y resolución de identidad | Código de validación OIDC y resolución de identidad externa en PC `main`. | IMPLEMENTADO | La etiqueta se limita al código del backend. La validación real documentada cubre una lectura de proyecto en STAGING. |
| Lectura de un proyecto con identidad real | Log de ejecución fechado 2026-10-03 reporta una respuesta HTTP 200 en STAGING. | IMPLEMENTADO | Solo para el recorrido y contexto descritos en ese log; resultado informado por el owner y no reproducido en esta auditoría. |
| PostgreSQL | Modelo canónico DB 2.2.0 y documentación posterior de migración/runtime 2.2.2 en STAGING. | PARCIAL | 2.2.0 es una baseline histórica; el despliegue 2.2.2 se describe en registros, sin comprobación directa actual de GCP. |
| Aplicación de escritorio Tauri | Configuración y código Tauri presentes en PC. | PARCIAL | Este compendio no encontró evidencia de empaquetado y distribución actual que permita declarar el ciclo de escritorio cerrado. |

## Capacidades solo planteadas

El documento de módulos fechado **2026-08-15** enumera alcance de producto e integraciones. Sus descripciones se consideran **PROPUESTO** salvo cuando una fila anterior cite implementación o validación concreta. El plazo y las estimaciones de ese documento no se presentan como avance real.

## Fuentes

- Código actual: `PR-SUM-CO-PC` en `main`, HEAD `62d80cc`.
- Alcance histórico: `PR-SUM-CO-DOCS/01-Documentacion/SUMATORIA/Planteamiento/DESCRIPCION_MODULOS_PROYECTO_SUMATORIA_ERP.txt`.
- Validación acotada: [Pruebas y validaciones](../pruebas-y-validacion/resultados.md).
