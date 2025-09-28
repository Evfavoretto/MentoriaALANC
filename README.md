<html lang="pt-br">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <title>Mentoria ALANC — Alavancagem de Carreira e Negócios</title>
  <meta name="description" content="Mentoria ALANC: alavancagem de carreira e negócios com clareza, propósito e equilíbrio. Para mulheres e casais que querem prosperar sem abrir mão da família.">
  <meta name="robots" content="index,follow">

  <!-- Open Graph / Twitter -->
  <meta property="og:type" content="website">
  <meta property="og:title" content="Mentoria ALANC — Clareza, Propósito e Equilíbrio">
  <meta property="og:description" content="Alavanque sua carreira e seus negócios sem abrir mão da família, do equilíbrio e do propósito.">
  <meta property="og:image" content="logo.jpeg">
  <meta property="og:locale" content="pt_BR">
  <meta name="twitter:card" content="summary_large_image">

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800;900&display=swap" rel="stylesheet">

  <style>
    :root{
      --pink:#E91E63;      /* rosa principal */
      --pink-2:#FDE8F1;    /* rosa claro */
      --red:#D61E1E;       /* vermelho (CTA e destaques) */
      --ink:#0F172A;       /* texto principal */
      --soft:#667085;      /* texto secundário */
      --line:#E9EEF5;      /* divisórias */
      --bg:#FFFFFF;        /* fundo */
      --ok:#10B981;        /* ícone check */
    }

    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:var(--bg);color:var(--ink);
      font-family:"Inter",ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,"Helvetica Neue",Arial}
    img{max-width:100%;display:block}
    a{text-decoration:none}
    .wrap{max-width:1100px;margin:0 auto;padding:0 20px}

    /* 🔥 Remover header padrão do GitHub Pages */
    header, .page-header, .site-header, .project-name, .project-tagline {
      display: none !important;
    }

    /* Barra rosa colada no topo da página (mais alta) */
    .top-bar{
      background:var(--pink); color:#fff; text-align:center;
      padding:70px 10px; /* antes 20px, agora +50px */
      font-weight:900; letter-spacing:.04em; text-transform:uppercase;
      font-size:clamp(18px,4.4vw,26px);
    }

    /* HERO */
    .hero{padding:34px 0 10px}
    .hero-card{
      background:#fff; border:1px solid var(--line); border-radius:22px;
      padding:28px 22px 30px; box-shadow:0 16px 36px rgba(0,0,0,.06); text-align:center
    }
    .logo{max-height:160px;width:auto;margin:0 auto 16px}
    .hero h1{
      margin:0 0 10px; font-size:clamp(28px,4.6vw,46px); line-height:1.08; font-weight:900
    }
    .lead{
      margin:8px auto 0; max-width:860px; color:var(--soft); font-size:clamp(16px,2.4vw,20px)
    }
    .divider{height:10px;margin:22px auto;max-width:320px;border-radius:999px;
      background:linear-gradient(90deg,var(--pink),var(--red))}

    /* Botões */
    .cta{display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin:18px 0 0}
    .btn{display:inline-block;padding:14px 20px;border-radius:14px;font-weight:900;box-shadow:0 10px 24px rgba(0,0,0,.08)}
    .primary{background:var(--red);color:#fff}
    .ghost{background:#fff;border:2px solid var(--pink);color:var(--pink)}
    .primary:hover{filter:brightness(1.04)}
    .ghost:hover{background:var(--pink);color:#fff}
    a:focus, .btn:focus, .faq-q:focus{outline:3px solid #ffd1d9; outline-offset:2px; border-radius:12px}

    /* Seções base */
    section{padding:56px 0;border-bottom:1px solid var(--line)}
    .section-title{
      font-size:clamp(28px,4.2vw,42px);font-weight:900;margin:0 0 10px;text-align:center;
      background:linear-gradient(90deg,var(--pink),var(--red));
      -webkit-background-clip:text;background-clip:text;color:transparent;
    }
    p,li{font-size:18px;color:var(--soft)}
    ul{margin:10px 0 0 18px}
    .grid{display:grid;gap:22px}
    .two{grid-template-columns:1fr}
    @media(min-width:900px){.two{grid-template-columns:1fr 1fr}}
    .card{background:#fff;border:1px solid var(--line);border-radius:18px;padding:22px;box-shadow:0 10px 28px rgba(31,35,48,.05)}
    .pink{background:var(--pink-2)}
    .grad-left{
      font-size:clamp(24px,3.6vw,32px);line-height:1.1;margin:0 0 10px;font-weight:900;
      background:linear-gradient(90deg,var(--pink),var(--red));-webkit-background-clip:text;background-clip:text;color:transparent;text-align:left;
    }

    /* Listas */
    .list-check li{list-style:none;padding-left:28px;position:relative}
    .list-check li:before{content:"✓";position:absolute;left:0;top:0;color:var(--ok);font-weight:900}
    .list-dot li{list-style:none;padding-left:28px;position:relative}
    .list-dot li:before{content:"•";position:absolute;left:6px;top:0;color:var(--red);font-weight:900}

    /* Bio */
    .bio{display:grid;gap:24px;align-items:center}
    .bio img{border-radius:16px;box-shadow:0 12px 28px rgba(0,0,0,.08)}
    @media(min-width:900px){.bio{grid-template-columns:360px 1fr}}

    /* Depoimentos (cards só rosa) */
    .testimonials{display:grid;gap:18px}
    @media(min-width:900px){.testimonials{grid-template-columns:1fr 1fr}}
    .t-card{border:1px solid #F7CDD0;border-radius:16px;padding:16px 18px;background:var(--pink-2);box-shadow:0 8px 22px rgba(0,0,0,.05)}
    .t-name{font-weight:900;margin:0 0 6px;font-size:16px;color:var(--ink)}

    /* FAQ — pergunta vermelha / resposta rosa */
    .faq{max-width:980px;margin:0 auto}
    .faq-item{margin:12px 0;border-radius:14px;overflow:hidden;box-shadow:0 6px 18px rgba(0,0,0,.06);border:1px solid var(--line)}
    .faq-q{width:100%;text-align:left;background:var(--red);border:0;padding:16px 18px;font-size:18px;font-weight:900;color:#fff;cursor:pointer;display:flex;justify-content:space-between;align-items:center}
    .faq-q .mark{flex:0 0 auto;font-weight:900;color:#fff}
    .faq-a{max-height:0;overflow:hidden;transition:max-height .28s ease;background:var(--pink-2);color:var(--ink);border-top:1px solid var(--line)}
    .faq-a-inner{padding:16px 18px;font-size:16px;line-height:1.55}
    .faq-item.open .faq-a{max-height:360px}

    /* CTA final + rodapé */
    .footer-cta{background:var(--pink-2);border:1px solid #f8c6d5;border-radius:16px;padding:26px;display:flex;gap:16px;flex-wrap:wrap;align-items:center;justify-content:space-between}
    footer{padding:28px 0;background:var(--red);color:#fff;font-size:14px;text-align:center}

    /* WhatsApp flutuante */
    .whats-float{
      position:fixed; right:40px; top:50%; transform:translateY(-50%); z-index:1000;
      width:60px; height:60px; border-radius:50%; background:#25D366; box-shadow:0 12px 28px rgba(0,0,0,.18);
      display:flex; align-items:center; justify-content:center
    }
    .whats-float svg{width:30px;height:30px;fill:#fff}
    @media (max-width:640px){
      .whats-float{top:auto; bottom:18px; right:18px; transform:none}
    }
  </style>
</head>
<body>

  <!-- Barra rosa colada no topo -->
  <div class="top-bar" role="banner">Mentoria ALANC — Alavancagem de Carreira e Negócios</div>

  <!-- HERO -->
  <section class="hero" aria-labelledby="titulo-hero">
    <div class="wrap">
      <div class="hero-card">
        <img src="logo.jpeg" alt="Logo Mentoria ALANC" class="logo" width="600" height="200" decoding="async">
        <h1 id="titulo-hero">Alavancagem de Carreira e Negócios com Clareza, Propósito e Equilíbrio</h1>
        <p class="lead"><strong>Alavanque sua carreira e seus negócios sem abrir mão da família, do equilíbrio e do propósito.</strong> A Mentoria ALANC é para mulheres e casais que sabem que podem mais, mas não querem crescer sozinhos.</p>
        <div class="divider" aria-hidden="true"></div>
        <div class="cta" role="group" aria-label="Ações principais">
          <a class="btn primary" href="https://forms.gle/3KbznEmAkpgoNaab9" target="_blank" rel="noopener">Quero entrar na Mentoria ALANC</a>
          <a class="btn ghost" href="#faq">Perguntas frequentes</a>
        </div>
      </div>
    </div>
  </section>

  <!-- (demais seções iguais ao anterior) -->

  <!-- DEPOIMENTOS -->
  <section id="depoimentos" aria-labelledby="t-dep">
    <div class="wrap">
      <h2 id="t-dep" class="section-title">Depoimentos Reais de Transformação</h2>
      <div class="testimonials">
        <!-- Joel -->
        <article class="t-card"><p class="t-name">Joel Souza – Terapeuta</p><p>“A minha maior trava estava em como vender meu produto [...] vencer as limitantes sobre ser empresário.”</p></article>
        <!-- Amanda -->
        <article class="t-card"><p class="t-name">Amanda Aragão — Dentista e empresária</p><p>“O processo de mentoria foi um divisor de águas [...] direção clara para conquistar o que está por vir.”</p></article>
        <!-- Joice e Adriano -->
        <article class="t-card"><p class="t-name">Joice e Adriano — Empresários</p><p>“Após trabalharmos o fluxo de caixa [...] fluxo de caixa melhorou muito.”</p></article>
        <!-- Juciele -->
        <article class="t-card"><p class="t-name">Juciele Cadore — Empresária</p><p>“A cada encontro é uma nova descoberta [...] melhor coisa que me aconteceu!”</p></article>
        <!-- Alini -->
        <article class="t-card"><p class="t-name">Alini de Paris — Consultora financeira</p><p>“Antes da Mentoria ALANC eu estava cheia de dúvidas [...] preparada para construir a vida e a carreira que desejo.”</p></article>
        <!-- Karine e Edson -->
        <article class="t-card"><p class="t-name">Karine e Edson — Empresários</p><p>“O que percebemos foi a necessidade de fortalecer nossa união [...] nos conectou ainda mais como casal e como família.”</p></article>
      </div>
    </div>
  </section>

  <!-- (restante: diferenciais, FAQ, CTA final, rodapé, WhatsApp, JS iguais ao anterior) -->

</body>
</html>
