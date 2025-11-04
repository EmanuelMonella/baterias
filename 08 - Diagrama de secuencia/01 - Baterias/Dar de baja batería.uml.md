@startuml
actor Usuario

participant "Pantalla Gestión de Baterías" as Pantalla
participant "Sistema" as Sistema
participant "Base de Datos" as BD

== Flujo normal ==

Usuario -> Pantalla : Selecciona batería a dar de baja
Pantalla -> Sistema : Solicita motivos de baja
Sistema -> Pantalla : Muestra opciones:\n- Defecto de fabricación\n- Fin de vida útil\n- Retiro del mercado

Usuario -> Pantalla : Selecciona motivo de baja
Pantalla -> Sistema : Envía motivo seleccionado
Sistema -> Pantalla : Solicita confirmación

alt Usuario no confirma
    Usuario -> Pantalla : No confirma operación
    Pantalla -> Sistema : Cancela baja
    Sistema -> Pantalla : Retorna a selección de motivo
else Usuario confirma
    Usuario -> Pantalla : Confirma operación
    Pantalla -> Sistema : Envía confirmación y motivo
    Sistema -> BD : Actualiza estado de batería a "Inactiva"\nReduce stock
    BD --> Sistema : Confirmación de actualización
    Sistema -> Pantalla : Muestra mensaje de confirmación
end

alt Usuario descarta operación en cualquier momento
    Usuario -> Pantalla : Cancela la operación
    Pantalla -> Sistema : Cancela baja
    Sistema -> Pantalla : Retorna a vista principal
end

@enduml
