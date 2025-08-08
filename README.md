
<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Festas de Vizela 2025 — Programa e Horários</title>

  <style>
    :root{
      --bg:#f8f9fa;
      --ink:#222;
      --brand:#1abc9c;
      --brand-700:#16a085;
      --nav:#34495e;
      --nav-ink:#fff;
      --header:#2c3e50;
      --card:#fff;
      --border:#e5e7eb;
      --submenu:#3d566e;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
      background:var(--bg);
      color:var(--ink);
      display:flex;
      flex-direction:column;
      min-height:100vh;
    }

    /* Header */
    header{
      background:var(--header);
      color:#fff;
      text-align:center;
      padding:1rem 1.25rem;
    }
    header h1{margin:.25rem 0 .35rem 0;font-size:clamp(1.25rem,2.2vw,1.75rem)}
    header p{margin:0;opacity:.9}

    /* Container */
    .container{ width:min(1100px, 100%); margin:0 auto; padding:0 1.25rem }

    /* Top nav */
    nav{
      display:flex; flex-wrap:wrap; gap:0;
      background:var(--nav);
    }
    nav a{
      color:var(--nav-ink);
      text-decoration:none;
      padding:1rem 1.25rem;
      flex:1 1 auto;
      text-align:center;
      transition:background .25s ease;
    }
    nav a:hover{background:#2c3e50}
    @media (min-width:768px){
      nav{justify-content:center}
      nav a{flex:0 0 auto; padding:1rem 1.5rem}
    }

    /* Submenu (dias) */
    .submenu{
      display:none;
      flex-direction:column;
      background:var(--submenu);
      padding:.75rem 0;
    }
    .submenu-inner{ width:min(1100px, 100%); margin:0 auto; padding:0 1.25rem }
    .dia{ margin-bottom:.9rem }           /* mais espaçamento entre dias */
    .dia > button{
      width:100%;
      text-align:left;
      background:transparent;
      color:#fff;
      border:0;
      cursor:pointer;
      padding:.75rem .85rem;
      border-radius:6px;
      transition:background .2s ease;
      font-size:1rem;
    }
    .dia > button:hover{ background:rgba(255,255,255,.1) }
    .dia > button.active{ background:var(--brand) }
    .dia-content{
      display:none;
      background:#ecf0f1;
      padding:1rem 1rem 1.1rem 1rem;
      border-radius:6px;
      margin-top:.45rem;
      line-height:1.55;
    }

    /* Content */
    main.content{ padding:1.25rem 0; flex:1 }
    .card{
      background:var(--card);
      border:1px solid var(--border);
      border-radius:14px;
      box-shadow:0 2px 10px rgba(0,0,0,.05);
      padding:1.1rem 1.2rem;
      margin:0 0 1rem 0;
    }
    .card h2{ margin:.25rem 0 1rem 0; font-size:1.25rem }

    .btn{
      display:inline-block;
      padding:.6rem 1rem;
      background:var(--brand);
      color:#fff;
      text-decoration:none;
      border-radius:8px;
      font-weight:600;
      margin-top:.5rem;
    }
    .btn:hover{ background:var(--brand-700) }

    /* Lists / tables */
    .horarios p{ margin:.7rem 0 }      /* espaçamento confortável */
    .horarios p strong{ font-weight:700 }

    table{ width:100%; border-collapse:collapse; margin-top:.75rem }
    th,td{ border:1px solid #d1d5db; padding:.65rem .6rem; text-align:center }
    th{ background:var(--nav); color:#fff; font-weight:700 }

    /* Map always visible */
    .map-wrap{ margin-top:1rem }
    iframe.map{ width:100%; height:340px; border:0; display:block }

    /* Footer */
    footer{
      background:var(--header);
      color:#fff;
      text-align:center;
      padding:.9rem 1rem;
      font-size:.95rem;
    }
    footer a{ color:var(--brand); text-decoration:none }
    footer a:hover{ text-decoration:underline }
  </style>
</head>
<body>

  <header>
    <div class="container">
      <h1>Festas de Vizela 2025</h1>
      <p>Horários, Cartaz, Regulamentos e Licença de Ruído</p>
    </div>
  </header>

  <!-- Navegação principal -->
  <nav aria-label="Navegação principal">
    <div class="container" style="display:flex;flex-wrap:wrap;gap:0">
      <a href="#" onclick="mostrarSecao('diversoes');return false;">Horários das Diversões</a>
      <a href="#" onclick="mostrarSecao('bares');return false;">Horários dos Bares</a>
      <a href="#" onclick="toggleSubmenu();return false;">Cartaz da Festa ▼</a>
      <a href="https://drive.google.com/file/d/1rCoUVLLwstb8wKrJLo7fhMFPWM0Re8nk/view?usp=drivesdk" target="_blank" rel="noopener">Licença de Ruído</a>
    </div>
  </nav>

  <!-- Submenu (Dias) -->
  <div id="submenu" class="submenu" aria-label="Programa por dias">
    <div class="submenu-inner">
      <div class="dia">
        <button onclick="toggleDia('8', this)">8 de Agosto</button>
        <div id="dia-8" class="dia-content">
          <strong>Silent Party</strong> — 22h–02h, Rua Dr. Pereira Caldas. Rua com 2 DJs (MPP e House)
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('9', this)">9 de Agosto</button>
        <div id="dia-9" class="dia-content">
          <p><strong>NAPA</strong> — 23h, Multiusos.</p>
          <p><strong>DJ BAIJON</strong> — Multiusos.</p>
          <p><strong>DJ LOWIE</strong> — Multiusos.</p>
          <hr>
          <p><em>Agenda do dia (resumo):</em> 09h Torneio de Minigolfe · 14h Pedalada às Tasquinhas · 15h Sueca · 18h30 Corrida 6km · 22h Blank (Praça da República).</p>
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('10', this)">10 de Agosto</button>
        <div id="dia-10" class="dia-content">
          <strong>Hybrid Theory</strong> — 22h, Multiusos (Tributo Linkin Park).<br>
          22h Pedro Costa &amp; Maria Damasceno — Praça da República.
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('11', this)">11 de Agosto</button>
        <div id="dia-11" class="dia-content">
          <strong>Deixem o Pimba em Paz</strong> — 22h, Multiusos (Manuela Azevedo &amp; Bruno Nogueira).<br>
          22h Zé Miguel &amp; Band — Praça da República.
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('12', this)">12 de Agosto</button>
        <div id="dia-12" class="dia-content">
          <strong>4 Mens</strong> — 22h, Multiusos.<br>
          09h–12h30 &amp; 14h–19h Colheita de Sangue — Praça da República.<br>
          22h VIMA Acústico — Praça da República.
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('13', this)">13 de Agosto</button>
        <div id="dia-13" class="dia-content">
          <strong>Orquestra Ligeira SFV</strong> — 22h, Multiusos. Lugares sentados com pulseira; em pé gratuito.<br>
          22h André Martins — Praça da República.
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('14', this)">14 de Agosto</button>
        <div id="dia-14" class="dia-content">
          <p><strong>“Vizela dos Tempos Idos”</strong> — 22h30, Centro de Vizela. Desfile histórico (&gt;700 figurantes).<br>
          <em>Trajeto:</em> Rua da Saudade → Rua Dr. Abílio Torres → Rua Dr. Bráulio Caldas → Av. Manuel Campelos → Multiusos.</p>
          <p><strong>Memo à Tuga!</strong> — Praça da República.</p>
          <p><strong>Fogo de Artifício</strong> — Jardim Manuel Faria.</p>
        </div>
      </div>

      <div class="dia">
        <button onclick="toggleDia('15', this)">15 de Agosto</button>
        <div id="dia-15" class="dia-content">
          Encerramento das Festas até às 06h00 da manhã.
        </div>
      </div>
    </div>
  </div>

  <!-- Conteúdo principal -->
  <main class="content">
    <div class="container">

      <!-- Horários das Diversões -->
      <section id="diversoes" class="card" style="display:none">
        <h2>Regulamento e Horário das Diversões</h2>
        <div class="horarios" style="line-height:1.85">
          <p><strong>26 de julho a 07 de agosto:</strong> das 10h até à 24h <em>(sem amplificação a partir das 22h)</em></p>
          <p><strong>08 de agosto:</strong> das 10h até à 01h <em>(sem amplificação a partir das 22h)</em></p>
          <p><strong>09, 10, 11, 12 e 13 de agosto:</strong> das 10h até às 02h <em>(a partir das 22h haverá espetáculos no Multiusos; a amplificação deve ser desligada às 22h e não pode voltar a ligar)</em></p>
          <p><strong>14 de agosto:</strong> das 10h até às 02h <em>(sem restrição)</em></p>
          <p><strong>15 a 25 de agosto:</strong> das 10h até às 24h <em>(sem amplificação a partir das 22h)</em></p>
          <hr>
          <p><strong>CALENDÁRIO:</strong><br>Os espaços estarão disponíveis no intervalo do licenciamento camarário, desde o dia 28 de julho de 2025 até ao dia 25 de agosto de 2025.</p>
        </div>
        <a class="btn" target="_blank" rel="noopener"
           href="https://drive.google.com/file/d/1TkzyWyEMG1rkJjMcshniwjIcKF3XMclZ/view?usp=drivesdk">
           Ver PDF Regulamento das Diversões
        </a>
      </section>

      <!-- Horários dos Bares -->
      <section id="bares" class="card" style="display:none">
        <h2>Regulamento e Horário dos Bares</h2>

        <table aria-label="Horários dos Bares e do P.A. por dia">
          <thead>
            <tr><th>Dia</th><th>Horário Bar</th><th>Horário P.A.</th></tr>
          </thead>
          <tbody>
            <tr><td>Sexta, 08 Agosto</td><td>04:00</td><td>04:00</td></tr>
            <tr><td>Sábado, 09 Agosto</td><td>05:00</td><td>05:00</td></tr>
            <tr><td>Domingo, 10 Agosto</td><td>02:00</td><td>02:00</td></tr>
            <tr><td>Segunda, 11 Agosto</td><td>02:00</td><td>02:00</td></tr>
            <tr><td>Terça, 12 Agosto</td><td>02:00</td><td>02:00</td></tr>
            <tr><td>Quarta, 13 Agosto</td><td>02:00</td><td>02:00</td></tr>
            <tr><td>Quinta, 14 Agosto</td><td>06:00</td><td>06:00</td></tr>
          </tbody>
        </table>

        <a class="btn" target="_blank" rel="noopener"
           href="https://drive.google.com/file/d/1QYsv8J2LJ26m-ElBkLOyoHRf9p56KL26/view?usp=drivesdk">
           Ver PDF Regulamento Bares
        </a>
      </section>

      <!-- Mapa sempre visível -->
      <section class="map-wrap">
        <iframe class="map"
          src="https://www.google.com/maps/d/embed?mid=17aLmpSMZESsy8czZKtoYbFeqDaI&hl=pt-PT&ehbc=2E312F"
          allowfullscreen
          title="Mapa - Festas da Cidade de Vizela 2025">
        </iframe>
      </section>

    </div>
  </main>

  <footer>
    📍 <a href="https://www.google.com/maps/d/u/0/edit?mid=1jqVeOgyXn4yDp7jGGPGsOgjI14CUH2U&usp=sharing" target="_blank" rel="noopener">
      Mapa — Festas da Cidade de Vizela 2025
    </a>
  </footer>

  <script>
    // Esconde secções e recolhe conteúdos do submenu
    function esconderTudo(){
      document.getElementById('diversoes').style.display = 'none';
      document.getElementById('bares').style.display = 'none';
      document.querySelectorAll('.dia-content').forEach(dc => dc.style.display = 'none');
      document.querySelectorAll('.dia > button').forEach(b => b.classList.remove('active'));
    }

    function mostrarSecao(secao){
      // ao abrir uma secção, recolhe submenu
      document.getElementById('submenu').style.display = 'none';
      esconderTudo();
      document.getElementById(secao).style.display = 'block';
      window.scrollTo({top:0, behavior:'smooth'});
    }

    function toggleSubmenu(){
      esconderTudo(); // garante que não ficam secções por baixo
      const el = document.getElementById('submenu');
      el.style.display = (el.style.display === 'flex' || el.style.display === 'block') ? 'none' : 'flex';
    }

    function toggleDia(dia, btn){
      const el = document.getElementById(`dia-${dia}`);
      const visivel = el.style.display === 'block';

      // recolhe todos
      document.querySelectorAll('.dia-content').forEach(dc => dc.style.display = 'none');
      document.querySelectorAll('.dia > button').forEach(b => b.classList.remove('active'));

      // abre o selecionado se estava fechado
      if(!visivel){
        el.style.display = 'block';
        btn.classList.add('active');

        // opcional: scroll para posicionar o cabeçalho do dia
        const rect = btn.getBoundingClientRect();
        const offset = window.pageYOffset + rect.top - 10;
        window.scrollTo({ top: offset, behavior: 'smooth' });
      }
    }
  </script>
</body>
</html>
