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
      --red:#D61E1E;       /* vermelho */
      --ink:#0F172A;       /* texto principal */
      --soft:#667085;      /* texto secundário */
      --line:#E9EEF5;      /* linhas divisórias */
      --bg:#FFFFFF;        /* fundo branco */
      --ok:#10B981;        /* ícones de check */
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

    /* Cabeçalho vermelho */
    .top-bar{
      background:var(--red); color:#fff; text-align:center;
      padding:14px 10px; font-weight:900; letter-spacing:.04em; text-transform:uppercase;
      font-size:clamp(18px,4.4vw,26px)
    }

    /* Hero */
    .hero{padding:34px 0 10px}
    .hero-card{
      background:#fff; border:1px solid var(--line); border-radius:22px;
      padding:28px 22px 30px; box-shadow:0 16px 36px rgba(0,0,0,.06); text-align:center
    }
    .logo{max-height:160px;width:auto;margin:0 auto 16px}
    .hero h1{
      margin:0 0 10px; font-size:clamp(28px,4.6vw,46px); line-height:1.08; font-weight:900; color:var(--ink)
    }
    .hero p.lead{
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

    /* Depoimentos */
    .testimonials{display:grid;gap:18px}
    @media(min-width:900px){.testimonials{grid-template-columns:1fr 1fr}}
    .t-card{border:1px solid #F7CDD0;border-radius:16px;padding:16px 18px;background:var(--pink-2);box-shadow:0 8px 22px rgba(0,0,0,.05)}
    .t-name{font-weight:900;margin:0 0 6px;font-size:16px;color:var(--ink)}

    /* FAQ */
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

  <!-- Cabeçalho -->
  <div class="top-bar" role="banner">Mentoria ALANC — Alavancagem de Carreira e Negócios</div>

  <!-- HERO -->
  <section class="hero" aria-labelledby="titulo-hero">
    <div class="wrap">
      <div class="hero-card">
        <img src="logo.jpeg" alt="Logo Mentoria ALANC" class="logo" width="600" height="200">
        <h1 id="titulo-hero">Alavancagem de Carreira e Negócios com Clareza, Propósito e Equilíbrio</h1>
        <p class="lead"><strong>Alavanque sua carreira e seus negócios sem abrir mão da família, do equilíbrio e do propósito.</strong> A Mentoria ALANC é para mulheres e casais que sabem que podem mais, mas não querem crescer sozinhos.</p>
        <div class="divider"></div>
        <div class="cta">
          <a class="btn primary" href="https://forms.gle/3KbznEmAkpgoNaab9" target="_blank" rel="noopener">Quero entrar na Mentoria ALANC</a>
          <a class="btn ghost" href="#faq">Perguntas frequentes</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Quem sou eu -->
  <section id="quem-sou" aria-labelledby="t-quem">
    <div class="wrap">
      <h2 id="t-quem" class="section-title">Quem Sou Eu</h2>
      <div class="bio">
        <img src="alinne.jpg" alt="Foto de Alinne de Pasinatto" width="720" height="540" loading="lazy">
        <div>
          <h3 class="grad-left">Alinne de Pasinatto</h3>
          <p>Fundadora da Mentoria ALANC, contadora de formação, autora do livro <em>8 Habilidades de um Líder Extraordinário</em> e especialista em desenvolvimento pessoal, empresarial e constelação organizacional.</p>
          <p>Comecei cedo, vendendo roupas e cosméticos aos 16 anos, enfrentei dores profundas na minha família de origem e precisei assumir responsabilidades antes da hora. Transformei essas experiências em força e, com disciplina e conhecimento, criei empresas, escrevi um livro e hoje ajudo mulheres e casais a prosperarem sem perder o que realmente importa: a essência e a família.</p>
          <div class="cta">
            <a class="btn primary" href="https://forms.gle/3KbznEmAkpgoNaab9" target="_blank" rel="noopener">Aplicar para a Mentoria</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Rodapé -->
  <footer>
    © Mentoria ALANC — Todos os direitos reservados.
  </footer>

  <!-- Botão flutuante WhatsApp -->
  <a class="whats-float" href="https://wa.me/5549999726831?text=Quero%20saber%20mais%20sobre%20a%20Mentoria%20ALANC" target="_blank" rel="noopener">
    <svg viewBox="0 0 24 24"><path d="M20.5 3.5A10 10 0 0 0 3.2 17.7L2 22l4.4-1.2A10 10 0 1 0 20.5 3.5Zm-8.4 2.2c4.1 0 7.4 3.3 7.4 7.4a7.4 7.4 0 0 1-10.1 6.8l-.3-.1-2.6.7.7-2.5-.1-.3a7.4 7.4 0 0 1 5-11.9Zm4.2 9.8c-.2.6-1.1 1-1.5 1.1-.4.1-.9.1-1.5 0s-1.5-.5-2.6-1.1c-1-.6-1.8-1.6-2.1-2.1-.3-.5-.5-1.3-.1-1.9.2-.3.5-.8.8-.8h.6c.1 0 .4-.1.6.5.2.6.8 2 .9 2.2.1.2.1.4 0 .6s-.2.4-.4.6c-.2.2-.4.4-.2.7.2.3.9 1.4 2.1 2 .9.5 1.6.6 1.9.4.3-.2.4-.5.6-.8.2-.3.5-.4.8-.3l1.9.9c.3.1.5.3.6.5Z"/></svg>
  </a>

  <!-- JS FAQ -->
  <script>
    (function(){
      const items = document.querySelectorAll('.faq-item');
      items.forEach((item) => {
        const btn = item.querySelector('.faq-q');
        const panel = item.querySelector('.faq-a');
        btn && btn.addEventListener('click', () => {
          items.forEach(i => {
            if(i !== item){
              i.classList.remove('open');
              const b = i.querySelector('.faq-q');
              const p = i.querySelector('.faq-a');
              b && b.setAttribute('aria-expanded','false');
              p && p.setAttribute('aria-hidden','true');
            }
          });
          const isOpen = item.classList.toggle('open');
          btn.setAttribute('aria-expanded', isOpen ? 'true' : 'false');
          panel && panel.setAttribute('aria-hidden', isOpen ? 'false' : 'true');
        });
      });
    })();
  </script>
</body>
</html>
