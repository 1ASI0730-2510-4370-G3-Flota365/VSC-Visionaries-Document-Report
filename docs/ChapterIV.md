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
<img src="../images/LandingPageWireframe.png" alt="Landing Page Wireframe" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">
</p>

<h4 id="landingMockUp">4.3.2. Landing Page Mock-up</h4>
<img src="../images/LandingPageMockup.jpg" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

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
Diagrama de clases:
<img src="../images/diagrama clases.png" alt="diagrama clases" style="display: block; margin: 50 auto 0 auto;"/>
linck del diagrama de clases en plantmul:https://editor.plantuml.com/uml/hLPDJnin4BqZyH-id58W4VIuGX5HQQH8fKL4ukvu9ukBrtRz4GWj_xspzYviDWuaWbms6RyPpvjvCzaBwwXnlXI71_QUIqqDBGaJrDgnSuRFlOCfKtB6du2SRc0cIhfmTFRryE3mG5DsJmiWlKjLKYvxv6zb9VW9QF9DbPhA5Ja_7nU5WO8w83TAkHFoNJhkLgDHvK7gpu3d6PbX4h9e6IKj8M5sz76QWdEPU-lCQlFe-8xQIyENOFfvU6Ga_loIaRbI0gXiWGjm4m7WR1-FVt3hpiFFKOGyh_ESUGrcoQqoIFN3rBIot74b4nGAa62mYZ7n6z3Ak4qsqPvm2nHghqNrFIF1rF7fi8jnFuEPu0oaxPnqRWi9VKWnELXckDvIGfhdjt37cO3-CZupKXkm34l5ynQOKS6ym2IkmIoKAQbaK0dY2Z0iI-PVnzghNBgwugSlvrKRDqvBbOD8s76IdRS9YYRqSXQE-oazU9tZXJL0miDiBT9Q6Jhi8d4aTqk51_9h_XkOwr3SqlnbvP6HXL0qhREOvbw5mqtbGBf43U0ng3pDfTbBlRCU6GpmCHmUzTfJd14ejL0hIqPlUTIJiICwAZiZwa6-8AEjmXsz0Xi9PQJYXukr0nyCHgHt6g1rFn3PAFK5swBJSgYBd15khO_WvxLLFjOQnvHMqxEnpyFrLrGYiCIopwhu3DfjEaOOBsGpOUqbSqBUdxSz5rMSqJjWztN4MjA9Yv8RPmkVgbnD2x5TEgHaYP9hRKZxDKqkmwdTmUErsxRkMAejKxam5F_OF7FUGAip72V0B2W6cqwe5suigLWzeIhRNT46SixSX7A1thQ_MNaQtQwfmt3IRXcSA8FnD5pYEBCuhHor7qZPJWRh0_p9EKGPO4lNxcZqStqvwSSjs0ZcpQMc97VAT8FbtE9YNksfgNPnXiD_eqvHtfL3fuiPyNOd6RqM1DTHM7wxUBMeP-IF1yDRuhi0V9cgtXJ_0m00

<h4 id="classDictionary">4.7.2. Class Dictionary</h4>
Para una mejor comprensión acerca del propósito de creación que cada una de las clases con sus 
respectivas propiedades, se detallará en esta sección cada uno de ellos:
<br>
<h3>Class Company</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Company ID</td></tr>
  <tr><td>name</td><td>String</td><td>Name of the company</td></tr>
  <tr><td>taxId</td><td>String</td><td>Tax identifier</td></tr>
  <tr><td>industry</td><td>String</td><td>Industry sector</td></tr>
</table>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>hasDriver(driver: Driver)</td><td>boolean</td><td>Checks if the driver is employed</td></tr>
  <tr><td>getFleets()</td><td>List&lt;Fleet&gt;</td><td>Returns all fleets owned</td></tr>
</table>

<h3>Class Fleet</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Fleet ID</td></tr>
  <tr><td>description</td><td>String</td><td>Description of the fleet</td></tr>
</table>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>addVehicle(vehicle: Vehicle)</td><td>void</td><td>Adds vehicle to fleet</td></tr>
  <tr><td>calculatePerformance()</td><td>Metric</td><td>Calculates fleet performance</td></tr>
</table>

<h3>Class Vehicle</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Vehicle ID</td></tr>
  <tr><td>plateNumber</td><td>String</td><td>License plate</td></tr>
  <tr><td>model</td><td>String</td><td>Vehicle model</td></tr>
  <tr><td>status</td><td>String</td><td>Current vehicle status</td></tr>
</table>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>reportStatus()</td><td>Report</td><td>Generates vehicle report</td></tr>
  <tr><td>updateStatus(newStatus: String)</td><td>void</td><td>Updates vehicle status</td></tr>
</table>

<h3>Class Driver</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Driver ID</td></tr>
  <tr><td>name</td><td>String</td><td>Name of the driver</td></tr>
  <tr><td>license</td><td>String</td><td>Driver license</td></tr>
</table>

<h3>Class Supervisor</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Supervisor ID</td></tr>
  <tr><td>name</td><td>String</td><td>Name of the supervisor</td></tr>
  <tr><td>position</td><td>String</td><td>Position of supervisor</td></tr>
</table>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>generateDriverReport(driver: Driver)</td><td>Report</td><td>Creates a report for driver</td></tr>
  <tr><td>generateFleetReport(fleet: Fleet)</td><td>Report</td><td>Creates a report for fleet</td></tr>
</table>
<h3>Class Report</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>id</td><td>String</td><td>Report ID</td></tr>
  <tr><td>content</td><td>String</td><td>Content of the report</td></tr>
</table>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>export()</td><td>void</td><td>Exports report</td></tr>
</table>
<h3>Class Metric</h3>
<table border="1">
  <tr><th>Attribute</th><th>Type</th><th>Description</th></tr>
  <tr><td>name</td><td>String</td><td>Name of the metric</td></tr>
  <tr><td>value</td><td>float</td><td>Numeric value</td></tr>
</table>
<h3>Class AIAnalytics</h3>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>predictFailures()</td><td>void</td><td>Predicts vehicle failures</td></tr>
  <tr><td>analyzePatterns()</td><td>void</td><td>Analyzes performance patterns</td></tr>
</table>
<h3>Class Reporting</h3>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>generatePDF(report: Report)</td><td>void</td><td>Generates a PDF from report</td></tr>
</table>
<h3>Class Monitoring</h3>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>displayStatus(vehicle: Vehicle)</td><td>String</td><td>Shows vehicle status</td></tr>
</table>
<h3>Class FleetManagementService</h3>
<table border="1">
  <tr><th>Method</th><th>Return Type</th><th>Description</th></tr>
  <tr><td>assignVehicle(fleet: Fleet, vehicle: Vehicle)</td><td>void</td><td>Assigns a vehicle to fleet</td></tr>
  <tr><td>generateFleetReport(fleet: Fleet)</td><td>Report</td><td>Generates a fleet report</td></tr>
  <tr><td>checkVehicleStatus(vehicle: Vehicle)</td><td>String</td><td>Returns vehicle status</td></tr>
</table>

<h3 id="dbDesign">4.8. Database Design</h3>

<h4 id="dbDiagram">4.8.1. Database Diagram</h4>
Diagrama de base de datos:

<p align="center">
<img src="../images/Database diagram.jpeg" alt="Database diagram" style="display: block; margin: 50 auto 0 auto;"/>
</p>
