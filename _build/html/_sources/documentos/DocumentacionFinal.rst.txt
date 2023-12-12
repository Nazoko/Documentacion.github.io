Documentación de Tatto Zaiko
=============================

Problema:
---------
La empresa de Tatto Zaiko tiene dos problemas, El principal es la manera de 
agendar sus citas de sus clientes o futuros clientes ya que su método de agendamiento dependiendo
de una persona que es la recepcionista que no da abasto con atender de forma presencial y por llamada
y anotando las citas en una bitácora done los datos pueden perderse o ser redundantes, esto causa que 
la empresa quede en confusión con las citas y de una mala imagen de la empresa.

El otro problema es la forma de vender los productos de la empresa ya que la única manera de dar a conocer
sus productos son de manera presencial o por Instagram donde lo promocionan.

solución Propuesta:
-------------------

Nosotros hemos propuesto la idea de crear una página web que agende las citas 
de los usuarios y crear un carrito de compras para esta misma página.

Objetivo:
---------
Nosotros Debemos hacer una página web que para los usuarios normales puedan agendar una cita y 
en caso de un problema editar o eliminar esta misma, también poder comprar productos de la empresa 
con un carrito de compras.

El administrador podrá ver las estadísticas de los tatuajes hechos y cual es el mas vendido en un periodo
 de tiempo que se determinara la empresa y crear productos nuevos para la venta, reabastecer o actualizar 
 estos mismos y eliminarlos.

Esto se lograra con los lenguajes de Python y JavaScript con sus respectivos Framework que son Django y React con Vite



Documentación Back End
========================

Moldes
-------

Los Models de Django son la conexion de Python con su respectivo Framework (Django) 
y la Base de datos que se utiliza el programa


serializer
------------
un serializer es como un traductor entre los datos de tu aplicación y formatos que puedan ser 
fáciles de enviar por la web, como JSON. Piensa en un serializer como un medio para convertir 
objetos complejos de Python


Views
------
es una función de Python o una clase que toma una solicitud web y devuelve una respuesta. 
La respuesta puede ser HTML renderizado, datos JSON para una API, o cualquier otra forma de respuesta HTTP.



Documentación Front End
========================

Agendar
--------

La funcionalidad de 'Agendar' proporciona a nuestros usuarios la posibilidad de organizar
 y solicitar citas con su tatuador de confianza. No solo te brinda la flexibilidad para programar
  nuevas citas, sino que también te permite realizar modificaciones en caso de inconvenientes o 
  cualquier circunstancia imprevista. Además, tienes la opción de eliminar citas que ya no se ajusten
   a tus planes o necesidades. Queremos asegurarnos de que tu experiencia de programación de citas sea 
   lo más conveniente y adaptable posible.


Productos
----------

La sección de 'Productos' constituye el espacio dedicado a la venta de los productos ofrecidos 
por nuestra empresa. En este apartado, el administrador tiene el control total, pudiendo agregar, 
actualizar y eliminar productos según sea necesario. Esta flexibilidad permite mantener actualizado 
y diversificado nuestro catálogo, asegurando que nuestros clientes siempre tengan acceso a una amplia 
gama de productos de calidad. Nuestra plataforma está diseñada para brindar al administrador un manejo 
eficiente y sencillo de la tienda en línea, garantizando una experiencia de compra óptima para nuestros clientes.



Cuentas
-------

La sección de 'Cuentas' alberga los perfiles de nuestros clientes y administradores. 
Dentro de este apartado, los administradores tienen la capacidad de gestionar no solo el típico C.R.U.D 
Crear, Leer, Actualizar, Eliminar de cuentas, sino también otorgar permisos especiales a otros usuarios 
según sea necesario. Mientras tanto, los usuarios normales tienen la capacidad de realizar las acciones típicas  
de C.R.U.D en sus propios perfiles, centrándose principalmente en la modificación de sus propios datos. Esta estructura  
proporciona una gestión de cuentas eficiente y personalizada, garantizando que tanto los administradores como los usuarios  
regulares tengan una experiencia fluida y segura en nuestra plataforma.



Horarios
---------
Esta sección proporciona a los usuarios una visión detallada de los horarios ocupados de los tatuadores.
 Aquí, los usuarios pueden explorar de manera visual los intervalos de tiempo en los cuales los tatuadores 
 están reservados o tienen citas programadas. Esta funcionalidad permite a los usuarios tomar decisiones informadas
  al elegir un horario disponible que se ajuste a sus preferencias y facilita la planificación de citas de manera eficiente.

Inicio
-------
La página de Inicio sirve como una presentación inicial a las diversas funcionalidades que nuestra 
plataforma web ofrece. Además de ofrecer una visión general de lo que los usuarios pueden encontrar en el sitio, 
la página de Inicio proporciona opciones clave como 'Iniciar Sesión' y 'Registrarse'. Estas funciones son puntos 
de entrada esenciales que permiten a los usuarios acceder a sus perfiles, agendar citas, explorar productos y disfrutar  
de todas las características personalizadas que nuestra plataforma tiene para ofrecer. 


Iniciar Sección
----------------
El formulario de ingreso es la puerta de acceso que te permite ingresar como usuario. Dependiendo del tipo de usuario 
que seas, tendrás acceso a un conjunto específico de secciones dentro de la plataforma. Este formulario personalizado es 
el primer paso para experimentar las funcionalidades adaptadas a tus necesidades. Ya sea que seas un cliente, un administrador 
u otro tipo de usuario, este formulario asegura una experiencia de inicio de sesión intuitiva y te dirige al área correspondiente 
de la plataforma, ofreciéndote acceso rápido y directo a las herramientas y servicios que necesitas.



Perfil
-------

En este apartado, podrás visualizar de manera integral los detalles de tu cuenta, que incluyen información personal, 
citas agendadas y productos adquiridos. Además de proporcionar un resumen detallado de tu historial en la plataforma, 
tendrás la capacidad de realizar acciones específicas, como editar o eliminar citas según tus necesidades. Este espacio 
está diseñado para brindarte un acceso fácil y completo a tu información, permitiéndote gestionar y personalizar tu experiencia 
de usuario de manera eficiente y conveniente.

Documentacion Apis:
---------------------

Las APIs que se describen a continuación están diseñadas para realizar operaciones relacionadas con usuarios,
 agendas, productos de compra y detalles de compra en un servidor local. Aquí está una descripción general de cada API:

Registro de Usuario:

Descripción: Esta API se utiliza para gestionar usuarios.
Operaciones:
RegistrarTodoUsuario: Realiza una solicitud GET para obtener información de usuario.
CrearRegistrousuario: Realiza una solicitud POST para registrar un nuevo usuario.

Agendar :

Descripción: API destinada a la gestión de agendas.
Operaciones:
MostrarTodoAgendar: Realiza una solicitud GET para obtener todas las agendas.
CrearAgendar: Realiza una solicitud POST para crear una nueva entrada en la agenda.
actualizarAgendar: Realiza una solicitud PUT para actualizar una entrada en la agenda por su ID.
EliminarAgendarPorId: Realiza una solicitud DELETE para eliminar una entrada en la agenda por su ID.

Productos de Compra:

Descripción: Esta API está relacionada con la gestión de productos de compra.
Operaciones:
MostrarTodoProductos: Realiza una solicitud GET para obtener todos los productos de compra.
ActualizarStock: Representa una URL para actualizar el stock de productos
Registro de Compra:


Descripción: API para gestionar los detalles de las compras.
Operaciones:
MostrarTodoDetalleDeCompra: Realiza una solicitud GET para obtener todos los detalles de las compras.
InsertarDetallesProducto: Representa una URL para insertar detalles de productos en el registro de compra 
.
Estas APIs están construidas utilizando Axios, una biblioteca para realizar solicitudes HTTP en JavaScript. 
Las operaciones expuestas GET, POST, PUT, DELETE permiten interactuar con los recursos en el servidor y realizar 
diversas acciones según la funcionalidad específica de cada API.