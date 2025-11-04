@startuml
actor Usuario

Usuario -> PantallaGestiónStock : seleccionarBateria(codigo)
activate PantallaGestiónStock
PantallaGestiónStock -> PantallaModificarStock : mostrarFormulario(bateria)
activate PantallaModificarStock
PantallaModificarStock --> PantallaGestiónStock : formularioMostrado()
deactivate PantallaGestiónStock

Usuario -> PantallaModificarStock : ingresarNuevaCantidad(cantidad)
Usuario -> PantallaModificarStock : clickGuardar()

PantallaModificarStock -> ControladorStock : modificarStock(bateria, nuevaCantidad)
activate ControladorStock

ControladorStock -> Bateria : verificarCodigoExistente(bateria.codigo)
activate Bateria

alt Código existente
    Bateria --> ControladorStock : true
    deactivate Bateria

    ControladorStock -> Bateria : actualizarCantidad(nuevaCantidad)
    activate Bateria
    Bateria --> ControladorStock : cantidadActualizada()
    deactivate Bateria

    ControladorStock -> PantallaModificarStock : mostrarConfirmación("Stock actualizado correctamente")
    deactivate ControladorStock
    activate PantallaModificarStock
    PantallaModificarStock --> Usuario : confirmaciónMostrada()
    deactivate PantallaModificarStock

else Código no encontrado
    Bateria --> ControladorStock : false
    deactivate Bateria

    ControladorStock -> PantallaModificarStock : mostrarAlerta("Código no encontrado")
    deactivate ControladorStock
    activate PantallaModificarStock
    PantallaModificarStock --> Usuario : alertaMostrada()
    deactivate PantallaModificarStock
end

== Flujo alternativo: cancelar ==

Usuario -> PantallaModificarStock : clickCancelar()
activate PantallaModificarStock
PantallaModificarStock -> PantallaGestiónStock : volverAGestión()
activate PantallaGestiónStock
PantallaGestiónStock --> PantallaModificarStock : vistaPrincipalMostrada()
deactivate PantallaGestiónStock
deactivate PantallaModificarStock

@enduml