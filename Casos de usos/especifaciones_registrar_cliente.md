# **Caso de Uso:** Registrar Cliente

## **Actores**
- Usuario del sistema

## **Precondiciones**
✅ El usuario debe estar autenticado en el sistema

## **Requerimientos**
📋 Campos obligatorios para registro:
1. Nombre del cliente
2. Vehículo asociado
3. Teléfono de contacto
4. Dirección física

---

## **Flujo Principal**

1. **Usuario:** Selecciona opción "Clientes" en el menú  
   → *Sistema muestra pantalla de gestión de clientes*

2. **Usuario:** Hace clic en botón "Agregar"  
   → *Sistema carga pantalla "Agregar cliente"*

3. **Usuario:** Completa formulario con datos requeridos

4. **Usuario:** Presiona botón "Guardar"  
   → *Sistema ejecuta validación de datos*

5. **Sistema:** Registra cliente en base de datos  
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
