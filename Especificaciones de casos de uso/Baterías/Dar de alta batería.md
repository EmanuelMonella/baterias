# CASO DE USO: Dar alta batería

## ACTORES  
Usuario

## PRECONDICIONES 
1. Usuario logueado 
2. Proveedor registrado en el sistema  
3. Código único disponible (no duplicado)  

## REQUERIMIENTOS 
El usuario puede registrar el alta.

## FLUJO NORMAL  
1. Sistema muestra formulario con:  
   - Datos básicos: Modelo, Fabricante, SKU  
   - Especificaciones técnicas:  
     • Voltaje (12V/24V/48V)  
     • Capacidad (Ah)  
     • Química (Li-ion/Plomo-ácido)  
     • Ciclos de vida garantizados  
   - Datos logísticos:  
     • Proveedor principal  
     • Almacén destino  
     • Stock inicial  
2. Usuario completa datos y adjunta:  
   - Ficha técnica PDF  
   - Certificado de cumplimiento normativo  
3. Sistema:  
   - Genera código QR con datos críticos  
   - Crea registro en base de datos relacional  
   - Dispara notificación a control de calidad  

## FLUJO ALTERNATIVO 
1.1. SKU duplicado → Alerta "Código ya existente"  
2.1. Datos incompletos → Resalta campos faltantes en rojo  

## POSTCONDICIONES  
- Batería disponible en catálogo  
- Evento registrado en log de auditoría  