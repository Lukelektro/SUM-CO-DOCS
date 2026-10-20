# Tecnologías

## Aplicación

- **React 19** para la interfaz.
- **Tauri 2** para empaquetar la aplicación de escritorio.
- **Vite** para el entorno de desarrollo y construcción del frontend.
- **Zustand** para estado de interfaz y cliente.

## Backend y persistencia

- **Node.js** con **Fastify** para la API.
- **PostgreSQL 16** como base de datos relacional.
- Validación de configuración y contratos en los límites de la aplicación.
- Contenedores para comprobar localmente la construcción y ejecución del backend.

## Plataforma prevista

La arquitectura contempla **Google Cloud Platform** y servicios administrados para ejecutar la API, alojar PostgreSQL y gestionar identidad y secretos. La infraestructura real y la configuración de cada entorno no se detallan en este repositorio público.

## Herramientas de calidad

El trabajo incorpora pruebas automatizadas, comprobación de tipos, pruebas con PostgreSQL local desechable y validación del ciclo de vida del contenedor. Los resultados se describen en términos generales en [Avance](06-avance.md), sin publicar registros internos.
