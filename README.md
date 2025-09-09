<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Nombre de Marca | Soluciones Digitales</title>
  <meta name="description" content="Landing page moderna y responsiva para presentar productos o servicios profesionales." />
  <meta name="robots" content="index, follow" />
  <!-- Open Graph / Social -->
  <meta property="og:title" content="Nombre de Marca | Soluciones Digitales" />
  <meta property="og:description" content="Landing page moderna y responsiva para presentar productos o servicios profesionales." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://ejemplo.com" />
  <meta property="og:image" content="https://ejemplo.com/og-image.jpg" />
  <link rel="icon" href="/favicon.ico" />

  <style>
    /* ============================
       Variables y Reset Básico
       ============================ */
    :root {
      --bg: #0b0f1a;            /* Fondo principal */
      --panel: #11182a;         /* Tarjetas/Secciones */
      --text: #e6edf6;          /* Texto principal */
      --muted: #a9b3c9;         /* Texto secundario */
      --brand: #6ee7ff;         /* Acento (primario) */
      --brand-2: #7c3aed;       /* Acento secundario */
      --ok: #22c55e;
      --warn: #f59e0b;
      --danger: #ef4444;
      --radius: 16px;
      --shadow: 0 10px 30px rgba(0,0,0,.25);
      --maxw: 1120px;
    }
    *, *::before, *::after { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, "Helvetica Neue", Arial, "Apple Color Emoji", "Segoe UI Emoji";
      color: var(--text);
      background: radial-gradient(1200px 600px at 10% -10%, rgba(124,58,237,.12), transparent 60%),
                  radial-gradient(1000px 600px at 90% 0%, rgba(110,231,255,.10), transparent 60%),
                  var(--bg);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }
    a { color: inherit; text-decoration: none; }
    img { max-width: 100%; display: block; border-radius: calc(var(--radius) - 6px); }
    .container { width: min(100% - 2rem, var(--maxw)); margin-inline: auto; }

    /* ============================
       Cabecera / Navegación
       ============================ */
    header {
      position: sticky; top: 0; z-index: 50;
      backdrop-filter: saturate(140%) blur(8px);
      background: color-mix(in oklab, var(--bg) 80%, transparent);
      border-bottom: 1px solid rgba(255,255,255,.08);
    }
    .nav { display: flex; align-items: center; justify-content: space-between; padding: .9rem 0; }
    .brand { display: inline-flex; align-items: center; gap: .6rem; font-weight: 700; letter-spacing: .3px; }
    .brand-badge { width: 1.4rem; height: 1.4rem; border-radius: 10px; background: linear-gradient(135deg, var(--brand), var(--brand-2)); box-shadow: var(--shadow); }
    .menu { display: flex; align-items: center; gap: 1.1rem; }
    .btn { display: inline-flex; align-items: center; gap: .5rem; padding: .7rem 1rem; border-radius: 999px; border: 1px solid rgba(255,255,255,.14); background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02)); color: var(--text); font-weight: 600; transition: transform .2s ease, border-color .2s ease, box-shadow .2s ease; }
    .btn:hover { transform: translateY(-1px); border-color: rgba(255,255,255,.28); box-shadow: 0 8px 20px rgba(124,58,237,.25); }
    .btn.primary { border: 0; background: linear-gradient(135deg, var(--brand), var(--brand-2)); color: #0a0a0a; }

    /* ============================
       Hero
       ============================ */
    .hero { padding: 64px 0 28px; }
    .hero-grid { display: grid; grid-template-columns: 1.2fr .8fr; gap: 2rem; align-items: center; }
    .eyebrow { font-size: .85rem; color: var(--muted); letter-spacing: .12em; text-transform: uppercase; }
    h1 { font-size: clamp(2rem, 3.5vw + .5rem, 3.2rem); line-height: 1.1; margin: .4rem 0 1rem; }
    .lead { color: var(--muted); font-size: 1.05rem; }
    .cta { margin-top: 1.4rem; display: flex; gap: .75rem; flex-wrap: wrap; }
    .hero-card { background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02)); border: 1px solid rgba(255,255,255,.12); padding: 1rem; border-radius: var(--radius); box-shadow: var(--shadow); }
    .stats { display: grid; grid-template-columns: repeat(3, 1fr); gap: .8rem; margin-top: 1rem; }
    .stat { background: color-mix(in oklab, var(--panel) 84%, black 10%); border: 1px solid rgba(255,255,255,.08); padding: .9rem; border-radius: calc(var(--radius) - 8px); text-align: center; }
    .stat strong { display: block; font-size: 1.4rem; }

    /* ============================
       Secciones comunes
       ============================ */
    section { padding: 56px 0; }
    .section-title { font-size: clamp(1.4rem, 2.4vw + .5rem, 2rem); margin: 0 0 .75rem; }
    .section-lead { color: var(--muted); margin-bottom: 1.6rem; }

    /* ============================
       Features / Servicios
       ============================ */
    .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; }
    .card { background: color-mix(in oklab, var(--panel) 86%, black 8%); border: 1px solid rgba(255,255,255,.08); padding: 1.2rem; border-radius: var(--radius); box-shadow: var(--shadow); }
    .card h3 { margin: .2rem 0 .4rem; }
    .badge { display: inline-block; font-size: .8rem; padding: .25rem .6rem; border-radius: 999px; background: linear-gradient(135deg, var(--brand), var(--brand-2)); color: #0a0a0a; font-weight: 700; letter-spacing: .02em; }

    /* ============================
       Portafolio
       ============================ */
    .grid-portfolio { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; }
    .portfolio-item { position: relative; overflow: hidden; border-radius: var(--radius); }
    .portfolio-item figcaption { position: absolute; inset: auto 0 0 0; padding: .7rem .9rem; background: linear-gradient(180deg, transparent, rgba(0,0,0,.6)); font-weight: 600; }

    /* ============================
       Testimonios
       ============================ */
    .testimonials { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; }
    .quote { font-size: 1rem; color: var(--muted); }
    .avatar { width: 42px; height: 42px; border-radius: 50%; object-fit: cover; }

    /* ============================
       Pricing
       ============================ */
    .pricing { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; }
    .price-card { position: relative; border: 1px solid rgba(255,255,255,.12); border-radius: var(--radius); background: linear-gradient(180deg, rgba(255,255,255,.07), rgba(255,255,255,.02)); padding: 1.2rem; box-shadow: var(--shadow); }
    .price { font-size: 2rem; font-weight: 800; }
    .features { margin: 1rem 0; display: grid; gap: .45rem; color: var(--muted); }

    /* ============================
       Contacto
       ============================ */
    form { display: grid; gap: .75rem; }
    .field { display: grid; gap: .35rem; }
    .input, textarea {
      color: var(--text);
      background: color-mix(in oklab, var(--panel) 86%, black 8%);
      border: 1px solid rgba(255,255,255,.12);
      border-radius: 12px;
      padding: .8rem .9rem;
      outline: none;
    }
    .input:focus, textarea:focus { border-color: color-mix(in oklab, var(--brand) 70%, white 30%); box-shadow: 0 0 0 4px rgba(110,231,255,.12); }

    /* ============================
       Footer
       ============================ */
    footer { padding: 40px 0; border-top: 1px solid rgba(255,255,255,.08); color: var(--muted); }

    /* ============================
       Responsividad
       ============================ */
    @media (max-width: 980px) {
      .hero-grid { grid-template-columns: 1fr; }
      .grid-3, .grid-portfolio, .testimonials, .pricing { grid-template-columns: 1fr 1fr; }
    }
    @media (max-width: 640px) {
      .grid-3, .grid-portfolio, .testimonials, .pricing { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <!-- Header / Nav -->
  <header role="banner">
    <div class="container nav" aria-label="Navegación principal">
      <a href="#inicio" class="brand" aria-label="Inicio">
        <span class="brand-badge" aria-hidden="true"></span>
        <span>Nombre de Marca</span>
      </a>
      <nav class="menu" aria-label="Secciones">
        <a href="#servicios">Servicios</a>
        <a href="#portafolio">Portafolio</a>
        <a href="#precios">Precios</a>
        <a href="#contacto" class="btn">Contacto</a>
        <a href="#" class="btn primary">Cotizar ahora</a>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section id="inicio" class="hero">
    <div class="container hero-grid">
      <div>
        <p class="eyebrow">Impulsa tu presencia digital</p>
        <h1>Diseño y desarrollo web <span style="background:linear-gradient(135deg,var(--brand),var(--brand-2));-webkit-background-clip:text;background-clip:text;color:transparent">moderno y efectivo</span>.</h1>
        <p class="lead">Creamos sitios rápidos, accesibles y listos para convertir. Presenta tu marca con una experiencia premium y mide resultados desde el primer día.</p>
        <div class="cta">
          <a href="#precios" class="btn primary" aria-label="Ver planes y precios">Ver planes</a>
          <a href="#portafolio" class="btn" aria-label="Ver trabajos del portafolio">Ver trabajos</a>
        </div>
        <div class="stats" role="list" aria-label="Métricas clave">
          <div class="stat" role="listitem"><strong>+120</strong> proyectos lanzados</div>
          <div class="stat" role="listitem"><strong>98%</strong> satisfacción</div>
          <div class="stat" role="listitem"><strong>0.9s</strong> tiempo de carga</div>
        </div>
      </div>
      <div class="hero-card" aria-hidden="true">
        <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1600&auto=format&fit=crop" alt="Interfaz de diseño web en un portátil" />
      </div>
    </div>
  </section>

  <!-- Servicios / Features -->
  <section id="servicios">
    <div class="container">
      <h2 class="section-title">Servicios que convierten</h2>
      <p class="section-lead">Todo lo que necesitas para lanzar o renovar tu sitio con estándares modernos.</p>

      <div class="grid-3">
        <article class="card">
          <span class="badge" aria-hidden="true">UX/UI</span>
          <h3>Diseño centrado en el usuario</h3>
          <p>Arquitectura de información, wireframes y prototipos para sitios que se entienden y se disfrutan.</p>
        </article>
        <article class="card">
          <span class="badge" aria-hidden="true">Web</span>
          <h3>Desarrollo rápido y SEO</h3>
          <p>Código limpio, performance alto y etiquetas SEO listas para posicionar tu marca.</p>
        </article>
        <article class="card">
          <span class="badge" aria-hidden="true">Brand</span>
          <h3>Identidad visual</h3>
          <p>Paleta, tipografías y componentes reutilizables para mantener consistencia de marca.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- Portafolio -->
  <section id="portafolio">
    <div class="container">
      <h2 class="section-title">Trabajos recientes</h2>
      <p class="section-lead">Ejemplos de sitios responsivos con alto impacto visual.</p>
      <div class="grid-portfolio" role="list">
        <figure class="portfolio-item" role="listitem">
          <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=1600&auto=format&fit=crop" alt="Sitio para agencia creativa" />
          <figcaption>Agencia creativa</figcaption>
        </figure>
        <figure class="portfolio-item" role="listitem">
          <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?q=80&w=1600&auto=format&fit=crop" alt="Landing de SaaS" />
          <figcaption>Landing SaaS</figcaption>
        </figure>
        <figure class="portfolio-item" role="listitem">
          <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1600&auto=format&fit=crop" alt="Portafolio personal" />
          <figcaption>Portafolio personal</figcaption>
        </figure>
      </div>
    </div>
  </section>

  <!-- Testimonios -->
  <section aria-label="Testimonios de clientes">
    <div class="container">
      <h2 class="section-title">Lo que dicen nuestros clientes</h2>
      <div class="testimonials">
        <article class="card">
          <p class="quote">“Pasamos de no tener presencia digital a captar leads desde la primera semana. Gran trabajo.”</p>
          <div style="display:flex;align-items:center;gap:.6rem;margin-top:.6rem">
            <img class="avatar" src="https://images.unsplash.com/photo-1502685104226-ee32379fefbe?q=80&w=400&auto=format&fit=crop" alt="Foto de cliente" />
            <div><strong>María P.</strong><br><small>Directora de Marketing</small></div>
          </div>
        </article>
        <article class="card">
          <p class="quote">“El rendimiento y el SEO mejoraron notablemente. El soporte post-lanzamiento es excelente.”</p>
          <div style="display:flex;align-items:center;gap:.6rem;margin-top:.6rem">
            <img class="avatar" src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=400&auto=format&fit=crop" alt="Foto de cliente" />
            <div><strong>Carlos M.</strong><br><small>Fundador</small></div>
          </div>
        </article>
        <article class="card">
          <p class="quote">“Proceso claro, entregables puntuales y excelente comunicación. Los recomendaría sin dudar.”</p>
          <div style="display:flex;align-items:center;gap:.6rem;margin-top:.6rem">
            <img class="avatar" src="https://images.unsplash.com/photo-1547425260-76bcadfb4f2c?q=80&w=400&auto=format&fit=crop" alt="Foto de cliente" />
            <div><strong>Lucía R.</strong><br><small>Emprendedora</small></div>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- Precios -->
  <section id="precios">
    <div class="container">
      <h2 class="section-title">Planes pensados para crecer</h2>
      <p class="section-lead">Elige el plan que mejor se adapte a tu proyecto. Todos incluyen diseño responsive y optimización base de SEO.</p>

      <div class="pricing" role="list">
        <article class="price-card" role="listitem">
          <h3>Básico</h3>
          <p class="price">$ 399</p>
          <div class="features">
            <span>• 1 sección / Landing</span>
            <span>• Entrega en 3 días</span>
            <span>• SEO on-page básico</span>
          </div>
          <a href="#contacto" class="btn" aria-label="Seleccionar plan básico">Elegir</a>
        </article>

        <article class="price-card" role="listitem" aria-label="Plan recomendado" style="outline:2px solid color-mix(in oklab, var(--brand) 60%, white 40%);">
          <h3>Profesional <span class="badge" style="margin-left:.4rem">Recomendado</span></h3>
          <p class="price">$ 799</p>
          <div class="features">
            <span>• 3–5 secciones</span>
            <span>• Blog o portafolio</span>
            <span>• Integración analítica</span>
          </div>
          <a href="#contacto" class="btn primary" aria-label="Seleccionar plan profesional">Elegir</a>
        </article>

        <article class="price-card" role="listitem">
          <h3>Empresa</h3>
          <p class="price">$ 1499</p>
          <div class="features">
            <span>• +5 secciones</span>
            <span>• Integraciones (API, CRM)</span>
            <span>• Soporte prioritario</span>
          </div>
          <a href="#contacto" class="btn" aria-label="Seleccionar plan empresa">Elegir</a>
        </article>
      </div>
    </div>
  </section>

  <!-- Contacto -->
  <section id="contacto">
    <div class="container">
      <h2 class="section-title">Conversemos tu proyecto</h2>
      <p class="section-lead">Cuéntanos los objetivos y te enviamos una cotización en 24 horas.</p>

      <form action="mailto:ventas@tu-dominio.com" method="post" enctype="text/plain" aria-label="Formulario de contacto">
        <!-- Para usar Formspree u otro backend, reemplaza el action y method -->
        <div class="field">
          <label for="nombre">Nombre</label>
          <input class="input" id="nombre" name="nombre" type="text" required placeholder="Tu nombre" />
        </div>
        <div class="field">
          <label for="email">Correo</label>
          <input class="input" id="email" name="email" type="email" required placeholder="tu@correo.com" />
        </div>
        <div class="field">
          <label for="mensaje">Mensaje</label>
          <textarea id="mensaje" name="mensaje" rows="5" required placeholder="Cuéntanos qué necesitas"></textarea>
        </div>
        <button class="btn primary" type="submit">Enviar</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer role="contentinfo">
    <div class="container" style="display:flex;flex-wrap:wrap;gap:1rem;align-items:center;justify-content:space-between">
      <small>© <span id="year"></span> Nombre de Marca. Todos los derechos reservados.</small>
      <div style="display:flex;gap:1rem;align-items:center">
        <a href="#" aria-label="Términos y condiciones">Términos</a>
        <a href="#" aria-label="Política de privacidad">Privacidad</a>
        <a href="#inicio" class="btn" aria-label="Volver arriba">↑</a>
      </div>
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
