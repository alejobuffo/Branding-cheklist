# Branding-cheklist
Cliqueable para branding
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Checklist de Branding</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --ink: #1a1208;
    --paper: #faf8f3;
    --cream: #f2ede3;
    --gold: #c9963a;
    --gold-light: #e8c97a;
    --rust: #b84c1e;
    --sage: #6b7c5a;
    --border: #d4c9b0;
    --shadow: rgba(26,18,8,0.12);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--paper);
    color: var(--ink);
    font-family: 'DM Sans', sans-serif;
    font-size: 15px;
    line-height: 1.65;
    min-height: 100vh;
  }

  /* HEADER */
  .header {
    background: var(--ink);
    color: var(--paper);
    padding: 56px 40px 48px;
    position: relative;
    overflow: hidden;
  }
  .header::before {
    content: '';
    position: absolute;
    top: -60px; right: -60px;
    width: 320px; height: 320px;
    border-radius: 50%;
    border: 1px solid rgba(201,150,58,0.25);
  }
  .header::after {
    content: '';
    position: absolute;
    bottom: -80px; left: -40px;
    width: 220px; height: 220px;
    border-radius: 50%;
    border: 1px solid rgba(201,150,58,0.15);
  }
  .header-inner {
    max-width: 820px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }
  .header-tag {
    display: inline-block;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--gold);
    border: 1px solid var(--gold);
    padding: 4px 14px;
    margin-bottom: 22px;
  }
  .header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2.2rem, 5vw, 3.2rem);
    font-weight: 900;
    line-height: 1.15;
    letter-spacing: -0.01em;
    margin-bottom: 18px;
  }
  .header h1 em {
    font-style: italic;
    color: var(--gold-light);
  }
  .header p {
    font-size: 15px;
    font-weight: 300;
    color: rgba(250,248,243,0.75);
    max-width: 560px;
    line-height: 1.7;
  }

  /* PROGRESS */
  .progress-bar-wrap {
    background: var(--cream);
    border-bottom: 1px solid var(--border);
    padding: 16px 40px;
    position: sticky;
    top: 0;
    z-index: 100;
    backdrop-filter: blur(6px);
  }
  .progress-bar-inner {
    max-width: 820px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    gap: 16px;
  }
  .progress-track {
    flex: 1;
    height: 4px;
    background: var(--border);
    border-radius: 2px;
    overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--gold), var(--gold-light));
    border-radius: 2px;
    width: 0%;
    transition: width 0.4s ease;
  }
  .progress-label {
    font-size: 12px;
    font-weight: 600;
    color: var(--gold);
    letter-spacing: 0.05em;
    white-space: nowrap;
  }
  .progress-count {
    font-size: 12px;
    color: #888;
    white-space: nowrap;
  }

  /* MAIN */
  .main {
    max-width: 820px;
    margin: 0 auto;
    padding: 48px 40px 80px;
  }

  /* INTRO NOTE */
  .intro-note {
    background: var(--cream);
    border-left: 3px solid var(--gold);
    padding: 18px 22px;
    margin-bottom: 48px;
    font-size: 14px;
    color: #5a5040;
    line-height: 1.7;
  }
  .intro-note strong { color: var(--ink); }

  /* PHASE SECTION */
  .phase {
    margin-bottom: 52px;
  }
  .phase-header {
    display: flex;
    align-items: flex-start;
    gap: 18px;
    margin-bottom: 24px;
    padding-bottom: 18px;
    border-bottom: 2px solid var(--ink);
  }
  .phase-num {
    font-family: 'Playfair Display', serif;
    font-size: 3rem;
    font-weight: 900;
    line-height: 1;
    color: var(--gold);
    opacity: 0.5;
    flex-shrink: 0;
    margin-top: -6px;
  }
  .phase-title-block {}
  .phase-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.35rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.2;
  }
  .phase-subtitle {
    font-size: 12px;
    font-weight: 500;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--gold);
    margin-top: 4px;
  }

  /* CHECKLIST ITEM */
  .checklist-item {
    display: flex;
    gap: 16px;
    padding: 18px 0;
    border-bottom: 1px solid var(--border);
    cursor: pointer;
    transition: background 0.15s;
    border-radius: 4px;
    padding-left: 8px;
    padding-right: 8px;
  }
  .checklist-item:hover {
    background: rgba(201,150,58,0.05);
  }
  .checklist-item.checked {
    background: rgba(201,150,58,0.08);
  }
  .checklist-item.checked .item-name {
    color: var(--sage);
  }

  /* CUSTOM CHECKBOX */
  .checkbox-wrap {
    flex-shrink: 0;
    margin-top: 2px;
  }
  .checkbox-wrap input[type="checkbox"] {
    display: none;
  }
  .checkbox-visual {
    width: 22px;
    height: 22px;
    border: 2px solid var(--border);
    border-radius: 3px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.2s;
    background: white;
  }
  .checklist-item.checked .checkbox-visual {
    background: var(--gold);
    border-color: var(--gold);
  }
  .checkbox-visual svg {
    opacity: 0;
    transform: scale(0.5);
    transition: all 0.2s;
  }
  .checklist-item.checked .checkbox-visual svg {
    opacity: 1;
    transform: scale(1);
  }

  /* ITEM CONTENT */
  .item-content {
    flex: 1;
  }
  .item-name {
    font-weight: 600;
    font-size: 15px;
    color: var(--ink);
    margin-bottom: 5px;
    transition: color 0.2s;
  }
  .item-name .optional-tag {
    display: inline-block;
    font-size: 10px;
    font-weight: 600;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--rust);
    border: 1px solid var(--rust);
    padding: 1px 7px;
    border-radius: 2px;
    margin-left: 8px;
    vertical-align: middle;
  }
  .item-what {
    font-size: 13.5px;
    color: #6b6050;
    margin-bottom: 6px;
    line-height: 1.6;
  }
  .item-why {
    font-size: 13px;
    color: var(--sage);
    font-weight: 500;
    display: flex;
    align-items: flex-start;
    gap: 6px;
    line-height: 1.55;
  }
  .item-why::before {
    content: '✦';
    font-size: 9px;
    flex-shrink: 0;
    margin-top: 3px;
    color: var(--gold);
  }

  /* QUESTIONS SECTION */
  .questions-section {
    margin-top: 64px;
    background: var(--ink);
    color: var(--paper);
    padding: 44px 40px;
    border-radius: 2px;
    position: relative;
    overflow: hidden;
  }
  .questions-section::before {
    content: '?';
    font-family: 'Playfair Display', serif;
    font-size: 280px;
    font-weight: 900;
    position: absolute;
    right: -20px;
    top: -60px;
    color: rgba(201,150,58,0.07);
    line-height: 1;
    pointer-events: none;
  }
  .questions-header {
    margin-bottom: 32px;
    position: relative;
  }
  .questions-tag {
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 10px;
  }
  .questions-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
    font-weight: 700;
    line-height: 1.2;
  }
  .question-item {
    margin-bottom: 24px;
    position: relative;
  }
  .question-num {
    font-family: 'Playfair Display', serif;
    font-size: 0.75rem;
    font-weight: 700;
    color: var(--gold);
    letter-spacing: 0.08em;
    margin-bottom: 6px;
  }
  .question-text {
    font-weight: 600;
    font-size: 15px;
    color: var(--paper);
    margin-bottom: 10px;
    line-height: 1.5;
  }
  .question-input {
    width: 100%;
    background: rgba(255,255,255,0.07);
    border: 1px solid rgba(201,150,58,0.3);
    border-radius: 3px;
    padding: 12px 16px;
    color: var(--paper);
    font-family: 'DM Sans', sans-serif;
    font-size: 14px;
    resize: vertical;
    min-height: 72px;
    outline: none;
    transition: border-color 0.2s;
  }
  .question-input::placeholder { color: rgba(250,248,243,0.3); }
  .question-input:focus { border-color: var(--gold); }

  /* SUMMARY */
  .summary-section {
    margin-top: 36px;
    padding: 28px 32px;
    background: var(--cream);
    border: 1px solid var(--border);
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 16px;
  }
  .summary-left {}
  .summary-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    font-weight: 700;
    margin-bottom: 4px;
  }
  .summary-sub {
    font-size: 13px;
    color: #888;
  }
  .summary-count {
    font-family: 'Playfair Display', serif;
    font-size: 2.4rem;
    font-weight: 900;
    color: var(--gold);
    line-height: 1;
  }
  .summary-count span {
    font-family: 'DM Sans', sans-serif;
    font-size: 13px;
    font-weight: 400;
    color: #aaa;
    margin-left: 4px;
  }
  .btn-primary {
    background: var(--gold);
    color: var(--ink);
    font-family: 'DM Sans', sans-serif;
    font-weight: 700;
    font-size: 13.5px;
    letter-spacing: 0.05em;
    padding: 14px 28px;
    border: none;
    cursor: pointer;
    text-transform: uppercase;
    transition: background 0.2s, transform 0.15s;
    border-radius: 2px;
  }
  .btn-primary:hover {
    background: var(--gold-light);
    transform: translateY(-1px);
  }

  /* FOOTER */
  footer {
    text-align: center;
    padding: 28px;
    font-size: 12px;
    color: #bbb;
    border-top: 1px solid var(--border);
    letter-spacing: 0.05em;
  }

  @media (max-width: 600px) {
    .header { padding: 36px 20px 32px; }
    .main { padding: 32px 20px 60px; }
    .progress-bar-wrap { padding: 12px 20px; }
    .questions-section { padding: 32px 22px; }
    .summary-section { padding: 20px; }
    .phase-num { font-size: 2.2rem; }
  }

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
