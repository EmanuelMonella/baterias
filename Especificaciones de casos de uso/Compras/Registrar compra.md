# CASO DE USO: Registrar compra
**ACTORES**  
Responsable de compras

**PRECONDICIONES**  
1. Proveedor registrado y validado en el sistema  
2. Productos existentes en catálogo  
3. Usuario con permisos de registro de compras  

**REQUERIMIENTOS**  
1. Validación automática de facturas (evitar duplicados)  
2. Cálculo de totales con impuestos aplicables  
3. Integración con módulo contable  

**FLUJO NORMAL**  
1. Sistema muestra formulario con:  
   - Selector de proveedor (autocompletado con historial reciente)  
   - Listado de productos con precios de referencia  
   - Campos: cantidad, precio unitario negociado, condiciones de pago  
2. Usuario:  
   a) Ingresa número de factura y tipo (A/B/C)  
   b) Selecciona método de pago (transferencia/cheque/efectivo)  
   c) Adjunta digitalmente la factura escaneada  
3. Sistema:  
   - Verifica unicidad de número de factura  
   - Calcula totales con IVA correspondiente  
   - Genera asiento contable automático  
   - Muestra resumen para confirmación  

**FLUJO ALTERNATIVO**  
2.1. Factura duplicada → Alerta "N° de factura ya registrado"  
3.1. Discrepancia de precios → Notifica diferencia >10% vs. histórico  
3.2. Stock máximo superado → Sugiere ajustar cantidad o almacenamiento temporal  

**POSTCONDICIONES**  
- Registro de compra en base de datos con estado "Confirmada"  
- Actualización de inventario automática  