# CASO DE USO: Registrar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado en el sistema

## REQUERIMIENTOS
Los clientes deben registrarse

## FLUJO NORMAL
1. Usuario selecciona la opcion "Clientes"
2. Sistema abre la pantalla de clientes
3. Usuario completa los datos del cliente: NOMBRE, VEHICULO, TELEFONO Y DIRECCIÓN, luego seleeciona "Agregar"
4. Sistema valida los datos esten completos, registra y almacena al nuevo cliente

## FLUJO ALTERNATIVO
- **1.*.** El usuario puede cancelar la operacion seleccionando descartar
- **6.1.** El sistema valida los datos ingresados, encuentra errores, avisa al usuario y retorna al punto 3

## POSTCONDICIONES
- Queda registrado y guardado el nuevo cliente
