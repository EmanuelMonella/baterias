# CASO DE USO: Dar baja batería 

## ACTORES  
Usuario  

## PRECONDICIONES  
1. Batería en estado "Activa"  
2. Sin transacciones pendientes  

## REQUERIMIENTOS
El usuario registra la baja de stock.

## FLUJO NORMAL
1. Usuario selecciona batería y elige motivo de baja:  
   - Defecto de fabricación  
   - Fin de vida útil  
   - Retiro del mercado  
2. Sistema pide confirmacion.
3. Usuario confirma la operacion.
4. Sistema modifica stock y muestra mensaje de confirmacion.

## FLUJO ALTERNATIVO  
*.1 Usuario puede descartar la operacion.
3.1 Usuario no confirma la operacion y vuelve al paso 1.

## POSTCONDICIONES  
- Stock modificado