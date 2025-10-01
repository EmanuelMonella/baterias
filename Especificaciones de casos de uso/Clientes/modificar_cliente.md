# CASO DE USO: Modificar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado al sistema
- Encontrarse en la pantalla clientes
- Tener al cliente filtrado

## REQUERIMIENTOS
- El usuario puede modificar los datos de los clientes

## FLUJO NORMAL
1. El sistema muestra la pantalla de "Clientes"
2. El usuario selecciona un cliente de la tabla y hace click en el boton "Modificar"
3. El sistema muestra la pantalla Modificar Cliente con los datos del cliente seleccionado
4. El usuario modifica los campos que necesita y presiona el boton "Guardar"
5. El sistema valida los datos y guarda los datos modificados

## FLUJO ALTERNATIVO
- **3.*.** El usuario puede hacer click en el boton "Descartar" y anular la operacion
- **5.1.** El sistema encuentra datos invalidos o nulos, avisa al usuario y vuelve al paso 3

## POSTCONDICIONES
- Los datos del cliente son modificados

