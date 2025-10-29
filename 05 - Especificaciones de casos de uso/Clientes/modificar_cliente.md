# CASO DE USO: Modificar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla clientes

## REQUERIMIENTOS
- El usuario puede modificar los datos de los clientes

## FLUJO NORMAL
1. Usuario introduce el nombre del usuario y selecciona FILTRAR
2. Sistema muestra la pantalla de "Clientes"
3. Usuario selecciona un cliente de la tabla y hace click en el boton "Modificar"
4. Sistema muestra la pantalla Modificar Cliente con los datos de NOMBRE, VEHICULO, TELEFONO y DIRECCIÓN del cliente seleccionado
5. Usuario modifica los campos que necesita y presiona el boton "Guardar"
6. Sistema valida los datos y guarda los datos modificados

## FLUJO ALTERNATIVO
- **3.*.** El usuario puede seleccionar "Descartar" o "Salir" y anular la operación
- **5.1.** El sistema encuentra datos invalidos o nulos, avisa al usuario y vuelve al paso 3

## POSTCONDICIONES
- Los datos del cliente son modificados

