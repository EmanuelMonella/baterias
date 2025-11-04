@startuml
actor Usuario

== Consultar Histórico Compra ==

Usuario -> PantallaReportes : ingresarApartado("REPORTES")
PantallaReportes -> ControladorReportes : mostrarCasilleros()

Usuario -> PantallaReportes : ingresarDatos(marca, tipoOperacion)
PantallaReportes -> ControladorReportes : buscarHistorial(marca, tipoOperacion)

ControladorReportes -> HistorialCompras : buscarPorMarcaYOperacion(marca, tipoOperacion)
alt registros encontrados
    HistorialCompras -> Registro : obtenerDatos()
    Registro --> HistorialCompras : listaDatos
    HistorialCompras --> ControladorReportes   : listaDatos
    ControladorReportes -> PantallaReportes : mostrarResultados(listaDatos)
else sin registros
    HistorialCompras --> ControladorReportes : vacío
    ControladorReportes -> PantallaReportes : mostrarMensaje("NO HAY REGISTROS")
end

alt usuario cancela
    Usuario -> PantallaReportes : seleccionar("SALIR")
    PantallaReportes -> ControladorReportes : cancelarConsulta()
end

ControladorReportes --> Usuario : historial en pantalla o mensaje correspondiente

@enduml