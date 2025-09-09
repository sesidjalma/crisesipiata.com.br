[InscriçõesMUN.html](https://github.com/user-attachments/files/22239045/InscricoesMUN.html)
<index.html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CRI - Clube de Relações Internacionais SESI Piatã</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 50px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
    }
 /* Menu */
    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }
    
    /* ==================== BARRA COLORIDA (no lugar do banner) ==================== */
    .hero {
      height: 6px;
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    /* ==================== INFORMAÇÕES ==================== */
    .info {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
      display: flex;
      align-items: center;
      gap: 20px;
    }

    .info-left {
      flex: 1;
    }

    .info-right img {
      max-width: 300px;
      border-radius: 10px;
    }

    .info h2 {
      font-size: 2rem;
      font-weight: 900;
      background: linear-gradient(to right, #c81d3c, #012b65);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 20px;
      text-transform: uppercase;
    }

    .info p, .info li, .info strong {
      font-size: 1.1rem;
      text-transform: uppercase;
      font-weight: bold;
      background: linear-gradient(to right, #c81d3c, #012b65);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .link {
      display: block;
      margin-top: 20px;
      font-weight: bold;
      text-transform: uppercase;
      text-decoration: underline;
      color: #012b65;
    }

    /* ==================== COMITÊS ==================== */
    .committees {
      padding: 40px 20px;
      background: #f7f7f7;
      text-align: center;
    }

    .committees h2 {
      font-size: 1.5rem;
      font-weight: 900;
      text-transform: uppercase;
      background: linear-gradient(to right, #c81d3c, #012b65);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      display: inline-block;
      padding: 5px 15px;
      background-color: rgba(0,0,0,0.1);
      border-radius: 6px;
      margin-bottom: 30px;
    }

    .trapezoid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
      justify-content: center;
      margin-bottom: 20px;
    }

    .trapezoid-bottom {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
      justify-content: center;
    }

    .card {
      background-size: cover;
      background-position: center;
      padding: 40px 20px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.3);
      color: white;
      font-weight: 900;
      text-transform: uppercase;
    }

    .card p {
      margin-top: 15px;
      font-size: 0.9rem;
      text-decoration: underline;
    }

    /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }
  /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

<!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0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">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>
    <!-- Botão hambúrguer -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="#" class="highlight">Incrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- Linha colorida -->
  <section class="hero"></section>

  <!-- Informações -->
  <section class="info">
    <div class="info-left">
      <h2>MUN SESI Piatã</h2>
      <p>Pensando em África: continuidades e rupturas</p>
      <p>DATAS:</p> 06 e 07 de Outubro</p>
      <p>HORÁRIO: </p>07h às 18h30</p>
      <p>LOCAL:</p> Escola SESI Piatã</p>
      <p></p> Av. Orlando Gomes, 1737 - Piatã, Salvador - BA</p>
      <p>INSCRIÇÕES:</p> 05 à 15 de Setembro de 2025</p>
           <a href="https://www.instagram.com/sesi.cri" class="link">Dúvidas? Fale com a gente!</a> <a href="mailto:cripiata.sesi@gmail.com">cripiata.sesi@gmail.com</a>
    </div>
    <div class="info-right">
     <img alt="" src="data:image/jpeg;base64,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" />
    </div>
  </section>

  <!-- Comitês -->
  <section class="committees">
    <h2>Confira nossos comitês e se inscreva!</h2>
    <div class="trapezoid">
      <div class="card">
        <a href="pagina-unodc.html">Escritório da ONU sobre Drogas e Crime</a>
      </div>
      <div class="card">
        <a href="pagina-unsc.html">Conselho de Segurança da ONU</a>
      </div>
      <div class="card">
        <a href="pagina-icj.html">Tribunal Penal Internacional Histórico</a>
      </div>
    </div>
    <div class="trapezoid-bottom">
      <div class="card">
        <a href="pagina-unwomen.html">ONU Mulheres</a>
      </div>
      <div class="card">
        <a href="pagina-unhcr.html">Comitê Executivo da ACNUR</a>
      </div>
    </div>
  </section>

  <!-- Rodapé -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>
</body>
</html>

[pagina-unsc.html](https://github.com/user-attachments/files/22239064/pagina-unsc.html)
<pagina-unsc.html/>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clube de Relações Internacionais - CSNU</title>
  <style>
    /* ==================== RESET ==================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 60px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }

    /* ==================== HERO ==================== */
    .bg-gradient {
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    .hero {
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #0d1b2a; /* cor escura legível sobre degradê */
      padding: 20px;
    }

    .hero h1 {
      font-size: 2rem;
      font-weight: 900;
      margin-bottom: 10px;
      color: #0d1b2a; /* cor escura legível */
    }

    .hero p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #0d1b2a; /* cor escura legível */
    }

    .btn-cta {
      background: #012b65;
      color: #fff;
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    .btn-cta:hover {
      background: #c81d3c;
    }

    /* ==================== COMITÊ ==================== */
    .committee-header {
      text-align: center;
      padding: 40px 20px;
      background: #f7f7f7;
    }

    .committee-header h1 {
      color: #012b65;
      margin-bottom: 20px;
    }

    .committee-links a {
      margin: 5px 10px;
      text-decoration: none;
      color: #007bff;
      font-weight: 500;
      display: inline-block;
    }

    .committee-description {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .committee-description h2 {
      color: #012b65;
      margin-bottom: 15px;
    }

    .committee-description p {
      margin-bottom: 15px;
      text-align: justify;
      line-height: 1.6;
    }

    .committee-list {
      text-align: center;
      padding: 40px 20px;
    }

    .committee-list h2 {
      color: #012b65;
      margin-bottom: 10px;
    }

    .committee-list .note {
      font-size: 0.9rem;
      margin-bottom: 20px;
    }

    .country-list {
      max-width: 400px;
      margin: auto;
      text-align: left;
      line-height: 1.8;
    }

    .country-list li a {
      color: #007bff;
      text-decoration: none;
    }

    .country-list li a.unavailable {
      color: #888;
      pointer-events: none;
    }

     /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }

    /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .hero {
        height: auto;
        padding: 60px 20px;
      }

      .hero h1 {
        font-size: 1.6rem;
      }

      .hero p {
        font-size: 0.95rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0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">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>

    <!-- Botão hambúrguer do lado direito -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="https://forms.gle/SEU-LINK" class="highlight">Inscrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero bg-gradient">
    <div class="hero-content">
      <h1>Bem-vindo ao Clube de Relações Internacionais</h1>
      <p>Escola SESI Djalma Pessoa</p>
    </div>
  </section>

  <!-- COMITÊ CSNU -->
  <section class="committee-header">
    <h1>Comitê: Conselho de Segurança das Nações Unidas</h1>
    <div class="committee-links">
      <a href="https://forms.gle/SEU-LINK">📄 Inscrição</a> 
      <a href="#">🌍 Lista de Países</a>
      <a href="#">📘 Manual</a>
      <a href="#">📑 Guia de Estudos</a>
    </div>
  </section>

  <section class="committee-description">
    <h2>Enfrentamentos aos Grupos Paramilitares na Região do Sahel</h2>
    <p>
      O Conselho de Segurança (CSNU) é o principal órgão da ONU responsável pela manutenção da paz e segurança internacionais. Criado em 1945 pela Carta das Nações Unidas, desempenha papel central em situações de conflito, podendo autorizar missões de paz, sanções econômicas e, em casos extremos, o uso da força militar. Considerado um dos comitês mais estratégicos em simulações, o CSNU desafia os delegados a lidar com disputas geopolíticas, crises armadas e ameaças à estabilidade internacional.
    </p>
    <p>
      O Conselho é formado por 15 membros, sendo 5 permanentes com poder de veto (China, Estados Unidos, França, Reino Unido e Rússia) e 10 membros não permanentes eleitos por mandatos de dois anos. Suas sessões podem ser convocadas a qualquer momento, dada a natureza emergencial de sua função. Nas simulações, os delegados devem propor resoluções, negociar alianças e buscar equilíbrio entre interesses nacionais e a preservação da paz global.
    </p>
  </section>

  <!-- LISTA DE PAÍSES -->
  <section class="committee-list">
    <h2>Lista de Países Envolvidos</h2>
    <p class="note">(Os nomes na cor cinza estão indisponíveis)<br>

    <ol class="country-list">
      <li><a href="#">Burkina Faso - Dupla</a></li>
      <li><a href="#">Estados Unidos da América - Dupla</a></li>
      <li><a href="#">Federação Russa - Dupla</a></li>
      <li><a href="#">República da França - Dupla</a></li>
      <li><a href="#">Reino Unido da Grã-Bretanha e Irlanda do Norte - Dupla</a></li>
      <li><a href="#">República Federativa do Brasil - Dupla</a></li>
      <li><a href="#">República da Alemanha - Dupla</a></li>
      <li><a href="#">República Democrática Federal da Etiópia - Dupla</></li>
      <li><a href="#">República do Chade - Dupla</a></li>
      <li><a href="#">República do Mali - Dupla</a></li>
      <li><a href="#">República do Níger - Dupla</a></li>
      <li><a href="#">República do Senegal - Dupla</a></li>
      <li><a href="#">República do Sudão - Dupla</a></li>
      <li><a href="#">República Federal da Nigéria - Dupla</a></li>
      <li><a href="#">República Islâmica da Mauritânia - Dupla</a></li>
      <li><a href="#">República Popular da China - Dupla</a></li>
      <!-- resto da lista -->
    </ol>
  </section>

  <!-- RODAPÉ -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <!-- SCRIPT MENU HAMBÚRGUER -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>
</body>
</html>

[pagina-unodc.html](https://github.com/user-attachments/files/22239065/pagina-unodc.html)
<pagina-unodc.html/>
<html lang="pt-BR">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clube de Relações Internacionais - UNDOC</title>
  <style>
    /* ==================== RESET ==================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 60px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }

    /* ==================== HERO ==================== */
    .bg-gradient {
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    .hero {
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #0d1b2a; /* cor escura legível sobre degradê */
      padding: 20px;
    }

    .hero h1 {
      font-size: 2rem;
      font-weight: 900;
      margin-bottom: 10px;
      color: #0d1b2a; /* cor escura legível */
    }

    .hero p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #0d1b2a; /* cor escura legível */
    }

    .btn-cta {
      background: #012b65;
      color: #fff;
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    .btn-cta:hover {
      background: #c81d3c;
    }

    /* ==================== COMITÊ ==================== */
    .committee-header {
      text-align: center;
      padding: 40px 20px;
      background: #f7f7f7;
    }

    .committee-header h1 {
      color: #012b65;
      margin-bottom: 20px;
    }

    .committee-links a {
      margin: 5px 10px;
      text-decoration: none;
      color: #007bff;
      font-weight: 500;
      display: inline-block;
    }

    .committee-description {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .committee-description h2 {
      color: #012b65;
      margin-bottom: 15px;
    }

    .committee-description p {
      margin-bottom: 15px;
      text-align: justify;
      line-height: 1.6;
    }

    .committee-list {
      text-align: center;
      padding: 40px 20px;
    }

    .committee-list h2 {
      color: #012b65;
      margin-bottom: 10px;
    }

    .committee-list .note {
      font-size: 0.9rem;
      margin-bottom: 20px;
    }

    .country-list {
      max-width: 400px;
      margin: auto;
      text-align: left;
      line-height: 1.8;
    }

    .country-list li a {
      color: #007bff;
      text-decoration: none;
    }

    .country-list li a.unavailable {
      color: #888;
      pointer-events: none;
    }

   /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }

    /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .hero {
        height: auto;
        padding: 60px 20px;
      }

      .hero h1 {
        font-size: 1.6rem;
      }

      .hero p {
        font-size: 0.95rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0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">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>

    <!-- Botão hambúrguer do lado direito -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="https://forms.gle/SEU-LINK" class="highlight">Inscrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero bg-gradient">
    <div class="hero-content">
      <h1>Bem-vindo ao Clube de Relações Internacionais</h1>
      <p>Escola SESI Djalma Pessoa</p>
    </div>
  </section>

  <!-- COMITÊ CSNU -->
  <section class="committee-header">
    <h1>Comitê: Escritório das Nações Unidas Sobre Drogas e Crime</h1>
    <div class="committee-links">
      <a href="https://forms.gle/SEU-LINK">📄 Inscrição</a> 
      <a href="#">🌍 Lista de Países</a>
      <a href="#">📘 Manual</a>
      <a href="#">📑 Guia de Estudos</a>
    </div>
  </section>

  <section class="committee-description">
    <h2> <p>Tema: Pirataria na Somália - Impactos globais dos crimes marítimos no chifre africano</h2>
    <p>
      O Escritório das Nações Unidas sobre Drogas e Crime (UNODC), criado em 1997, é a agência responsável por liderar os esforços internacionais no combate ao crime organizado transnacional, tráfico de drogas, corrupção, terrorismo e crimes cibernéticos. Sua missão é fortalecer a cooperação internacional e apoiar os Estados-membros na criação de políticas de prevenção e justiça criminal. Nas simulações, o UNODC proporciona debates sobre desafios globais contemporâneos, que exigem equilíbrio entre segurança, direitos humanos e desenvolvimento sustentável.
    </p>
     <h4>Estrutura e Funcionamento:</h4>
    <p>
      O UNODC tem sede em Viena e atua em mais de 80 países por meio de escritórios regionais. Seus trabalhos são guiados pela Comissão de Entorpecentes e pela Comissão de Prevenção ao Crime e Justiça Criminal. Nas simulações, os delegados representam Estados-membros e organismos parceiros, discutindo estratégias multilaterais para enfrentar crimes transnacionais e reduzir os impactos sociais do narcotráfico e da criminalidade organizada.
    </p>
  </section>

  <!-- LISTA DE PAÍSES -->
  <section class="committee-list">
    <h2>Lista de Países Envolvidos</h2>
     <h5>COMITÊ INDIVIDUAL!</h5>
    <p class="note">(Os nomes na cor cinza estão indisponíveis)<br>


    <ol class="country-list">
      <li><a href="#">Emirados Árabes Unidos</a></li>
      <li><a href="#">Estado do Japão</a></li>
      <li><a href="#">Estados Unidos da América</a></li>
      <li><a href="#">Federação Russa</</a></li>
      <li><a href="#">Reino da Arábia Saudita</a></li>
      <li><a href="#">Reino Unido da Grã-Bretanha e Irlanda do Norte</a></li>
      <li><a href="#">República Árabe do Egito</a></li>
      <li><a href="#">República da África do Sul</></li>
      <li><a href="#">República da Coreia</a></li>
      <li><a href="#">Reino da Espanha</a></li> 
      <li><a href="#">República do Iêmen</a></li> 
      <li><a href="#">República do Quênia</a></li> 
      <li><a href="#">República Federal da Alemanha</a></li> 
      <li><a href="#">República Popular da China</a></li> 
      <li><a href="#">República Federativa do Brasil</a></li> 
      <li><a href="#">República da França</a></li>
      <li><a href="#">República da Índia</a></li>
      <li><a href="#">República da Turquia</a></li>
      <li><a href="#">República das Seicheles</a></li>
      <li><a href="#">República do Djibuti</a></li>
      <li><a href="#">República Popular de Bangladesh
      </a></li>
      <li><a href="#">República Federal da Somália</a></li>
      <!-- resto da lista -->
    </ol>
  </section>

  <!-- RODAPÉ -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <!-- SCRIPT MENU HAMBÚRGUER -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>

</body>
</html>

[pagina-icj.html](https://github.com/user-attachments/files/22239076/pagina-icj.html)
 <index.html/>
<html lang="pt-BR">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clube de Relações Internacionais - Tpi Histórico</title>
  <style>
    /* ==================== RESET ==================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 60px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }

    /* ==================== HERO ==================== */
    .bg-gradient {
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    .hero {
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #0d1b2a; /* cor escura legível sobre degradê */
      padding: 20px;
    }

    .hero h1 {
      font-size: 2rem;
      font-weight: 900;
      margin-bottom: 10px;
      color: #0d1b2a; /* cor escura legível */
    }

    .hero p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #0d1b2a; /* cor escura legível */
    }

    .btn-cta {
      background: #012b65;
      color: #fff;
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    .btn-cta:hover {
      background: #c81d3c;
    }

    /* ==================== COMITÊ ==================== */
    .committee-header {
      text-align: center;
      padding: 40px 20px;
      background: #f7f7f7;
    }

    .committee-header h1 {
      color: #012b65;
      margin-bottom: 20px;
    }

    .committee-links a {
      margin: 5px 10px;
      text-decoration: none;
      color: #007bff;
      font-weight: 500;
      display: inline-block;
    }

    .committee-description {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .committee-description h2 {
      color: #012b65;
      margin-bottom: 15px;
    }

    .committee-description p {
      margin-bottom: 15px;
      text-align: justify;
      line-height: 1.6;
    }

    .committee-list {
      text-align: center;
      padding: 40px 20px;
    }

    .committee-list h2 {
      color: #012b65;
      margin-bottom: 10px;
    }

    .committee-list .note {
      font-size: 0.9rem;
      margin-bottom: 20px;
    }

    .country-list {
      max-width: 400px;
      margin: auto;
      text-align: left;
      line-height: 1.8;
    }

    .country-list li a {
      color: #007bff;
      text-decoration: none;
    }

    .country-list li a.unavailable {
      color: #888;
      pointer-events: none;
    }

   /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }

    /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .hero {
        height: auto;
        padding: 60px 20px;
      }

      .hero h1 {
        font-size: 1.6rem;
      }

      .hero p {
        font-size: 0.95rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0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">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>

    <!-- Botão hambúrguer do lado direito -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="https://forms.gle/SEU-LINK" class="highlight">Inscrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero bg-gradient">
    <div class="hero-content">
      <h1>Bem-vindo ao Clube de Relações Internacionais</h1>
      <p>Escola SESI Djalma Pessoa</p>
    </div>
  </section>

  <!-- COMITÊ CSNU -->
  <section class="committee-header">
    <h1>Comitê: Tribunal Penal Internacional Histórico</h1>
    <div class="committee-links">
      <a href="https://forms.gle/SEU-LINK">📄 Inscrição</a> 
      <a href="#">🌍 Lista de Países</a>
      <a href="#">📘 Manual</a>
      <a href="#">📑 Guia de Estudos</a>
    </div>
  </section>

  <section class="committee-description">
    <h2> <p>Tema: Acusação contra Omar Hassan Ahmad al-Bashir (a situação em Darfur/2009)</h2>
    <p>
      O Tribunal Penal Internacional Histórico (TPI Histórico) é um comitê de caráter jurídico que simula julgamentos de crimes de guerra, genocídios e crimes contra a humanidade em contextos específicos do passado. Diferente do Tribunal Penal Internacional contemporâneo, sua proposta é revisitar casos históricos de relevância internacional, promovendo debates que unem justiça, memória histórica e diplomacia. O comitê proporciona aos delegados a oportunidade de aprofundar-se em argumentos jurídicos, explorar dilemas éticos e compreender o impacto político dos julgamentos no cenário mundial.
    </p>
     <h4>Estrutura e Funcionamento:</h4>
    <p>
     O TPI Histórico é composto por juízes, promotores e defesa, que desempenham papéis fundamentais na análise dos casos. Os participantes devem utilizar princípios do direito internacional e tratados aplicáveis à época dos acontecimentos julgados. As sessões são caracterizadas por sustentações orais, apresentação de provas e elaboração de votos, exigindo dos delegados argumentação sólida, raciocínio crítico e rigor jurídico.
    </p>
  </section>

  <!-- LISTA DE PAÍSES -->
  <section class="committee-list">
     <h5>COMITÊ COM PARTICIPAÇÃO EXCLUSIVA DE CONVIDADOS!</h5>

  </section>

  <!-- RODAPÉ -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <!-- SCRIPT MENU HAMBÚRGUER -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>
</body>
</html>


[pagina-unwomen.html](https://github.com/user-attachments/files/22239124/pagina-unwomen.html)
<pagina-unwomen.html/>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clube de Relações Internacionais - ONU Mulheres</title>
  <style>
    /* ==================== RESET ==================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 60px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }

    /* ==================== HERO ==================== */
    .bg-gradient {
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    .hero {
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #0d1b2a; /* cor escura legível sobre degradê */
      padding: 20px;
    }

    .hero h1 {
      font-size: 2rem;
      font-weight: 900;
      margin-bottom: 10px;
      color: #0d1b2a; /* cor escura legível */
    }

    .hero p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #0d1b2a; /* cor escura legível */
    }

    .btn-cta {
      background: #012b65;
      color: #fff;
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    .btn-cta:hover {
      background: #c81d3c;
    }

    /* ==================== COMITÊ ==================== */
    .committee-header {
      text-align: center;
      padding: 40px 20px;
      background: #f7f7f7;
    }

    .committee-header h1 {
      color: #012b65;
      margin-bottom: 20px;
    }

    .committee-links a {
      margin: 5px 10px;
      text-decoration: none;
      color: #007bff;
      font-weight: 500;
      display: inline-block;
    }

    .committee-description {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .committee-description h2 {
      color: #012b65;
      margin-bottom: 15px;
    }

    .committee-description p {
      margin-bottom: 15px;
      text-align: justify;
      line-height: 1.6;
    }

    .committee-list {
      text-align: center;
      padding: 40px 20px;
    }

    .committee-list h2 {
      color: #012b65;
      margin-bottom: 10px;
    }

    .committee-list .note {
      font-size: 0.9rem;
      margin-bottom: 20px;
    }

    .country-list {
      max-width: 400px;
      margin: auto;
      text-align: left;
      line-height: 1.8;
    }

    .country-list li a {
      color: #007bff;
      text-decoration: none;
    }

    .country-list li a.unavailable {
      color: #888;
      pointer-events: none;
    }

   /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }

    /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .hero {
        height: auto;
        padding: 60px 20px;
      }

      .hero h1 {
        font-size: 1.6rem;
      }

      .hero p {
        font-size: 0.95rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0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">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>

    <!-- Botão hambúrguer do lado direito -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="https://forms.gle/SEU-LINK" class="highlight">Inscrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero bg-gradient">
    <div class="hero-content">
      <h1>Bem-vindo ao Clube de Relações Internacionais</h1>
      <p>Escola SESI Djalma Pessoa</p>
    </div>
  </section>

  <!-- COMITÊ CSNU -->
  <section class="committee-header">
    <h1>Comitê: ONU Mulheres</h1>
    <div class="committee-links">
      <a href="https://forms.gle/SEU-LINK">📄 Inscrição</a> 
      <a href="#">🌍 Lista de Países</a>
      <a href="#">📘 Manual</a>
      <a href="#">📑 Guia de Estudos</a>
    </div>
  </section>

  <section class="committee-description">
    <h2>Convenção da União Africana sobre o fim da violência contra mulheres e meninas: Perspectivas femininas no processo de enfrentamento à violência de gênero em África</h2>
    <p>
      A ONU Mulheres é a entidade das Nações Unidas dedicada à igualdade de gênero e ao empoderamento feminino, criada em 2010 para unificar esforços já existentes dentro do sistema ONU. Seu objetivo central é a promoção dos direitos das mulheres e a eliminação de barreiras estruturais que limitam sua participação plena na sociedade. Em simulações, os delegados discutem temas como violência de gênero, desigualdade econômica, representatividade política e acesso à educação, articulando soluções internacionais para esses desafios.
    </p>
     <h2>Estrutura e Funcionamento</h2>
    <p>
      Com sede em Nova Iorque, a ONU Mulheres conta com o apoio dos Estados-membros da ONU e trabalha em cooperação com outras agências e organismos internacionais. Suas sessões no âmbito das simulações são compostas por representantes de diferentes países que propõem recomendações, elaboram resoluções e buscam consenso em torno de políticas públicas globais.
    </p>
  </section>

  <!-- LISTA DE PAÍSES -->
  <section class="committee-list">
    <h2>Lista de Países Envolvidos</h2>
     <h5>COMITÊ EXCLUSIVO PARA MULHERES!</h5>
    <p class="note">(Os nomes na cor cinza estão indisponíveis)<br>


    <ol class="country-list">
      <li><a href="#">Burkina Faso</a></li>
      <li><a href="#">Reino de Marrocos</a></li>
      <li><a href="#">República Árabe do Egito</a></li>
      <li><a href="#">República da África do Sul</</a></li>
      <li><a href="#">República da Tunísia</a></li>
      <li><a href="#">República de Angola</a></li>
      <li><a href="#">República de Moçambique</a></li>
      <li><a href="#">República de Ruanda</></li>
      <li><a href="#">República Democrática do Congo</a></li>
      <li><a href="#">República do Botsuana</a></li>
      <li><a href="#">República do Djibuti</a></li>
      <li><a href="#">República do Quênia</a></li>
      <li><a href="#">República do Sudão do Sul</a></li>
      <li><a href="#">República do Zimbábue</a></li>
      <li><a href="#">República Federal da Nigéria
      </a></li>
      <li><a href="#">República Federal da Somália</a></li>
      <!-- resto da lista -->
    </ol>
  </section>

  <!-- RODAPÉ -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <!-- SCRIPT MENU HAMBÚRGUER -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>

</body>
</html>

[pagina-unhcr.html](https://github.com/user-attachments/files/22239129/pagina-unhcr.html)
<pagina-unhcr.html/>
<html lang="pt-BR">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clube de Relações Internacionais - ExCOM</title>
  <style>
    /* ==================== RESET ==================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* ==================== CABEÇALHO ==================== */
    .top-bar {
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      border-bottom: 2px solid #e5e5e5;
      flex-wrap: wrap;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 60px;
    }

    .club-name h1 {
      font-size: 1.2rem;
      font-weight: 900;
      color: #000;
    }

    .club-name span {
      font-size: 0.85rem;
      font-weight: 500;
      background: #fff;
      border: 1px solid #ccc;
      padding: 2px 6px;
      border-radius: 12px;
      display: inline-block;
      margin-top: 3px;
    }

    nav ul {
      display: flex;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    nav ul li a.highlight {
      background: #012b65;
      color: #fff;
      padding: 8px 14px;
      border-radius: 6px;
      font-weight: bold;
      transition: background 0.3s;
    }

    nav ul li a.highlight:hover {
      background: #c81d3c;
    }

    /* Botão hambúrguer */
    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
      user-select: none;
    }

    /* ==================== HERO ==================== */
    .bg-gradient {
      background: linear-gradient(to right, #c81d3c, #ffffff, #012b65);
    }

    .hero {
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #0d1b2a; /* cor escura legível sobre degradê */
      padding: 20px;
    }

    .hero h1 {
      font-size: 2rem;
      font-weight: 900;
      margin-bottom: 10px;
      color: #0d1b2a; /* cor escura legível */
    }

    .hero p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #0d1b2a; /* cor escura legível */
    }

    .btn-cta {
      background: #012b65;
      color: #fff;
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    .btn-cta:hover {
      background: #c81d3c;
    }

    /* ==================== COMITÊ ==================== */
    .committee-header {
      text-align: center;
      padding: 40px 20px;
      background: #f7f7f7;
    }

    .committee-header h1 {
      color: #012b65;
      margin-bottom: 20px;
    }

    .committee-links a {
      margin: 5px 10px;
      text-decoration: none;
      color: #007bff;
      font-weight: 500;
      display: inline-block;
    }

    .committee-description {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .committee-description h2 {
      color: #012b65;
      margin-bottom: 15px;
    }

    .committee-description p {
      margin-bottom: 15px;
      text-align: justify;
      line-height: 1.6;
    }

    .committee-list {
      text-align: center;
      padding: 40px 20px;
    }

    .committee-list h2 {
      color: #012b65;
      margin-bottom: 10px;
    }

    .committee-list .note {
      font-size: 0.9rem;
      margin-bottom: 20px;
    }

    .country-list {
      max-width: 400px;
      margin: auto;
      text-align: left;
      line-height: 1.8;
    }

    .country-list li a {
      color: #007bff;
      text-decoration: none;
    }

    .country-list li a.unavailable {
      color: #888;
      pointer-events: none;
    }

   /* ==================== RODAPÉ ==================== */
    .footer {
      background: linear-gradient(to right, #012b65, #c81d3c);
      color: #fff;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .info {
        flex-direction: column;
        text-align: center;
      }
      .trapezoid, .trapezoid-bottom {
        grid-template-columns: 1fr;
      }
    }

    /* ==================== RESPONSIVIDADE ==================== */
    @media (max-width: 768px) {
      .top-bar {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
      }

      nav {
        display: none;
        width: 100%;
        background: #fff;
        border-top: 1px solid #ccc;
      }

      nav.active {
        display: block;
      }

      nav ul {
        flex-direction: column;
        padding: 10px 0;
      }

      nav ul li {
        margin: 10px 0;
        text-align: center;
      }

      nav ul li a {
        display: block;
        padding: 10px;
        font-size: 1.1rem;
      }

      .menu-toggle {
        display: block;
        color: #012b65;
      }

      .club-name h1 {
        font-size: 1rem;
      }

      .hero {
        height: auto;
        padding: 60px 20px;
      }

      .hero h1 {
        font-size: 1.6rem;
      }

      .hero p {
        font-size: 0.95rem;
      }

      .committee-header h1 {
        font-size: 1.3rem;
      }

      .committee-description h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- CABEÇALHO -->
  <header class="top-bar">
    <div class="header-left">
      <img alt="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAEumlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4bWxuczp4PSdhZG9iZTpuczptZXRhLyc+CjxyZGY6UkRGIHhtbG5zOnJkZj0naHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyc+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczpBdHRyaWI9J2h0dHA6Ly9ucy5hdHRyaWJ1dGlvbi5jb20vYWRzLzEuMC8nPgogIDxBdHRyaWI6QWRzPgogICA8cmRmOlNlcT4KICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0nUmVzb3VyY2UnPgogICAgIDxBdHRyaWI6Q3JlYXRlZD4yMDI1LTA5LTAzPC9BdHRyaWI6Q3JlYXRlZD4KICAgICA8QXR0cmliOkV4dElkPjVmYzIxODJjLWYyYTItNGM2YS05OTcyLTI4ZTMxNWM4YmU2NTwvQXR0cmliOkV4dElkPgogICAgIDxBdHRyaWI6RmJJZD41MjUyNjU5MTQxNzk1ODA8L0F0dHJpYjpGYklkPgogICAgIDxBdHRyaWI6VG91Y2hUeXBlPjI8L0F0dHJpYjpUb3VjaFR5cGU+CiAgICA8L3JkZjpsaT4KICAgPC9yZGY6U2VxPgogIDwvQXR0cmliOkFkcz4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6ZGM9J2h0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvJz4KICA8ZGM6dGl0bGU+CiAgIDxyZGY6QWx0PgogICAgPHJkZjpsaSB4bWw6bGFuZz0neC1kZWZhdWx0Jz5sb2dvIC0gMTwvcmRmOmxpPgogICA8L3JkZjpBbHQ+CiAgPC9kYzp0aXRsZT4KIDwvcmRmOkRlc2NyaXB0aW9uPgoKIDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PScnCiAgeG1sbnM6cGRmPSdodHRwOi8vbnMuYWRvYmUuY29tL3BkZi8xLjMvJz4KICA8cGRmOkF1dGhvcj5MYXl6YSBDdW5oYSBkb3MgU2FudG9zPC9wZGY6QXV0aG9yPgogPC9yZGY6RGVzY3JpcHRpb24+CgogPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9JycKICB4bWxuczp4bXA9J2h0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8nPgogIDx4bXA6Q3JlYXRvclRvb2w+Q2FudmEgKFJlbmRlcmVyKSBkb2M9REFHeDdPVURaaGsgdXNlcj1VQUdOeE5sRUhPWSBicmFuZD1CQUZuenJYeE4tYyB0ZW1wbGF0ZT08L3htcDpDcmVhdG9yVG9vbD4KIDwvcmRmOkRlc2NyaXB0aW9uPgo8L3JkZjpSREY+CjwveDp4bXBtZXRhPgo8P3hwYWNrZXQgZW5kPSdyJz8+DFS34gAAFeVJREFUeJztmnmUXVWZ9p/33fucc+d7a7ipqqRSqcwTJkBIwhCGgBACAhKJNBqZRInYiqKtgN02rK9VRLuVT1vUBpHGtIgtRAhRMHQIJISATCFknlNDKjXfW/eeeb/9B7SrbZtMBPv7bJ+1zj93rf3c57f2cM5+9yb8LxP9Twf4Y+vPwH/q+qMBTwHQBKATwEIAqwCMAfBZTEUP3sDcP1IO9W6a3wfgeABpAB+npNNq51OzhdCUaLr6PfrEcoO2ChvS1lWa6dVcVIleeTfDvCV9rA1bAXwfCpsTWYDrzh4r3D9Gm94g0stTwKcim08eEHyBuHOWB/s3IrKq063zt+MAADnWcf5AfCzNWgHcwEnda4/5cjEuzlEx/+sWy6uJI30HiWhA7xGDxQysiQ3dSCIjJFCrQyc/7exUY+pYZnk7HZMhfSaAv9dJuphzBdGFeRr6DmHsE+CcOqNXCuR6AQ0zJDcAyAowXojGC1EKShpD7TdPk6BjYlhqX3UsAh1Ex2RIL0ANaig9/wAnFyUE6w3AIjILBFuEvguiNQBOI6Ivx8bsAfGHmOgRADMI0uko+nZvKYm9mEM1eFFq0Ywd2HEsov2B3tEq3QpgPiX1aWpEoyL5phCNEaIXReR6AYYM4acCGl4v3u1dKtlvgONjk26K2D0pZpoUgRpiZickimJCb0S0rU3Mi2GQfzZP5U1rg+4hP4pkA7qPDS3eIfBtACbY474IwngxkgbRBwS0Q0juA5CGrZavd92eSTpxpQEuNUSTDAgRgWIiiYleiYheioiaIqL3RsSpiAghkwmJd4fMy6uhc3/Qn3u5A8vx9P8k8HfsompVgsG4sIoIRRHkBMiCsCli/jwF2BixuVUxXWNAGUOQmPBcDLxkiK+PRd+ciPDDznCD79kTOGlFx0VW9qGIEAZEW2NWF4XEHDJ7AdGyuDL0xZfL7p4O9GIAA0cNfFSr9BJdWyxw4ascNBgDqcSCViHc+0ZcGmdbvECRqRdtnmPGyQbYKyQDAvm0YfM5gD7MLJ953eXv/jTc4N8O4OvBVvNYxV3vhXIRgAyAjUbMtQL0GjHPCyQZZ3PrJjU3fbImkbGLKB418BH38H0AVGbC3DiIf82EBQZ0H0RiAJ2MxF8KuZcYoU8w4bYYPFMIpym4l9ohvzFoOyuEeafjq2uvizZG/9X7ZDTTSdnCqbZlLYskOKvKSUc0PxoQ7w+ZJ4bM1VCpJ9y0+ui26k539+7dRwx8RKv0BNjI27naoXCo01DSNYQHRWQpxdb1Km049N1/AOhc0XRZHGOOQE4nWO93vPjlvqSzgIgmmSh5xcyoI5oHG4QWysKGiwjdiGQ/dgq7o9YZq/KIUc63FOP1UMQSxlgBvkZW/AsTqyVcxfIx2TFXDBQG9g8MHNnwPuweXgjgQl3T6Fq1Pw8lsdAh7xERzAJhpWL9aRNHNwE41zbVeZF2JsZG39sk7kXL/Zq1M6028qxhqwxwggFWhqLXUTz4BqilLcPJakUCu1PCBkuXJgW2nhmxOiMiHhEy/ZsHc1vE9sRIqb/vit1TKJvss8PE0oDZ8yqFec93/TYEdh974L8FI21NH5bQgy8z0S4IpghkYTbufbbC9TcAuLlqgnNzlBgMSdYS010v++Vv9sSQ8626mb4V/gokX4pBUw2p9xhgeExIx0RWRBRHRNUIfCAi2hzArA6Vvixm1ab86uK9bqNOFd2fh8Tkh/bCoXxYx3HyiZDUi3sGS4ur4cbgcHv6sID/FsB5ds3pDyacrtFx6goR+hsCSgL5GQO/BOhhCDrF0BmscCuAGRxm5m4Ot7qTUUWYHn+PALWW374wjoqmwapwO9lpoZZkGo7uRBT3Evmd2DQ03UuFPSgTFYadU3VyPw4r6WkvDXX3nZiNRg3mh73sGfxFj1NZkUrWTo1Ca1XEfNNLWyr3v7n/OkbAAuAr6TG3MWguIPcz6GvM8tWaMPxJr7J/xSRvwFA9iCZAUJsIey95Mux/zgPwXqc2DV2/QRtz+053+4+/d1ixgA+nz0nozODGsBJ8Yv1Q+5OtOAXxyIE7IuaT2vZ3nztQO1IaU7hGtH27hNZJ23Ye6KpizSF9D+u1dBqA/kT8qE80yyf6lkfYG7De3qWdBQGh1jX5z4Swr/YJgc8UDgPtr8NItAIAJ44LCcUG07fCO0xYAOgKt/oR0co4l7ooQlG2YAvISz4QE59UnyzO1p2bpNfN/zQGtoUJ+TvCGYfle0jgVgCT7UKGy+nXA5avBkypgLGvFJZeqjLd7BN9rb36ymA56op9ohEBofeNRN2zzanMPFIj1JDOzPYJWx71+9p+dATAg4GLiPBMDDl/rDNStRSL4/yUf5chsuJa62MZNR+l6m9cUtEdQrwwP7JrInDWOwduRJ6yqfpFYdL/tsvEPuO50NYfjInP9wm8I+hb2g9gSCfP95krkbHPC4DvhFb8k0I68/2A6Fxf04q2I4AFAJOIxBBeDZmHybChr6gUrzaErgi4xTCfxflyzcDAALaZ4lMx8YZUTeVDamT/IX0PuT0cDh+1Opk02r4zJjo7InoyMGZGpJ0LIqLnkkNtj5R4AuVSzk2G0LmzvOn+lUG0Zrjkn2IbV8XEZ4VEe2rt0W/Msag8PjjV1GIHUpiCkbAwAWU0ogZ5jEGIENdiDCbao5WdrG+ILJ4fszovZh4vAf1Vf5/cbpzcRthyK2Xc3/T1NO1rSK2XXE1N2Zf0DfGIunu9XRvidwTcbCXtJjvp+0rtNczvi0GpmOjeiPiGstfz169G7r7mBNLsZP66Elb+5cmg9EoHfAzEPZ0TqeVfPdssjokMcXhzpJPn6/TQOCdZn2vixkSzY6kWW+xaZ1g+bzc1N2WyJ1QL1oIwzX8lDn/FMI2NWFFE/AMHue890/uUjC7N8cNi5cyYdFhId6zdvnc7EpmGPnLqP+9awa89K9iPvr635TnokD4DwEwnPaJkp1f5Slc9ok6XaX6VSPtMkRfKC68DCJxRBY+5mcV9tvWttgEs7KADtT4R3Jg+oN3qDDfOLAuIZlvK+keV7lsZpMymnszwXUOZ5FbJDq51ErJEFF8eErZnSt7FopInh4qfjbVqyXMeALBO+4iVWmWUPhVpSD6fRyLV2CCs0jZy54MO/uI56KflMwByIu028QEi+oEQ9QnwDQK2MOiFRDQ+rsc6xLY/zANJCdjz8lttLYwkooZRvqr0+16+us3d3dnsDt0JnPWNauqZZIamNjo0WAjRYaWo1pQwvBxib1dfUOg/ye/EGrgIS4LsmJpdwvr4J8tPAQAaGl6jmMZvEMXXTpowiazkic4Q23dB6TgR6lMw4RzCtm1vWxw7KPAUAO1cwxRWrhieyC4DqNgbVL5TZ2euB2F9GuukDpPIIx7GxD0pmhr/xwdAgD1SpWCE4vr+NA34azEEYAjAz6WlimoGdTsTGECITqTgoQyBQQc2YwtW/y7BACZ7J+ypydWdl7Sn2ECX396+TbRTtytdGN6wpS3MDDF/Tik9NmL9dbBelNjwGxzs9XdQ4KkA9ab1vSD7BR+0EUS+bafLAXMjiF7YiHryECLUqQJEBl2Ev2vbhhj1drLWVlzqof2/tzPaCwDY+J9+6X/r+X21tExFodh6IPL99KTJSXtfF3zAR7qpUJLACiNJfMrS1id8HV9lxRaFbN1oYVLKQ18F6PpvmQ46h9ejCDGpRyPir/vMF/ukFoiyJnqgggc1uh8DEiOGR6R9pZKSC7m10Pq79rXpmhqPVHk7xwddOd9OmUxA6Zzpj5WdNMwWABQKrSjZNZ5RVlm0fYtbStzUbdp/3Ts6XRZlKRw/Oo1pLW/reVDgLeiWcjp63DPxhwLi7oB5ZVdYWR1oLYHicyYn5jODESoVBqymVrV6oqlxxPhT8qcQAPhKJwOlvc7B7qMuOMfgSqxsy7BWdXWXIJk9NZtync9AOY22St7Rv6t2iRflIbERkCYyzPiDnfZhAk/BFJgISyIncX7AvCNkNSGVzC8ISAchq6l7k+0ntaAFPtRAQKojYNUd+rQqalQ3TJ5wnPZAVqD0O6quG6WjWDuqw0tyTUvulFxLYSW0/ZGY7Wpvc2JTNH0lsHEEsOl0x7AWU1PwUZs7OuCN2AgKnH+IQGdHpM4IiBsM6JmQuSdgzaYmddOu2n0caNXjs05W2L86UvR3QaS/YJthqyPtTA1JO9n0J6k1NQVIpw8btFA4HX2+hX6TtmPtJEnSd6tMzeOGrRdDTs412ulzS71+MNgN2AESxdeKoqwhtfqMIaye87a+h6x4uJ73AuXs0yXiW4T4xEowpNK6pt0IXiXw+XZh/OyAgzYS6Iqbqlc9fLddwMN+Xl0D0E0gUi3N27+T8iY8XGG1tnvCdA9PrJFstgf19fUkIgRkUKkkpbv7RcGU6+GoDVxnZkzhnH9x4OvLRXEyJi55ln92T3difXq415gJ8xkh9ebKNLyDlG4eK1Btgxe8FuG7tx8t8BTsp4YZdWH5R8K8kUiNsxO1/xKA7wTTyRC+BxTdNeSWLk2nansqXmb6Pn97W7Gre3+q2nyHbhy+Vml6nIDJpYz5SR2Ndeo6Khtk+owNIN5DrAZBygexdooqWzt6ehMYk8DTjxeKM2Bna0yqZEi90r+n++N9lWUB0mnkErfUmHxXCkOnbUc5gHWigQn1NIF6FYc4oDrE5mEjXP/F5yLme2LWZ0SsiiHxgxHo5Zj1hEjpn0SsYWeK34pY7842mDmYZNCNbuwp90nP4MhXI7bcUFmfH3Jkhi98SaT0T2PWrmFrZsx6oVHWR42yF4my5hplZQ1bz8akF/dLz0lkqzNDTmyNlbOjVHNViO5uIHsC6ULvcTHbbaVC/yD2/Qh25oSsIevESKWfwgvLD0p0yCFNuh5hQj3i1tfek+oqrxRSsbCMIqP3RhKf7lW7rkhnW1YQca0QpW3KcAAYYA9M3dZypIvrAHVJ+94tt6GnpxMTnDXYulVQ9wWMOGWQxg814oAziI37AsHGZ4HifkJQFEgbyucv0sXe/EwQ/Tjyim/23AWzxbzG5wjxM7A3C0ZcB2lvniSZ/XVuPnoar286OM+hgLN1Z+pcHT8pxHUC5RCrcaXu7XMzDZMuBni235N8r4wMxiQC9QuAmikOTh/YuW+9674EjJmG5trpiwR8Z7dlpgSbnh3AwO5D/eWbmnYpsmPPnpytDK0rOzVnlnc89QoqL8CadkW6EDftBOG67l2rl6FhsdRltn5PwMVKyr7c/9k15mC2h9wPl3sRlXrrPmpIbRdWiZhUmGp4zzaYxBOGrWkyOp45sH7K5t7eyrkx212RnX3cnjrjfYnJlzrIj0bZLj0Ws11tCK3FPHbR4dfBbZ9S1ep5MdvtnmO/ho0/B1LLkaTRlxm23EqNWovqAcnZr40wpBZZIg/4ry8/KOxhAQOrUO7N7Y5Jb4pZ/5shHRim/xtadG7M1kPs2Z9HzqdwRE+Hx+6XjLKbLDK/yGSLS7NOy7xqolD1dOrLvp2+MVOtjsd/+hI7mNKtFypD9kJ/QH4Y0m8NAOjxLzscy8cMeGnVH9bDxY8SO/nPxaJ39JriCnQMP6TvYRbid4pfCZZYuWFLhXQCpC41TO+PYO+0mNakRw9dXNlv/9JNY5nOWmsI5IGpyyI8aHn5PQT6oWFri11P91h1l88LDzzuwSsJ9o7G75VlhncANf2kWkaA2XtPTPZUP9f0YTy8FKifCgfRqYb1tKDiXIktu8mZ0DI1hrmKkubKqGt9FQN3HZLkiI5aCscvnMzC1wjpa8Hqs7FYLim6iIhP83RirlcwbZlB60Qt8XKw+mas5JeWUQuE+P3EPI2IbRCvEPBKAu+JSqO6/YFxPoGg8tsdVTxQT2y3EOlJAp4D0NZq37hLg+fPi3Dib5Edvn6ZEO0dckd8UlWdVKJ+z+NEaHOL1SvjexYfcjgfGbBlITnhjEbHalwjpEaC1QGQ7go48T6b4ocMuLva2/bB2N4apRrOmmeF6Z9Fmr7ihfItO7QVgtcapfb405OkvwZwE4j3gzgJYgVSACsjUENg1S5Cm0D6MsPyhfLz67+PCcORKLTOURw9HpE+LdLW5kQUfFuAC6Vv+Bz39cfaMfjtw8I4/NPDMIRbzu6v9ucvAKsfCGlfSHdHVnLIQHeArUnJhrHfUw2nJqvBridDwkeU2J9NW4l7onyu1p08ba93HC2JBsdeLKx3GdbPR6RmVSkzzmsOx7pRU2tpczh6YGR8qkt8mwHHflj3CrIzoMY2Kub4VgEvD5HYbEfhjYb4MkPW1W607rBhjwwYAPYuRbCnssWwvRystwupsxOx/yVhXe8nZSGRdWEyGvZd1d6kq932stDOzhXocYk4+G0ySH7MOpC3ysXaV12n9lwhq4XYeswwjfb9ZJ/X11gyux6L8cxqESudMKRIEp6HORo8mJooRHOE5G6d6f8bA7416h52ndfxz6vw/K1HhHAUl1oGoTPHVSgh54J1TkifI6weDQbblym7NkVsnaML+Ys4x897icK2uNk8aJUpYE9/Tnn4iGV6w9joDWEhuE8H1lhFdKfl6oSKvPVRY+DCPxk6HhVyqryYVfRSVKl/w6HqFSJ8vIALFNiXGye+Lnzi0sfQseiI0x8F8ADC3slDcbn4C9Pi308SBUTJj+tEnSWkJiW0vjKGmsekv8Sh55l9rfvYLp9mmNtA7BHzIsWymD01KszG/6Q8edQo+4uUjD/O2eZBacy8HlnaV+KOhah5ajD9MySDTwlotoCaDPOFUf+2Vdh9dHf33sEdj7OQnTNroRG+G6xqQEoM8VIh9bQAa1jp0wj8MRArgBNC1EHEo0FkhHgnQACpaQDtAtHjIJ4K8Fwh3g0l34hTwVYeSq8AsFfA0wCCAAfE4pnRw3fvO9zDs2MIDKgxy5UzcuUMMs5kIZUHW7eBuCSMh1xHbk4EejSR9QKI94uQCOF5ZlUl8AcMaB+IvkzEY0D8QQHNBCgS4ixAIuADIBomAEOI3oxKhpiuCbYsfQBbHjy6zO8EWPqXSDjkd6jGyS6gFxKrySBVAKnJWiwPrPuJ1CIT6flkYZChTxHis4U4A+JRQux5dv1tUYbuR0/xAbHdNiIyAsoIqAEghd8VmokEAATTODv7AXOgwUOw9ogzH4PbtK2wJ19dpxv0h4RUQbSziiGtAr5FwHUg7o+ymBl1zCjxgKN43OvNHHoTmblF3Mxz/sqmjcBcoHgDcBZABxYQF3rqEQeTFanTjeAcgGYBSL4VWUBYErv562TFBeHBkr1LwABaW4HcCcC2dsA5GbhkkAizLD3oXJir7+3ovWf5ut+bc7PmE/oAdI4SVL7/33u2jAaGvgGcSaQ6ijlp6jhDGznPGDoZwChm+T/xiL5/jO9+yBzJfH737ku3tgLVJDClAXj66Xfmlb8RGNEB1HyaSEVK13e1qFiOR5xb7S2788D/G8DvtmbNJ7zwqyOuiP7/C3yU+jPwn7r+DPynrv91wP8OwX/ztVOJmW4AAAAASUVORK5CYII=">
      <div class="club-name">
        <h1>CLUBE DE RELAÇÕES INTERNACIONAIS</h1>
        <span>Escola SESI Djalma Pessoa</span>
      </div>
    </div>

    <!-- Botão hambúrguer do lado direito -->
    <div class="menu-toggle" id="menu-toggle">☰</div>

    <!-- Navegação -->
    <nav id="menu">
      <ul>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="https://forms.gle/SEU-LINK" class="highlight">Inscrições MUN</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero bg-gradient">
    <div class="hero-content">
      <h1>Bem-vindo ao Clube de Relações Internacionais</h1>
      <p>Escola SESI Djalma Pessoa</p>
    </div>
  </section>

  <!-- COMITÊ CSNU -->
  <section class="committee-header">
    <h1>Comitê Executivo da ACNUR</h1>
    <div class="committee-links">
      <a href="https://forms.gle/SEU-LINK">📄 Inscrição</a> 
      <a href="#">🌍 Lista de Países</a>
      <a href="#">📘 Manual</a>
      <a href="#">📑 Guia de Estudos</a>
    </div>
  </section>

  <section class="committee-description">
    <h2> <p>Tema: Crise de Refugiados em África</h2>
    <p>
      O Comitê Executivo do Alto Comissariado das Nações Unidas para Refugiados (ACNUR) tem como principal responsabilidade supervisionar e apoiar os trabalhos relacionados à proteção internacional de refugiados, deslocados internos e apátridas. Criado em 1958, este comitê garante que as operações do ACNUR sejam eficazes, humanitárias e sustentadas por cooperação internacional. Em simulações, os delegados enfrentam cenários de crises humanitárias, debatendo soluções práticas e sustentáveis para deslocamentos forçados.
    </p>
     <h4>Estrutura e Funcionamento:</h4>
    <p>
      O Comitê Executivo do ACNUR é composto por Estados-membros eleitos pela Assembleia Geral da ONU. Suas sessões ocorrem anualmente em Genebra, onde são debatidos relatórios, aprovadas diretrizes e revisadas as operações humanitárias. Nas simulações, os delegados assumem o papel de representantes nacionais, devendo articular políticas de acolhimento, financiamento e proteção de refugiados em meio a interesses diplomáticos divergentes.
    </p>
  </section>

  <!-- LISTA DE PAÍSES -->
  <section class="committee-list">
    <h2>Lista de Países Envolvidos</h2>
     <h5>COMITÊ INDIVIDUAL!</h5>
    <p class="note">(Os nomes na cor cinza estão indisponíveis)<br>


    <ol class="country-list">
      <li><a href="#">Burkina Faso</a></li>
      <li><a href="#">Estados Unidos da América</a></li>
      <li><a href="#">Reino da Espanha</a></li>
      <li><a href="#">República Centro-Africana</</a></li>
      <li><a href="#">República da África do Sul</a></li>
      <li><a href="#">República de Uganda</a></li>
      <li><a href="#">República Democrática do Congo</a></li>
      <li><a href="#">República de Ruanda</></li>
      <li><a href="#">República Democrática Federal da Etiópia</a></li>
      <li><a href="#">República Federal da Alemanha</a></li>
      <li><a href="#">República do Burundi</a></li>
      <li><a href="#">República do Chade</a></li>
      <li><a href="#">República do Mali</a></li>
      <li><a href="#">República do Sudão</a></li>
      <li><a href="#">República dos Camarões
      </a></li>
       <li><a href="#">República do Burundi</a></li>
      <li><a href="#">República do Quênia</a></li>
      <li><a href="#">República do Sudão do Sul</a></li>
      <li><a href="#">República Francesa</a></li>
      <li><a href="#">República Federal da Nigéria
      </a></li>
      <li><a href="#">República Federal da Somália</a></li>
      <li><a href="#">República Italiana</a></li>
      <li><a href="#">República Francesa</a></li>
      <!-- resto da lista -->
    </ol>
  </section>

  <!-- RODAPÉ -->
  <footer class="footer">
    <p>Todos os direitos reservados ao CRI SESI Piatã ®</p>
  </footer>

  <!-- SCRIPT MENU HAMBÚRGUER -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const menu = document.getElementById("menu");

    toggle.addEventListener("click", () => {
      menu.classList.toggle("active");
    });
  </script>

</body>
</html>
