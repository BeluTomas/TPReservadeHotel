# TP e-commerce

## Grupo
### Integrantes
* 49330 - Dignani, Clara Josefina
* 49702 - Periolo, Ángela Sol
* 48814 - Tomas, Maria Belen
* 49256 - Muller, Dafne

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)

## Tema
### Descripción
Esta plataforma de comercio electrónico se especializa en la venta de prendas de ropa. Los usuarios pueden explorar y seleccionar productos de un catálogo publicado por el vendedor. Ofrecemos la opción de iniciar sesión para mantener un registro de datos personales y compras realizadas. Nuestro sistema facilita todas las etapas de la transacción, desde agregar productos al carrito hasta completar el pago. Además, mantenemos un registro actualizado del stock disponible y los pedidos realizados para una experiencia de compra sin complicaciones.

### Modelo
![imagen del modelo](https://github.com/BeluTomas/TPReservadeHotel/blob/0c96812e3d4866297dab3df2cbeca8ff66befcc2/ER.drawio.png)

### Reglas de negocio
1. Solo se pueden realizar reservas de habitaciones disponibles.
2. El pago debe ser realizado en la reserva. 
3. El check-in solo puede ser realizado por un huésped con una reserva confirmada.
4. El check-out debe ser realizado antes de la fecha de salida programada.
5. Se requiere la presentación de documentación de identidad válida durante el check-in.
6. La reserva tiene un único estado en un momento determinado (cancelada, completada, en curso, confirmada).
7. Si la fecha de check-out de la reserva es anterior a la fecha actual, la reserva ha finalizado y la habitación está disponible.
8. Si la fecha de check-in de la reserva es posterior a la fecha actual, la reserva aún no ha comenzado y la habitación está disponible.
9. Si 7 o 8 no se cumple, la reserva está en curso y la habitación no está disponible.
   
## Alcance Funcional 

### Alcance Mínimo

|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitación<br>2. CRUD Habitación<br>3. CRUD Cliente<br>4. CRUD Facturacion<br>5. CRUD Reserva|
|CRUD simple|1. CRUD Tipo Habitacion<br> 2. CRUD Cliente|
|CRUD dependiente|1. CRUD Habitación {depende de} CRUD Tipo Habitacion<br>2. CRUD Reserva {depende de} CRUD Habitación y CRUD Cliente|
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|[CUU01. Reservar una habitación para la estadía](https://github.com/angelaperiolo/CUU01/blob/adffcdb7aade3f0c74fdc58516d306b6d9a3d308/README.md)<br>[CUU02. Realizar el check-in de una reserva](https://github.com/angelaperiolo/CUU02/blob/06bcf107fdb7f5e2fc1e23d1b5ba1373b395ad18/README.md)<br>[CUU03. Realizar el check-out y facturación de estadía](https://github.com/angelaperiolo/CUU03/blob/2e6b3b5206b55a7a11d3509415bb3e044a3de395/README.md)|
