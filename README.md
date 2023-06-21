# TPReservadeHotel

## Grupo
### Integrantes
* 49330 - Dignani, Clara Josefina
* 49702 - Periolo, Angela Sol
* 48814 - Tomas, Maria Belen
* 49256 - Muller, Dafne

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)


## Tema
### Descripción
Un sistema de gestión hotelera que permite reservar habitaciones, realizar pagos, hacer check-in y check-out. Los clientes podrán seleccionar fechas de llegada y salida, número de huéspedes y preferencias de habitaciones. El sistema calculará el costo total. Los empleados podrán hacer check-in, verificar identidad y asignar llaves. Al hacer check-out  se proporcionará una factura. El sistema debe ser intuitivo, seguro y generar informes de reservas, ingresos y disponibilidad de habitaciones. 


### Modelo
![imagen del modelo](https://github.com/BeluTomas/TPReservadeHotel/blob/11246e28b2f52561e9a338306582d71f5f1bc2d2/ER.drawio.png)

## Alcance Funcional 

### Alcance Mínimo

|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Habitacion<br> 2. CRUD Provincia|
|CRUD dependiente|1. CRUD Habitación {depende de} CRUD Tipo Habitacion<br>|
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Localidad<br>3. CRUD Habitación<br>4. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía|


