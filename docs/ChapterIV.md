<h2 id="productDesign">CAPÍTULO 4: PRODUCT DESIGN</h2>

<h3 id="styleGuidelines">4.1. Style Guidelines</h3>

<h4 id="generalStyleGuidelines">4.1.1. General Style Guidelines</h4>
<p>
  El diseño visual de la aplicación FLOTA365 sigue una estética moderna y minimalista, en coherencia con la identidad de VSC-Visionaries, apoyándose en los siguientes principios y elementos de diseño:
</p>

<h5>Branding</h5>
<p>
  Se adopta un sistema de diseño inspirado en Material Design con adaptaciones específicas para la identidad de VSC-Visionaries.<br>
  El logotipo se presenta consistentemente en todas las secciones, manteniendo una altura de 100px en el header.<br>
  La imagen de marca proyecta profesionalismo, eficiencia y tecnología, valores fundamentales para una solución de gestión de flotas.<br>
  Las formas utilizadas son limpias y geométricas, con predominio de líneas rectas y ángulos suaves que transmiten confiabilidad y orden.
</p>

<h5>Typography</h5>
<p>
  La tipografía principal es <b>Arial</b>, seleccionada por su excelente legibilidad en pantallas y su disponibilidad universal.<br>
  Jerarquía tipográfica clara: títulos principales a 36px, subtítulos a 24px-28px, cuerpo de texto a 16px con interlineado de 1.6.<br>
  Los pesos tipográficos varían estratégicamente: normal (400) para texto regular, semi-bold (600) para subtítulos y bold (700) para títulos y elementos destacados.<br>
  Se mantiene alto contraste entre texto y fondo para asegurar accesibilidad (ratio mínimo de 4.5:1 según WCAG 2.1 AA).
</p>

<h5>Colors</h5>
<p>
  <b>Paleta principal</b>: Fondos blancos (#fff) como base para maximizar la legibilidad, turquesa claro (#6CDAE7) como color primario de acento, gris oscuro (#333) para textos principales.<br>
  <b>Paleta secundaria</b>: Gris claro (#f9f9f9) para secciones alternas, gris medio (#ddd) para bordes y separadores, negro (#121212) para el footer y elementos contrastantes.<br>
  <b>Colores funcionales</b>: Se reserva el uso de verde (#4CAF50) para indicadores de éxito, rojo (#F44336) para errores y amarillo (#FFC107) para advertencias.<br>
  Esta combinación cromática refleja los valores de la marca: el turquesa transmite tecnología y confianza, mientras que la base clara aporta modernidad y limpieza visual.
</p>

<h5>Spacing</h5>
<p>
  Sistema de espaciado basado en unidades de 8px para mantener consistencia y ritmo visual en toda la aplicación.<br>
  Márgenes internos generosos (padding) de 60px en secciones principales y 30px para contenedores secundarios.<br>
  Separación vertical significativa entre secciones (60px) para mejorar la legibilidad y crear pausas visuales.<br>
  Espaciado entre elementos relacionados de 15-30px, manteniendo una densidad de información adecuada sin generar sobrecarga visual.
</p>

<h5>Tono de Comunicación</h5>
<p>
  <b>Equilibrio</b>: Formal pero accesible (70% formal, 30% casual) para proyectar profesionalismo sin resultar distante.<br>
  <b>Actitud</b>: Respetuoso y sereno (90%) con toques entusiastas (10%) en llamados a la acción.<br>
  <b>Lenguaje</b>: Directo y orientado a beneficios, evitando jerga técnica innecesaria.<br>
  <b>Voz</b>: Experta y confiable, posicionando FLOTA365 como solución autorizada en gestión de flotas.<br>
  Este enfoque comunicacional busca conectar con profesionales de logística y gestión de flotas que valoran la eficiencia y resultados concretos.
</p>

<p>
  El diseño responsive se implementa con breakpoints estratégicos a 768px y 992px, asegurando adaptabilidad a dispositivos móviles, tablets y escritorio sin comprometer la experiencia de usuario.
</p>
<h4 id="webStyleGuidelines">4.1.2. Web Style Guidelines</h4>
<p>
  Estructura basada en etiquetas estándar de HTML como <code>&lt;div&gt;</code>, <code>&lt;table&gt;</code>, <code>&lt;form&gt;</code>.<br>
  CSS personalizado sin frameworks.<br>
  Botones: fondo negro, borde celeste y texto blanco. En hover, fondo celeste con texto negro.<br>
  Formularios claros, inputs con fondo oscuro y texto claro, adaptados a la estética visual.<br>
  Layout basado en <code>&lt;div&gt;</code> con uso de clases para controlar el diseño visual.
</p>
<h3 id="infoArchitecture">4.2. Information Architecture</h3>

<h4 id="orgSystem">4.2.1. Organization Systems</h4>
<p>
  Se sigue una estructura jerárquica: Inicio, Características, Módulos (Tracking, Mantenimiento, Combustible, Entregas), Contacto.<br>
  Los módulos agrupan funcionalidades relacionadas en pestañas o secciones.<br>
  La arquitectura está diseñada para permitir escalabilidad futura.
</p>
<h4 id="labelSystem">4.2.2. Labeling Systems</h4>
<p>
  Las etiquetas utilizadas en la interfaz son simples, claras y orientadas a usuarios logísticos: "Pedidos", "Ubicación", "Combustible", "Conductores", etc.<br>
  Se evita el uso de términos técnicos o ambiguos. El lenguaje está pensado para ser comprendido rápidamente.<br>
  Se mantiene consistencia terminológica en menús, botones y formularios para fortalecer la experiencia de usuario.
</p>
<h4 id="seoTags">4.2.3. SEO Tags and Meta Tags</h4>
<p>
  <code>&lt;title&gt;FleetControl - Gestión Inteligente de Flotas | VSC-Visionaries&lt;/title&gt;</code><br>
  <code>&lt;meta name="description" content="Solución moderna para gestión de flotas con seguimiento en tiempo real, mantenimiento, control de entregas y consumo de combustible."&gt;</code><br>
  <code>&lt;meta name="keywords" content="gestión de flotas, logística, rastreo, mantenimiento, VSC-Visionaries"&gt;</code><br>
  Implementación de etiquetas <strong>Open Graph</strong> y <strong>Twitter Cards</strong> para correcta visualización en redes sociales.<br>
  Uso correcto de encabezados (<code>h1</code>, <code>h2</code>, <code>h3</code>) para facilitar la indexación.
</p>
<h4 id="searchSystem">4.2.4. Searching Systems</h4>
<p>
  Sistema de búsqueda implementado por palabra clave, con filtros por estado, fecha, módulo y tipo de recurso.<br>
  Se desarrollará con <b>Vue.js</b> como framework principal del frontend y <b>C#</b> en el backend, permitiendo alta integración con datos.<br>
  Se permitirá el uso de <b>JavaScript clásico</b> para funciones específicas dentro de los componentes o formularios.<br>
  Se proyecta la incorporación de autocompletado y sugerencias dinámicas.<br>
  La búsqueda estará optimizada para resultados rápidos y relevantes, dentro de un entorno de interfaz oscura.
</p>
<h4 id="navigationSystem">4.2.5. Navigation System</h4>

<h3 id="landingDesign">4.3. Landing Page UI Design</h3>

<h4 id="landingWireframe">4.3.1. Landing Page Wireframe</h4>

<h4 id="landingMockUp">4.3.2. Landing Page Mock-up</h4>

<h3 id="webAppDesign">4.4. Web Applications UX/UI Design</h3>

<h4 id="webAppWireframes">4.4.1. Web Applications Wireframes</h4>

<h4 id="webAppUserFlow">4.4.4. Web Applications User Flow Diagrams</h4>

<h3 id="webAppPrototyping">4.5. Web Applications Prototyping</h3>

<h3 id="DDD">4.6. Domain-Driven Software Architecture</h3>

<h4 id="contextDiagram">4.6.1. Software Architecture Context Diagrams</h4>

<h4 id="containerDiagram">4.6.2. Software Architecture Container Diagrams</h4>

<h4 id="componentDiagram">4.6.3. Software Architecture Components Diagrams</h4>

<h3 id="softwareObjectOrientedDesign">4.7. Software Object-Oriented Design</h3>

<h4 id="classDiagram">4.7.1. Class Diagrams</h4>

<h4 id="classDictionary">4.7.2. Class Dictionary</h4>
Para una mejor comprensión acerca del propósito de creación que cada una de las clases con sus 
respectivas propiedades, se detallará en esta sección cada uno de ellos:

<br>

<h3 id="dbDesign">4.8. Database Design</h3>

<h4 id="dbDiagram">4.8.1. Database Diagram</h4>
