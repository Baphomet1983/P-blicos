# Suscripto Chile 🇨🇱

Aplicación web móvil para registrar suscripciones, estimar gasto mensual y revisar renovaciones próximas y pruebas gratuitas.

## Demo / archivos
- App: `index.html`
- Página de oferta: `ventas.html`
- Privacidad preliminar: `privacidad.html`
- Manifest Android/PWA: `app.webmanifest`
- Caché estática básica: `sw.js`
- Oferta y plan de validación: `PLAN_VENTAS_7_DIAS.md`
- Guía de publicación sin pago: `PUBLICAR_CLOUDFLARE_PAGES.md`

## Funciones
- Añadir, editar, pausar y eliminar suscripciones.
- Resumen de gasto mensual activo y renovaciones de los siguientes 7 días.
- Etiquetas para pruebas gratis.
- Datos locales en el navegador.
- Exportación/importación JSON para respaldo.
- Manifest de instalación y service worker para recursos estáticos básicos.

## Publicar gratis
Sigue los pasos de [PUBLICAR_CLOUDFLARE_PAGES.md](./PUBLICAR_CLOUDFLARE_PAGES.md). La conexión inicial con GitHub requiere autorización desde tu cuenta de Cloudflare; una vez conectada, cada cambio en `main` se puede publicar automáticamente.

## Alcance y límites
Esta es una versión inicial para validar la necesidad del producto. No tiene autenticación, base de datos compartida, sincronización entre dispositivos, recordatorios push, facturación ni pagos/cobros recurrentes. No se deben guardar datos de tarjetas en la página.

El precio fundador de configuración guiada que aparece en `ventas.html` es una oferta de prueba; el alcance y la fecha de entrega deben acordarse antes de cobrar. El producto no debe describirse como un SaaS con cobro automático ya operativo.
