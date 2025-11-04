@startuml
actor Usuario

== Registrar Compra ==

Usuario -> PantallaCompras : ingresarModulo("COMPRAS")
PantallaCompras -> ControladorCompras : mostrarCampoProveedor()

Usuario -> PantallaCompras : ingresarNombreProveedor(nombre)
PantallaCompras -> ControladorCompras : buscarProveedor(nombre)

ControladorCompras -> Proveedores : buscarPorNombre(nombre)
alt proveedor encontrado
    Proveedores --> ControladorCompras : listaProveedores
    ControladorCompras -> PantallaCompras : mostrarListaProveedores(listaProveedores)
    Usuario -> PantallaCompras : seleccionarProveedor(proveedor)
    PantallaCompras -> ControladorCompras : mostrarFormularioCompra()
else no encontrado
    Proveedores --> ControladorCompras : vacío
    ControladorCompras -> PantallaCompras : mostrarMensaje("Proveedor no registrado")
end

Usuario -> PantallaCompras : completarFormulario(marca, modelo, cantidad)
PantallaCompras -> ControladorCompras : validarDatos(marca, modelo, cantidad)

alt datos válidos
    ControladorCompras -> PantallaCompras : solicitarConfirmacion()
    Usuario -> PantallaCompras : confirmarOperacion()
    PantallaCompras -> ControladorCompras : registrarCompra()
    ControladorCompras -> Compra : crearCompra(proveedor, marca, modelo, cantidad)
    Compra -> Inventario : actualizarStock(marca, modelo, cantidad)
    Inventario --> Compra : stockActualizado
    Compra --> ControladorCompras : compraConfirmada
    ControladorCompras -> PantallaCompras : mostrarMensaje("Compra registrada")
else datos inválidos
    ControladorCompras -> PantallaCompras : resaltarCamposInvalidos()
end

alt usuario cancela
    Usuario -> PantallaCompras : seleccionar("DESCARTAR")
    PantallaCompras -> ControladorCompras : cancelarOperacion()
end

ControladorCompras --> Usuario : mensaje final o vista actualizada

@enduml
