# CASO DE USO: Registrar venta

## ACTORES 
Usuario

## PRECONDICIONES  
1. Usuario autenticado con rol "Ventas"  
2. Stock actualizado de productos  
3. Cliente registrado en el sistema  

## REQUERIMIENTOS  
1. Validación en tiempo real de stock disponible  
2. Cálculo automático de totales (subtotal, IVA, total general)  
3. Integración con sistema tributario para tipos de facturación  

## FLUJO NORMAL  
1. Sistema muestra formulario con:  
   - Selector de cliente (búsqueda predictiva)  
   - Listado de productos con stock >0  
   - Campos: cantidad, precio unitario, descuentos  
2. Usuario completa datos y selecciona medio de pago (efectivo/tarjeta/transferencia)  
3. Sistema:  
   a) Reserva stock temporalmente  
   b) Genera pre-factura con cálculo de impuestos  
   c) Muestra resumen para confirmación  
4. Usuario confirma operación  

## FLUJO ALTERNATIVO  
2.1. Stock insuficiente → Notifica "Cantidad supera stock disponible"  
3.1. Datos fiscales incompletos → Solicita completar información requerida  
4.1. Cancelación → Libera stock reservado y cancela transacción  

## POSTCONDICIONES
- Stock actualizado en base de datos  
- Registro de venta en historial con estado "Completada" 