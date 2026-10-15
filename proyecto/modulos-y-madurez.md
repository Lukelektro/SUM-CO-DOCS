# Módulos y madurez funcional

La tabla distingue el código observado de un recorrido completo validado. La fecha de corte es el `main` remoto y local observado después del fast-forward del 15-10-2026, indicado en [estado agregado](../planificacion-y-avances/estado-agregado.md).

| Área | Estado | Evidencia y límite |
|---|---|---|
| Cartera y ficha de proyecto | PARCIAL | El checkout contiene vistas, rutas de lectura y una ruta de creación delegada integrada en `main`. La creación fue validada localmente según los registros; no se acredita despliegue ni el ciclo completo de edición y sincronización. |
| Planificación, WBS y Gantt | PARCIAL | Hay interfaces y estructuras de planificación. No hay evidencia suficiente de un recorrido integral persistido y aprobado. |
| Tareas y Kanban | PARCIAL | Se observan vistas y componentes de tareas. La interfaz no demuestra por sí sola sincronización, permisos ni operación completa. |
| Minutas y calidad | PARCIAL | Hay componentes y entidades documentadas; no se acredita el flujo completo de captura, seguimiento y cierre. |
| Catálogo y abastecimiento | PROTOTIPO | La UI y el modelo de datos describen capacidades. No se presenta un recorrido de compra integral validado en el runtime actual. |
| Documentos y almacenamiento externo | PARCIAL | Existen componentes backend y documentación de autorización. No se certifican todas las operaciones externas. |
| OCR | PROTOTIPO | El material consultado describe un laboratorio de procesamiento; no se acredita como flujo productivo integrado. |
| API de proyectos, usuario, auditoría y almacenamiento | PARCIAL | Hay rutas Fastify integradas; en proyectos, lectura y alta delegada tienen código y pruebas de alcance acotado. No se afirma que todos los dominios tengan cobertura completa. |
| Autenticación OIDC y resolución de identidad | IMPLEMENTADO | La validación de token y resolución de identidad externa permanecen integradas. Los registros distinguen el flujo de escritorio de una lectura específica en STAGING. |
| Inicio de sesión Google en escritorio | IMPLEMENTADO en código | El runtime Tauri contiene OAuth con PKCE, intercambio con Identity Platform y sesión en memoria nativa. La validación está documentada; no hay evidencia aquí de empaquetado o distribución. |
| Creación de proyectos sobre Database 2.2.3 | PARCIAL | La ruta y el contrato de persistencia están integrados en `main`. Los registros informan validación local del candidato y de la API; no hay despliegue ni asignación productiva documentados. |
| Lectura real de proyecto en staging | IMPLEMENTADO, alcance acotado | Un log fechado 03-10-2026 reporta HTTP 200 en un escenario. El resultado fue informado por el owner y no se reejecutó para este compendio. |
| Modelo PostgreSQL | IMPLEMENTADO como artefacto; runtime PARCIAL | La baseline DB 2.2.0 tiene documentación de release, DB 2.2.2 se reporta en STAGING y DB 2.2.3 figura como candidata validada localmente. No se inspeccionó GCP. |
| Aplicación de escritorio Tauri | PARCIAL | El código incluye Tauri. No se obtuvo evidencia contemporánea suficiente de empaquetado, firma y distribución. |
| Infraestructura de producción | PENDIENTE / no verificada | No se inspeccionó GCP. El informe se limita a despliegues de STAGING descritos en registros. |

## Alcance propuesto

Las listas de módulos de planificación son **PROPUESTO** salvo las filas con evidencia explícita de código o prueba. No se usa el total de módulos para calcular avance porcentual. La descripción amplia de funcionalidades y las cifras comerciales de documentos antiguos no se presentan como resultados.

## Fuentes

Código de PR-SUM-CO-PC `main` en `ceb973b`; registros de validación y ejecución de PR-SUM-CO-DOCS `main` en `cd46933`, fechados entre 26-09 y 15-10-2026; documentación de planificación de módulos. Véase [pruebas y validaciones](../pruebas-y-validacion/resultados.md).
