# CASO DE USO: Generar factura  
**ACTORES**  
Sistema automatizado/Vendedor  

**PRECONDICIONES**  
1. Venta registrada y validada  
2. Datos fiscales del cliente completos  

**REQUERIMIENTOS**  
1. Numeración correlativa según tipo de factura (A, B, C)  
2. Formato según Resolución General AFIP 5434/2024  
3. Firmado digital con certificado tributario  

**FLUJO NORMAL**  
1. Sistema genera factura electrónica con:  
   - Encabezado: fecha, número único, datos cliente  
   - Detalle: productos, cantidades, precios unitarios  
   - Totales: neto, IVA, retenciones, total final  
2. Incluye:  
   - Código QR válido para verificación  
   - CAE (Código de Autorización Electrónica)  
3. Opciones de exportación: PDF, XML (formato FE)  

**FLUJO ALTERNATIVO**  
1.1. Error en numeración → Sistema genera alerta y notifica a administrador  
2.1. Cliente ocasional → Genera ticket no fiscal con leyenda "Consumidor Final"  

**POSTCONDICIONES**  
- Factura almacenada en repositorio digital por 10 años  
- Envío automático por email al cliente  