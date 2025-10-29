# CASO DE USO: Registrar compra

## ACTORES 
Usuario

## PRECONDICIONES  
Usuario logueado 

## REQUERIMIENTOS  
- Registrar comprar con datos de proveedor, marca, modelo y cantidad

## FLUJO NORMAL  
1. Usuario ingresa al modulo COMPRAS
2. Sistema muestra el campo con los datos solicitados Nombre de proveedor
3. Usuario ingresa el nombre del proveedor
4. Sistema muestra los proveedores con ese nombre
5. Usuario selecciona el proveedor
6. Sistema muestra el formulario con los campos marca, modelo y cantidad
7. Usuario completa el formulario y selecciona GUARDAR
8. Sistema valida los datos ingresados y pide confirmación
9. Usuario confirma la operación 
10. Sistema muestra mensaje "Compra registrada" y modifica el stock 

## FLUJO ALTERNATIVO  
- **1.*.** El usuario puede cancelar seleccionando DESCARTAR
- **4.1.** EL sistema no encuentra un proveedor con el nombre ingresado y muestra mensaje "Proveedor no registrado"
- **8.1.** El sistema encuentra errores en la validación del formulario, resalta los campos invalidos y vuelve al paso 3
- **9.1.** El usuario no confirma la operación y vuelve al paso 2

## POSTCONDICIONES
- Registro de compra en base de datos con estado "Confirmada"  
- Actualización de inventario automática  