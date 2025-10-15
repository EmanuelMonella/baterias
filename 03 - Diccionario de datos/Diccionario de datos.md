# Diccionario de datos - Baterías Badía



## Gestión de Baterias
- Identifiacion: Marca, modelo, amperaje, codigo, precio compra, precio venta, stock


## Gestión de Usuarios
- Usuarios: Unico
- Identificación: Nombre de usuario, contraseña
- Acceso: Total a todas las funcionalidades

## Gestión de Clientes
- Datos solicitados al cliente: Nombre, patente del vehiculo, teléfono, dirección física

## Gestión de Proveedores
- Datos del proovedor: Nombre/ razón social, teléfono, identifiacion fiscal

## Gestión de Ventas
- Datos de la venta: Cliente, batería, cantidad, precio de venta, método de pago


## Gestión de Compras
- Datos de la compra: Proovedor, cantidad de baterías, precio de la unidad, metodo de pago


# 📘 Tablas de Datos - Baterías Badía

---

## 🔋 Gestión de Baterías

| Nombre del campo | Tipo de dato | Tamaño | Descripción                                | Dominio         |
|------------------|--------------|--------|--------------------------------------------|-----------------|
| marca            | Texto        | 50     | Marca de la batería                        | Discreto        |
| modelo           | Texto        | 50     | Modelo de la batería                       | Discreto        |
| amperaje         | Entero       | -      | Amperaje nominal                           | Continuo        |
| codigo           | Texto        | 30     | Código único de la batería                 | Discreto        |
| precio_compra    | Decimal      | 10,2   | Precio de compra por unidad                | Continuo        |
| precio_venta     | Decimal      | 10,2   | Precio de venta por unidad                 | Continuo        |
| stock            | Entero       | -      | Cantidad disponible en stock               | Discreto        |

---

## 👤 Gestión de Usuarios

| Nombre del campo | Tipo de dato | Tamaño | Descripción                            | Dominio         |
|------------------|--------------|--------|----------------------------------------|-----------------|
| nombre_usuario   | Texto        | 50     | Nombre de login del usuario            | Discreto        |
| contraseña       | Texto        | 255    | Contraseña encriptada                  | Discreto        |
| rol              | Texto        | 20     | Rol del usuario                        | {Administrador} |

---

## 👨‍🔧 Gestión de Clientes

| Nombre del campo     | Tipo de dato | Tamaño | Descripción                             | Dominio         |
|----------------------|--------------|--------|-----------------------------------------|-----------------|
| nombre               | Texto        | 100    | Nombre completo del cliente             | Discreto        |
| patente_vehiculo     | Texto        | 20     | Patente del vehículo del cliente        | Discreto        |
| telefono             | Texto        | 20     | Teléfono de contacto                    | Discreto        |
| direccion            | Texto        | 255    | Dirección física del cliente            | Discreto        |

---

## 🏢 Gestión de Proveedores

| Nombre del campo | Tipo de dato | Tamaño | Descripción                          | Dominio         |
|------------------|--------------|--------|--------------------------------------|-----------------|
| razon_social     | Texto        | 100    | Nombre o razón social del proveedor | Discreto        |
| telefono         | Texto        | 20     | Teléfono de contacto                | Discreto        |
| cuit             | Texto        | 20     | CUIT o identificación fiscal        | Discreto único  |

---

## 💸 Gestión de Ventas

| Nombre del campo | Tipo de dato | Tamaño | Descripción                            | Dominio                                      |
|------------------|--------------|--------|----------------------------------------|----------------------------------------------|
| cliente          | Relación     | -      | Cliente asociado a la venta            | Discreto (FK a Cliente)                      |
| bateria          | Relación     | -      | Batería vendida                        | Discreto (FK a Batería)                      |
| cantidad         | Entero       | -      | Unidades vendidas                      | Discreto                                     |
| precio_venta     | Decimal      | 10,2   | Precio unitario de venta               | Continuo                                     |
| metodo_pago      | Texto        | 30     | Método de pago utilizado               | {Efectivo, Transferencia, Tarjeta}           |
| fecha_venta      | FechaHora    | -      | Fecha y hora de la transacción         | Discreto                                     |
| numero_factura   | Texto        | 30     | Número de factura                      | Discreto (único por venta)                   |

---

## 🛒 Gestión de Compras

| Nombre del campo | Tipo de dato | Tamaño | Descripción                            | Dominio                                      |
|------------------|--------------|--------|----------------------------------------|----------------------------------------------|
| proveedor        | Relación     | -      | Proveedor asociado a la compra         | Discreto (FK a Proveedor)                    |
| bateria          | Relación     | -      | Batería comprada                       | Discreto (FK a Batería)                      |
| cantidad         | Entero       | -      | Unidades compradas                     | Discreto                                     |
| precio_unitario  | Decimal      | 10,2   | Precio por unidad comprada             | Continuo                                     |
| metodo_pago      | Texto        | 30     | Método de pago                         | {Efectivo, Transferencia}                    |
| fecha_compra     | FechaHora    | -      | Fecha de compra                        | Discreto                                     |
| numero_factura   | Texto        | 30     | Número de factura del proveedor        | Discreto (único por compra)                  |
