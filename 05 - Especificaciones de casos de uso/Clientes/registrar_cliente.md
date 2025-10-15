# CASO DE USO: Registrar cliente

## ACTORES
- Usuario

## PRECONDICIONES
- Estar logueado en el sistema

## REQUERIMIENTOS
Los clientes deben registrarse con los siguientes datos:
- Nombre
- Vehiculo
- Telefono
- Direccion

## FLUJO NORMAL
1. El usuario selecciona la opcion "Clientes"
2. El sistema abre la pantalla de clientes
3. El usuario hace click en el boton "Agregar"
4. El sistema pasa a la pantalla "Agregar cliente"
5. El usuario completa los formularios que solicita el sistema y hace click en el boton guardar
6. El sistema valida los datos, registra y almacena al nuevo cliente

## FLUJO ALTERNATIVO
1-* El usuario puede cancelar la operacion haciendo click en el boton descartar

6.1- El sistema valida los datos ingresados, encuentra errores, avisa al usuario y retorna al punto 5

## POSTCONDICIONES
- Queda registrado y guardado el nuevo cliente
