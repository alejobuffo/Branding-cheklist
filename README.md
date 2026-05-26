# Branding-cheklist
Cliqueable para branding

  /* PRINT */
  @media print {
    .progress-bar-wrap, .btn-primary { display: none; }
    .checklist-item { break-inside: avoid; }
  }
</style>
</head>
<body>

<div class="header">
  <div class="header-inner">
    <div class="header-tag">Diagnóstico de Proyecto</div>
    <h1>Checklist de <em>Branding</em><br>& Identidad Visual</h1>
    <p>Seleccioná los servicios que necesitás para tu marca. Esta lista nos permite diseñar una propuesta a medida, sin pagar por lo que no necesitás.</p>
  </div>
</div>

<div class="progress-bar-wrap">
  <div class="progress-bar-inner">
    <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
    <div class="progress-label" id="progressLabel">0% completado</div>
    <div class="progress-count" id="progressCount">0 / 0 ítems</div>
  </div>
</div>

<div class="main">

  <div class="intro-note">
    <strong>¿Cómo funciona?</strong> Revisá cada ítem, leé la descripción y marcá todo lo que necesitás o creés que puede ayudarte. No te preocupes si no estás seguro/a — podemos hablar de cada uno en la reunión de diagnóstico. Al final encontrarás 3 preguntas clave para entender mejor tu proyecto.
  </div>

  <!-- FASE 1 -->
  <div class="phase">
    <div class="phase-header">
      <div class="phase-num">01</div>
      <div class="phase-title-block">
        <div class="phase-title">Fase Estratégica</div>
        <div class="phase-subtitle">El ADN de la marca</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Diagnóstico y análisis de competencia</div>
        <div class="item-what">Estudiamos tu mercado, tus competidores directos e indirectos y el posicionamiento actual de tu marca (si ya existe). Detectamos oportunidades y riesgos antes de diseñar nada.</div>
        <div class="item-why">Saber dónde estás parado antes de moverte evita errores costosos. Es la diferencia entre diseñar con estrategia o con intuición.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Propósito, valores y personalidad de marca</div>
        <div class="item-what">Definimos el "por qué" de tu negocio, los valores que lo guían y el tipo de personalidad que transmite (¿es seria? ¿cercana? ¿innovadora?). Es la base de todo lo que viene después.</div>
        <div class="item-why">Las marcas con propósito claro generan más confianza, fidelidad y conexión emocional con sus clientes ideales.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Tono de voz y pilares de comunicación <span class="optional-tag">Copywriting</span></div>
        <div class="item-what">Definimos cómo habla tu marca: qué palabras usa, cuáles evita, cómo se dirige a su audiencia. Incluye los mensajes clave y los temas principales sobre los que comunicarás.</div>
        <div class="item-why">Una marca que habla de forma consistente genera reconocimiento. Tus textos, posteos y correos deben sonar igual de coherentes que tu logo.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Creación de Eslogan / Tagline corporativo</div>
        <div class="item-what">Una frase corta, memorable y estratégica que resume la esencia de tu marca. No es solo un lema bonito: es una herramienta de posicionamiento.</div>
        <div class="item-why">Un buen tagline hace que tu propuesta de valor sea recordable en segundos. Es lo que la gente repite cuando habla de vos.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Naming — Creación del nombre de marca <span class="optional-tag">si aplica</span></div>
        <div class="item-what">Creamos el nombre de tu empresa o producto desde cero: con búsqueda de disponibilidad, análisis fonético, significado y potencial de registro.</div>
        <div class="item-why">El nombre es lo primero que escuchan tus clientes. Un buen nombre es una ventaja competitiva que trabaja sola las 24hs.</div>
      </div>
    </div>
  </div>

  <!-- FASE 2 -->
  <div class="phase">
    <div class="phase-header">
      <div class="phase-num">02</div>
      <div class="phase-title-block">
        <div class="phase-title">Identidad Visual Core</div>
        <div class="phase-subtitle">Lo indispensable</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Logotipo principal y versiones secundarias (adaptables)</div>
        <div class="item-what">Diseñamos el logo central de tu marca más todas sus variantes: versión horizontal, vertical, reducida (solo ícono), en negativo (para fondos oscuros) y en blanco y negro.</div>
        <div class="item-why">Un logo con versiones adaptables funciona en cualquier contexto sin verse deformado. Es la diferencia entre una marca amateur y una marca profesional.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Paleta de colores estratégica y tipografías institucionales</div>
        <div class="item-what">Elegimos los colores oficiales de tu marca (con sus códigos exactos para digital e impresión) y las fuentes tipográficas que la representan, incluyendo cuándo y cómo usar cada una.</div>
        <div class="item-why">El color y la tipografía son responsables de hasta el 80% del reconocimiento visual de una marca. Usarlos bien es consistencia; usarlos mal es confusión.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Manual de marca básico (guía de uso)</div>
        <div class="item-what">Un documento simple que explica cómo usar correctamente el logo, los colores y las tipografías. Incluye ejemplos de usos correctos y los errores más comunes a evitar.</div>
        <div class="item-why">Sin un manual, cada persona que use tu logo lo hará a su manera. El manual protege la coherencia de tu identidad cuando la marca crece o delega.</div>
      </div>
    </div>
  </div>

  <!-- FASE 3 -->
  <div class="phase">
    <div class="phase-header">
      <div class="phase-num">03</div>
      <div class="phase-title-block">
        <div class="phase-title">Universo Visual & Aplicaciones</div>
        <div class="phase-subtitle">Para salir a la cancha</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Papelería institucional</div>
        <div class="item-what">Diseño de tarjetas de presentación, hojas membretadas, sobres y firma de correo electrónico, todo bajo la identidad visual de tu marca.</div>
        <div class="item-why">Cada punto de contacto físico refuerza la profesionalidad. Una tarjeta bien diseñada sigue trabajando para vos mucho después de esa reunión.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Plantillas editables para Redes Sociales</div>
        <div class="item-what">Pack de plantillas personalizadas para publicaciones del feed, historias y portadas de tus perfiles. Editables por vos en Canva o similares, sin depender de un diseñador cada semana.</div>
        <div class="item-why">La consistencia en redes construye reconocimiento de marca. Con plantillas propias, publicás de forma profesional en minutos.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Placas promocionales o institucionales específicas</div>
        <div class="item-what">Diseño de piezas puntuales para campañas, lanzamientos, fechas especiales o comunicados. Cada pieza respeta la identidad pero tiene un objetivo comunicacional concreto.</div>
        <div class="item-why">Para momentos específicos necesitás piezas específicas. Diseñarlas a medida garantiza impacto sin romper la coherencia de tu marca.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Packaging & Etiquetas <span class="optional-tag">si aplica</span></div>
        <div class="item-what">Diseño de envases, etiquetas, sachets, etiquetas colgantes o cualquier superficie física sobre la que se aplique tu marca para un producto.</div>
        <div class="item-why">El packaging es el primer vendedor silencioso de tu producto. Un diseño estratégico puede ser el factor decisivo en el punto de venta.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Manual de marca corporativo completo</div>
        <div class="item-what">El manual extendido: incluye todo el universo visual de la marca (patrones, texturas, íconos, fotografía), mockups de aplicaciones reales y layouts para cada soporte importante.</div>
        <div class="item-why">Cuando la marca escala, el equipo crece o trabajás con proveedores externos, el manual corporativo es el documento que garantiza que todos hablen el mismo idioma visual.</div>
      </div>
    </div>
  </div>

  <!-- FASE 4 -->
  <div class="phase">
    <div class="phase-header">
      <div class="phase-num">04</div>
      <div class="phase-title-block">
        <div class="phase-title">Puntos de Contacto Digitales & Extras</div>
        <div class="phase-subtitle">Presencia y alcance</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Diseño de Landing Page o Sitio Web Institucional</div>
        <div class="item-what">Diseño de tu presencia web: desde una página de captura (landing) hasta un sitio completo con secciones de servicios, equipo, contacto y más. Adaptado a tu marca y tus objetivos.</div>
        <div class="item-why">Tu sitio web trabaja para vos las 24hs. Es tu vendedor más accesible y la primera referencia que busca cualquier cliente potencial antes de contactarte.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Plantilla de presentación corporativa</div>
        <div class="item-what">Diseño de una plantilla profesional en PowerPoint o Canva que uses para presentar tu empresa, tus servicios o cerrar ventas. Editable, ordenada y con el look de tu marca.</div>
        <div class="item-why">Una presentación con diseño profesional transmite confianza antes de que digas una sola palabra. Proyectás seriedad y diferenciación desde el primer slide.</div>
      </div>
    </div>

    <div class="checklist-item" onclick="toggleItem(this)">
      <div class="checkbox-wrap">
        <input type="checkbox">
        <div class="checkbox-visual">
          <svg width="13" height="10" viewBox="0 0 13 10" fill="none"><path d="M1.5 5L5 8.5L11.5 1.5" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
      </div>
      <div class="item-content">
        <div class="item-name">Señalética, vehículos y uniformes <span class="optional-tag">si aplica</span></div>
        <div class="item-what">Aplicación de la marca en el espacio físico: carteles, viniles para local o vehículos, diseño de uniformes o merchandising. Transforma tu entorno en una extensión de tu identidad.</div>
        <div class="item-why">Cada superficie que ven tus clientes es una oportunidad de reforzar la marca. El branding físico genera presencia y credibilidad difíciles de ignorar.</div>
      </div>
    </div>
  </div>

  <!-- SUMMARY -->
  <div class="summary-section">
    <div class="summary-left">
      <div class="summary-title">Ítems seleccionados</div>
      <div class="summary-sub">Estos ítems conformarán tu propuesta a medida</div>
    </div>
    <div class="summary-count"><span id="selectedCount">0</span><span>/ 13 ítems</span></div>
    <button class="btn-primary" onclick="printChecklist()">Imprimir / Guardar PDF</button>
  </div>

  <!-- QUESTIONS -->
  <div class="questions-section">
    <div class="questions-header">
      <div class="questions-tag">Para ajustar la propuesta</div>
      <div class="questions-title">3 preguntas clave<br>antes de cotizar</div>
    </div>

    <div class="question-item">
      <div class="question-num">PREGUNTA 01</div>
      <div class="question-text">¿Cuál es el presupuesto estimado o rango de inversión que tienen asignado para este proyecto?</div>
      <textarea class="question-input" placeholder="Ej: Tenemos entre $X y $Y disponibles, o bien no tenemos un número definido aún..."></textarea>
    </div>

    <div class="question-item">
      <div class="question-num">PREGUNTA 02</div>
      <div class="question-text">¿Cuál es la fecha límite ideal para el lanzamiento o entrega del proyecto?</div>
      <textarea class="question-input" placeholder="Ej: Necesitamos lanzar antes del 15 de agosto, o en los próximos 2 meses..."></textarea>
    </div>

    <div class="question-item" style="margin-bottom:0">
      <div class="question-num">PREGUNTA 03</div>
      <div class="question-text">¿Cuál es el principal problema que quieren resolver con este branding o rebranding?</div>
      <textarea class="question-input" placeholder="Ej: Nuestra imagen no refleja el nivel de nuestros servicios, los clientes nos confunden con la competencia, necesitamos transmitir más confianza..."></textarea>
    </div>
  </div>

</div>

<footer>Checklist generado para diagnóstico de proyecto · Completalo y envialo para recibir tu propuesta a medida</footer>

<script>
  const totalItems = document.querySelectorAll('.checklist-item').length;
  document.getElementById('progressCount').textContent = `0 / ${totalItems} ítems`;

  function toggleItem(el) {
    el.classList.toggle('checked');
    const cb = el.querySelector('input[type="checkbox"]');
    cb.checked = !cb.checked;
    updateProgress();
  }

  function updateProgress() {
    const checked = document.querySelectorAll('.checklist-item.checked').length;
    const pct = Math.round((checked / totalItems) * 100);
    document.getElementById('progressFill').style.width = pct + '%';
    document.getElementById('progressLabel').textContent = pct + '% completado';
    document.getElementById('progressCount').textContent = `${checked} / ${totalItems} ítems`;
    document.getElementById('selectedCount').textContent = checked;
  }

  function printChecklist() {
    window.print();
  }

  updateProgress();
</script>
</body>
</html>
