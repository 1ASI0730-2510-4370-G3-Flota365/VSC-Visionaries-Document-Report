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
  FLOTA365 implementa un conjunto de estándares visuales y de interacción cuidadosamente definidos para sus interfaces web responsive:
</p>

<h5>Estructura y Layout</h5>
<p>
  La aplicación utiliza un sistema de layout basado en contenedores flexibles (<code>&lt;div&gt;</code> con display: flex) que proporciona consistencia visual y adaptabilidad.<br>
  Se emplea una estructura semántica de etiquetas HTML5 como <code>&lt;header&gt;</code>, <code>&lt;section&gt;</code>, <code>&lt;footer&gt;</code> y <code>&lt;nav&gt;</code> para mejorar SEO y accesibilidad.<br>
  Se mantiene una distribución con container de ancho máximo (1200px) con márgenes automáticos para centrado en pantallas grandes.<br>
  Grid system personalizado con divisiones en 12 columnas para layouts complejos, implementado con CSS Grid y Flexbox.
</p>

<h5>Componentes UI</h5>
<p>
  <b>Botones:</b> Dos variantes principales, siguiendo patrones de interacción consistentes:<br>
  &nbsp;&nbsp;• Botón primario: Fondo turquesa (#6CDAE7), sin borde, texto contrastante negro (#121212), padding 8px 16px, border-radius 4px.<br>
  &nbsp;&nbsp;• Botón secundario (outline): Transparente con borde turquesa (#6CDAE7), texto turquesa, mismo padding y border-radius.<br>
  &nbsp;&nbsp;• Estados hover: Cambio sutil de opacidad (0.9) para mostrar interactividad sin romper cohesión visual.<br>
  
  <b>Formularios:</b> Campos con diseño consistente para mejorar usabilidad:<br>
  &nbsp;&nbsp;• Inputs: Alto de 40px, border-radius 4px, borde #ddd, padding lateral 12px.<br>
  &nbsp;&nbsp;• Labels: Posicionados arriba del campo, margen inferior 8px, tamaño 14px.<br>
  &nbsp;&nbsp;• Validación: Feedback visual inmediato con bordes color #F44336 (error) y mensajes descriptivos.<br>
  &nbsp;&nbsp;• Estados focus: Borde turquesa (#6CDAE7) para indicar campo activo, con transición suave de 0.3s.<br>
  
  <b>Cards:</b> Contenedores para información relacionada:<br>
  &nbsp;&nbsp;• Fondo blanco con sombra sutil (0 2px 8px rgba(0,0,0,0.1)).<br>
  &nbsp;&nbsp;• Padding interno consistente de 20px.<br>
  &nbsp;&nbsp;• Border-radius 8px para consistencia con otros elementos.<br>
  
  <b>Tablas:</b> Estructuras para visualización de datos:<br>
  &nbsp;&nbsp;• Encabezados con fondo #f9f9f9 y texto en negrita.<br>
  &nbsp;&nbsp;• Bordes horizontales finos (#eee) entre filas.<br>
  &nbsp;&nbsp;• Hover en filas con cambio sutil de fondo para mejorar seguimiento visual.<br>
  &nbsp;&nbsp;• Versión responsive con scroll horizontal en móviles.
</p>

<h5>Navegación y Patrones de Interacción</h5>
<p>
  <b>Menú principal:</b> Horizontal en desktop, hamburguesa en móvil (breakpoint 768px).<br>
  <b>Estados activos:</b> Indicadores visuales sutiles (subrayado turquesa) para ubicación actual.<br>
  <b>Dropdowns:</b> Desplegables con animación suave (0.3s) y sombra para profundidad visual.<br>
  <b>Feedback de interacción:</b> Todos los elementos interactivos tienen hover states identificables y transiciones de 0.2-0.3s.<br>
  <b>Scroll:</b> Suave y sin interferencias, con elementos de "volver arriba" en páginas largas.
</p>

<h5>Responsive Behavior</h5>
<p>
  <b>Enfoque Mobile-first:</b> CSS base para móviles con media queries para pantallas más grandes.<br>
  <b>Breakpoints estratégicos:</b><br>
  &nbsp;&nbsp;• Mobile: Base hasta 767px - Layout de una columna, menú hamburguesa, elementos apilados.<br>
  &nbsp;&nbsp;• Tablet: 768px a 991px - Dos columnas en secciones clave, menú condensado.<br>
  &nbsp;&nbsp;• Desktop: 992px en adelante - Layout completo, menú horizontal expandido.<br>
  <b>Imágenes:</b> Optimizadas con atributos srcset para diferentes densidades de píxeles.<br>
  <b>Touch targets:</b> Mínimo 44px×44px para áreas táctiles en interfaces móviles siguiendo directrices WCAG.
</p>

<h5>Micro-interacciones y Animaciones</h5>
<p>
  Transiciones CSS sutiles para elementos interactivos con duración de 200-300ms para balance entre respuesta y suavidad.<br>
  Animaciones de carga (loading states) para procesos que demandan tiempo, implementados con CSS o SVG simples.<br>
  Efectos de hover sutiles para elementos interactivos: escala (1.02-1.05), opacidad o cambios de color.<br>
  Feedback visual para acciones completadas (success, error, etc.) mediante iconos y mensajes temporales.
</p>

<p>
  Todo el CSS está organizado modularmente con nomenclatura descriptiva de clases, evitando el uso de !important y minimizando la especificidad para facilitar mantenimiento y escalabilidad.
</p>

<h3 id="infoArchitecture">4.2. Information Architecture</h3>

<h4 id="orgSystem">4.2.1. Organization Systems</h4>
<p>
  FLOTA365 implementa sistemas de organización cuidadosamente seleccionados para diferentes contextos de la plataforma:
</p>

<h5>Organización Jerárquica (Visual Hierarchy)</h5>
<p>
  Se aplica en la estructura general del sitio y aplicación, estableciendo niveles claros de importancia:<br>
  • Nivel 1: Navegación principal (Home, About, Features, Pricing, Contact) - Siempre visible en el header.<br>
  • Nivel 2: Categorías de funcionalidades en la sección Features (Mantenimiento, Combustible, Documentos, etc.).<br>
  • Nivel 3: Elementos específicos dentro de cada módulo funcional.<br>
  Esta jerarquía se refuerza visualmente mediante tamaños tipográficos, colores y espaciado para crear un recorrido visual intuitivo.
</p>

<h5>Organización Secuencial (Step-by-Step)</h5>
<p>
  Implementada en procesos que requieren completar varios pasos en orden específico:<br>
  • Proceso de registro y onboarding de nuevos usuarios.<br>
  • Configuración inicial de la flota de vehículos.<br>
  • Wizards para creación de reportes personalizados.<br>
  • Procedimientos de mantenimiento preventivo.<br>
  Cada secuencia presenta indicadores visuales del progreso actual y pasos restantes.
</p>

<h5>Organización Matricial</h5>
<p>
  Utilizada en las vistas de dashboard y reportes, donde:<br>
  • El eje vertical representa categorías de datos (vehículos, conductores, rutas).<br>
  • El eje horizontal representa dimensiones temporales o métricas comparativas.<br>
  • La intersección permite análisis multidimensional de la información.<br>
  Esta organización facilita el descubrimiento de patrones y correlaciones en grandes volúmenes de datos.
</p>

<h5>Esquemas de Categorización</h5>
<p>
  <b>Categorización Alfabética:</b> Aplicada en listados de recursos numerosos como:<br>
  • Directorios de conductores.<br>
  • Catálogos de repuestos y servicios.<br>
  • Listados de proveedores.<br>
  
  <b>Categorización Cronológica:</b> Implementada en:<br>
  • Historial de mantenimientos realizados.<br>
  • Registro de recargas de combustible.<br>
  • Timelines de actividad de vehículos.<br>
  • Calendarios de servicios programados.<br>
  
  <b>Categorización por Tópicos:</b> Utilizada en:<br>
  • Agrupación de funcionalidades por módulos temáticos (Tracking, Mantenimiento, Combustible, etc.).<br>
  • Organización de la documentación de ayuda.<br>
  • Clasificación de reportes y analíticas.<br>
  
  <b>Categorización por Audiencia:</b> Implementada para personalizar vistas según roles:<br>
  • Administradores: Acceso completo con enfoque en KPIs y administración global.<br>
  • Gestores de flota: Enfoque en planificación y optimización de recursos.<br>
  • Mecánicos: Acceso prioritario a información técnica y calendarios de mantenimiento.<br>
  • Conductores: Vista simplificada orientada a rutas, checklists y reportes diarios.
</p>

<p>
  Esta combinación de sistemas organizativos permite a usuarios con diferentes necesidades navegar eficientemente por la plataforma, encontrando rápidamente la información relevante para sus tareas específicas.
</p>
<h4 id="labelSystem">4.2.2. Labeling Systems</h4>
<p>
  El sistema de etiquetado de FLOTA365 está diseñado para maximizar la claridad y minimizar la carga cognitiva, siguiendo estos principios:
</p>

<h5>Principios de Etiquetado</h5>
<p>
  • <b>Concisión:</b> Etiquetas con máximo 1-3 palabras para facilitar escaneo visual y comprensión inmediata.<br>
  • <b>Consistencia:</b> Mismo término para el mismo concepto en toda la plataforma (ej: siempre "Vehículos", nunca alternar con "Flotilla" o "Autos").<br>
  • <b>Familiaridad:</b> Uso de terminología estándar en la industria logística y de transporte.<br>
  • <b>Claridad:</b> Evitar ambigüedades y tecnicismos innecesarios que puedan confundir a usuarios no especializados.
</p>

<h5>Categorías de Etiquetas</h5>
<p>
  <b>Etiquetas de Navegación:</b><br>
  • Menú principal: "Inicio", "Nosotros", "Características", "Precios", "Contacto".<br>
  • Navegación contextual: "Volver", "Continuar", "Ver todos", "Más detalles".<br>
  
  <b>Etiquetas para Módulos Funcionales:</b><br>
  • "Seguimiento GPS" (en lugar de "Tracking" o "Monitoreo de Posición").<br>
  • "Mantenimiento" (en lugar de "Reparaciones y Servicios").<br>
  • "Combustible" (en lugar de "Gestión de Carburante").<br>
  • "Documentos" (en lugar de "Gestión Documental").<br>
  • "Neumáticos" (directamente, en lugar de "Gestión de Neumáticos").<br>
  • "Inventario" (en lugar de "Gestión de Stock y Repuestos").<br>
  • "Viajes" (en lugar de "Programación de Desplazamientos").<br>
  
  <b>Etiquetas de Acción (Call-to-Action):</b><br>
  • "INICIAR PRUEBA" (en lugar de "Comenzar Periodo de Evaluación Gratuito").<br>
  • "ELEGIR PLAN" (en lugar de "Seleccionar Opción de Suscripción").<br>
  • "ENVIAR" (en lugar de "Procesar Formulario").<br>
  • "AÑADIR VEHÍCULO" (en lugar de "Crear Nuevo Registro de Unidad").<br>
  
  <b>Etiquetas para Datos y Métricas:</b><br>
  • "Rendimiento" (para eficiencia de combustible).<br>
  • "Próximo servicio" (para mantenimiento programado).<br>
  • "Disponibilidad" (para estado operativo).<br>
  • "Retraso" (para desviaciones en tiempos de entrega).
</p>

<h5>Asociaciones entre Etiquetas</h5>
<p>
  Se establecen relaciones semánticas claras mediante:<br>
  • Agrupación visual de etiquetas relacionadas en la interfaz.<br>
  • Uso de iconografía complementaria que refuerza el significado.<br>
  • Implementación de migas de pan (breadcrumbs) que muestran jerarquías de navegación.<br>
  • Codificación por colores para reforzar categorías (ej: mantenimiento en naranja, combustible en verde).
</p>

<p>
  Este sistema de etiquetado permite a los usuarios identificar rápidamente contenidos y funcionalidades, reduciendo la curva de aprendizaje y mejorando la eficiencia en el uso diario de la plataforma.
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
