# CASO DE USO: Eliminar proveedor

## ACTORES  
Usuario 

## PRECONDICIONES 
1. Proveedor sin compras registradas en últimos 6 meses  
2. Proveedor seleccionado en listado

## REQUERIMIENTOS  
1. Validar historial de compras asociado  
2. Registro de auditoría con usuario y fecha de eliminación

## FLUJO NORMAL  
1. Usuario selecciona "Eliminar" en registro  
2. Sistema muestra confirmación con datos del proveedor  
3. Usuario confirma eliminación  
4. Sistema desactiva proveedor (borrado lógico)

## FLUJO ALTERNATIVO  
2.1. Usuario cancela → Vuelve al listado  
3.1. Proveedor con compras activas → Muestra "No se puede eliminar por historial existente"

## POSTCONDICIONES  
Proveedor marcado como inactivo en el sistema