<div align="center">
    <h3>Universidad Peruana de Ciencias Aplicadas</h3>
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png"></img><br>
    <strong>Ingeniería de Software - 7mo Ciclo</strong><br>
    <strong>Desarrollo de Soluciones IOT</strong><br>
    <strong>1ASI0572</strong><br>
    <strong>Profesor: Marco Antonio León Baca</strong><br>
    <br><strong>Report</strong><br>
    <br><strong>Tavolo</strong><br>
    <!--<strong>name startup</strong>-->
</div>

<h3> Team Members: </h3>

<div align="center">

| Member                              |    Code    |
| :---------------------------------- | :--------: |
| Baldeon Fabian, Aldo Alberto        | u202122633 |
| Cama Salvatierra, Jimena Tamara     | u202210778 |
| Castillo Castillo, Jair Alexander   | u202211390 |
| La Torre Valle, Franz Jair          | u202012378 |
| Quezada Portalatino, Barbara Susana | u202211800 |

</div>

<h3 align="center">Abril, 2025</h3>

<br><br>

<div align="justify">

## Registro de Versiones del Informe

El objetivo de esta sección es resumir las modificaciones relevantes que se realizan al informe durante el ciclo de vida del proyecto. Esta sección inicia en una página nueva e incluye un cuadro con la siguiente estructura:

<table>
  <thead>
    <tr>
      <th>Versión</th>
      <th>Fecha</th>
      <th>Autor</th>
      <th>Descripción de modificación</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0.1</td>
      <td>-</td>
      <td>-</td>
      <td>-</td>
    </tr>
    
  </tbody>
</table>



## 1.3. Segmentos objetivo

## 3.1. To-Be Scenario Mapping

### ¿Qué hace el Dueño del Café?

| Phases | Registro del local | Configuración del sistema de sensores | Monitoreo del local | Análisis de datos de ocupación |
|--------|-------------------|-------------------------------------|-------------------|------------------------------|
| **Doing** | • Instala la app Tavolo.<br>• Crea su cuenta como dueño de local. | • Registra la distribución de mesas en el sistema.<br>• Conecta los sensores IoT con la aplicación. | • Entra a la sección de Monitoreo en tiempo real.<br>• Verifica el estatus de ocupación de su local. | • Revisa el resumen diario de ocupación.<br>• Consulta los momentos más concurridos de la semana. |
| **Thinking** | "Qué fácil es crear un perfil para mi café." | "El sistema de sensores se integra perfectamente con la app." | "Puedo ver exactamente qué mesas están ocupadas." | "Estos datos me ayudarán a mejorar la distribución y optimizar mi negocio." |
| **Feeling** | Satisfacción | Confianza | Tranquilidad | Entusiasmo |

### ¿Qué hace el Usuario?

| Phases | Descubrimiento de la aplicación | Registro de datos personales | Búsqueda de cafeterías | Reserva de asientos |
|--------|-------------------------------|----------------------------|------------------------|-------------------|
| **Doing** | • Descarga Tavolo desde la tienda de aplicaciones.<br>• Explora las funcionalidades principales. | • Registra sus datos en Tavolo.<br>• Configura sus cafeterias favoritas. | • Utiliza la función de búsqueda por ubicación.<br>• Revisa la disponibilidad en tiempo real. | • Selecciona una mesa disponible.<br>• Confirma la reserva para una hora específica. |
| **Thinking** | "Esta app me ayudará a no perder tiempo buscando lugares disponibles." | "El proceso de registro es rápido." | "Me encanta poder ver exactamente dónde hay espacio antes de ir." | "La reserva fue sencilla y ahora tengo mi lugar asegurado." |
| **Feeling** | Curiosidad | Comodidad | Alivio | Satisfacción |


## 3.2. User Stories
### Épicas de Tavolo

| Epic ID | Nombre |
|---------|--------|
| EPIC-LANDING-001 | Funcionalidades landing page |
| EPIC-CLIENT-002 | Funcionalidades user comensal |
| EPIC-ADMIN-003 | Funcionalidades user administrador |
| EPIC-SUPERADMIN-004 | Funcionalidades user superadmin |

### Landing Page (EPIC-LANDING-001)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US001 | Ver sección "¿Qué es Tavolo?" | Como visitante de la página, quiero entender qué es Tavolo desde la landing page para conocer su propósito y cómo puede ayudarme como comensal o administrador de cafetería. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el visitante accede a la landing page<br>Cuando hace scroll o clic en "¿Qué es Tavolo?"<br>Entonces debe mostrarse una sección que describa claramente el objetivo de la solución |
| US002 | Ver sección "Características clave" | Como visitante, quiero revisar una lista de características principales de Tavolo para evaluar si cubre mis necesidades como usuario final o administrador. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el usuario navega la landing<br>Cuando accede a la sección "Características clave"<br>Entonces debe ver un resumen de las funcionalidades más importantes del sistema |
| US003 | Ver la galería virtual | Como visitante, quiero ver una galería virtual en la landing para visualizar cómo luce Tavolo, su interfaz y los sensores en acción. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el usuario accede a la sección "Galería Virtual"<br>Cuando visualiza las imágenes o videos<br>Entonces debe ver contenido visual real o ilustrativo del sistema en uso |
| US004 | Usar el formulario de contacto | Como visitante interesado, quiero tener acceso a un formulario o medio de contacto en la landing para comunicarme con el equipo de Tavolo. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el visitante accede a "Contáctanos"<br>Cuando completa el formulario con sus datos<br>Entonces el sistema debe confirmar el envío y notificar al equipo de Tavolo |

### Usuario Comensal (EPIC-CLIENT-002)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US005 | Ver menú digital de una sede | Como comensal, quiero visualizar el menú de una sede específica para conocer los productos disponibles antes de asistir. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal accede a la app<br>Cuando selecciona una sede<br>Entonces el sistema debe mostrar el menú completo de esa sede |
| US006 | Visualizar reserva activa | Como comensal, quiero poder visualizar mi reserva activa desde la aplicación, para confirmar los detalles de mi mesa y el horario reservado antes de llegar a la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal ha iniciado sesión en la aplicación<br>Y tiene al menos una reserva activa<br>Cuando accede a la sección principal<br>Entonces debe visualizar la información de la reserva actual incluyendo horario, sede y número de mesa |
| US007 | Ver disponibilidad de mesas en tiempo real | Como comensal, quiero conocer la disponibilidad de mesas para decidir si visitar o no la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal visualiza el estado de las mesas<br>Cuando hay una actualización desde los sensores<br>Entonces el sistema debe reflejar el nuevo estado en menos de 5 segundos<br><br>**Escenario 2:**<br>Dado que todas las mesas están ocupadas<br>Cuando el comensal visualiza la disponibilidad<br>Entonces el sistema debe informar que no hay mesas disponibles actualmente |
| US008 | Reservar una mesa | Como comensal, quiero reservar una mesa para asegurarme un lugar al llegar a la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal selecciona sede, hora y estadía aproximada<br>Cuando hay mesas disponibles<br>Entonces el sistema debe permitir realizar la reserva<br><br>**Escenario 2:**<br>Dado que el comensal ya tiene una reserva activa<br>Cuando intenta crear una nueva<br>Entonces el sistema debe evitarlo e informar que ya tiene una reserva activa |
| US009 | Visualizar más sedes en un mapa | Como comensal, quiero poder ver más sedes en el mapa para poder identificar el más cercano. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal quiere ver más sedes<br>Cuando elige ver sedes<br>Entonces el sistema debe mostrar todas las sedes de la cafetería en el mapa |
| US015 | Registro de cuenta de comensal | Como visitante, quiero poder registrarme como comensal en el sistema Tavolo para poder acceder a las funcionalidades de reserva y visualización de mesas. | EPIC-CLIENT-002 | Visitante | **Escenario 1:**<br>Dado que un visitante accede a la aplicación<br>Cuando completa el formulario de registro con nombre, correo y contraseña<br>Y acepta los términos y condiciones<br>Entonces el sistema debe crear una cuenta nueva<br>Y permitir el acceso a las funcionalidades de comensal |
| US016 | Login de cuenta de comensal | Como comensal registrado, quiero poder iniciar sesión en el sistema para acceder a mis reservas y funcionalidades personalizadas. | EPIC-CLIENT-002 | Comensal registrado | **Escenario 1:**<br>Dado que un comensal registrado accede a la pantalla de login<br>Cuando ingresa sus credenciales correctas (email y contraseña)<br>Entonces el sistema debe autenticarlo<br>Y redirigirlo al dashboard principal<br><br>**Escenario 2:**<br>Dado que un usuario ingresa credenciales incorrectas<br>Cuando intenta iniciar sesión<br>Entonces el sistema debe mostrar un mensaje de error<br>Y permitir reintentar |

### Usuario Administrador (EPIC-ADMIN-003)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US010 | Agregar nuevas mesas | Como administrador de cafetería, quiero agregar mesas al sistema para gestionar mejor la ocupación. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin accede al panel de su sede<br>Cuando registra una nueva mesa<br>Entonces el sistema debe guardarla con su identificador y estado inicial |
| US011 | Visualizar reservas realizadas | Como administrador, quiero ver las reservas registradas en mi sede para planificar el servicio. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin accede a su sede<br>Cuando solicita ver las reservas<br>Entonces el sistema debe mostrar las reservas activas y pasadas con usuario, fecha y hora |
| US012 | Ver la sede asignada | Como administrador, quiero confirmar qué sede tengo asignada para asegurarme de gestionar la correcta. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin inicia sesión<br>Cuando accede a su información<br>Entonces el sistema debe mostrar la sede asociada a su cuenta |
| US013 | Eliminar mesas | Como administrador, quiero poder eliminar mesas que ya no están en uso en mi sede, para mantener el sistema actualizado y evitar asignaciones incorrectas. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el administrador ha iniciado sesión<br>Y se encuentra en la sección "Ver Mesas"<br>Cuando selecciona una mesa existente y confirma su eliminación<br>Entonces la mesa es eliminada del sistema y deja de aparecer en la lista |
| US017 | Login de administrador | Como administrador, quiero poder iniciar sesión en el sistema con mis credenciales específicas para acceder al panel de administración de mi sede. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que un administrador accede a la pantalla de login<br>Cuando ingresa sus credenciales válidas<br>Entonces el sistema debe autenticarlo<br>Y mostrar el panel de administración con las funcionalidades asociadas a su sede<br><br>**Escenario 2:**<br>Dado que un administrador ingresa credenciales incorrectas<br>Cuando intenta acceder<br>Entonces el sistema debe mostrar un mensaje de error<br>Y registrar el intento fallido por seguridad |

### Usuario Superadmin (EPIC-SUPERADMIN-004)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US014 | Acceder a todos los módulos del sistema | Como superadmin, quiero tener acceso a todas las funcionalidades del sistema para realizar pruebas, crear sedes y admins. | EPIC-SUPERADMIN-004 | Superadmin | **Escenario 1:**<br>Dado que el superadmin accede al sistema<br>Cuando desea visualizar sedes o usuarios<br>Entonces el sistema debe permitirle ver toda la información<br><br>**Escenario 2:**<br>Dado que el superadmin crea un nuevo admin o sede<br>Cuando registra los datos<br>Entonces el sistema debe almacenarlos y mostrar confirmación |
