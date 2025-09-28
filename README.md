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
      --pink:#E91E63;      /* rosa principal do logo */
      --pink-2:#FDE8F1;    /* rosa claro para fundos */
      --red:#D61E1E;       /* vermelho para destaques e CTA */
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

    /* Listas marcadas */
    .list-check li{list-style:none;padding-left:28px;position:relative}
    .list-check li:before{content:"✓";position:absolute;left:0;top:0;color:var(--ok);font-weight:900}
    .list-dot li{list-style:none;padding-left:28px;position:relative}
    .list-dot li:before{content:"•";position:absolute;left:6px;top:0;color:var(--red);font-weight:900}

    /* Bio */
    .bio{display:grid;gap:24px;align-items:center}
    .bio img{border-radius:16px;box-shadow:0 12px 28px rgba(0,0,0,.08)}
    @media(min-width:900px){.bio{grid-template-columns:360px 1fr}}

    /* Depoimentos (apenas rosa) */
    .testimonials{display:grid;gap:18px}
    @media(min-width:900px){.testimonials{grid-template-columns:1fr 1fr}}
    .t-card{border:1px solid #F7CDD0;border-radius:16px;padding:16px 18px;background:var(--pink-2);box-shadow:0 8px 22px rgba(0,0,0,.05)}
    .t-name{font-weight:900;margin:0 0 6px;font-size:16px;color:var(--ink)}

    /* FAQ — pergunta vermelha / resposta rosa */
    .faq{max-width:980px;margin:0 auto}
    .faq-item{margin:12px 0;border-radius:14px;overflow:hidden;box-shadow:0 6px 18px rgba(0,0,0,.06);border:1px solid var(--line)}
    .faq-q{width:100%;text-align:left;background:var(--red);border:0;padding:16px 18px;font-size:18px;font-weight:900;color:#fff;cursor:pointer;display:flex;justify-content:space-between;align-items:center}
    .faq-q .mark{flex:0 0 auto;font-weight:900;color:#fff}
    .faq-q:focus{outline:3px solid #ffd1d9}
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

    /* Foco visível */
    a:focus, .btn:focus, .faq-q:focus{outline:3px solid #ffd1d9; outline-offset:2px; border-radius:12px}
    /* 🔥 Remover header padrão do GitHub Pages */
header, .page-header, .site-header, .project-name, .project-tagline {
  display: none !important;
}
  </style>
</head>
<body>

  <!-- Cabeçalho -->
  <div class="top-bar" role="banner">Mentoria ALANC — Alavancagem de Carreira e Negócios</div>

  <!-- HERO -->
  <header class="hero" aria-labelledby="titulo-hero">
    <div class="wrap">
      <div class="hero-card">
        <img src="logo.jpeg" alt="Logo Mentoria ALANC" class="logo" width="600" height="200">
        <h1 id="titulo-hero">Alavancagem de Carreira e Negócios com Clareza, Propósito e Equilíbrio</h1>
        <p class="lead"><strong>Alavanque sua carreira e seus negócios sem abrir mão da família, do equilíbrio e do propósito.</strong> A Mentoria ALANC é para mulheres e casais que sabem que podem mais, mas não querem crescer sozinhos.</p>
        <div class="divider" aria-hidden="true"></div>
        <div class="cta" role="group" aria-label="Ações principais">
          <a class="btn primary" href="https://forms.gle/3KbznEmAkpgoNaab9" target="_blank" rel="noopener" aria-label="Abrir formulário de aplicação em nova guia">Quero entrar na Mentoria ALANC</a>
          <a class="btn ghost" href="#faq">Perguntas frequentes</a>
        </div>
      </div>
    </div>
  </header>

  <!-- Identificação com a dor -->
  <section id="dor" aria-labelledby="t-dor">
    <div class="wrap">
      <h2 id="t-dor" class="section-title">Você já se pegou pensando…</h2>
      <div class="card">
        <ul class="list-dot">
          <li>“Quero empreender, mas tenho medo de arriscar.”</li>
          <li>“Me sinto presa em uma rotina que não faz mais sentido.”</li>
          <li>“Carrego a culpa de não dar conta da família e do trabalho.”</li>
          <li>“Tenho potencial, mas não sei qual o próximo passo certo.”</li>
        </ul>
        <p style="margin-top:14px"><strong> Não é falta de esforço.</strong> É falta de clareza, método e apoio certo.</p>
      </div>
    </div>
  </section>

  <!-- Transformação prometida -->
  <section id="transformacao" aria-labelledby="t-transf">
    <div class="wrap">
      <h2 id="t-transf" class="section-title">A transformação que você leva</h2>
      <div class="grid two">
        <div class="card pink">
          <h3 class="grad-left">Estratégia & Clareza</h3>
          <ul class="list-check">
            <li>Estruturar seu negócio com clareza e estratégia.</li>
            <li>Alinhar propósito, família e prosperidade — sem abrir mão de nenhum.</li>
          </ul>
        </div>
        <div class="card">
          <h3 class="grad-left">Confiança & Método</h3>
          <ul class="list-check">
            <li>Superar bloqueios emocionais e crenças limitantes.</li>
            <li>Alavancar vendas com método prático e consistente.</li>
            <li>Construir um negócio com alma e impacto real, com Constelação Empresarial como base.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Quem sou eu -->
  <section id="quem-sou" aria-labelledby="t-quem">
    <div class="wrap">
      <h2 id="t-quem" class="section-title">Quem Sou Eu</h2>
      <div class="bio">
        <img src="Alinne.jpg" alt="Foto de Alinne de Pasinatto" width="720" height="540" loading="lazy">
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

  <!-- Para quem é -->
  <section id="publico" aria-labelledby="t-publico">
    <div class="wrap">
      <h2 id="t-publico" class="section-title">Para quem é a Mentoria ALANC</h2>
      <div class="card">
        <ul class="list-check">
          <li>Mulheres em transição de carreira que desejam criar negócios prósperos.</li>
          <li>Casais que querem alinhar vida, propósito e empresa.</li>
          <li>Empreendedores(as) com negócio ativo que querem destravar vendas e crescer.</li>
          <li>Profissionais que desejam transformar carreira em propósito.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Benefícios reais -->
  <section id="beneficios" aria-labelledby="t-beneficios">
    <div class="wrap">
      <h2 id="t-beneficios" class="section-title">Benefícios Reais</h2>
      <div class="grid two">
        <div class="card pink">
          <h3 class="grad-left">Clareza do próximo passo</h3>
          <p>Avançar sem medo de errar.</p>
        </div>
        <div class="card pink">
          <h3 class="grad-left">Equilíbrio</h3>
          <p>Negócios e família convivendo com leveza.</p>
        </div>
        <div class="card pink">
          <h3 class="grad-left">Vendas com propósito</h3>
          <p>Comunicação segura e alinhada a valores.</p>
        </div>
        <div class="card pink">
          <h3 class="grad-left">Negócio com alma</h3>
          <p>Impacto real, conectado à sua história.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Depoimentos (somente rosa) -->
  <section id="depoimentos" aria-labelledby="t-dep">
    <div class="wrap">
      <h2 id="t-dep" class="section-title">Depoimentos Reais de Transformação</h2>
      <div class="testimonials">
        <article class="t-card" aria-label="Depoimento de Joel Souza – Terapeuta">
          <p class="t-name">Joel Souza – Terapeuta</p>
          <p>“A minha maior trava estava em como vender meu produto e como ser o profissional que me tornei hoje. Com a Mentoria ALANC venci bloqueios, medos e desafios de aparecer. Já estou há cinco meses fora da CLT, atuando com segurança. Essa mentoria fortaleceu minhas crenças positivas e me ajudou a vencer as limitantes sobre ser empresário.”</p>
        </article>
        <article class="t-card" aria-label="Depoimento de Amanda Aragão">
          <p class="t-name">Amanda Aragão — Dentista e empresária</p>
          <p>“O processo de mentoria foi um divisor de águas na minha transição para o empreendedorismo. Mais do que clareza profissional, me trouxe leveza emocional e entendimento profundo sobre mim mesma. Hoje me sinto mais preparada, leve e com direção clara para conquistar o que está por vir.”</p>
        </article>
        <article class="t-card" aria-label="Depoimento de Joice e Adriano">
          <p class="t-name">Joice e Adriano — empresária</p>
          <p>“Após trabalharmos o fluxo de caixa a minha empresa mudou completamente. Abrimos espaço para novos clientes do perfil certo, fechamos vários orçamentos e o fluxo de caixa melhorou muito.”</p>
        </article>
        <article class="t-card" aria-label="Depoimento de Juciele Cadore">
          <p class="t-name">Juciele Cadore — empresária</p>
          <p>“A cada encontro é uma nova descoberta, um aprendizado único e maravilhoso. A mentoria transformou minha vida! Todo investimento que fazemos em nós mesmos retorna em dobro.”</p>
        </article>
        <article class="t-card" aria-label="Depoimento de Alini de Paris">
          <p class="t-name">Alini de Paris — Consultora financeira</p>
          <p>“Antes da Mentoria ALANC eu estava cheia de dúvidas: carreira, vida pessoal e até sobre mim mesma. Trabalhei minhas emoções, ganhei clareza e confiança. Fiz uma transição segura e alinhada ao que eu realmente queria.”</p>
        </article>
      </div>
    </div>
  </section>

  <!-- Diferenciais -->
  <section id="diferenciais" aria-labelledby="t-dif">
    <div class="wrap">
      <h2 id="t-dif" class="section-title">Por que a Mentoria ALANC é Diferente?</h2>
      <div class="card">
        <p><strong>Estratégia de negócios + Constelação empresarial + Inteligência emocional.</strong> Você não aprende só a vender. Aprende a crescer com equilíbrio, respeitando sua história, seu propósito e a sua família.</p>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq" aria-labelledby="t-faq">
    <div class="wrap">
      <h2 id="t-faq" class="section-title">Perguntas Frequentes</h2>
      <div class="faq" role="list">

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false"><span>Como faço minha aplicação?</span><span class="mark">+</span></button>
          <div class="faq-a" aria-hidden="true"><div class="faq-a-inner">
            Clique em <strong>“Quero entrar na Mentoria ALANC”</strong>. O formulário abre em nova guia para você preencher.
          </div></div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false"><span>Para quem é a mentoria?</span><span class="mark">+</span></button>
          <div class="faq-a" aria-hidden="true"><div class="faq-a-inner">
            Mulheres em transição, casais empreendedores, quem já tem negócio e quer destravar vendas, e profissionais que buscam propósito na carreira.
          </div></div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false"><span>Preciso ter empresa aberta?</span><span class="mark">+</span></button>
          <div class="faq-a" aria-hidden="true"><div class="faq-a-inner">
            Não. O importante é compromisso com um caminho prático, sustentável e alinhado aos seus valores.
          </div></div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false"><span>Qual é a abordagem de trabalho?</span><span class="mark">+</span></button>
          <div class="faq-a" aria-hidden="true"><div class="faq-a-inner">
            Método de gestão e vendas somado à Constelação Empresarial e desenvolvimento emocional para decisões maduras e consistentes.
          </div></div>
        </div>

      </div>
    </div>
  </section>

  <!-- CTA final -->
  <section aria-labelledby="t-cta" style="padding:32px 0">
    <div class="wrap">
      <div class="footer-cta">
        <div>
          <div style="font-weight:800;color:var(--red);letter-spacing:.06em;text-transform:uppercase;font-size:12px">Pronta(o) para alavancar?</div>
          <h3 id="t-cta" style="margin:6px 0 0;font-size:22px;color:var(--ink)">Agora é a sua vez de crescer com clareza, propósito e equilíbrio.</h3>
        </div>
        <div class="cta" style="margin:0">
          <a class="btn primary" href="https://forms.gle/3KbznEmAkpgoNaab9" target="_blank" rel="noopener" aria-label="Abrir formulário de aplicação">Fazer minha aplicação</a>
          <a class="btn ghost" href="https://wa.me/5549999726831?text=Quero%20saber%20mais%20sobre%20a%20Mentoria%20ALANC" target="_blank" rel="noopener">Falar no WhatsApp</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Rodapé -->
  <footer role="contentinfo">
    © Mentoria ALANC — Todos os direitos reservados.
  </footer>

  <!-- Botão flutuante WhatsApp -->
  <a class="whats-float" href="https://wa.me/5549999726831?text=Quero%20saber%20mais%20sobre%20a%20Mentoria%20ALANC" 
     target="_blank" rel="noopener" aria-label="Falar no WhatsApp">
    <svg viewBox="0 0 24 24" aria-hidden="true">
      <path d="M20.5 3.5A10 10 0 0 0 3.2 17.7L2 22l4.4-1.2A10 10 0 1 0 20.5 3.5Zm-8.4 2.2c4.1 0 7.4 3.3 7.4 7.4a7.4 7.4 0 0 1-10.1 6.8l-.3-.1-2.6.7.7-2.5-.1-.3a7.4 7.4 0 0 1 5-11.9Zm4.2 9.8c-.2.6-1.1 1-1.5 1.1-.4.1-.9.1-1.5 0s-1.5-.5-2.6-1.1c-1-.6-1.8-1.6-2.1-2.1-.3-.5-.5-1.3-.1-1.9.2-.3.5-.8.8-.8h.6c.1 0 .4-.1.6.5.2.6.8 2 .9 2.2.1.2.1.4 0 .6s-.2.4-.4.6c-.2.2-.4.4-.2.7.2.3.9 1.4 2.1 2 .9.5 1.6.6 1.9.4.3-.2.4-.5.6-.8.2-.3.5-.4.8-.3l1.9.9c.3.1.5.3.6.5Z"/>
    </svg>
  </a>

  <!-- JS do FAQ (abre um por vez + ARIA) -->
  <script>
    (function(){
      const items = document.querySelectorAll('.faq-item');
      items.forEach((item) => {
        const btn = item.querySelector('.faq-q');
        const panel = item.querySelector('.faq-a');
        btn.addEventListener('click', () => {
          // fecha os outros
          items.forEach(i => {
            if(i !== item){
              i.classList.remove('open');
              const b = i.querySelector('.faq-q');
              const p = i.querySelector('.faq-a');
              b && b.setAttribute('aria-expanded','false');
              p && p.setAttribute('aria-hidden','true');
            }
          });
          // alterna este
          const isOpen = item.classList.toggle('open');
          btn.setAttribute('aria-expanded', isOpen ? 'true' : 'false');
          panel.setAttribute('aria-hidden', isOpen ? 'false' : 'true');
        });
      });
    })();
  </script>
</body>
</html>
