# CASO DE USO: Consultar proveedor

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema

## REQUERIMIENTOS
- El sistema debe facilitar la busqueda de cada proveedor

## FLUJO NORMAL
1. Usuario selecciona la pantalla de PROVEEDORES
2. Sistema muestra una pantalla con los datos de los proveedores ya precargados
3. Usuario introduce el nombre del proveedor que desea buscar, luego selecciona BUSCAR
4. Sistema filtra a los proveedores que tengan ese nombre y muestra los proveedores que contienen ese nombre

## FLUJO ALTERNATIVO
- **1.*.**  El usuario puede cancelar la operación seleccionando "Salir"
- **3.1.** El sistema no encuentra ningun cliente con ese nombre y muestra un cartel, donde informa que no hay clientes con ese nombre

## POSTCONDICIONES
- El proveedor fue consultado
