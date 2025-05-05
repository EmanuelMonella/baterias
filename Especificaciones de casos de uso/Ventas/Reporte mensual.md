# CASO DE USO: Generar reporte mensual  

## ACTORES  
Usuario  

## PRECONDICIONES  
1. Mes cerrado contablemente  
2. Datos consolidados disponibles  

## REQUERIMIENTOS  
1. Comparativo mes actual vs. mes anterior vs. mismo mes año anterior  
2. Análisis ABC de productos  
3. Márgenes de ganancia por categoría  

## FLUJO NORMAL  
1. Sistema compila datos y genera:  
   - Dashboard interactivo con 5 vistas clave:  
     1. Evolución diaria de ventas  
     2. Mix de medios de pago  
     3. Top 10 clientes  
     4. Rentabilidad por línea de productos  
     5. Cumplimiento de metas  
2. Incluye:  
   - Gráficos combinados (barras + líneas)  
   - Tablas resumen con KPIs  
   - Análisis predictivo para próximo mes  
3. Opciones de exportación:  
   - Presentación ejecutiva (PPT)  
   - Datos crudos (SQL dump)  
   - Formato impresión optimizado  

## FLUJO ALTERNATIVO  
1.1. Datos inconsistentes → Genera reporte parcial con alertas de validación  
2.1. Personalización → Permite agregar métricas personalizadas vía SQL query  

## POSTCONDICIONES  
- Reporte archivado en sección documentación  
- Dispara notificaciones a stakeholders vía email  