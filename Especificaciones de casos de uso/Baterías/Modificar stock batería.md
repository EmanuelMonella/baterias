# CASO DE USO: Modificar stock batería  

## ACTORES  
Usuario

## PRECONDICIONES  
Batería en stock
Estar dentro de la pantalla de stock

## REQUERIMIENTOS  
El usuario debe registrar la modificación del stock de una batería

## FLUJO NORMAL  
1. Sistema muestra las baterías con su stock.
2. Usuario selecciona la batería y oprime el botón modificar.
3. Sistema habilita el campo stock para que el usuario pueda modificarlo.
4. Usuario modifica el campo y oprime aceptar.
5. Sistema pide confirmanción mediante un cartel.
6. Usuario confirma la modificación.
7. Sistema guarda el cambio.

## FLUJO ALTERNATIVO  
- **4.1.** Usuario oprime el botón descartar y vuelve al paso 1.
- **6.1.** Usuario no acepta la modificación oprimiendo el botón descartar y vuelve al paso 1.

## POSTCONDICIONES
- Stock de batería modificado.
