# CASO DE USO: Agregar proveedor
**ACTORES**  
Usuario del sistema

**PRECONDICIONES**  
1. Estar autenticado en el sistema  
2. Acceder al menú "Gestión de Proveedores"

**REQUERIMIENTOS**  
1. Validar formato de CUIT/DNI según normas tributarias  
2. Verificar unicidad del CUIT/DNI en el sistema  
3. Campos obligatorios: Nombre (mín. 5 caracteres), Teléfono (formato numérico), CUIT/DNI

**FLUJO NORMAL**  
1. Sistema muestra formulario con campos: Nombre, Teléfono, CUIT/DNI  
2. Usuario completa datos y presiona "Guardar"  
3. Sistema valida formato y unicidad del CUIT/DNI  
4. Sistema registra proveedor y muestra mensaje de confirmación

**FLUJO ALTERNATIVO**  
2.1. Usuario cancela operación con botón "Cancelar"  
3.1. Datos incompletos/inválidos → Sistema muestra errores específicos  
3.2. CUIT/DNI existente → Sistema alerta "Proveedor ya registrado"

**POSTCONDICIONES**  
Nuevo proveedor queda registrado en la base de datos