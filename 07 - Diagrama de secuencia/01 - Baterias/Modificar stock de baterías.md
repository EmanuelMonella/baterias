@startuml
actor Usuario

participant "Pantalla Gestión de Baterías" as Pantalla
participant "Sistema" as Sistema
participant "Base de Datos" as BD

== Inicio del proceso ==

Usuario -> Pantalla : Selecciona batería a modificar
Pantalla -> Sistema : Solicita datos actuales
Sistema -> BD : Consulta batería por ID
BD --> Sistema : Devuelve datos actuales
Sistema -> Pantalla : Muestra datos actuales y panel de edición

== Edición por parte del usuario ==

Usuario -> Pantalla : Edita campos + Ingresa descripción del cambio
Pantalla -> Sistema : Envía cambios y descripción

alt Modificación crítica
    Sistema -> Usuario : Solicita aprobación adicional
    Usuario -> Sistema : Aprueba modificación
end

== Actualización y confirmación ==

Sistema -> BD : Guarda nueva versión de batería
BD --> Sistema : Confirmación de actualización

Sistema -> BD : Archiva versión anterior
Sistema -> BD : Actualiza fecha de última modificación
Sistema -> Pantalla : Muestra mensaje de confirmación

@enduml