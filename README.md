# actividad-de-arquitectura-servidor/cliente 

Este es un que se hace con el fin de mostrar que mediante los saberes previos de programación es posible crear aplicaciones que nos beneficia en el día a día. El desarrollo de este tipo de trabajos ayuda a automatizar los procesos  y mejorar eficientemente nuestra capacidad de gestionar las ventas y compras llevar un control óptimo del inventario a través del nuestro lenguaje de programación Java y el uso de la base de datos relacionales. 
 
Montaje y Explicación de aplicativo de ventas de Tienda de Computadoras.

Para el ejercicio se va a montar la base de datos con el siguiente modelo.

 
Como se observa nuestra aplicación tiene varias tablas. 

La tabla de usuario
Posee información de los empleados y administradores del negocio
 
 Nombre- Nombre completo del empleado o administrador
Correo electrónico- El usuario debe digitar el correo personal.
Contraseña- esta debe ser o pass esta debe contener números y letras o solo números depende del empleado.
Rol-sea empleado o administrador.


La tabla de Proveedor
Es el apartado perteneciente a las compañías que le vende a nuestra tienda de computadora, puede ser distintas empresas, la cual posee las siguientes características.
 
Ruc – Es el registro único Tributario “Rut”.
Nombre- Nombre del proveedor o la empresa que distribuye a la tienda de computadora.
Teléfono- Es el teléfono de Domicilio de la empresa.
Dirección- Al ser una empresa conformada debe tener una ubicación de residencia. 

Tabla de Clientes.
Esta tabla posee información de los clientes que van a menudo a la tienda.
 
CC- Se refiere al número de cédula de ciudadanía o dni.
Nombre- Nombre del Cliente, este contiene apellidos y nombres completos.
Teléfono – Sea celular o número fijo.
Dirección- Se refiere a la dirección de residencia esto incluye el departamento, la ciudad y dirección.
Fecha- Se refiere a la fecha de registro del usuario.





Tabla de Producto
 
Es el registro de los productos que nuestra tienda de computadores adquiere, estos tienen los siguientes parámetros.
Código- es el código de barras que el producto posee o registro.
Nombre- es el Nombre del producto sea un teclado u algún componente.
Id_proveedor- se refiere al id del proveedor de quien nos vendió el producto, esta relación con la tabla de proveedor es 1 a muchos ya que un proveedor puede distribuir más componentes.
Stock- Se refiere a la cantidad de productos que se dispone.
Precio- Es el precio al que nosotros vamos a vender el producto.
Fecha- Se refiere a la fecha de adquisición del producto.

Tabla de Ventas 
Se refiere a la factura de ventas , allí almacenamos nuestras ventas que hacemos a los distintos clientes.

 
Id_cliente- Se refiere al cliente que adquirió nuestro producto , esta relación es de 1 a muchas ya que un cliente puede ir varias veces a nuestro atienda y adquirir nuestros productos, si juan lo guarde con el id “1” en la tabla de clientes, este número debe ir en la tabla de ventas en el caso que juan compre algún componente de pc.
Id_empleado: Se refiere al empleado que lo atendió en el momento , este se conecta de 1 a muchos con la tabla de usuario. 
Total : Es el total de la compra, si se supone una compra de varios componentes esta suma de esos componentes nos debe de dar un total.
Fecha : es la fecha del cual hicimos la venta.

Tabla de detalles

Los detalles se refieren a los productos, que productos se vendió y en que cantidades. Información más detallada de nuestra Venta.
 
Id_Venta: Se refiere al producto como tal que se anda vendiendo. Este tiene una relación de uno a muchos con la factura.
Cod_producto: Es el id del producto que se vendió, tiene una relación de uno a muchos ya que con el detalle puede venderse 1 producto varias veces.
Cantidad: se refiere a cuantas existencias del producto se ha vendido.
Precio: Es el precio unitario del producto.

Para el montaje de nuestro proyecto se sigue los siguientes pasos:
Paso 1: Se crea la data base y se usa automáticamente:
 
Ya sea en mysql o admin en mysql y a continuación se inserta las tablas presentadas anteriormente. 
Paso 2: se mysql ingresar un usuario por definición
 

Paso 3: Correr nuestro Proyecto
A CONTINUACIÓN CORREMOS NUESTRO PROYECTO

Vamos a nuestra carpeta donde tenemos el proyecto y vamos a la ruta dist y elegimos el ícono donde está uestro proyecto.
 
Por definición se abre con los siguientes datos predeterminados.
 
Ingreso en login  y entramos al siguiente imagen 
 
Como se puede ver tiene botones que vamos a hacerlo por el siguiente orden .
Paso 4. Primero registramos Proveedores.
 
 
Donde si ingresamos datos de un proveedor al azar 
 
En el ícono de caset se guarda información 
 
Y aparecerá en nuestros registros 
 
Podemos editar , por ejemplo las direcciones están mal digitadas entonces le cambiamos la haciendo clic sobre ellas 
 
A continuación editamos la dirección
 
Y le damos en el icono azul para editar
 
Si queremos borrar de igual manera, pero en el icono rojo seleccionando el proveedor.
 
Ahora bien, vamos a ir a la parte de ingresar nuevo cliente
Al igual que proveedor clientes tiene los mismos comandos 

Por otro lado en el comando de registrar usuario no tiene esa opción si no solo de registrar usuario o empleados
 
El administrador debe registrar al empleado y su rol-.
 
Ingresa sus datos y a continuación queda registrado, ya registrado el nuevo empleado sale la tabla 

 

Po otro lado podemos registrar los Productos 
 
 
Al igual que los demás comandos sale registrar los productos, no obstante el proveedor sale la lista los cuales ya hemos registrado.
 
 
Ya registrado nuestro producto Podemos actualizar y borrar si queremos. A continuación, vamos a registrar una compra.
Vamos a comprar el tablero virtual y un monitor el total sería $440.000 por nuestra compra con los usuarios ya registrados.
 
En el parto de ventas hacemos clic
Luego se digita el código del producto 
 
Ya digitado el producto le damos ENTER.
 
Se despega el nombre de producto y el precio automáticamente, a continuación digitamos la cantidad y a continuación la tecla ENTER.
 
Como se ve registramos nuestro primer producto, de igual manera registramos el mauz.
 
Podemos eliminar mauz de fila y digitar de nuevo dando clic en el ícono de eliminar fila y clic en el producto
 
 
En este caso digitamos la cantidad de mauz mal, pero podemos revertir en el comando.
 

Digitamos la cédula del cliente y observamos que el total de la compra es igual a $440.000
A continuación registramos nuestra compra 
 
A continuación me genera el pdf o recibo de la compra

 
Ahove veremos las ventas que se ha hecho 
 
Al igual se despliega un cuadro de las ventas 
 
Estas se pueden imprimir igual que el recibo, nuestra ´´útima venta se puede ver seleccionando la fila 
 
Y luego en el ícono del pdf
 
 
Y se despliega el recibo hecho o la venta. 

                                                                          
	Conclusión
En este tipo de aplicativo, el servidor sería responsable de gestionar bases de datos, procesar transacciones, manejar inventarios y controlar la lógica de negocios (como la gestión de usuarios, productos, precios, etc.). Por otro punto de vista, el cliente sería la interfaz de usuario que podría estar en una computadora, Tablet o móvil, desde la cual los usuarios (empleados o clientes) interactúan para realizar acciones como ver productos, hacer compras o gestionar inventarios.

