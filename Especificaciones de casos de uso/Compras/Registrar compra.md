# CASO DE USO: Registrar compra

## ACTORES 
Usuario

## PRECONDICIONES  
1. Proveedor registrado y validado en el sistema  
2. Productos existentes en catálogo  
3. Usuario con permisos de registro de compras  

## REQUERIMIENTOS  
1. Validación automática de facturas (evitar duplicados)  
2. Integración con módulo contable  

## FLUJO NORMAL  
1. Sistema muestra formulario con los campos para que el usuario lo complete: proveedor, listado de productos, cantidad, numero de factura y forma de pago.
2. Usuario completa formulario con los datos pedidos en el formulario.
3. Sistema verifica pide confirmación.
4. Usuario confirma la venta.
5. Sistema verifica que los datos sean correctos, registra la venta y modifica el stock.

## FLUJO ALTERNATIVO  
- **3.1.** El usuario oprime descartar y vuelve al paso 2.
- **5.1.** El sistema encuentras datos incorrectos, muestra mensaje con el error y vuelve al paso 2.

## POSTCONDICIONES
- Registro de compra en base de datos con estado "Confirmada"  
- Actualización de inventario automática  
