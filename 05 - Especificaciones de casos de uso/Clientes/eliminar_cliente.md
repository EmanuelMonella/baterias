# CASO DE USO: Eliminar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla usuarios

## REQUERIMIENTOS
- El usuario puede eliminar los datos del cliente

## FLUJO NORMAL
1. Usuario introduce el nombre del usuario y selecciona FILTRAR
2. Sistema muestra los datos de los clientes filtrados
3. Usuario selecciona el cliente que desea eliminar y luego selecciona ELIMINAR
4. Sistema pide confirmación para eliminar cliente
5. Usuario confirma la eliminación
6. Sistema elimina al cliente de la base de datos

## FLUJO ALTERNATIVO
- **1.*.** El usuario puede cancelar la operación seleccionando "Salir"
- **4.1.** El usuario no confirma la eliminación y se vuelve a la pantalla anterior

## POSTCONDICIONES
- El cliente eliminado de la base de datos

