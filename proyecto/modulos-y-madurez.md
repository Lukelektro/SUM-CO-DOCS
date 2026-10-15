# Módulos y madurez funcional

La tabla distingue el código observado de un recorrido completo validado. La fecha de corte del código es el commit local de PC main indicado en [estado agregado](../planificacion-y-avances/estado-agregado.md).

| Área | Estado | Evidencia y límite |
|---|---|---|
| Cartera y ficha de proyecto | PARCIAL | El checkout contiene vistas y rutas de lectura de proyectos. No se acredita aquí el ciclo completo de creación, edición y sincronización. |
| Planificación, WBS y Gantt | PARCIAL | Hay interfaces y estructuras de planificación. No hay evidencia suficiente de un recorrido integral persistido y aprobado. |
| Tareas y Kanban | PARCIAL | Se observan vistas y componentes de tareas. La interfaz no demuestra por sí sola sincronización, permisos ni operación completa. |
| Minutas y calidad | PARCIAL | Hay componentes y entidades documentadas; no se acredita el flujo completo de captura, seguimiento y cierre. |
| Catálogo y abastecimiento | PROTOTIPO | La UI y el modelo de datos describen capacidades. No se presenta un recorrido de compra integral validado en el runtime actual. |
| Documentos y almacenamiento externo | PARCIAL | Existen componentes backend y documentación de autorización. No se certifican todas las operaciones externas. |
| OCR | PROTOTIPO | El material consultado describe un laboratorio de procesamiento; no se acredita como flujo productivo integrado. |
| API de proyectos, usuario, auditoría y almacenamiento | IMPLEMENTADO | Hay rutas Fastify y componentes de runtime en el código de PC main. Esta etiqueta se limita al código y no implica cobertura completa. |
| Autenticación OIDC y resolución de identidad | IMPLEMENTADO | El código actual contiene validación de token y resolución de identidad externa. La evidencia E2E documentada es una lectura específica. |
| Lectura real de proyecto en staging | IMPLEMENTADO, alcance acotado | Un log fechado 03-10-2026 reporta HTTP 200 en un escenario. El resultado fue informado por el owner y no se reejecutó para este compendio. |
| Modelo PostgreSQL | IMPLEMENTADO como artefacto; runtime PARCIAL | La baseline DB 2.2.0 tiene documentación de release y validaciones locales. Hay migraciones y registros posteriores de staging; no se inspeccionó el entorno actual. |
| Aplicación de escritorio Tauri | PARCIAL | El código incluye Tauri. No se obtuvo evidencia contemporánea suficiente de empaquetado, firma y distribución. |
| Infraestructura de producción | PENDIENTE / no verificada | No se inspeccionó GCP. El informe se limita a despliegues de STAGING descritos en registros. |

## Alcance propuesto

Las listas de módulos de planificación son **PROPUESTO** salvo las filas con evidencia explícita de código o prueba. No se usa el total de módulos para calcular avance porcentual. La descripción amplia de funcionalidades y las cifras comerciales de documentos antiguos no se presentan como resultados.

## Fuentes

Código local de PR-SUM-CO-PC main; registros de validación y ejecución de PR-SUM-CO-DOCS fechados entre 26-09 y 03-10-2026; documentación de planificación de módulos. Véase [pruebas y validaciones](../pruebas-y-validacion/resultados.md).
