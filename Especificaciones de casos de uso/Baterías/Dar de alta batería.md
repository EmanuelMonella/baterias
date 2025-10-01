# CASO DE USO: Dar alta batería

## ACTORES  
- Usuario

## PRECONDICIONES  
- Estar logueado en el sistema  
- Existencia de un proveedor registrado en el sistema  
- Código de batería no debe estar previamente registrado (único)

## REQUERIMIENTOS  
El usuario debe registrar una batería.

## FLUJO NORMAL  
1. El usuario selecciona la opción STOCK 
2. El sistema abre la pantalla de gestión de stock 
3. El usuario hace clic en el botón DAR DE ALTA 
4. El sistema muestra la pantalla ALTA DE STOCK con el formulario correspondiente  
5. El usuario completa los campos requeridos 
6. El usuario hace clic en el botón GUARDAR 
7. El sistema valida los datos ingresados y registra el nuevo STOCK

## FLUJO ALTERNATIVO  
- **5.1** El usuario puede cancelar la operación haciendo clic en el botón DESCARTAR  
- **7.1** Si el código ingresado ya existe, el sistema muestra el mensaje de alerta: CODIGO YA EXISTENTE y retorna al paso 5  
- **7.2** Si hay datos incompletos o inválidos, el sistema resalta los campos con errores y retorna al paso 5

## POSTCONDICIONES  
- La batería queda registrada y disponible en el catálogo  

