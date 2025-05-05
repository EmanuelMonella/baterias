# CASO DE USO: Consultar histórico

## ACTORES  
Usuario   

## PRECONDICIONES  
1. Acceso al módulo de reportes  
2. Período consultado no mayor a 5 años  

## REQUERIMIENTOS  
1. Filtros combinables:  
   - Rango de fechas (desde-hasta)  
   - Tipo de cliente (minorista/mayorista)  
   - Vendedor responsable  
   - Estado (pagada/anulada/pendiente)  

## FLUJO NORMAL  
1. Sistema muestra panel de control con:  
   - Gráfico temporal de ventas  
   - Tabla dinámica con columnas personalizables  
   - Filtros avanzados en sidebar  
2. Usuario aplica múltiples criterios de búsqueda  
3. Sistema genera vista con:  
   - Detalle de transacciones  
   - Totales parciales por categoría  
   - Opción de exportar a Excel/CSV  

## FLUJO ALTERNATIVO  
2.1. Sin resultados → Sugiere ampliar rango de fechas  
3.1. Selección masiva → Habilita acciones por lote (reasignar vendedor, exportar múltiples)  

## POSTCONDICIONES  
- Registro de consulta en auditoría  
- Cache de resultados para próximas consultas similares