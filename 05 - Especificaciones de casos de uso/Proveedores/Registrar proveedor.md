# CASO DE USO: Registrar proveedor

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado en el sistema

## REQUERIMIENTOS
Los proveedores deben registrarse

## FLUJO NORMAL
1. Usuario selecciona la opcion "Proveedores"
2. Sistema abre la pantalla de PROVEEDORES
3. Usuario completa los datos del proveedor: NOMBRE, CUIT y TELEFÓNO, luego seleeciona "Agregar"
4. Sistema valida los datos esten completos, registra y almacena al nuevo proveedor

## FLUJO ALTERNATIVO
- **1.*.** El usuario puede cancelar la operacion seleccionando descartar
- **6.1.** El sistema valida los datos ingresados, encuentra errores, avisa al usuario y retorna al punto 3

## POSTCONDICIONES
- Queda registrado y guardado el nuevo proveedor
