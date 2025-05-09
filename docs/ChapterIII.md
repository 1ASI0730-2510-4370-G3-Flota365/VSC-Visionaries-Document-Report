<h2>id="requirementsSpecification">CAPÍTULO 3: REQUIREMENTS SPECIFICATION</h2>

<h3 id="toBeScenario">3.1. To-Be Scenario Mapping</h3>

<h4 id="toBeScenario">Segmento 1: Gerentes o administradores.</h4>
    
<img src="../images/To-Be Escenario Segmento 1.jpeg" alt="To-Be map segment 1" width="auto" height="370"/>

<h4 id="toBeScenario">Segmento 2: Conductores.</h4>
    
<img src="../images/To-Be Escenario Segmento 2.jpeg" alt="To-Be map segment 2" width="auto" height="370"/>



<h3 id="userStories">3.2. User Stories</h3> 

Se presentan los siguientes user stories:

<table border="1" cellpadding="5" cellspacing="0">
  <thead>
    <tr>
      <th>Epic / Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>Relacionado con (Epic ID)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>US01</td><td>Landing Page informativa</td><td>Como gestor, quiero ver información sobre la empresa, para decidir si la plataforma es confiable.</td><td>Se muestra información clara sobre la empresa (misión, visión, servicios).

El contenido es accesible sin necesidad de iniciar sesión.

El diseño debe transmitir confianza (uso de imágenes, testimonios, logos de clientes).

Al hacer scroll, el usuario encuentra secciones bien diferenciadas.</td><td>1</td></tr>
<tr><td>US02</td><td>Responsive</td><td>Como gestor o conductor, quiero que la página sea responsive, para usarla cómodamente desde cualquier dispositivo.</td><td>El sitio se adapta correctamente a resoluciones móviles, tabletas y escritorio.

No hay necesidad de desplazamiento horizontal en dispositivos móviles.

Elementos clave (menú, botones, textos) se redistribuyen correctamente por pantalla.

Las pruebas de dispositivos simulados (Chrome DevTools o similares) pasan sin errores visuales.</td><td>1</td></tr>
<tr><td>US03</td><td>Comparador de planes</td><td>Como gestor, deseo comparar los planes disponibles, para elegir el más adecuado para mi empresa.</td><td>El usuario puede ver al menos 2 o más planes comparados en una tabla o tarjeta.

Cada plan incluye detalles de precio, beneficios y condiciones.

Existe una acción visual clara para seleccionar o contratar un plan.

Si un plan no está disponible, se muestra una indicación (ej. desactivado).</td><td>1</td></tr>
<tr><td>US04</td><td>switcher idiomas</td><td>Como gestor o conductor, quiero poder cambiar el idioma entre español e inglés, para entender el contenido fácilmente.</td><td>1.Existe un botón o selector visible para cambiar entre español e inglés.

2.Todo el contenido de texto cambia de idioma al instante.

3. El idioma seleccionado se conserva al navegar entre páginas.

4.El idioma por    
defecto es español si no hay selección previa.</td><td>1</td></tr>
<tr><td>US05</td><td>tema de colores</td><td>Como gestor o conductor, deseo cambiar el tema de colores, para personalizar la interfaz a mi gusto.</td><td>El usuario puede elegir entre al menos dos temas (ej. claro y oscuro).

Al cambiar de tema, los colores se aplican automáticamente a la interfaz.

La selección de tema se guarda en el navegador (localStorage o similar).

Todos los elementos del sitio respetan el tema seleccionado (no quedan elementos con color incorrecto).</td><td>1</td></tr>
<tr><td>US06</td><td>vista de developers</td><td>Como gestor, quiero saber quiénes son los desarrolladores, para tener mayor confianza en la plataforma.</td><td>1.
Existe una sección accesible desde la landing page con información del equipo.

2.
Se muestran nombres, roles y fotos (opcional) de los desarrolladores.

3.
La sección tiene diseño consistente con el resto del sitio.</td><td>1</td></tr>
<tr><td>US07</td><td>Registro de nuevo usuario</td><td>Como gestor, quiero registrarme en la plataforma, para probar las funcionalidades y evaluar su utilidad.</td><td>1.
El formulario solicita :,nombre o email, contraseña.

2.
Se validan los campos requeridos y el formato del email.


3.
Al registrarse exitosamente, el usuario recibe una confirmación visual.

4.
No se permite registrar con un correo ya existente.</td><td>2</td></tr>
<tr><td>US08</td><td>alerta de cerrar
sesión</td><td>Como gestor o conductor, deseo recibir una alerta al cerrar sesión, para asegurarse de cerrar correctamente y evitar accesos no deseados.</td><td>Antes de cerrar sesión, se muestra una alerta de confirmación (modal o toast).

Si el usuario confirma, se cierra la sesión y redirige a la landing page.

Si cancela, permanece en la misma vista sin cambios.

La sesión se invalida correctamente en backend (no puede volver atrás con el navegador).</td><td>2</td></tr>
<tr><td>US09</td><td>Registro de vehiculo</td><td>Como gestor  quiero registrar los vehículos para 
saber cuántos hay.</td><td>Se puede registrar placa, marca, modelo y tipo de vehículo.

El sistema valida que la placa no esté duplicada.

El nuevo vehículo aparece en el listado automáticamente.

Se muestra un mensaje confirmando el registro exitoso</td><td>3</td></tr>
<tr><td>US10</td><td>Delegar de vehiculo</td><td>Como gestor quiero delegar un vehiculo a un conductor para que él pueda usarlo</td><td>El gestor puede seleccionar un conductor y un vehículo.

El sistema registra la asignación correctamente.

Si el vehículo ya está asignado, se muestra una advertencia.

El conductor puede ver su vehículo asignado.</td><td>3</td></tr>
<tr><td>US11</td><td>Footer informativo</td><td>Como gestor, quiero ver un footer con información útil, para conocer términos, contactos y redes sociales.</td><td>El footer incluye enlaces a contacto, términos y redes sociales.

Los enlaces funcionan correctamente.

El diseño del footer es coherente con el sitio.

Es visible en todas las páginas.</td><td>1</td></tr>
<tr><td>US12</td><td>Información conductor</td><td>Como conductor quiero ver mis datos personales para saber que están correctos</td><td>Se muestran nombre, DNI, correo y teléfono del conductor.

El conductor puede revisar sus datos desde su perfil.

Si hay errores, puede solicitar corrección.

El diseño es claro y organizado.</td><td>5</td></tr>
<tr><td>US13</td><td>Reportar incidencia</td><td>Como conductor, quiero reportar un incidente durante el uso del vehículo, para notificar al gestor de cualquier problema.</td><td>El conductor puede registrar tipo de incidencia y descripción.

Se puede adjuntar foto si es necesario.

El sistema notifica al gestor inmediatamente.

La incidencia queda guardada con fecha y hora.</td><td>4</td></tr>
<tr><td>US14</td><td>Informacion del vehiculo</td><td>Como conductor, quiero consultar el estado técnico del vehículo antes de usarlo, para asegurarme de que está en condiciones.</td><td>Se muestra el estado técnico del vehículo.

Si hay una falla pendiente, se indica claramente.

El conductor accede a esta info antes del servicio.

El estado se actualiza desde mantenimiento.

</td><td>3</td></tr>
<tr><td>US15</td><td>Registro de combustible</td><td>Como conductor, quiero registrar el combustible cargado al vehículo, para llevar control del consumo.</td><td>
    El conductor puede registrar el tipo y cantidad de combustible cargado.

Se permite subir una foto del ticket o del odómetro.

El sistema guarda el registro con fecha, hora y vehículo.

El gestor puede revisar los registros en un historial de consumo.</td><td>5</td></tr>
<tr><td>US16</td><td>Registro de pausas</td><td>Como conductor, quiero registrar descansos o pausas durante el servicio, para que queden reflejados en la asignación.</td><td>El conductor indica inicio y fin de cada pausa.

La duración se calcula automáticamente.

Las pausas se reflejan en el reporte del servicio.

El gestor puede ver todas las pausas registradas.</td><td>5</td></tr>
<tr><td>US17</td><td>Confirmación de evidencia</td><td>Como conductor, quiero recibir una confirmación cuando se registra mi evidencia de uso, para asegurarme de que fue enviada correctamente.</td><td>El conductor recibe una notificación tras enviar la evidencia de uso.

La evidencia incluye  hora y contenido.

Si hay error en el envío, el sistema lo notifica .

La confirmación queda registrada en el historial del viaje.</td><td>4</td></tr>
<tr><td>US18</td><td>Ver que vehículos están en uso</td><td>Como gestor de flota, quiero ver qué vehículos están en uso, para tomar decisiones rápidamente.</td><td>Se muestra una lista de vehículos activos.

Se indica quién los está usando y desde cuándo.

Se puede filtrar por sede, tipo o conductor.

Vehículos libres aparecen con estado “Disponible”.</td><td>3</td></tr>
<tr><td>US19</td><td>Resolver incidencias</td><td>Como gestor de flota, quiero saber  si hay incidencias , para resolverlas lo mas rápido que se pueda.</td><td>El gestor puede ver todas las incidencias registradas.

Se muestra su estado (pendiente, resuelta).

Puede asignar un técnico responsable</td><td>4</td></tr>
<tr><td>US20</td><td>Asignar mantenimiento</td><td>Como gestor de flota, quiero asignar mantenimiento preventivo  para evitar fallas futuras.</td><td>El gestor puede programar mantenimientos preventivos.

Se define fecha, vehículo y tipo de servicio.

El sistema notifica al conductor asignado.

El mantenimiento queda registrado en el historial.</td><td>4</td></tr>
<tr><td>US21</td><td>Asignar técnico</td><td>Como gestor de flota, quiero asignar técnicos a órdenes de mantenimiento , para asegurar que las tareas se realicen a tiempo.</td><td>El gestor puede elegir un técnico disponible.

Se asigna a una orden de mantenimiento específica.

El técnico recibe una notificación.

</td><td>4</td></tr>
<tr><td>US22</td><td>Cambio de contraseña</td><td>Como conductor o gestor , quiero cambiar mi contraseña, para mantener mi cuenta segura.</td><td>El usuario puede cambiar su contraseña desde el perfil.

El sistema valida la contraseña actual antes de cambiarla.

Se muestra confirmación del cambio exitoso.

No se permite usar la misma contraseña anterior.</td><td>2</td></tr>
<tr><td>US23</td><td>Estadísticas personales del conductor</td><td>Como conductor, quiero ver mis estadísticas de rendimiento, para mejorar mi desempeño.</td><td>El conductor puede ver sus viajes completados y rendimiento.


Puede filtrar por semana, mes o año.

El gestor también puede ver este reporte.</td><td>5</td></tr>
<tr><td>US24</td><td>Cambiar foto de perfil</td><td>Como conductor o gestor, quiero cambiar mi foto de perfil, para personalizar mi cuenta.</td><td>1. Elegir foto.<br>2. Solo formatos JPG, PNG.<br>3. Visible para el gestor y conductor.</td><td>2</td></tr>
<tr><td>US25</td><td>Solicitud de cambio de turno</td><td>Como conductor, quiero solicitar un cambio de turno, para organizar mejor mi jornada.</td><td>1. Solicitud vía formulario.<br>2. El gestor puede aceptar o rechazar.<br>3. Se guarda en historial de solicitudes.</td><td>5</td></tr>
<tr><td>US26</td><td>Visualización de vehículo asignado</td><td>Como conductor, quiero ver claramente cuál es mi vehículo asignado del día, para evitar confusiones.</td><td>Al iniciar sesión, el conductor ve el vehículo asignado del día.

Se muestran placa, tipo y horario asignado.

Si no hay asignación, el sistema lo indica claramente.

El diseño es accesible desde el inicio.

</td><td>5</td></tr>
<tr><td>US27</td><td>Visualización de rutas completadas vs planificadas</td><td>Como gestor, quiero ver cuántas rutas fueron completadas frente a las planificadas, para evaluar cumplimiento.</td><td>El gestor puede ver rutas planificadas frente a las realizadas.

Se muestran porcentajes de cumplimiento diario o semanal.

Puede filtrar por conductor, zona o fecha.</td><td>6</td></tr>

  </tbody>
</table>

<h3 id="impactMapping">3.3. Impact Mapping</h3>

<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>Meta (Goal)</th>
      <th>Actor</th>
      <th>Impacto esperado</th>
      <th>User Stories (Entregables)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Mejorar la experiencia de navegación y conversión</td>
      <td>Visitante / Gestor</td>
      <td>Comprender el valor de la plataforma y navegar desde cualquier dispositivo</td>
      <td>US01, US02, US03, US04, US05, US06, US11</td>
    </tr>
    <tr>
      <td>Facilitar el acceso a la plataforma</td>
      <td>Gestor / Conductor</td>
      <td>Registrarse, personalizar y proteger su cuenta</td>
      <td>US07, US08, US22, US24</td>
    </tr>
    <tr>
      <td>Control y delegación eficiente de vehículos</td>
      <td>Gestor</td>
      <td>Registrar vehículos, asignarlos y supervisar su estado</td>
      <td>US09, US10, US14, US18, US20, US21</td>
    </tr>
    <tr>
      <td>Gestión de incidencias en flota</td>
      <td>Gestor</td>
      <td>Detectar y atender incidencias, realizar mantenimiento preventivo</td>
      <td>US13, US17, US19, US20, US21</td>
    </tr>
    <tr>
      <td>Autonomía y eficiencia operativa del conductor</td>
      <td>Conductor</td>
      <td>Consultar información, registrar acciones y ver su desempeño</td>
      <td>US12, US15, US16, US23, US25, US26</td>
    </tr>
    <tr>
      <td>Control logístico del desempeño</td>
      <td>Gestor</td>
      <td>Evaluar cumplimiento de rutas y eficiencia logística</td>
      <td>US27</td>
    </tr>
  </tbody>
</table>


<h3 id="productBacklog">3.4. Product Backlog</h3>


<table border="1" cellpadding="5" cellspacing="0">
  <thead>
    <tr>
      <th>#Orden</th>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Story Points</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>US11</td><td>Landing Page informativa</td><td>Como visitante, deseo ver una página informativa sobre Flota365, para conocer sus beneficios.</td><td>2</td></tr>
    <tr><td>2</td><td>US12</td><td>Comparador de planes</td><td>Como visitante, deseo comparar los planes disponibles, para elegir el que se ajuste a mi empresa.</td><td>3</td></tr>
    <tr><td>3</td><td>US13</td><td>Registro de nuevo usuario</td><td>Como visitante, deseo registrarme para acceder al panel de pruebas, para evaluar la plataforma.</td><td>3</td></tr>
    <tr><td>4</td><td>US01</td><td>Asignación de rutas</td><td>Como gestor, deseo asignar rutas a los conductores desde la plataforma, para optimizar la logística diaria.</td><td>3</td></tr>
    <tr><td>5</td><td>US02</td><td>Consulta de disponibilidad</td><td>Como gestor, deseo ver el estado de pedidos y unidades, para planificar correctamente.</td><td>2</td></tr>
    <tr><td>6</td><td>US14</td><td>Creación de servicio logístico</td><td>Como gestor, deseo crear un servicio con ruta, unidad y chofer, para organizar una entrega.</td><td>3</td></tr>
    <tr><td>7</td><td>US07</td><td>Revisión de entregas del día</td><td>Como conductor, deseo revisar mis entregas asignadas al inicio del día, para organizar mi recorrido.</td><td>2</td></tr>
    <tr><td>8</td><td>US05</td><td>Reporte de fallas</td><td>Como conductor, deseo reportar fallas técnicas desde la app, para recibir soporte inmediato.</td><td>3</td></tr>
    <tr><td>9</td><td>US10</td><td>Control de checklist vehicular</td><td>Como conductor, deseo verificar el estado del vehículo antes de iniciar el servicio, para operar con seguridad.</td><td>3</td></tr>
    <tr><td>10</td><td>US06</td><td>Registro de consumo de combustible</td><td>Como conductor, deseo registrar el consumo con foto del odómetro, para controlar gastos.</td><td>3</td></tr>
    <tr><td>11</td><td>US15</td><td>Visualización de historial</td><td>Como gestor, deseo consultar el historial de servicios pasados, para analizar el desempeño.</td><td>3</td></tr>
    <tr><td>12</td><td>US08</td><td>Dashboard de indicadores</td><td>Como administrador, deseo ver KPIs de eficiencia y cumplimiento, para tomar decisiones.</td><td>5</td></tr>
    <tr><td>13</td><td>US16</td><td>Exportación de reportes PDF</td><td>Como gestor, deseo exportar reportes en PDF, para compartirlos con otras áreas.</td><td>3</td></tr>
    <tr><td>14</td><td>US03</td><td>Geolocalización en tiempo real</td><td>Como gestor, deseo visualizar en tiempo real la ubicación de cada unidad, para detectar desviaciones.</td><td>5</td></tr>
    <tr><td>15</td><td>US04</td><td>Carga de evidencia de entrega</td><td>Como conductor, deseo registrar fotos y kilometraje, para dejar constancia de las entregas.</td><td>3</td></tr>
    <tr><td>16</td><td>US09</td><td>Notificaciones por incidencia</td><td>Como gestor, deseo recibir notificaciones de incidencias, para tomar acciones rápidas.</td><td>2</td></tr>
    <tr><td>17</td><td>US17</td><td>Creación de perfiles de usuario</td><td>Como administrador, deseo crear perfiles con permisos, para controlar el acceso a funcionalidades.</td><td>3</td></tr>
    <tr><td>18</td><td>US18</td><td>API para consulta de servicios</td><td>Como developer, deseo exponer un endpoint para consultar servicios, para integrarlo con sistemas externos.</td><td>5</td></tr>
    <tr><td>19</td><td>US19</td><td>API para registrar evidencia</td><td>Como developer, deseo un endpoint para registrar evidencia, para integrarla desde apps externas.</td><td>5</td></tr>
    <tr><td>20</td><td>US20</td><td>API para incidencias</td><td>Como developer, deseo exponer un endpoint para recibir incidencias, para automatizar su gestión.</td><td>5</td></tr>
  </tbody>
</table>
