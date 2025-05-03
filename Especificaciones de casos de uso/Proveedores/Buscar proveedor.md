# CASO DE USO: Buscar proveedor  
**ACTORES**  
Usuario

**PRECONDICIONES**  
1. Tener permisos de consulta  
2. Estar en la pantalla "Listado de Proveedores"

**REQUERIMIENTOS**  
1. Búsqueda por: Nombre (coincidencia parcial), CUIT/DNI (exacto)  
2. Resultados en tabla con columnas: Nombre, Teléfono, CUIT/DNI, Última compra

**FLUJO NORMAL**  
1. Sistema muestra campo de búsqueda y tabla vacía  
2. Usuario ingresa criterios y presiona "Buscar"  
3. Sistema filtra proveedores y muestra resultados paginados

**FLUJO ALTERNATIVO**  
2.1. Usuario vacía criterios → Sistema muestra últimos 20 registros  
3.1. Sin resultados → Muestra "No se encontraron proveedores"

**POSTCONDICIONES**  
Listado actualizado según criterios de búsqueda