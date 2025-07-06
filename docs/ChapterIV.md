<h2 id="productDesign">CAPÍTULO 4: PRODUCT DESIGN</h2>

<h3 id="styleGuidelines">4.1. Style Guidelines</h3>

<h4 id="generalStyleGuidelines">4.1.1. General Style Guidelines</h4>

El diseño visual de la aplicación *Flota365*, sigue una estética entre lo moderno y lo minimalista, esto porque va relacioanado a la identidad que tiene el startup **VSC-Visionaries** y el compromiso que tenemos por ofrecer soluciones de calidad hacia el sector de transportistas.

Es por esto que, este capitulo, describriremos cada uno de los detalles y estilos que estaremos utilizando al momento de desarrollar la aplicación (siguiendo los principios UX y UI).

**Branding**

El logo principal cuenta con el nombre de la aplicación, el cual viene a ser Flota365. De ahi va el propósito de lo que nosotros estaramos ofreciendo en nuestra aplicación, una ayuda a los gestores de flota. Adicional a ello, estamos incluyendo un *icon* representativo de un automovil que complementa la información visual de lo que nos referimos en nuestro propósito - resaltando la innovación, soporte y confiabilidad que ofrece dicho vehiculo solo que asociandolo que a lo que estaremos desarrollando -.

<br>

<p align="center">
  <img src="../images/Flota365-Branding.jpg" alt="Flota365-Logo" width="400px" height="auto"/>
</p>

<br>

**Typography**

La tipografía empleada será **Arial** con sus respectivas variantes como los son Regular, Bold y SemiBold. La principal razon de su elección es por su excelente legibilidad en diferentes tipos de pantallas y su disponibilidad universal en los dispositivos tecnológicos que usamos hoy en día (celulares, ordenadores, tabletas, etc)

El tamaño de letra que se utilizará para cada parte del contenido web será mediante la siguiente distribución:

1. **Títulos principales**: segmentado en el tipo de tamaño de 2.25rem (36px).
2. **Subtítulos**: segmentado entre 1.5 rem (25px) a 1.75 rem (28px).
3. **Cuerpo del texto**: segmentado en 1 rem (16px) con un interlineado de 1.6px.

Con estos detalle, se logrará un alto contrates entre el texto y el fondo, dando mayor accesbilidad en un ratio mínimo de 4.5:1 según WCAG 2.1 AA.

<br>

**Colors**

Hemos distribuido nuestra paleta de colores en 3 categorías (desde la más prioritaria hasta las complementarias).

* **Paleta principal**: Fondos blancos (#fff) como base para maximizar la legibilidad, turquesaclaro (#6CDAE7) como color primario, gris oscuro (#333) para textos principales.

<br>

<p align="center">
  <img src="../images/Primary-Color-Palette.png" alt="Primary Color Palette" width="500px" height="auto"/>
</p>

<br>

* **Paleta secundaria**: Gris claro (#f9f9f9) para secciones alternas, gris medio (#ddd) para los bordes y separadores, negro (#121212) para la sección del *footer* de nuestro landing page y para dar contraste a los elementos.

<br>

<p align="center">
  <img src="../images/Secondary-Color-Palette.png" alt="Primary Color Palette" width="500px" height="auto"/>
</p>

<br>

* **Colores funcionales**: Se reserva el uso de verde (#4CAF50) para indicadores de éxito, rojo(#F44336) para errores y amarillo (#FFC107) para advertencias. 

<br>

<p align="center">
  <img src="../images/Additional-Color-Palette.png" alt="Primary Color Palette" width="500px" height="auto"/>
</p>

<br>

Esta combinación cromática reflejará cada uno de valores que tiene la marca del cual queremos transmitir al público.

<br>

**Spacing**

El spacing mantiene:

* Spacing de 0.5 rem (8px) para mantener consistencia y ritmo visual en toda la aplicación.

* Margin interno generoso **(padding)** de 3.75 rem (60px) en secciones principales y 1.875 rem (30px) para contenedores secundarios.

* Line height entre secciones de 3.75 rem (60px) para mejorar la legibilidad y crear pausas visuales. 

* Spacing entre elementos relacionados entre 0.938 rem a 1.875 rem (15px-30px), manteniendo una densidad de información adecuadasin generar sobrecarga visual.

<br>

**Tono de Comunicación**

* **Equilibrio**: Formal pero accesible (70% formal, 30% casual) para proyectar profesionalismo sin resultar distante.

* **Actitud**: Respetuoso y sereno (90%) con toques entusiastas (10%) en llamados a la acción.

* **Lenguaje**: Directo y orientado a beneficios, evitando jerga técnica innecesaria.

* **Voz**: Experta y confiable, posicionando FLOTA365 como solución autorizada en gestión de flotas

Este enfoque comunicacional busca conectar con profesionales de logística y gestión de flotas que valoran la eficiencia y resultados concretos.

<h4 id="webStyleGuidelines">4.1.2. Web Style Guidelines</h4>

Se utilizó la tendencia web *functional minimalism* con el color blanco como predominante en el fondo en la mayoría de las secciones para así brindar una experiencia visual más limpia y consistenete de los elementos.

<br>

<p align="center">
  <img src="../images/Web-Style-Guidelines.png" alt="Web Style Guidelines" width="500px" height="auto"/>
</p>

<br>

No obstante, se emplearon ciertos iconos coloridos acordes al propósito que tiene cada una de las secciones para complementar la paleta de colores y darle un más minimalismo.

<br>

<p align="center">
  <img src="../images/Web-Style-Guidelines-2.png" alt="Web Style Guidelines including icons" width="500px" height="auto"/>
</p>

<br>

Para el caso de las versiones móviles, la sección de *feaetures* se ha reemplazado por un scroll horizontal para así garantizar una mejor experiancia para el usuario que utlicen estos tipos de dispositivos.

<h3 id="infoArchitecture">4.2. Information Architecture</h3>

<h4 id="orgSystem">4.2.1. Organization Systems</h4>

Flota365 implementa sistemas de organización cuidadosamente seleccionados para diferentes contextos de la plataforma:

**Organización Jerárquica (Visual Hierarchy)**:

<p>
  Se aplica en la estructura general del sitio y aplicación, estableciendo niveles claros de importancia:
  <br>
  • Nivel 1: Navegación principal (Home, About, Features, Pricing, Contact) - Siempre visible en el header.
  <br>
  • Nivel 2: Categorías de funcionalidades en la sección Features (Mantenimiento, Combustible, Documentos, etc.).
  <br>
  • Nivel 3: Elementos específicos dentro de cada módulo funcional.<br>
  Esta jerarquía se refuerza visualmente mediante tamaños tipográficos, colores y espaciado para crear un recorrido visual intuitivo.
</p>

**Organización Secuencial (Step-by-Step)**:

<p>
  Implementada en procesos que requieren completar varios pasos en orden específico:
  <br>
  • Proceso de registro y onboarding de nuevos usuarios.
  <br>
  • Configuración inicial de la flota de vehículos.
  <br>
  • Wizards para creación de reportes personalizados.
  <br>
  • Procedimientos de mantenimiento preventivo.
  <br>
  Cada secuencia presenta indicadores visuales del progreso actual y pasos restantes.
</p>

**Organización Matricial**:

<p>
  Utilizada en las vistas de dashboard y reportes, donde:
  <br>
  • El eje vertical representa categorías de datos (vehículos, conductores, rutas).
  <br>
  • El eje horizontal representa dimensiones temporales o métricas comparativas.
  <br>
  • La intersección permite análisis multidimensional de la información.
  <br>
  Esta organización facilita el descubrimiento de patrones y correlaciones en grandes volúmenes de datos.
</p>

**Esquemas de Categorización**:

<p>
  <b>Categorización Alfabética:</b> Aplicada en listados de recursos numerosos como:
  <br>
  • Directorios de conductores.
  <br>
  • Catálogos de repuestos y servicios.<br>
  • Listados de proveedores.<br>
  
  <b>Categorización Cronológica:</b> Implementada en:
  <br>
  • Historial de mantenimientos realizados.
  <br>
  • Registro de recargas de combustible. <br>
  • Timelines de actividad de vehículos.
  <br>
  • Calendarios de servicios programados.
  <br>
  
  <b>Categorización por Tópicos:</b> Utilizada en:
  <br>
  • Agrupación de funcionalidades por módulos temáticos (Tracking, Mantenimiento, Combustible, etc.)
  <br>
  • Organización de la documentación de ayuda.
  <br>
  • Clasificación de reportes y analíticas.
  <br>
  
  <b>Categorización por Audiencia:</b> Implementada para personalizar vistas según roles:
  <br>
  • Administradores: Acceso completo con enfoque en KPIs y administración global.
  <br>
  • Gestores de flota: Enfoque en planificación y optimización de recursos.
  <br>
  • Mecánicos: Acceso prioritario a información técnica y calendarios de mantenimiento.
  <br>
  • Conductores: Vista simplificada orientada a rutas, checklists y reportes diarios.
</p>

Esta combinación de sistemas organizativos permite a usuarios con diferentes necesidades navegar eficientemente por la plataforma, encontrando rápidamente la información relevante para sus tareas específicas.

<h4 id="labelSystem">4.2.2. Labeling Systems</h4>

El sistema de etiquetado de Flota365 está diseñado para maximizar la claridad y minimizar la carga cognitiva, siguiendo estos principios:

**Principios de Etiquetado**:

<p>
  • <b>Concisión:</b> Etiquetas con máximo 1-3 palabras para facilitar escaneo visual y comprensión inmediata. <br>
  • <b>Consistencia:</b> Mismo término para el mismo concepto en toda la plataforma (ej: siempre "Vehículos", nunca alternar con "Flotilla" o "Autos"). <br>
  • <b>Familiaridad:</b> Uso de terminología estándar en la industria logística y de transporte. <br>
  • <b>Claridad:</b> Evitar ambigüedades y tecnicismos innecesarios que puedan confundir a usuarios no especializados.
</p>

**Categorías de Etiquetas**:

<p>
  <b>Etiquetas de Navegación:</b> <br>
  • Menú principal: "Inicio", "Nosotros", "Características", "Precios", "Contacto". <br>
  • Navegación contextual: "Volver", "Continuar", "Ver todos", "Más detalles". <br>
  
  <b>Etiquetas para Módulos Funcionales:</b> <br>
  • "Seguimiento GPS" (en lugar de "Tracking" o "Monitoreo de Posición"). <br>
  • "Mantenimiento" (en lugar de "Reparaciones y Servicios"). <br>
  • "Combustible" (en lugar de "Gestión de Carburante"). <br>
  • "Documentos" (en lugar de "Gestión Documental"). <br>
  • "Neumáticos" (directamente, en lugar de "Gestión de Neumáticos"). <br>
  • "Inventario" (en lugar de "Gestión de Stock y Repuestos"). <br>
  • "Viajes" (en lugar de "Programación de Desplazamientos"). <br>
  
  <b>Etiquetas de Acción (Call-to-Action):</b><br>
  • "INICIAR PRUEBA" (en lugar de "Comenzar Periodo de Evaluación Gratuito"). <br>
  • "ELEGIR PLAN" (en lugar de "Seleccionar Opción de Suscripción"). <br>
  • "ENVIAR" (en lugar de "Procesar Formulario").<br>
  • "AÑADIR VEHÍCULO" (en lugar de "Crear Nuevo Registro de Unidad"). <br>
  
  <b>Etiquetas para Datos y Métricas:</b> <br>
  • "Rendimiento" (para eficiencia de combustible). <br>
  • "Próximo servicio" (para mantenimiento programado). <br>
  • "Disponibilidad" (para estado operativo). <br>
  • "Retraso" (para desviaciones en tiempos de entrega).
</p>

**Asociaciones entre Etiquetas**:

<p>
  Se establecen relaciones semánticas claras mediante: <br>
  • Agrupación visual de etiquetas relacionadas en la interfaz. <br>
  • Uso de iconografía complementaria que refuerza el significado. <br>
  • Implementación de migas de pan (breadcrumbs) que muestran jerarquías de navegación. <br>
  • Codificación por colores para reforzar categorías (ej: mantenimiento en naranja, combustible en verde).
</p>

<p>
  Este sistema de etiquetado permite a los usuarios identificar rápidamente contenidos y funcionalidades, reduciendo la curva de aprendizaje y mejorando la eficiencia en el uso diario de la plataforma.
</p>

<h4 id="seoTags">4.2.3. SEO Tags and Meta Tags</h4>

Flota365 implementa una estrategia SEO comprensiva para maximizar visibilidad en motores de búsqueda, diferenciada por secciones:

**Landing Page (Sitio Web Estático)**:

<p>
  <b>Tags principales:</b><br>
  <code>&lt;title&gt;Flota365 - Gestión Integral de Flotas | VSC-Visionaries&lt;/title&gt;</code><br>
  <code>&lt;meta name="description" content="Optimiza tus operaciones y reduce costos con nuestra potente solución de gestión de flotas con seguimiento en tiempo real, mantenimiento y control de combustible."&gt;</code><br>
  <code>&lt;meta name="keywords" content="gestión de flotas, software logístico, seguimiento GPS, mantenimiento de vehículos, control de combustible, VSC-Visionaries"&gt;</code><br>
  <code>&lt;meta name="author" content="VSC-Visionaries"&gt;</code><br>
  
  <b>Tags de viewport y responsividad:</b><br>
  <code>&lt;meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=5"&gt;</code><br>
  <code>&lt;meta http-equiv="X-UA-Compatible" content="IE=edge"&gt;</code><br>
</p>

**Open Graph y Social Media Tags**:

<p>
  Implementación para mejorar compartición en redes sociales:<br>
  <code>&lt;meta property="og:title" content="Flota365 - Gestión Integral de Flotas"&gt;</code><br>
  <code>&lt;meta property="og:description" content="Optimiza tus operaciones y reduce costos con nuestra potente solución de gestión de flotas."&gt;</code><br>
  <code>&lt;meta property="og:image" content="https://flota365.com/assets/img/og-cover.jpg"&gt;</code><br>
  <code>&lt;meta property="og:url" content="https://flota365.com"&gt;</code><br>
  <code>&lt;meta property="og:type" content="website"&gt;</code><br>
  <code>&lt;meta name="twitter:card" content="summary_large_image"&gt;</code><br>
</p>

**Optimización para Secciones del Landing**:

<p>
  Al tratarse de un landing page con múltiples secciones (Home, About, Features, Pricing, Contact), se optimiza mediante:<br>
  • Uso correcto de encabezados jerárquicos (h1, h2, h3) para cada sección.<br>
  • IDs semánticos en cada sección para navegación por anclas (ej: <code>id="features"</code>, <code>id="pricing"</code>).<br>
  • Atributos alt descriptivos en todas las imágenes (ej: <code>alt="Dashboard de gestión de flota con indicadores de rendimiento"</code>).<br>
  • Texto optimizado con palabras clave relevantes distribuidas naturalmente a lo largo del contenido.<br>
  • Microdata (schema.org) para servicios y productos, mejorando la representación en resultados de búsqueda:
</p>

Esta implementación SEO garantiza que el landing page sea correctamente indexado y representado en los resultados de búsqueda, maximizando la visibilidad y atrayendo tráfico cualificado a la página.

<h4 id="searchSystem">4.2.4. Searching Systems</h4>

FLOTA365 implementa sistemas de búsqueda avanzados para facilitar el acceso rápido a la información en un entorno con grandes volúmenes de datos:

**Componentes del Sistema de Búsqueda**:

<p>
  <b>Barra de Búsqueda Global:</b><br>
  • Ubicada prominentemente en el header de la aplicación, siempre accesible. <br>
  • Campo de texto con placeholder descriptivo: "Buscar vehículos, conductores, documentos..." <br>
  • Icono de lupa como identificador visual universal. <br>
  • Activación rápida mediante atajo de teclado (Ctrl+K o Cmd+K). <br>
  
  <b>Búsquedas Contextuales:</b> <br>
  • Campos de búsqueda específicos dentro de cada módulo (ej: solo conductores, solo documentos). <br>
  • Adaptados para filtrar automáticamente según el contexto actual del usuario. <br>
  
  <b>Filtros Avanzados:</b> <br>
  • Expansibles desde la barra de búsqueda principal mediante botón "Filtros". <br>
  • Interfaz de filtros con diseño de acordeón para categorías principales.
</p>

**Opciones de Filtrado por Módulo**:

<p>
  <b>Módulo de Vehículos:</b> <br>
  • Por estado: Activo, En mantenimiento, Inactivo. <br>
  • Por tipo: Camión, Furgoneta, Turismo, Maquinaria. <br>
  • Por asignación: Conductor específico, Sin asignar .<br>
  • Por ubicación: Radio geográfico, Región, Ruta específica. <br>
  
  <b>Módulo de Mantenimiento:</b> <br>
  • Por tipo: Preventivo, Correctivo, Revisión. <br>
  • Por estado: Programado, En proceso, Completado, Cancelado. <br>
  • Por período: Día actual, Semana, Mes, Personalizado. <br>
  • Por responsable: Taller interno, Proveedor externo. <br>
  
  <b>Módulo de Combustible:</b> <br>
  • Por tipo: Diesel, Gasolina, Eléctrico, Gas. <br>
  • Por período de repostaje: Últimas 24h, Semana, Mes. <br>
  • Por consumo: Alto, Medio, Bajo (percentiles). <br>
  • Por proveedor: Estaciones específicas, Tarjetas de combustible.
</p>

**Funcionalidades Avanzadas**:

<p>
  <b>Autocompletado:</b><br>
  • Sugerencias dinámicas mientras el usuario escribe.<br>
  • Priorización de resultados basada en relevancia y uso frecuente.<br>
  • Corrección automática de errores tipográficos comunes.<br>
  
  <b>Búsqueda Semántica:</b><br>
  • Comprensión de consultas en lenguaje natural (ej: "camiones con mantenimiento pendiente").<br>
  • Reconocimiento de sinónimos y términos relacionados dentro del contexto logístico.<br>
  
  <b>Búsqueda por Voz:</b><br>
  • Activación mediante icono de micrófono en la barra de búsqueda.<br>
  • Procesamiento de comandos verbales simples para la navegación.
</p>

**Presentación de Resultados**:

<p>
  <b>Interfaz de Resultados:</b><br>
  • Diseño en formato de lista con elementos seleccionables.<br>
  • Cada resultado muestra información crítica (título, categoría, fecha relevante) sin sobrecarga visual.<br>
  • Paginación para conjuntos grandes de resultados (20 elementos por página).<br>
  
  <b>Agrupación y Ordenamiento:</b><br>
  • Resultados agrupados por categoría (Vehículos, Conductores, Documentos, etc.).<br>
  • Opciones para ordenar por relevancia, fecha, estado o alfabéticamente.<br>
  • Toggle para cambiar entre vista de lista y vista de tarjetas.<br>
  
  <b>Acciones Rápidas:</b><br>
  • Menú contextual en cada resultado para acciones frecuentes sin necesidad de abrir el elemento.<br>
  • Previsualización al pasar el cursor (hover) con datos adicionales relevantes.
</p>

<p>
  El sistema está implementado con Vue.js en el frontend para garantizar reactividad inmediata y experiencia fluida, mientras que el backend en C# proporciona indexación eficiente y tiempos de respuesta optimizados incluso para grandes volúmenes de datos.
</p>

<h4 id="navigationSystem">4.2.5. Navigation System</h4>

Flota365 implementa un sistema de navegación multicapa que guía intuitivamente a los usuarios a través de la plataforma:

**Navegación Global**:

<p>
  <b>Barra de Navegación Principal:</b><br>
  • Ubicada en la parte superior de todas las páginas, siempre visible.<br>
  • Contiene enlaces a secciones principales: Inicio, Nosotros, Características, Precios y Contacto.<br>
  • Incluye acceso prominente a "Iniciar Sesión" y "Registrarse" en el extremo derecho.<br>
  • En dispositivos móviles se colapsa en un menú hamburguesa con animación suave al expandirse.<br>
  
  <b>Navegación de Footer:</b><br>
  • Repite enlaces principales para acceso rápido al final de la página.<br>
  • Incluye enlaces adicionales a términos legales, política de privacidad y recursos de ayuda.<br>
  • Incorpora iconos de redes sociales y datos de contacto.
</p>

**Navegación Contextual**:

<p>
  <b>Menús Secundarios:</b><br>
  • En la sección de Características, navegación por pestañas para explorar diferentes módulos.<br>
  • Dentro de la aplicación, menú lateral izquierdo para acceder a diferentes secciones del módulo actual.<br>
  • Menús desplegables para opciones relacionadas con funciones específicas.<br>
  
  <b>Breadcrumbs:</b><br>
  • Implementados en todas las páginas internas de la aplicación.<br>
  • Muestran la ruta completa desde la página principal hasta la ubicación actual.<br>
  • Cada nivel es clickeable para facilitar la navegación hacia atrás.
</p>

**Navegación de Utilidad**:

<p>
  <b>Botones Call-to-Action:</b><br>
  • Estratégicamente ubicados para guiar al usuario hacia acciones principales (ej: "INICIAR PRUEBA GRATIS").<br>
  • Visualmente destacados con color turquesa (#6CDAE7) y tamaño prominente.<br>
  • Posicionados en puntos clave del recorrido del usuario (hero section, final de características, etc.).<br>
  
  <b>Enlaces Contextuales:</b><br>
  • Integrados en el contenido para facilitar el flujo natural entre páginas relacionadas.<br>
  • Diferenciados visualmente con subrayado o color distinto al texto normal.<br>
  
  <b>Botón "Volver Arriba":</b><br>
  • Aparece al desplazarse hacia abajo en páginas largas.<br>
  • Permite regresar al inicio de la página con un solo clic.
</p>

**Navegación de Usuario (En Aplicación)**:

<p>
  <b>Dashboard personalizado:</b><br>
  • Página inicial tras el login que presenta accesos directos a las funciones más utilizadas.<br>
  • Widgets configurables según preferencias y rol del usuario.<br>
  
  <b>Menú de Perfil:</b><br>
  • Accesible desde el avatar del usuario en la esquina superior derecha.<br>
  • Permite acceder a configuración de cuenta, preferencias y cierre de sesión.<br>
  
  <b>Navegación por Pestañas:</b><br>
  • Implementada en módulos complejos para organizar funcionalidades relacionadas.<br>
  • Permite cambiar entre vistas sin perder el contexto actual.
</p>


Esta arquitectura de navegación garantiza que los usuarios puedan moverse eficientemente por la plataforma, manteniendo siempre clara su ubicación actual y las opciones disponibles, reduciendo así la frustración y mejorando la experiencia general.

<h3 id="landingDesign">4.3. Landing Page UI Design</h3>

<h4 id="landingWireframe">4.3.1. Landing Page Wireframe</h4>

<p align="center">
<img src="../images/landing_wireframe.png" alt="Landing Page Wireframe" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">
</p>

<h4 id="landingMockUp">4.3.2. Landing Page Mock-up</h4>
<img src="../images/landing_update.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

<h3 id="webAppDesign">4.4. Web Applications UX/UI Design</h3>

<h4 id="webAppWireframes">4.4.1. Web Applications Wireframes</h4>
  
 <img src="../images/index.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/conductor.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/vehiculo.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/flota.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/Analitica.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/monitoreo.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
 <img src="../images/report.jpg" alt="Primary Color Palette" width="500px" height="auto"/>

<h4 id="webAppUserFlow">4.4.4. Web Applications User Flow Diagrams</h4>
<section>
  
  <p>
    Esta sección presenta los <strong>User Flows</strong> desarrollados para la aplicación web <strong>Flota365</strong>. Cada flujo corresponde a un objetivo específico (<strong>User Goal</strong>) identificado a partir de los perfiles de usuario definidos (<strong>User Personas</strong>).
    <br><br>
    Los diagramas ilustran tanto los <strong>"Happy Paths"</strong> (rutas ideales donde todo ocurre como se espera sin errores) como los <strong>"Unhappy Paths"</strong> (rutas alternativas donde ocurren fallos o errores del sistema). Ambos casos fueron diseñados para anticipar el comportamiento de la aplicación frente a escenarios reales de uso, y se alinean con los <strong>wireframes</strong> previamente diseñados.
  </p>

  <!-- User Persona 1 -->
  <h3>User Persona 1: Conductores de vehículos pesados</h3>

  <h4>User Goal 1: Reportar una incidencia durante el turno</h4>
  <ul>
    <li><strong>Happy Path:</strong> El conductor accede a la aplicación, ingresa al formulario de reporte, llena los campos correctamente y sube una imagen como evidencia. El sistema valida la información y envía el reporte sin inconvenientes.</li>
    <li><strong>Unhappy Path:</strong> Durante el proceso, el conductor omite algún campo obligatorio o no adjunta la imagen requerida. El sistema detecta el error y bloquea el envío hasta que se corrijan los problemas.</li>
  </ul>

  <h4>User Goal 2: Ver el estado de su vehículo asignado</h4>
  <ul>
    <li><strong>Happy Path:</strong> El conductor inicia sesión correctamente, accede a su panel principal y consulta la información del vehículo asignado, visualizando su estado actual sin inconvenientes.</li>
    <li><strong>Unhappy Path:</strong> El conductor no tiene un vehículo asignado o el sistema arroja un error al consultar los datos. En ese caso, se notifica la situación en pantalla.</li>
  </ul>

  <!-- User Persona 2 -->
  <h3>User Persona 2: Gestores de flota</h3>

  <h4>User Goal 1: Asignar un vehículo a un conductor disponible</h4>
  <ul>
    <li><strong>Happy Path:</strong> El gestor de flota accede correctamente a la aplicación, visualiza la lista de conductores disponibles y selecciona uno sin asignación previa. Luego elige un vehículo activo y no asignado, y completa exitosamente la operación de asignación.</li>
    <li><strong>Unhappy Path:</strong> El gestor intenta asignar un vehículo pero el conductor ya tiene uno asignado, el vehículo está en mantenimiento o ya fue asignado a otro conductor. En cualquiera de estos casos, el sistema emite un mensaje de error y la operación no se completa.</li>
  </ul>

  <h4>User Goal 2: Consultar reportes de incidencias enviadas por conductores</h4>
  <ul>
    <li><strong>Happy Path:</strong> El gestor inicia sesión correctamente y accede al módulo de reportes. El sistema muestra los registros de incidencias enviados por los conductores, junto con su evidencia correspondiente. El gestor puede visualizarlos sin problemas.</li>
    <li><strong>Unhappy Path:</strong> El gestor accede al módulo, pero no hay reportes disponibles en el sistema o alguno presenta errores como falta de evidencia o campos incompletos. En este caso, el sistema notifica la situación al usuario.</li>
  </ul>
</section>

<img src="../images/enlace1.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace2.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace3.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace4.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace5.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace6.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace7.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace8.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace9.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace10.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace11.png" alt="Primary Color Palette" width="500px" height="auto"/>
<img src="../images/enlace12.png" alt="Primary Color Palette" width="500px" height="auto"/>
<h3 id="webAppPrototyping">4.5. Web Applications Prototyping</h3>
Video de la aplicación web: https://drive.google.com/file/d/1_MWoiid6MOtvUOxqcHGoC-sVwGr-2juM/view?usp=sharing

<h3 id="DDD">4.6. Domain-Driven Software Architecture</h3>

<h4 id="contextDiagram">4.6.1. Software Architecture Context Diagrams</h4>

<p align="center">
  <img src="../images/Context (2).png" alt="C4 Context Diagram" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1auCN7geobg1CRTzkaGVo6XMGt1JyS0YD/view?usp=sharing">Ver Diagrama de Contexto - C4</a>
</p>

<h4 id="containerDiagram">4.6.2. Software Architecture Container Diagrams</h4>

<p align="center">
  <img src="../images/Container.png" alt="C4 Container Diagram" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1_Dvs68Z97v07_vYm85N1PQE9dCWQ7zf2/view?usp=sharing">Ver Diagrama de Contenedores - C4</a>
</p>

<h4 id="componentDiagram">4.6.3. Software Architecture Components Diagrams</h4>

**Authentication Context**:

<p align="center">
  <img src="../images/Auth.png" alt="C4 Component Diagram - Auth Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1_Cy9G3qEdmt2dCC_iFc_UmZtwCVElcU5/view?usp=sharing">Ver Diagrama de Componentes - Auth Context</a>
</p>

**Analytics Context**:

<p align="center">
  <img src="../images/Analytics.png" alt="C4 Component Diagram - Analytics Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1ELqVIEQfWePpe0PYqeErQJZmedSRPB56/view?usp=sharing">Ver Diagrama de Componentes - Analytics Context</a>
</p>

**Dashboard Context**:

<p align="center">
  <img src="../images/Dashboard.png" alt="C4 Component Diagram - Dashboard Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1uAB7ipjnfy8ErGsMytbzseolMMBqMJ6W/view?usp=sharing">Ver Diagrama de Componentes - Dashboard Context</a>
</p>

**Driver Context**:

<p align="center">
  <img src="../images/Driver.png" alt="C4 Component Diagram - Driver Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1FYCGkgbVYJObxsGfenGSZVAYWo0kcVSZ/view?usp=sharing">Ver Diagrama de Componentes - Driver Context</a>
</p>

**Fleet Context**:

<p align="center">
  <img src="../images/Fleet.png" alt="C4 Component Diagram - Fleet Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/14wNO2taqEbmpjvp3mnI5G9EmmFN0GQv6/view?usp=sharing">Ver Diagrama de Componentes - Fleet Context</a>
</p>

**Maintenance Context**:

<p align="center">
  <img src="../images/Maintenance.png" alt="C4 Component Diagram - Maintenance Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1qWWCZcmnJymR32ocphyejS0SQPCmRVsV/view?usp=sharing">Ver Diagrama de Componentes - Maintenance Context</a>
</p>

**Vehicle Context**:

<p align="center">
  <img src="../images/Vehicle.png" alt="C4 Component Diagram - Vehicle Context" style="width: 400px"/>
</p>

<p align="center">
  <a href="https://drive.google.com/file/d/1CoJWwKOyQEobL_niTVLO8VRutMjTNgBk/view?usp=sharing">Ver Diagrama de Componentes - Vehicle Context</a>
</p>

<h3 id="softwareObjectOrientedDesign">4.7. Software Object-Oriented Design</h3>

<h4 id="classDiagram">4.7.1. Class Diagrams</h4>

<img src="../images/diagrama_class.jpeg" alt="diagrama clases" style="display: block; margin: 50 auto 0 auto;"/>

<br>

* Diagrama de Clases: <a href="https://editor.plantuml.com/uml/jLbVSnet47zdXk-WuIKqjJt9wmt3v0B4kOa13s3Fz2aZxcHGVITHIKT3cdwnllQBTQNJ7U9EOEouVQWFQNUrsZ-_tLK-I8M5ohEqtPAFb6smm1dQuFWHhyXSxLA218aLPgkKk1HnYgL4VxLR2FuBbH9qcIiInPnzuamDUCe5MgOWnaCnfzy9UjTk_TrkjLjlq8Zb6H5OKSuaqj9HBZcAUVRlFwpT8h2BvWght1uN3XRH_KX_HPFzzzraE9fz7OVHP36QX9E1MPpUBRvEFtsTZsRtKR4IpkVHzMGqDD_tONGJVhmn6uFf-FPcj2XsRaUJOJIvjXeQ3Ux9ciOfMUmsf53Z9hh-lD0VdqVX_Mz6H3YxdXfsE6KqkHxDvgw4EqRLz65CiCo5bN4tYHQ5hCLefZ--H3VJwrauDbAYaTRP2B3-G1sh1Xg0aSatrK6ztaUUiuGaTgNVBvrIUAXawFL6J56rkq3XQYN82YiouzmXH-WIqIH0TtVHSB-oIO4m0FiBobRxvOmd96qkAx1Eu9fgloMD1mFhoVhwPoeL5xi0tS17pmeeIFiLxMNvzIlADmdeLH1q6VbpVY3zbm1jEKtsv71Va4l465Cm4iCi9jt4N6m8_r_GZ1om69CtJ6XZiDUxnsbEfilV8IqEpNViZl4QqeSaeTgVrzZyk2jCZzwCCGDN2mG9DD-1rjaRhrQVKaBKIzsQ41aBkj4fr_JYjhYlFFI6rmyuIUnsTrivtcF-Z6z9HLZyZQnI3UeOft6km-wMY0SkCkCje79-ZWce77lDqg0wxZ1GVujfYfSq1Gi6AE7vCYNkxie9c06Ngad3rPg8Y2KqnX30OB8ntlGAWrvOudvDpp8ZE-yxOCi-whpjr48iG9qrbcXT94MdO2lyhPduvQNBfCa1L1MeAZjrl70kS3vcE4nJaK0elZ3AQfwkuqGzxamX6XwavNwJiEJOrh6qOrmHwG4fhd3gysOji1TOFdQ1IFzj1cdAPM6Sxl40NfGdQHhth5hCwXCg6_zKwiQ-Qnqra2Bncj6OOjPmaMiAAUcABIfQOvFgL-Fs6HQFeHpmR9CIHPBkAMJTYtbfY36S-I9fGq1egfEwlhLPS-RX81aWWJSaVPPph4DbM818Qa1goNbACFD34uJtwzxJdqSRG3tIZ88u5u8mDLSyVWmGPBXJpYdpBUVGiGI7VOlF188aUKoCW2xE05cKaUCf0_8aJSrS3WhPzk3i7E4wCPkmGxPm_xAi5LRRLpNTvWAV3sGgnHh0gE7uhORZzrTNWCWcaG6EAOlJ71BLGhTPreXTmhs91A3BPOtctTMLhGfEQW1XaOCa0V3g7555CxbXwjLL4tdi2YSKjsyMaA6WMs0-ktPO-bSDynJYcKcY7MS-_hziVcPV6Qz9_6YLWYQ39d3Zfr30af_g8w6N82lJ3jTlGANCoJv4dHj_sr2ny-mSG9NHyRY2rdSwI2fB7qP3QE8mWpGwFo8SdjVk8nAZS7DTy5mROgR_EDGsgP_JGmYYtGErTWRuvwcuZdbD-p8dOakBVhKMAhOWbWHaInF2uYfuFMYvuK95BDPqgglBlfUs5bxcpgU2YmkwefxM0GvGb65_Nv40K6Z0-9ATR6HARSy6Qbp5XiUvfneTV-LBJe5tFHgj9q3N8GUyOFRtuOGW8SMJF2LxjlhySb6BmWiaREHTeCQCkHTJ0v7GcKIUFg4Xrv_FJkRfd7RIeRRZHhspvKuebMkXLcHuPyEpqpogDElLLT-L5Q1O452uSOfBNt_U20Axq07-Ft8Yw1FyXzKg28hV1zo7W3OprpWVp2pz2u4CM59FsAu8i-zVnqQSe-6EJo4I337LQDgb0Qf-d0AGYkWKYFZhz5QJ1p2fSgpyu6IiTrRYMPkKhmO5f-VjeDXeyfbnsN8zwEypUCeOjsmdA8TOhfSSY-JBRIJhXDMbRR3iKyXQzd3_x0GG-Zq3UbXf77zKX6Va3u9wD_WCUSsQ7mJxjPyKL9hS9wR-ab4yYptZ5QDWUDLMb2QJF5iISNRFkH7yWVgI_kbc5ETg3TNwkrjyFEEslgNxi7bwfjBKMj8DNvrTfOipF7qMZe-q2wU7gC8lpO6bM7Uhpg6-K7fIlgfcb3S8y8Cooj583tPSegwaq6NH1qYpXCjVsYtF0-wWU6-jqCVmbXRmzfhGCwN9lE4k297wW62fOpDg9rFcsi2ex7zV6-Z7fACQDORPo-BroIU_X8_BonzzxxNRBS_W-AD_H2KjyWDXYVdNeVy0">Ver Diagrama de Clases</a>

<h4 id="classDictionary">4.7.2. Class Dictionary</h4>

Para una mejor comprensión acerca del propósito de creación que cada una de las clases con sus 
respectivas propiedades, se detall

<h3>Documentación de Clases - Sistema de Gestión de Flotas</h3>

<h2>Clase Vehicle</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador único del vehículo</td></tr>
    <tr><td>plate</td><td>String</td><td>Número de placa</td></tr>
    <tr><td>model</td><td>String</td><td>Modelo del vehículo</td></tr>
    <tr><td>type</td><td>VehicleType</td><td>Tipo de vehículo (enumeración)</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado actual del vehículo</td></tr>
    <tr><td>statusHistory</td><td>List&lt;VehicleStatus&gt;</td><td>Historial de cambios de estado</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>updateStatus(newStatus)</td><td>void</td><td>Actualiza el estado del vehículo</td></tr>
    <tr><td>registerMaintenance(date)</td><td>void</td><td>Registra la fecha de mantenimiento</td></tr>
  </tbody>
</table>

<h2>Clase VehicleStatus (Value Object)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>status</td><td>Status</td><td>Estado del vehículo</td></tr>
    <tr><td>changedAt</td><td>DateTime</td><td>Fecha y hora del cambio de estado</td></tr>
    <tr><td>changedBy</td><td>UUID</td><td>ID del responsable del cambio (gerente o sistema)</td></tr>
  </tbody>
</table>

<h2>Clase Fleet</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador único de la flota</td></tr>
    <tr><td>description</td><td>String</td><td>Descripción de la flota</td></tr>
    <tr><td>vehicles</td><td>List&lt;Vehicle&gt;</td><td>Lista de vehículos en la flota</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>addVehicle(v)</td><td>void</td><td>Agrega un vehículo a la flota</td></tr>
    <tr><td>removeVehicle(vehicleId)</td><td>void</td><td>Remueve un vehículo de la flota por ID</td></tr>
    <tr><td>calculatePerformance()</td><td>PerformanceMetric</td><td>Calcula métricas de desempeño de la flota</td></tr>
  </tbody>
</table>

<h2>Clase PerformanceMetric (Value Object)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>availability</td><td>double</td><td>Porcentaje de disponibilidad</td></tr>
    <tr><td>avgMaintenanceCost</td><td>double</td><td>Costo promedio de mantenimiento</td></tr>
    <tr><td>otherIndicators</td><td>Map&lt;String, double&gt;</td><td>Otros indicadores</td></tr>
  </tbody>
</table>

<h2>Clase MaintenanceOrder</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador del pedido de mantenimiento</td></tr>
    <tr><td>vehicleId</td><td>UUID</td><td>Vehículo asociado al pedido</td></tr>
    <tr><td>type</td><td>String</td><td>Tipo de mantenimiento</td></tr>
    <tr><td>startDate</td><td>DateTime</td><td>Fecha inicio</td></tr>
    <tr><td>endDate</td><td>DateTime</td><td>Fecha fin</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado actual del pedido</td></tr>
    <tr><td>notes</td><td>String</td><td>Notas adicionales</td></tr>
    <tr><td>totalCost</td><td>double</td><td>Costo total</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>addTask(t)</td><td>void</td><td>Agrega una tarea de mantenimiento</td></tr>
    <tr><td>closeOrder()</td><td>void</td><td>Cierra el pedido</td></tr>
    <tr><td>calculateTotalCost()</td><td>double</td><td>Calcula el costo total del pedido</td></tr>
  </tbody>
</table>

<h2>Clase Task</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador de la tarea</td></tr>
    <tr><td>description</td><td>String</td><td>Descripción de la tarea</td></tr>
    <tr><td>cost</td><td>double</td><td>Costo de la tarea</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado de la tarea</td></tr>
    <tr><td>technicianId</td><td>UUID</td><td>Técnico asignado</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>assignTechnician(t)</td><td>void</td><td>Asigna técnico a la tarea</td></tr>
    <tr><td>markAsCompleted()</td><td>void</td><td>Marca tarea como completada</td></tr>
  </tbody>
</table>

<h2>Clase Technician</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador técnico</td></tr>
    <tr><td>name</td><td>String</td><td>Nombre</td></tr>
    <tr><td>specialty</td><td>String</td><td>Especialidad</td></tr>
    <tr><td>phone</td><td>String</td><td>Teléfono</td></tr>
    <tr><td>email</td><td>String</td><td>Correo electrónico</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado actual</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>isAvailable()</td><td>boolean</td><td>Indica si está disponible</td></tr>
  </tbody>
</table>

<h2>Clase Part</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador de pieza</td></tr>
    <tr><td>name</td><td>String</td><td>Nombre de la pieza</td></tr>
    <tr><td>type</td><td>String</td><td>Tipo o categoría</td></tr>
    <tr><td>price</td><td>double</td><td>Precio unitario</td></tr>
    <tr><td>currentStock</td><td>int</td><td>Stock actual</td></tr>
    <tr><td>minStock</td><td>int</td><td>Stock mínimo requerido</td></tr>
    <tr><td>unit</td><td>UnitOfMeasure</td><td>Unidad de medida</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>reduceStock(amount)</td><td>void</td><td>Reduce stock en cantidad indicada</td></tr>
    <tr><td>restock(amount)</td><td>void</td><td>Aumenta stock en cantidad indicada</td></tr>
  </tbody>
</table>

<h2>Clase MaintenanceHistory</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador del registro</td></tr>
    <tr><td>orderId</td><td>UUID</td><td>Pedido relacionado</td></tr>
    <tr><td>events</td><td>List&lt;String&gt;</td><td>Eventos o notas del mantenimiento</td></tr>
    <tr><td>recordDate</td><td>DateTime</td><td>Fecha de registro</td></tr>
  </tbody>
</table>

<h2>Clase Driver</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador conductor</td></tr>
    <tr><td>name</td><td>String</td><td>Nombre</td></tr>
    <tr><td>license</td><td>License (Value Object)</td><td>Licencia</td></tr>
    <tr><td>phone</td><td>String</td><td>Teléfono</td></tr>
    <tr><td>email</td><td>String</td><td>Correo electrónico</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado actual</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>updateStatus(newStatus)</td><td>void</td><td>Actualiza estado del conductor</td></tr>
    <tr><td>checkLicenseValidity()</td><td>boolean</td><td>Verifica validez de licencia</td></tr>
  </tbody>
</table>

<h2>Clase License (Value Object)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>category</td><td>String</td><td>Categoría de licencia</td></tr>
    <tr><td>issueDate</td><td>Date</td><td>Fecha de emisión</td></tr>
    <tr><td>expiryDate</td><td>Date</td><td>Fecha de expiración</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>isValid()</td><td>boolean</td><td>Verifica si la licencia está vigente</td></tr>
  </tbody>
</table>

<h2>Clase Assignment</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador de la asignación</td></tr>
    <tr><td>vehicleId</td><td>UUID</td><td>Vehículo asignado</td></tr>
    <tr><td>driverId</td><td>UUID</td><td>Conductor asignado</td></tr>
    <tr><td>route</td><td>Route (Value Object)</td><td>Ruta asignada</td></tr>
    <tr><td>dateTime</td><td>DateTime</td><td>Fecha y hora de la asignación</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado de la asignación</td></tr>
    <tr><td>rejectionReason</td><td>String</td><td>Motivo de rechazo (si aplica)</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>startService()</td><td>void</td><td>Marca la asignación como iniciada</td></tr>
    <tr><td>completeService(evidence)</td><td>void</td><td>Completa la asignación con evidencia</td></tr>
    <tr><td>reportIncident(desc)</td><td>void</td><td>Reporta un incidente</td></tr>
  </tbody>
</table>

<h2>Clase Route (Value Object)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>origin</td><td>String</td><td>Origen de la ruta</td></tr>
    <tr><td>destination</td><td>String</td><td>Destino de la ruta</td></tr>
    <tr><td>distanceKm</td><td>double</td><td>Distancia en kilómetros</td></tr>
  </tbody>
</table>

<h2>Clase Incident</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador de incidente</td></tr>
    <tr><td>assignmentId</td><td>UUID</td><td>ID de asignación relacionada</td></tr>
    <tr><td>description</td><td>String</td><td>Descripción del incidente</td></tr>
    <tr><td>type</td><td>String</td><td>Tipo de incidente</td></tr>
    <tr><td>date</td><td>DateTime</td><td>Fecha del incidente</td></tr>
  </tbody>
</table>

<h2>Clase AssignmentService (Domain Service)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>scheduleAssignment(vehicleId, driverId, route, date)</td><td>Assignment</td><td>Programa una nueva asignación</td></tr>
    <tr><td>checkAvailability(vehicleId, driverId, date)</td><td>boolean</td><td>Verifica disponibilidad de vehículo y conductor</td></tr>
  </tbody>
</table>

<h2>Clase Report</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador del reporte</td></tr>
    <tr><td>title</td><td>String</td><td>Título del reporte</td></tr>
    <tr><td>generationDate</td><td>DateTime</td><td>Fecha de generación</td></tr>
    <tr><td>type</td><td>String</td><td>Tipo de reporte</td></tr>
    <tr><td>data</td><td>String</td><td>Contenido del reporte</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>addIndicator(i)</td><td>void</td><td>Añade un indicador al reporte</td></tr>
  </tbody>
</table>

<h2>Clase Indicator (Value Object)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>name</td><td>String</td><td>Nombre del indicador</td></tr>
    <tr><td>value</td><td>Float</td><td>Valor numérico del indicador</td></tr>
  </tbody>
</table>

<h2>Clase ReportService (Domain Service)</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>generateVehicleReport(vehicleId)</td><td>Report</td><td>Genera reporte para vehículo</td></tr>
    <tr><td>generateFleetReport(fleetId)</td><td>Report</td><td>Genera reporte para flota</td></tr>
    <tr><td>generateIncidentReport()</td><td>Report</td><td>Genera reporte de incidentes</td></tr>
    <tr><td>generateDashboardKPIs()</td><td>Report</td><td>Genera reporte de KPIs</td></tr>
  </tbody>
</table>

<h2>Clase Manager</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador del gerente</td></tr>
    <tr><td>name</td><td>String</td><td>Nombre completo</td></tr>
    <tr><td>idNumber</td><td>String</td><td>Número de identificación</td></tr>
    <tr><td>email</td><td>String</td><td>Correo electrónico</td></tr>
    <tr><td>profile</td><td>String</td><td>Perfil o rol</td></tr>
    <tr><td>status</td><td>Status</td><td>Estado actual</td></tr>
  </tbody>
</table>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Métodos</strong></caption>
  <thead>
    <tr><th>Método</th><th>Tipo de Retorno</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>authorizeAssignment()</td><td>void</td><td>Autoriza asignaciones</td></tr>
    <tr><td>manageMaintenance()</td><td>void</td><td>Gestiona mantenimiento</td></tr>
  </tbody>
</table>

<h2>Clase ManagementLog</h2>
<table border="1" cellspacing="0" cellpadding="5">
  <caption><strong>Atributos</strong></caption>
  <thead>
    <tr><th>Atributo</th><th>Tipo</th><th>Descripción</th></tr>
  </thead>
  <tbody>
    <tr><td>id</td><td>UUID</td><td>Identificador del log</td></tr>
    <tr><td>managerId</td><td>UUID</td><td>ID del gerente asociado</td></tr>
    <tr><td>action</td><td>String</td><td>Acción registrada</td></tr>
    <tr><td>date</td><td>DateTime</td><td>Fecha y hora del registro</td></tr>
  </tbody>
</table>

</body>
</html>

<h3 id="dbDesign">4.8. Database Design</h3>

<h4 id="dbDiagram">4.8.1. Database Diagram</h4>
Diagrama de base de datos:

<p align="center">
<img src="../images/Database diagram.jpeg" alt="Database diagram" style="display: block; margin: 50 auto 0 auto;"/>
  <p>Diagrama de base de datos: 
  <a href="https://editor.plantuml.com/uml/pLXDRziu4BqRy7_GRRDO5qYpo1wCegYgC8uGHp9a9rU2fcYR24MffEHDqFQ_xr2o8rccbJHsWRqayioG6hxvUjGNdHEL5udezrOyPWxbYWhMx_LxJEOyVtRMRCL1eftl_PxZ_CLZP-XmcJkVFarkFtysiaoGd85qJHHT4NLsSVwd4SyLaN53V5c9apHcObzCKv6gXlZlIipaaak6DLCSNDXVLIW5VkA42qQMnecOKPuGSVRnV71HcWYYGK_0PIQ9f0p7bRVcdz5BzhIhVqnisomA9d3-d9cbJ1R9sOZeL81l0-SAN6DYu8mdeu7Z1QFI7c3D2xqr3YSeScT-6BZZWHE40TuHtBc1Eq9tA9ZLhw8a8zJWR_65AWREnvZaeCrvmk1bIMOqHHPRDJyR0MsSjIEe5CAq7rDBg67DzMPD4qK35MxikxKfqwqP0-Db5UdO9ixJd00QgSvjIEoYFFLkqDNz65qD73_0aoWSHMWwXPY4TvCncXcvvmOU0ejoTJg7l5gJdAVIx9539fGWWjJc-ibWBy7fm5wIf0don_CA_9XfgdXct6ruUpgl5ACCjkzmh6bj0MYpmKwP-C53w7jeu7prnv3g4VAGFvaDd71sWw8gXktQljXs1AXjo3U-Plk5huii4zmU9rtCowon9SoQMFFeeFrnw6wzx81qNcXe8bhZLj0lBYyhpyXJTSOMEYIE5Inh94AsIgKjRHX4JLZaD9KveJdEmByoeze6pJ1E9sw4CFoPGJrDKVG0COMdhn16Io6wtin_GAOAgwVJTYsS4_tu_YpD6Lr9JZcHDgszo7QFDq71bH-C3dMP3RhsZdKS2hNl7UTV54BifzC_LPmoS8Y8Sgwqu_sh2VJROsuQyJlFASkk3fF3LZig5I-9JUA4IwvpHV9K3HoYDVmWCXz06acW522B5RGWLK44-dzJ5LiAzRYZbZDVfCkEuswdOcj0jWRrvLi6jKXfcgIcisvxTNsQce80_1RmNcSdhtCojbX04ZD9hHiKaaDNKfnQrnvirLqZGR455xlyBOpyaQdVq0zW75tVep6Eq7KvfEhPT80X71Vh3QF6SKgB16I_HgsRdQpPe4CNZZ53tatWU-uO-y5qWZp3CA4p-P5tFoxf9lRS26YGqVbW1Ipqpf-PeftUHuOQDG-_zG_3_dEcB1s0Qrti4Mhsb75LGjRM67CkbtY3mtuDGP1iC_2tHA4v9OXWwZHXc4Je0NWyz3zyvq9ceM23gZ_6teqRZ0mJYjnR1B-GTmiHyoCpIAz2x_xb0j1HEQMdRLmFJASWdFdNlc6zy8fm_B37VuyaDnbH36U6plz_-6pjrAdyQHtJrbsw6zQs7-eyfO_LsYh8aYT5qXQNUwKBd32Y2sLpyvI4_rl15Nkb1xr2fnhuMBJV2h8jzkO13uBLnTsFp0owOd7H-I5ZQzAkh_VSXMj-lfTc9PsmyQaLppAh1YvMF8DvcLkprc0FgO8tvA3bfccTd1xIrgljdps80c-1HjcrQmvDcMhxc8Pv2wE0ISsi1YADbp0CRAhJzli_dAYyHi9c0B3kzrw-QFtuyU53-dttWyYmkXTnQJ7S7zn3PqKiXZMR6vRFtI_TZfzXrTqjndNk3kldVc_7SSk-BnVwZPklsLVtgg6pwGjlUaEZWmmToLYyksep6WuWBGpTNd3pfkRDfiCrg8z5gX9OK5qEx1ilcMH0GSo-zHMy6w2IojZicx7SA8rPU_Xj8zMOF-27Iejin_ejA1hUZUVF_TuN9kCY4Vy1" target="_blank">
    Ver diagrama de base de datos
  </a>
</p>
</p>
