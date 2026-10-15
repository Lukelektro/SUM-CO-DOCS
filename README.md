# SUM-CO-DOCS

## Compendio académico de Sumatoria

Este compendio reúne síntesis documentales para uso académico, seguimiento del proyecto y retroalimentación. Su fecha de corte es **2026-10-15**. No sustituye a los repositorios oficiales ni certifica por sí solo el funcionamiento del producto.

### Identidad y alcance

- **SumatoriaCO** es la empresa.
- **EFFIXI** es el equipo que desarrolla Sumatoria.
- **Sumatoria** es el sistema/proyecto.

El compendio contiene documentación y referencias; no contiene código del producto, instrucciones para agentes, datos de clientes, credenciales ni configuraciones operacionales. Las capacidades se etiquetan según su evidencia, no según la existencia de una propuesta o pantalla.

### Navegación

- [Glosario y mapa](glosario.md)
- [Visión y alcance](proyecto/vision-y-alcance.md)
- [Módulos y madurez](proyecto/modulos-y-madurez.md)
- [Arquitectura actual](arquitectura/estado-actual.md)
- [Decisiones y pendientes](arquitectura/decisiones-y-pendientes.md)
- [Hitos](planificacion-y-avances/hitos.md)
- [Estado agregado](planificacion-y-avances/estado-agregado.md)
- [Pruebas y validaciones](pruebas-y-validacion/resultados.md)

### Fuentes y fecha de corte

Se consultaron localmente `PR-SUM-CO-DOCS` (`main`, `4b4aea4290bd90aa2ff3bb4508516e7b70044064`) y `PR-SUM-CO-PC` (`main`, `62d80ccdad9ebb703c88ba7a507dd913182cb14c`). También se inspeccionaron las referencias de ramas disponibles en esos clones para distinguir cambios integrados de cambios no integrados.

El 2026-10-15, las consultas directas de ramas a GitHub fallaron porque el equipo no pudo resolver `github.com`. Por tanto, las referencias remotas locales se usan únicamente como evidencia cacheada; no confirman el estado remoto actual. Las fechas de commits se identifican como fechas de commit, no como horas o fechas de trabajo.

### Etiquetas de madurez

- **IMPLEMENTADO**: hay implementación en el código actual para el alcance indicado.
- **PARCIAL**: existe parte del flujo, pero faltan integración, cobertura o validación de extremo a extremo.
- **PROTOTIPO**: hay interfaz o prueba de concepto sin evidencia suficiente del flujo operativo completo.
- **PROPUESTO**: aparece en un diseño o plan, sin evidencia de implementación actual.
- **PENDIENTE**: el registro vigente lo deja por hacer o requiere decisión.
- **HISTÓRICO**: describe una etapa anterior; no es el estado actual.

Una etiqueta se aplica a una capacidad y alcance concretos. Un resultado documentado no equivale a una reproducción independiente. Los detalles y procedencia están en cada documento.

### Límites

El contenido evita nombres de responsables, asignaciones individuales, identificadores de infraestructura, datos personales, hallazgos de seguridad internos y documentos de terceros. La evidencia de STAGING se presenta con su alcance acotado y atribución documental. No se realizó una inspección independiente de GCP ni una nueva ejecución de pruebas.
