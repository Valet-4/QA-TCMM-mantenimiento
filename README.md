# QA-TCMM · Plataforma web para la gestión y documentación de casos de prueba

Prototipo funcional (alta fidelidad, corte vertical, evolutivo) del proyecto QA-TCMM.
Corporación Universitaria Iberoamericana · Ingeniería de Software.
Desarrollado en Gestión de Proyectos de Software y mantenido en Mantenimiento de Software (Actividad 4).
Autora: Lizeth Valentina Cuta Hernández (código 100225551).

## Qué hace

- Inicio de sesión con roles (Analista QA y Desarrollador).
- Proyectos y usuarios.
- Casos de prueba con pasos, requisito asociado, versionamiento, historial, búsqueda, filtros y duplicado.
- Ejecución paso a paso con resultado obtenido, evidencia en imagen y observaciones.
- Defectos creados automáticamente cuando una ejecución falla, con detección de reincidencia.
- Notificaciones al desarrollador y al analista QA.
- Panel de calidad, matriz de trazabilidad requisito → casos → defectos.
- Reportes: descarga de CSV e impresión a PDF.
- Modo oscuro automático según el sistema.

## Cuentas de ejemplo

| Rol | Correo | Clave |
|---|---|---|
| Analista QA | lizeth@qatcmm.co | qa2026 |
| Desarrollador | juan@qatcmm.co | dev2026 |

## Cómo ejecutarlo

No requiere instalación ni servidor.

1. Abre la versión publicada: https://valet-4.github.io/QA-TCMM/ , o
2. Descarga `index.html` y ábrelo con doble clic en Chrome, Edge o Firefox.

Los datos se guardan en el navegador (almacenamiento local). El botón "Restablecer datos" devuelve el estado inicial.

## Alcance de esta versión

Es un prototipo evolutivo: la interfaz y la lógica de estados se reutilizarán en la versión definitiva. Aún no tiene servidor ni base de datos compartida, la autenticación es de demostración y los datos son locales a cada navegador. La siguiente iteración incorpora la API REST y la base de datos relacional definidas en la EDT.

## Capturas

Están en la carpeta `docs/capturas/`.
