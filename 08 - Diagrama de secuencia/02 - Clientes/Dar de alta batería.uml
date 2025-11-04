@startuml
actor Usuario

Usuario -> PantallaGestiónStock : seleccionarOpciónStock()
PantallaGestiónStock -> PantallaAltaStock : mostrarFormularioAlta()

Usuario -> PantallaAltaStock : completarFormulario(bateria)
Usuario -> PantallaAltaStock : clickGuardar()

PantallaAltaStock -> ControladorStock : registrarBateria(bateria)

ControladorStock -> Bateria : verificarCodigoExistente(bateria.codigo)
alt Código existente
    Bateria --> ControladorStock : existe = true
    ControladorStock -> PantallaAltaStock : mostrarAlerta("CÓDIGO YA EXISTENTE")
    return
else Código no existente
    Bateria --> ControladorStock : existe = false
    ControladorStock -> Bateria : registrarStock(bateria)
    ControladorStock -> Auditoría : registrarEvento("Alta batería: " + bateria.codigo)
    ControladorStock -> PantallaAltaStock : mostrarConfirmación("Batería registrada")
end

== Flujo alternativo: cancelar ==
Usuario -> PantallaAltaStock : clickDescartar()
PantallaAltaStock -> PantallaGestiónStock : volverAGestión()

@enduml
