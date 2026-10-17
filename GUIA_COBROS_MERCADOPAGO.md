# Cobros y prueba gratuita de 7 días

## Lo primero: vender un servicio entregable
La oferta que aparece en `ventas.html` es una configuración guiada de pago único por $19.990 CLP (precio de validación). No es una suscripción de software. Antes de cobrar, acuerda alcance, plazo, política de devolución y qué se entregará. El servicio solo se puede cobrar cuando puedas cumplirlo.

## Crear un link de pago para el servicio de configuración
1. Entra a tu cuenta de Mercado Pago Chile.
2. Abre la opción Link de pago / Cobrar.
3. Crea un link por el monto acordado, con un título que describa el servicio de configuración.
4. Revisa las comisiones vigentes y los requisitos comerciales/tributarios de tu cuenta.
5. Comparte el link de pago solo con personas que hayan aceptado la propuesta.

La creación de links de pago está documentada por Mercado Pago y no exige una integración de código; las comisiones se aplican según la modalidad y la operación. Revisa los términos y tasas vigentes antes de cobrar.

## Cómo configurar una prueba gratuita de 7 días con cobro recurrente
Mercado Pago Chile dispone de **Planes de suscripción**. Su panel permite crear un plan, escoger periodicidad y precio, ofrecer una prueba gratuita de 7 días, y compartir un enlace de adhesión. Pasos de alto nivel:

1. Abre Mercado Pago → **Planes de suscripción**.
2. Selecciona **Crear nuevo plan**.
3. Define el nombre visible para el cliente, la descripción, el monto y la frecuencia (por ejemplo, mensual).
4. En **Prueba gratis**, elige 7 días.
5. Define si el plan es ilimitado o termina tras un número de cobros y revisa la fecha de facturación/prorrateo.
6. Lee la pantalla de resumen: confirma el precio, la frecuencia, el inicio del primer cobro y que el texto deje claro que el cobro será automático después de la prueba.
7. Publica el plan y copia el enlace que entrega Mercado Pago.

Documentación oficial: https://www.mercadopago.cl/developers/es/docs/subscription-plans/create-subscription-plan

## Restricción clave antes de vender Suscripto como SaaS
No uses el plan de suscripción para cobrar por la aplicación como producto recurrente hasta que el servicio realmente esté a la altura: esta versión no tiene cuentas, recuperación/sincronización de datos, servidor de clientes, control de acceso ni un proceso de cancelación dentro de la app. Crear el plan en Mercado Pago no añade esas funciones automáticamente.

Para vender una app de pago recurrente correctamente, después hay que conectar el estado de la suscripción a un backend seguro, escuchar las notificaciones de pago del proveedor, mantener el acceso actualizado y ofrecer instrucciones claras de cancelación. El prototipo actual es solo local.

## Formalidad tributaria en Chile
El SII indica que el inicio de actividades puede ser exigible al desarrollar actividades económicas que generan rentas, y que desde enero de 2026 hay obligaciones de verificación por parte de medios de pago en los casos descritos por la ley. Confirma tu situación con el SII antes de recibir pagos comerciales:
https://www.sii.cl/destacados/ley_cumplimiento_obligaciones_tributarias/inicio_actividades.html

**No almacenar ni enviar tarjetas o credenciales privadas en GitHub.** Si una integración API se construye más adelante, el Access Token debe estar en un secreto del servidor, nunca en HTML ni JavaScript público.
