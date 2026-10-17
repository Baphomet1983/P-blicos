# Publicación gratuita de Suscripto en Cloudflare Pages

Cloudflare Pages permite publicar un sitio HTML estático desde GitHub. El repositorio ya contiene todos los archivos y no necesita un build de React/Node.

## Conectar desde el teléfono
1. Abre el panel oficial: https://dash.cloudflare.com/
2. Entra en **Workers & Pages**.
3. Pulsa **Create application** y elige **Pages** → **Connect to Git**.
4. Autoriza Cloudflare Pages para acceder a tu cuenta de GitHub.
5. Selecciona el repositorio **Baphomet1983/P-blicos**.
6. Configura:
   - **Project name:** suscripto-chile (o uno disponible)
   - **Production branch:** main
   - **Framework preset:** None
   - **Build command:** dejar en blanco (sin build)
   - **Build output directory:** /
7. Pulsa **Save and Deploy**.
8. Abre el dominio `*.pages.dev` que muestre el panel.

Cloudflare documenta este flujo en https://developers.cloudflare.com/pages/get-started/git-integration/ y el despliegue de HTML estático en https://developers.cloudflare.com/pages/framework-guides/deploy-anything/.

## Rutas del sitio
- `/` o `/index.html`: aplicación
- `/ventas.html`: oferta de lanzamiento
- `/privacidad.html`: transparencia de privacidad
- `/app.webmanifest`: ajustes de instalación
- `/sw.js`: caché de recursos para uso sin conexión

## Prueba posterior al despliegue
1. Abre `/ventas.html` y después la demo.
2. Añade un servicio, actualízalo, paúsalo y elimínalo.
3. Pulsa **Descargar respaldo**.
4. Borra un registro e importa el respaldo para verificar la recuperación.
5. En Android/Chrome abre el menú y selecciona **Instalar aplicación** o **Añadir a pantalla de inicio** si el navegador lo ofrece.
6. Comprueba el sitio en una segunda pestaña y luego sin conexión.

## Alcance real
Los datos permanecen en el almacenamiento local del navegador. No existe usuario/contraseña, backend, sincronización, recordatorio push ni cobro automático. No guardar datos de tarjeta ni contraseñas.

## Costos y ventas
No hay costo de hosting con los límites del plan gratuito de Cloudflare Pages; hay que revisar los términos y límites vigentes. Un enlace de pago de un proveedor como Mercado Pago puede ser gratuito de crear y aun así descontar comisión por transacción. Los cobros recurrentes reales requieren el producto de suscripciones del proveedor y configuración desde la cuenta del vendedor. Este repositorio no contiene credenciales de pago.
