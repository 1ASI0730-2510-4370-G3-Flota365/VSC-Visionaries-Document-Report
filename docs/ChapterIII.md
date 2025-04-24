![image](https://github.com/user-attachments/assets/f473ce03-46a3-4706-be5d-99dd6ad9ca63)<h2 id="requirementsSpecification">CAPÍTULO 3: REQUIREMENTS SPECIFICATION</h2>

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
    <tr><td>US01</td><td>Asignación de rutas</td><td>Como gestor, deseo asignar rutas a los conductores desde la plataforma, para optimizar la logística diaria.</td><td>Given que el gestor accede al sistema, When selecciona una unidad y una ruta, Then el sistema asigna la ruta al conductor correspondiente.<br>Given que una ruta está asignada, When se desea reasignar, Then el sistema permite actualizarla sin perder el historial.</td><td>EP01</td></tr>
    <tr><td>US02</td><td>Consulta de disponibilidad</td><td>Como gestor, deseo ver el estado de pedidos y unidades, para planificar correctamente.</td><td>Given que el sistema está activo, When el gestor accede a la vista de unidades, Then se muestran su estado actual y disponibilidad.<br>Given que una unidad no está disponible, When se consulta, Then el sistema indica la razón de inactividad.</td><td>EP01</td></tr>
    <tr><td>US03</td><td>Geolocalización en tiempo real</td><td>Como gestor, deseo visualizar en tiempo real la ubicación de cada unidad, para detectar desviaciones.</td><td>Given que el GPS está activo, When la unidad está en movimiento, Then su ubicación se actualiza cada 30 segundos.<br>Given que una unidad se detiene, When permanece inactiva por más de 5 minutos, Then el sistema genera una alerta.</td><td>EP02</td></tr>
    <tr><td>US04</td><td>Carga de evidencia de entrega</td><td>Como conductor, deseo registrar fotos y kilometraje, para dejar constancia de las entregas.</td><td>Given que una entrega se completa, When el conductor sube una imagen, Then esta se almacena con hora y ubicación.<br>Given que se registra el kilometraje, When se guarda, Then se asocia al servicio correspondiente.</td><td>EP03</td></tr>
    <tr><td>US05</td><td>Reporte de fallas</td><td>Como conductor, deseo reportar fallas técnicas desde la app, para recibir soporte inmediato.</td><td>Given que ocurre una falla, When se reporta desde la app, Then el sistema notifica al gestor y al soporte técnico.<br>Given que se requiere revisión, When se aprueba el ticket, Then se genera una orden de mantenimiento.</td><td>EP03</td></tr>
    <tr><td>US06</td><td>Registro de consumo de combustible</td><td>Como conductor, deseo registrar el consumo con foto del odómetro, para controlar gastos.</td><td>Given que se ingresa el tipo de combustible, When se adjunta la foto, Then se guarda la información con fecha y hora.<br>Given que el dato fue registrado, When el gestor lo revisa, Then puede exportarlo en un reporte.</td><td>EP03</td></tr>
    <tr><td>US07</td><td>Revisión de entregas del día</td><td>Como conductor, deseo revisar mis entregas asignadas al inicio del día, para organizar mi recorrido.</td><td>Given que inicia la jornada, When el conductor accede al sistema, Then se muestra el listado de entregas asignadas.<br>Given que una entrega se realiza, When el conductor la marca como completada, Then se actualiza el estado.</td><td>EP01</td></tr>
    <tr><td>US08</td><td>Dashboard de indicadores</td><td>Como administrador, deseo ver KPIs de eficiencia y cumplimiento, para tomar decisiones.</td><td>Given que se accede al dashboard, When se selecciona un rango de fechas, Then se muestran indicadores filtrados.<br>Given que se exporta el reporte, When se descarga, Then contiene datos resumidos por unidad y conductor.</td><td>EP04</td></tr>
    <tr><td>US09</td><td>Notificaciones por incidencia</td><td>Como gestor, deseo recibir notificaciones de incidencias, para tomar acciones rápidas.</td><td>Given que ocurre una incidencia, When es registrada por un conductor, Then el sistema notifica al gestor correspondiente.<br>Given que el gestor recibe la alerta, When la revisa, Then puede asignarla a un técnico.</td><td>EP02</td></tr>
    <tr><td>US10</td><td>Control de checklist vehicular</td><td>Como conductor, deseo verificar el estado del vehículo antes de iniciar el servicio, para operar con seguridad.</td><td>Given que inicia el día, When se completa el checklist, Then el sistema lo marca como validado.<br>Given que una falla es reportada en checklist, When se aprueba, Then genera una alerta al gestor.</td><td>EP03</td></tr>
    <tr><td>US11</td><td>Landing Page informativa</td><td>Como visitante, deseo ver una página informativa sobre Co-box Logistic, para conocer sus beneficios.</td><td>Given que accedo a la web, When ingreso a la sección de funcionalidades, Then puedo leer descripciones claras del sistema.<br>Given que estoy interesado, When hago clic en "Contáctanos", Then puedo enviar un mensaje al equipo comercial.</td><td>EP05</td></tr>
    <tr><td>US12</td><td>Comparador de planes</td><td>Como visitante, deseo comparar los planes disponibles, para elegir el que se ajuste a mi empresa.</td><td>Given que accedo a la sección de precios, When comparo planes, Then veo sus características y costos.<br>Given que selecciono un plan, When hago clic en "Solicitar demo", Then recibo una confirmación por correo.</td><td>EP05</td></tr>
    <tr><td>US13</td><td>Registro de nuevo usuario</td><td>Como visitante, deseo registrarme para acceder al panel de pruebas, para evaluar la plataforma.</td><td>Given que accedo al formulario, When completo los datos, Then el sistema crea una cuenta temporal.<br>Given que me registro, When inicio sesión, Then puedo acceder al entorno de prueba.</td><td>EP05</td></tr>
    <tr><td>US14</td><td>Creación de servicio logístico</td><td>Como gestor, deseo crear un servicio con ruta, unidad y chofer, para organizar una entrega.</td><td>Given que el gestor accede al panel, When completa los datos, Then el sistema genera el servicio.<br>Given que se crea el servicio, When se asigna, Then se notifica al conductor.</td><td>EP01</td></tr>
    <tr><td>US15</td><td>Visualización de historial</td><td>Como gestor, deseo consultar el historial de servicios pasados, para analizar el desempeño.</td><td>Given que ingreso a la sección de historial, When filtro por fecha, Then veo los registros con detalle.<br>Given que selecciono un servicio, When abro el detalle, Then veo conductor, ruta y consumo.</td><td>EP04</td></tr>
    <tr><td>US16</td><td>Exportación de reportes PDF</td><td>Como gestor, deseo exportar reportes en PDF, para compartirlos con otras áreas.</td><td>Given que accedo al dashboard, When selecciono exportar, Then el sistema genera el archivo PDF.<br>Given que tengo varios servicios, When filtro por unidad, Then el PDF se ajusta a la selección.</td><td>EP04</td></tr>
    <tr><td>US17</td><td>Creación de perfiles de usuario</td><td>Como administrador, deseo crear perfiles con permisos, para controlar el acceso a funcionalidades.</td><td>Given que accedo a gestión de usuarios, When asigno un rol, Then el sistema restringe funcionalidades según permisos.<br>Given que un perfil es modificado, When se actualiza, Then los cambios se aplican de inmediato.</td><td>EP04</td></tr>
    <tr><td>US18</td><td>API para consulta de servicios</td><td>Como developer, deseo exponer un endpoint para consultar servicios, para integrarlo con sistemas externos.</td><td>Given que realizo un GET a /api/servicios, When el token es válido, Then recibo el listado en formato JSON.<br>Given que uso un filtro por fecha, When lo agrego a la request, Then el sistema responde solo con datos del rango.</td><td>EP06</td></tr>
    <tr><td>US19</td><td>API para registrar evidencia</td><td>Como developer, deseo un endpoint para registrar evidencia, para integrarla desde apps externas.</td><td>Given que realizo un POST a /api/evidencia, When el cuerpo es válido, Then se almacena correctamente.<br>Given que falta un dato, When hago la request, Then recibo un error 422 con mensaje descriptivo.</td><td>EP06</td></tr>
    <tr><td>US20</td><td>API para incidencias</td><td>Como developer, deseo exponer un endpoint para recibir incidencias, para automatizar su gestión.</td><td>Given que realizo un POST a /api/incidencias, When el request contiene unidad y descripción, Then el sistema crea una entrada.<br>Given que se almacena, When se consulta por GET, Then devuelve el estado de resolución.</td><td>EP06</td></tr>
  </tbody>
</table>

<h3 id="impactMapping">3.3. Impact Mapping</h3>

<table border="1" cellpadding="5" cellspacing="0">
  <thead>
    <tr>
      <th>Business Goal (SMART)</th>
      <th>Actor / Persona</th>
      <th>Impact (Cambio de comportamiento)</th>
      <th>Deliverables (Propuesta funcional)</th>
      <th>User Stories Relacionadas</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alcanzar 600 usuarios suscritos al plan B en 8 meses.</td>
      <td>Visitante del sitio web</td>
      <td>Investiga beneficios y se registra para usar la plataforma.</td>
      <td>Landing Page informativa, comparador de planes, formulario de registro.</td>
      <td>US11, US12, US13</td>
    </tr>
    <tr>
      <td>Reducir en 20% el número de entregas fallidas por incidencias en los primeros 6 meses.</td>
      <td>Conductor</td>
      <td>Reporta incidencias y completa checklist preventivo.</td>
      <td>Módulo de reporte de fallas, checklist vehicular en app.</td>
      <td>US05, US10</td>
    </tr>
    <tr>
      <td>Disminuir en 15% el consumo mensual de combustible por unidad en 5 meses.</td>
      <td>Conductor / Gestor</td>
      <td>Registra consumo y optimiza rutas con datos históricos.</td>
      <td>Registro de combustible con foto, historial de servicios.</td>
      <td>US06, US15</td>
    </tr>
    <tr>
      <td>Aumentar la adopción del sistema por parte de gestores reemplazando Excel antes de 4 meses.</td>
      <td>Gestor logístico</td>
      <td>Planifica rutas y gestiona servicios desde el panel.</td>
      <td>Panel web de asignación de rutas, consulta de disponibilidad, creación de servicios.</td>
      <td>US01, US02, US14</td>
    </tr>
    <tr>
      <td>Mejorar la toma de decisiones con datos en tiempo real antes del tercer mes.</td>
      <td>Administrador / Gestor</td>
      <td>Consulta reportes y exporta KPIs con filtros.</td>
      <td>Dashboard de indicadores, exportación a PDF.</td>
      <td>US08, US16</td>
    </tr>
    <tr>
      <td>Permitir integraciones con sistemas externos antes del mes 6.</td>
      <td>Developer</td>
      <td>Consume y expone endpoints RESTful.</td>
      <td>Endpoints para servicios, evidencias e incidencias.</td>
      <td>US18, US19, US20</td>
    </tr>
    <tr>
      <td>Aumentar retención mensual manteniendo churn &lt;5% mediante valor funcional.</td>
      <td>Todos los usuarios</td>
      <td>Usan frecuentemente la plataforma y la recomiendan.</td>
      <td>Interfaz intuitiva, roles diferenciados, funcionalidades clave accesibles.</td>
      <td>US17, US03, US04</td>
    </tr>
  </tbody>
</table>

<h3 id="productBacklog">3.4. Product Backlog</h3>


<table border="1" cellpadding="5" cellspacing="0">
    <thead>
        <tr>
            <th>Orden</th>
            <th>User Story ID</th>
            <th>Título</th>
            <th>Descripción</th>
            <th>Story Points</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>2</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>3</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>4</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>5</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>6</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>7</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>8</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>9</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>10</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>11</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>12</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>13</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>14</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>15</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>16</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>17</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>18</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>19</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>20</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>
