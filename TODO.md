# TODO: Implementar Boleta de Comprobante para Ventas

## Información Recopilada
- El registro de venta se realiza en `control/ventaController.php` en el tipo "registrar_venta".
- Después de éxito, retorna JSON con status true y mensaje 'venta registrada con exito'.
- Se necesita generar una boleta después del registro exitoso.
- Modificar `view/function/venta.js` para llamar a generar boleta después de éxito.

## Plan de Implementación
- [ ] Agregar método en `model/VentaModel.php` para obtener detalles de venta por ID.
- [ ] Agregar tipo "generar_boleta" en `control/ventaController.php` que genere la boleta HTML/PDF.
- [ ] Crear vista `view/boleta.php` para mostrar la boleta.
- [ ] Modificar `view/function/venta.js` en `realizarVenta()` para abrir la boleta después de éxito.
- [ ] Probar la generación de boleta.

## Pasos de Seguimiento
- [ ] Instalar librería para PDF si es necesario (ej. FPDF).
- [ ] Verificar que la boleta incluya: código de venta, fecha, productos, totales, cliente, vendedor.
