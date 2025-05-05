# CASO DE USO: Dar baja batería 

## ACTORES**  
Usuario  

## PRECONDICIONES  
1. Batería en estado "Activa"  
2. Sin transacciones pendientes  

## REQUERIMIENTOS
El usuario puede registrar el baja.

## FLUJO NORMAL
1. Usuario selecciona batería y elige motivo de baja:  
   - Defecto de fabricación  
   - Fin de vida útil  
   - Retiro del mercado  
2. Sistema verifica:  
   - Sin ventas asociadas en últimos 30 días  
   - No pertenece a kits activos  
3. Requiere:  
   - Carga documento de disposición final  
   - Firma digital del responsable  
4. Ejecuta baja lógica (no eliminación física)  

## FLUJO ALTERNATIVO  
1.1. Batería en garantía → Abre ticket con fabricante  
3.1. Baja masiva → Habilita proceso batch con validación por lote  

## POSTCONDICIONES  
- Estado actualizado a "Retirada"  
- Espacio liberado en almacén  