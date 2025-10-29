# CASO DE USO: Consultar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema

## REQUERIMIENTOS
- El sistema debe facilitar la busqueda de cada cliente

## FLUJO NORMAL
1. Usuario selecciona la pantalla de CLIENTES
2. Sistema muestra una pantalla con los datos de los clientes ya precargados
3. Usuario introduce el nombre del cliente que desea buscar, luego selecciona BUSCAR
4. Sistema filtra a los clientes que tengan ese nombre y muestra los clientes que contienen ese nombre

## FLUJO ALTERNATIVO
1-* El usuario puede cancelar la operación seleccionando "Salir"
3.1. El sistema no encuentra ningun cliente con ese nombre y muestra un cartel, donde informa que no hay clientes con ese nombre

## POSTCONDICIONES
- El cliente fue consultado
