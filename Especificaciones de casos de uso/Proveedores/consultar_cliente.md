# CASO DE USO: Consultar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla usuarios

## REQUERIMIENTOS
- El sistema debe facilitar la busqueda de cada cliente

## FLUJO NORMAL
1- El sistema muestra una pantalla con los datos de los clientes ya precargados
2- El usuario introduce el nombre del cliente que desea buscar, luego hace click en el boton buscar
3- El sistema filtra a los clientes que tengan ese nombre y muestra una tabla con los clientes que contienen ese nombre

## FLUJO ALTERNATIVO
1-* El usuario puede cancelar la operacion haciendo click en el boton "Salir"
3.1. El sistema no encuentra ningun cliente con ese nombre y muestra un cartel, donde informa que no hay clientes con ese nombre

## POSTCONDICIONES
- El cliente fue consultado

