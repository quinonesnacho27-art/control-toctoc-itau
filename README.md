# Control de pagos TOCTOC · Itaú

Herramienta web (un solo `index.html`, sin instalación) para controlar los pagos en UF a TOCTOC por los proyectos publicados en su landing:

- Dashboard, control de proyectos (meses de pago, cobrable / eliminar del cobro / cliente)
- Alertas automáticas, liquidación mensual, cierre e historial
- Importación CSV, exportación y respaldo JSON

## Cómo funciona

Publicada con **GitHub Pages**. Los datos se guardan en la nube (JSONBin.io, comprimidos) para que todo el equipo vea lo mismo.
La primera vez cada persona ingresa su nombre, la **Master Key** y el **BIN ID** (solo una vez por dispositivo).
Cada cambio se envía automáticamente y se mezcla con lo de otras personas; sin conexión queda en el equipo y se envía al reconectar.

## Actualizar la herramienta

Editar `index.html` en este repositorio y confirmar el cambio: GitHub Pages publica la nueva versión en ~1 minuto.
Los datos del equipo **no** se pierden al actualizar la página, porque viven en JSONBin.

> No se deben publicar aquí la Master Key ni el BIN ID.
