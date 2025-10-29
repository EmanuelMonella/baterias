# CASO DE USO: Registrar compra

## ACTORES 
Usuario

## PRECONDICIONES  
- Usuario logueado

## REQUERIMIENTOS  
- Registrar compra con datos de cliente, marca, modelo y cantidad

## FLUJO NORMAL  
1. Usuario ingresa al modulo VENTAS
2. Sistema muestra el campo con los datos solicitados Nombre de cliente
3. Usuario ingresa el nombre del cliente
4. Sistema muestra los clientes con ese nombre
5. Usuario selecciona el cliente
6. Sistema muestra el formulario con los campos marca, modelo y cantidad
7. Usuario completa el formulario y selecciona GUARDAR
8. Sistema valida los datos ingresados y pide confirmación
9. Usuario confirma la operación 
10. Sistema muestra mensaje "Venta registrada" y modifica el stock 

## FLUJO ALTERNATIVO  
- **1.*.** El usuario puede cancelar seleccionando DESCARTAR
- **4.1.** EL sistema no encuentra un cliente con el nombre ingresado y muestra mensaje "Cliente no registrado"
- **8.1.** El sistema encuentra errores en la validación del formulario, resalta los campos invalidos y vuelve al paso 3
- **9.1.** El usuario no confirma la operación y vuelve al paso 2

## POSTCONDICIONES
- Registro de venta en base de datos
- Actualización de inventario automática  