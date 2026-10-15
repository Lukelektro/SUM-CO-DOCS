# Estado agregado y evolución por ramas

## Estado integrado en los checkouts locales

Fecha de corte: **15-10-2026**. PC y DOCS se observaron en main en sus checkouts locales. Los checkouts estaban limpios en PC. DOCS conservaba una eliminación local del informe APT anterior y material DUOC sin seguimiento; nada de ese estado se modificó.

El checklist integrado de DOCS, revisado al 03-10-2026, contiene 39 unidades: **33 PENDING, 6 IN_PROGRESS, 0 BLOCKED, 0 FAIL y 0 PASS**. Es el estado de ese listado, no un indicador global del producto.

El gate formal MIG-ARCH-001 aparece PASS/CLOSED en el reporte del 01-10. Esa afirmación pertenece a su gate y a su matriz. No contradice que el checklist posterior mantenga trabajo de producto y tareas post-migración abiertos.

## Hitos integrados

El historial local de PC main incluye como ancestros la migración de arquitectura y el runtime de identidad. DOCS main contiene el gate formal y el registro de lectura en staging. La relación de ancestro acredita integración del commit en ese checkout; no prueba cobertura funcional completa.

## Cambios que solo aparecían en referencias cacheadas

| Repositorio | Evidencia disponible | Estado respecto de main local | Límite |
|---|---|---|---|
| PC | Un commit exclusivo de validación post-migración. | No integrado en main del checkout observado. | No atribuir su prueba o cambio a main. |
| DOCS | Siete commits exclusivos en una referencia de reconciliación de tareas. El snapshot indicado allí era 25 PENDING, 12 IN_PROGRESS y 2 BLOCKED. | No integrado en main del checkout observado. | No reemplaza el snapshot integrado de 39 unidades. |
| DOCS | Un commit exclusivo de handoff OIDC y tres commits en una referencia de borrador post-migración. | No integrados según el grafo local. | Los nombres y asignaciones individuales se omiten; las referencias actuales de GitHub no se verificaron. |
| PC | Referencia histórica anterior a la migración. | Divergente y no representativa de main actual. | Se clasifica como histórica por su relación con el historial local, no por estado remoto. |

## Estado remoto

La consulta de solo lectura a GitHub falló el 15-10-2026 porque este equipo no pudo resolver github.com. No se hizo fetch a las fuentes. Las referencias remotas citadas son las que ya estaban cacheadas y no permiten confirmar ramas nuevas, eliminadas ni cambios posteriores.
