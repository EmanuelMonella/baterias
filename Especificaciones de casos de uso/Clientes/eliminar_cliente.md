# CASO DE USO: Eliminar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla usuarios
- Tener al cliente filtrado

## REQUERIMIENTOS
- El usuario puede eliminar los datos del cliente

## FLUJO NORMAL
1- El sistema muestra una pantalla con los datos de los clientes filtrados
2- El usuario selecciona el cliente que desea eliminar y luego hace click en el boton eliminar
3- El sistema pide confirmacion para eliminar cliente
4- El usuario confirma la eliminacion
5- El sistema elimina al cliente de la base de datos

## FLUJO ALTERNATIVO
- ***.1.** El usuario puede cancelar la operacion haciendo click en el boton "Salir"
- **4.1.** El usuario no confirma la eliminacion y se vuelve a la pantalla anterior

## POSTCONDICIONES
- El cliente eliminado de la base de datos
