# Control de pagos TOCTOC · Itaú

Herramienta web (un solo `index.html`, sin instalación) para controlar los pagos en UF a TOCTOC por los proyectos publicados en su landing:

- Dashboard, control de proyectos (meses de pago, cobrable / eliminar del cobro / cliente)
- Alertas automáticas, liquidación mensual, cierre e historial
- Importación CSV, exportación y respaldo JSON

## Cómo funciona

Publicada con **GitHub Pages**. Los datos se guardan en un servidor propio y gratuito (**Google Apps Script** del proyecto "Sync Hipotecario Itau", cuenta del administrador), para que todo el equipo vea la misma información.
La primera vez cada persona solo escribe **su nombre**. No hay claves ni límite de solicitudes.
Cada cambio se envía automáticamente; el servidor acepta una escritura solo si nadie guardó antes, y si alguien lo hizo se mezclan ambos cambios, así no se pierde trabajo aunque dos personas guarden a la vez. Sin conexión, el cambio queda en el equipo y se reintenta solo.
El servidor conserva además la versión anterior como respaldo.

El código del servidor está en `servidor-apps-script.gs` (referencia; el que corre está en script.google.com).

## Actualizar la herramienta

Editar `index.html` en este repositorio (o reemplazarlo) y confirmar el cambio: GitHub Pages publica la nueva versión en ~1 minuto.
Los datos del equipo **no** se pierden al actualizar la página, porque viven en el servidor.

> Historial: hasta octubre de 2026 se usó JSONBin.io; se reemplazó porque su plan gratuito trae un cupo único de 10.000 solicitudes que se agotó.
