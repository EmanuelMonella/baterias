# **Caso de Uso:** Registrar Cliente

## **Actores**
- Usuario del sistema

## **Precondiciones**
✅ El usuario debe estar autenticado en el sistema

## **Requerimientos**
📋 Campos obligatorios para registro:
1. Nombre del cliente
2. Vehículo asociado
3. Teléfono de contacto
4. Dirección física

---

## **Flujo Principal**

1. **Usuario:** Selecciona opción "Clientes" en el menú  
   → *Sistema muestra pantalla de gestión de clientes*

2. **Usuario:** Hace clic en botón "Agregar"  
   → *Sistema carga pantalla "Agregar cliente"*

3. **Usuario:** Completa formulario con datos requeridos

4. **Usuario:** Presiona botón "Guardar"  
   → *Sistema ejecuta validación de datos*

5. **Sistema:** Registra cliente en base de datos  
   → *Muestra confirmación de éxito*

---

## **Flujo Alternativo**

### **A1: Cancelación de operación**
1. En cualquier paso anterior al 4:  
   → **Usuario:** Presiona botón "Descartar"  
   → *Sistema cancela operación y vuelve al menú principal*

### **A2: Datos inválidos**
1. Después del paso 4:  
   → **Sistema:** Detecta errores en formulario  
   → Muestra mensaje de error detallado  
   → **Usuario:** Corrige datos y reintenta guardar

---

## **Postcondiciones**
🗄️ El nuevo cliente queda registrado con:  
- Fecha de creación automática
- Estado activo por defecto
- Historial de cambios auditado

