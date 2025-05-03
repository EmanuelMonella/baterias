# CASO DE USO: Modificar proveedor  
**ACTORES**  
Usuario autorizado

**PRECONDICIONES**  
1. Proveedor existente en el sistema  
2. Sin modificaciones pendientes de aprobación

**REQUERIMIENTOS**  
1. Histórico de cambios con versión anterior y nueva  
2. Bloqueo de edición concurrente

**FLUJO NORMAL**  
1. Usuario selecciona "Editar" en registro  
2. Sistema muestra formulario con datos actuales  
3. Usuario modifica campos permitidos y guarda  
4. Sistema registra nueva versión y notifica actualización

**FLUJO ALTERNATIVO**  
3.1. Campos obligatorios vacíos → Resalta campos faltantes  
3.2. Otro usuario editando → Muestra "Registro en edición por [usuario]"

**POSTCONDICIONES**  
Datos actualizados con marca temporal de modificación
