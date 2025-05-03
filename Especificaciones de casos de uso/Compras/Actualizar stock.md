# CASO DE USO: Actualizar inventario  
**ACTORES**  
Sistema automatizado  

**PRECONDICIONES**  
1. Compra registrada y validada  
2. Productos con stock mínimo configurado  

**REQUERIMIENTOS**  
1. Ajuste paralelo de múltiples almacenes  
2. Notificaciones para reposición de stock  
3. Control de versiones de inventario  

**FLUJO NORMAL**  
1. Al confirmar compra:  
   - Sistema actualiza stock físico y disponible  
   - Calcula nuevo punto de reorden  
   - Genera etiquetas RFID/Lote automáticamente  
2. Integra con:  
   - Módulo de ventas (actualiza disponibilidad)  
   - Almacén inteligente (ubica productos según algoritmo)  

**FLUJO ALTERNATIVO**  
1.1. Producto nuevo → Crea registro en inventario con datos de compra  
1.2. Diferencia inventario físico vs. sistema → Genera reporte de discrepancias  

**POSTCONDICIONES**  
- Base de datos de inventario sincronizada  
- Notificación a logística si se alcanza stock máximo  
