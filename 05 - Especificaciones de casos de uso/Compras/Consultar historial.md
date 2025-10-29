# CASO DE USO: Consultar histórico compra

## ACTORES  
Usuario

## PRECONDICIONES
1. Usuario logueado 

## REQUERIMIENTOS  
1. Usuario puede consultar historial completo de adquisiciones

## FLUJO NORMAL 
1. Usuario ingresa al apartado REPORTES
2. Sistema muestra pantalla con casilleros para ingresar MARCA y seleccionar si es VENTA o COMPRA
3. Usuario ingresa MARCA y selecciona la operación (VENTA O COMPRA)
4. Sistema muestra los datos de la MARCA seleccionada con su OPERACIÓN

## FLUJO ALTERNATIVO 
- **1.*.** El usuario puede cancelar seleccionando SALIR
- **4.1.** El sistema no encuentra la MARCA con esa operación y muestra un mensaje "NO HAY REGISTROS"

## POSTCONDICIONES  
- Historial de baterias en pantalla