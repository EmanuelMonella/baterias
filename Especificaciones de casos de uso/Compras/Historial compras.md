# CASO DE USO: Consultar histórico  
**ACTORES**  
Auditor/Administrador  

**PRECONDICIONES**  
1. Acceso al módulo de reportes  
2. Período consultado ≤ 3 años  

**REQUERIMIENTOS**  
1. Búsqueda multicriterio:  
   - Proveedor específico o categoría  
   - Rango de montos (mín-máx)  
   - Estado de pago (pagado/pendiente)  
2. Visualización comparativa vs. presupuesto  

**FLUJO NORMAL**  
1. Sistema muestra interfaz con:  
   - Selector de período personalizado  
   - Filtros avanzados en panel lateral  
   - Vista de calendario con eventos clave  
2. Usuario configura parámetros de búsqueda  
3. Sistema genera:  
   - Gráfico evolutivo de compras por categoría  
   - Tabla detallada con capacidad de ordenamiento múltiple  
   - Resumen estadístico (promedios, máximos, tendencias)  

**FLUJO ALTERNATIVO**  
2.1. Sin filtros aplicados → Muestra último trimestre  
3.1. Exportación a Excel → Mantiene formato con encabezados personalizados  

**POSTCONDICIONES**  
- Generación de log de auditoría con parámetros de búsqueda  
- Almacenamiento temporal de resultados por 72h  