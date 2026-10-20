# Seguridad y calidad

## Principios

La aplicación separa la identidad del usuario de los permisos para realizar operaciones. La autenticación utiliza estándares OIDC; el backend determina la autorización y aplica controles de acceso en las operaciones protegidas.

El estado local de la interfaz no se trata como autoridad para conceder permisos. Las credenciales y la configuración sensible pertenecen a los entornos de ejecución protegidos y no a la documentación pública.

## Validación

Antes de integrar cambios se utilizan prácticas como:

- pruebas automatizadas de frontend y backend;
- comprobación de tipos y formato;
- pruebas de autorización y transacciones;
- pruebas de integración con PostgreSQL 16 local y desechable;
- pruebas de construcción, disponibilidad y cierre del contenedor;
- revisión del cambio antes de integrarlo.

Estas verificaciones respaldan el desarrollo local. No sustituyen las pruebas controladas de STAGING ni certifican la operación productiva.

## Protección de información

Este repositorio evita publicar credenciales, identificadores internos, direcciones privadas, datos reales de usuarios o clientes, configuración de infraestructura y registros operativos. Los ejemplos y diagramas se mantienen conceptuales.
