# Visión y alcance

## Identidad

- **Empresa:** SumatoriaCO.
- **Equipo de desarrollo:** EFFIXI.
- **Sistema/proyecto:** Sumatoria.

## Problema y objetivo

La documentación de planificación describe la necesidad de reunir información de proyectos de arquitectura y construcción que hoy puede estar repartida entre cartera, planificación, abastecimiento, documentos y seguimiento en terreno. El objetivo planteado para Sumatoria es apoyar la gestión operacional de proyectos y dar continuidad a la información desde su planificación hasta el seguimiento de actividades y compras.

Esta descripción resume el propósito documental. No afirma que todas las operaciones enumeradas estén automatizadas o integradas en la versión actual.

## Usuarios previstos

Las fuentes describen perfiles que participan en gestión de proyectos, trabajo en terreno, inspección técnica y compras/control de gestión. Se presentan como **usuarios previstos** del sistema; no se infiere que cada perfil, permiso o recorrido esté habilitado en producción.

## Alcance propuesto y estado observado

Los documentos de planteamiento proponen capacidades para cartera y fichas de proyecto, planificación, seguimiento visual, minutas, documentación, compras, materiales, proveedores, calidad y reportes. También describen integraciones externas. Ese alcance es **PROPUESTO** hasta que el código actual o una validación acotada respalden una capacidad específica.

En el código de `PR-SUM-CO-PC` hay interfaces React/Tauri y un backend Fastify con rutas para proyectos, usuario, auditoría y almacenamiento. La integración entre pantallas y backend varía por flujo. La documentación registra una lectura acotada de proyecto desde STAGING; no es evidencia de operación integral de todos los módulos. Véase [módulos y madurez](modulos-y-madurez.md) y [resultados](../pruebas-y-validacion/resultados.md).

## Procedencia y límites

Síntesis basada en `PR-SUM-CO-DOCS/00-Informacion-general/README-proyecto.md`, `PR-SUM-CO-DOCS/01-Documentacion/SUMATORIA/Planteamiento/DESCRIPCION_MODULOS_PROYECTO_SUMATORIA_ERP.txt` y el código de `PR-SUM-CO-PC` en `main` al corte. La descripción de módulos proviene de una propuesta emitida el **2026-08-15**; no se trasladan sus cifras comerciales, presupuesto, horas ni plazo.
