# CASO DE USO: Modificar proveedor

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla proveedores

## REQUERIMIENTOS
- El usuario puede modificar los datos de los proveedores

## FLUJO NORMAL
1. Usuario introduce el nombre del usuario y selecciona FILTRAR
2. Sistema muestra la pantalla de "Proveedores"
3. Usuario selecciona un proveedor de la tabla y hace click en el boton "Modificar"
4. Sistema muestra la pantalla Modificar Proveedor con los datos de NOMBRE, CUIT y TELEFÓNO del proveedor seleccionado
5. Usuario modifica los campos que necesita y presiona el boton "Guardar"
6. Sistema valida los datos y guarda los datos modificados

## FLUJO ALTERNATIVO
- **3.*.** El usuario puede seleccionar "Descartar" o "Salir" y anular la operación
- **5.1.** El sistema encuentra datos invalidos o nulos, avisa al usuario y vuelve al paso 3

## POSTCONDICIONES
- Los datos del proveedor son modificados

