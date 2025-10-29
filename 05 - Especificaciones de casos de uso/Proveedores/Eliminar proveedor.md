# CASO DE USO: Eliminar proveedor

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema

## REQUERIMIENTOS
- El usuario puede eliminar los datos del proveedor

## FLUJO NORMAL
1. Usuario introduce el nombre del proveedor y selecciona FILTRAR
2. Sistema muestra los datos de los proveedores filtrados
3. Usuario selecciona el proveedor que desea eliminar y luego selecciona ELIMINAR
4. Sistema pide confirmación para eliminar proveedor
5. Usuario confirma la eliminación
6. Sistema elimina al proveedor de la base de datos

## FLUJO ALTERNATIVO
- **1.*.** El usuario puede cancelar la operación seleccionando "Salir"
- **4.1.** El usuario no confirma la eliminación y se vuelve a la pantalla anterior

## POSTCONDICIONES
- El proveedor eliminado de la base de datos

