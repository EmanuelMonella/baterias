# CASO DE USO: Ver historial de compras  
**ACTORES**  
Usuario con rol de compras

**PRECONDICIONES**  
1. Proveedor seleccionado en listado  
2. Historial disponible en los últimos 5 años

**REQUERIMIENTOS**  
1. Visualización cronológica inversa (últimas primero)  
2. Filtros por: período, monto mínimo, tipo de producto  
3. Exportación a PDF/Excel

**FLUJO NORMAL**  
1. Usuario selecciona "Ver Historial" en registro  
2. Sistema muestra tabla con: Fecha, Producto, Cantidad, Monto, N° Factura  
3. Usuario aplica filtros y ordena columnas

**FLUJO ALTERNATIVO**  
2.1. Sin operaciones registradas → Muestra gráfico vacío con leyenda  
3.1. Selecciona factura → Muestra detalle ampliado

**POSTCONDICIONES**  
Consulta registrada en auditoría de acceso