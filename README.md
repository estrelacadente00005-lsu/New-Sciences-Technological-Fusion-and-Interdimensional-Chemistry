
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Impressora Quântica 6D - Novas Ciências Interdimensionais</title>
    <style>
        :root {
            --bg-dark: #030611;
            --panel-bg: rgba(6, 12, 28, 0.92);
            --border-cyan: rgba(0, 243, 255, 0.3);
            --neon-green: #00ff66;
            --neon-purple: #bd00ff;
            --neon-cyan: #00f3ff;
            --neon-gold: #ffcc00;
            --text-main: #d0f2ff;
            --font-code: 'Courier New', Courier, monospace;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: var(--font-code);
            user-select: none;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 15px;
            overflow-x: hidden;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(0, 255, 102, 0.08) 0%, transparent 40%),
                radial-gradient(circle at 85% 80%, rgba(189, 0, 255, 0.1) 0%, transparent 45%);
        }

        header {
            text-align: center;
            width: 100%;
            max-width: 1400px;
            margin-bottom: 12px;
            border-bottom: 1px solid var(--border-cyan);
            padding-bottom: 10px;
        }

        header h1 {
            font-size: 1.5rem;
            color: var(--neon-cyan);
            text-shadow: 0 0 12px rgba(0, 243, 255, 0.6);
            letter-spacing: 2px;
        }

        header p {
            font-size: 0.8rem;
            color: #83a5cc;
            margin-top: 4px;
        }

        .science-badge {
            display: inline-block;
            background: linear-gradient(90deg, var(--neon-green), var(--neon-purple), var(--neon-cyan));
            color: #000;
            padding: 3px 14px;
            font-size: 0.72rem;
            border-radius: 12px;
            font-weight: bold;
            margin-top: 6px;
            letter-spacing: 1px;
        }

        .app-container {
            display: grid;
            grid-template-columns: 360px 1fr 340px;
            gap: 15px;
            width: 100%;
            max-width: 1400px;
            height: calc(100vh - 120px);
            min-height: 680px;
        }

        @media (max-width: 1100px) {
            .app-container {
                grid-template-columns: 1fr;
                height: auto;
            }
        }

        .panel {
            background: var(--panel-bg);
            border: 1px solid var(--border-cyan);
            border-radius: 8px;
            padding: 14px;
            display: flex;
            flex-direction: column;
            gap: 10px;
            backdrop-filter: blur(8px);
            box-shadow: 0 0 15px rgba(0, 243, 255, 0.05);
            overflow-y: auto;
        }

        .panel-title {
            font-size: 0.85rem;
            color: var(--neon-cyan);
            border-bottom: 1px solid var(--border-cyan);
            padding-bottom: 6px;
            text-transform: uppercase;
            font-weight: bold;
            display: flex;
            justify-content: space-between;
        }

        .tab-btn {
            background: rgba(2, 8, 20, 0.8);
            border: 1px solid rgba(0, 243, 255, 0.2);
            color: #83a5cc;
            padding: 10px;
            border-radius: 6px;
            cursor: pointer;
            font-size: 0.72rem;
            font-weight: bold;
            transition: all 0.25s;
            text-align: left;
            display: flex;
            flex-direction: column;
            gap: 3px;
        }

        .tab-btn:hover {
            border-color: var(--neon-cyan);
            color: #fff;
        }

        .tab-btn.active-bio {
            border-color: var(--neon-green);
            background: rgba(0, 255, 102, 0.12);
            color: var(--neon-green);
            box-shadow: 0 0 10px rgba(0, 255, 102, 0.2);
        }

        .tab-btn.active-quark {
            border-color: var(--neon-purple);
            background: rgba(189, 0, 255, 0.15);
            color: var(--neon-purple);
            box-shadow: 0 0 10px rgba(189, 0, 255, 0.25);
        }

        .tab-btn.active-brana {
            border-color: var(--neon-cyan);
            background: rgba(0, 243, 255, 0.15);
            color: var(--neon-cyan);
            box-shadow: 0 0 10px rgba(0, 243, 255, 0.25);
        }

        .info-card {
            background: rgba(2, 6, 16, 0.85);
            border: 1px solid rgba(0, 243, 255, 0.15);
            border-radius: 6px;
            padding: 10px;
            font-size: 0.7rem;
            color: #83a5cc;
            line-height: 1.35;
        }

        .info-card h4 {
            font-size: 0.75rem;
            color: var(--neon-gold);
            margin-bottom: 4px;
        }

        .control-group {
            display: flex;
            flex-direction: column;
            gap: 3px;
        }

        .control-label {
            font-size: 0.7rem;
            color: #83a5cc;
            display: flex;
            justify-content: space-between;
        }

        .control-value {
            color: var(--neon-cyan);
            font-weight: bold;
        }

        input[type="range"] {
            appearance: none;
            -webkit-appearance: none;
            width: 100%;
            height: 5px;
            background: #0b1a30;
            border-radius: 3px;
            outline: none;
        }

        input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background: var(--neon-cyan);
            cursor: pointer;
            box-shadow: 0 0 8px var(--neon-cyan);
        }

        .btn-trigger {
            background: transparent;
            border: 1px solid var(--neon-cyan);
            color: var(--neon-cyan);
            padding: 10px;
            border-radius: 5px;
            font-weight: bold;
            font-size: 0.75rem;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s;
            margin-top: 5px;
        }

        .btn-trigger:hover {
            background: var(--neon-cyan);
            color: #000;
            box-shadow: 0 0 15px var(--neon-cyan);
        }

        .btn-trigger.danger {
            border-color: #ff0055;
            color: #ff0055;
        }

        .btn-trigger.danger:hover {
            background: #ff0055;
            color: #fff;
            box-shadow: 0 0 15px #ff0055;
        }

        .canvas-area {
            display: flex;
            flex-direction: column;
            position: relative;
            background: #010309;
            border: 1px solid var(--border-cyan);
            border-radius: 8px;
            overflow: hidden;
        }

        canvas {
            display: block;
            width: 100%;
            height: 100%;
        }

        .canvas-tag {
            position: absolute;
            top: 10px;
            left: 10px;
            background: rgba(0, 0, 0, 0.85);
            border: 1px solid var(--border-cyan);
            padding: 4px 10px;
            font-size: 0.7rem;
            color: var(--neon-cyan);
            border-radius: 4px;
            pointer-events: none;
            letter-spacing: 1px;
        }

        .canvas-hud {
            position: absolute;
            bottom: 10px;
            right: 10px;
            background: rgba(0, 0, 0, 0.85);
            border: 1px solid rgba(189, 0, 255, 0.4);
            padding: 6px 12px;
            font-size: 0.68rem;
            color: #aaccff;
            border-radius: 4px;
            pointer-events: none;
            text-align: right;
            line-height: 1.3;
        }

        .terminal {
            background: #01040a;
            border: 1px solid rgba(0, 243, 255, 0.2);
            border-radius: 5px;
            padding: 8px;
            height: 140px;
            overflow-y: auto;
            font-size: 0.66rem;
            color: #88c5ff;
            display: flex;
            flex-direction: column;
            gap: 4px;
        }

        .log-line { line-height: 1.25; }
        .log-line.green { color: var(--neon-green); }
        .log-line.purple { color: var(--neon-purple); }
        .log-line.gold { color: var(--neon-gold); }
    </style>
</head>
<body>

    <header>
        <h1>IMPRESSORA QUÂNTICA 6D — NOVAS CIÊNCIAS INTERDIMENSIONAIS</h1>
        <p>Química Atômica/Cósmica, Biotecnologia Bio-SAMS & Cristais de Memória de Brana (Calabi-Yau 11D)</p>
        <span class="science-badge">QUÍMICA & FISICA BEYOND THE PERIODIC TABLE</span>
    </header>

    <div class="app-container">
        <!-- PAINEL ESQUERDO: SELEÇÃO DE CIÊNCIA EXÓTICA -->
        <div class="panel">
            <div class="panel-title">
                <span>1. MÓDULOS DE CIÊNCIA EXÓTICA</span>
            </div>

            <div class="tab-btn active-bio" id="tabBio" onclick="selectModule('bio')">
                <span>🟢 1. BIOTECNOLOGIA BIO-SAMS</span>
                <span style="font-size: 0.62rem; opacity:0.8;">Tecido Biomecânico Vivo (Endurecimento Diamante)</span>
            </div>

            <div class="tab-btn" id="tabQuark" onclick="selectModule('quark')">
                <span>🟪 2. MATÉRIA DE QUARK-GLUON</span>
                <span style="font-size: 0.62rem; opacity:0.8;">Ligas Decaídas & Curvatura Gravitacional</span>
            </div>

            <div class="tab-btn" id="tabBrana" onclick="selectModule('brana')">
                <span>🔵 3. CRISTAIS DE MEMÓRIA DE BRANA</span>
                <span style="font-size: 0.62rem; opacity:0.8;">Armazenamento Calabi-Yau 11D Imune ao Fim do 4D</span>
            </div>

            <div class="info-card">
                <h4 id="moduleDescTitle">DESCRIÇÃO DA TECNOLOGIA</h4>
                <p id="moduleDescText">
                    Células biológicas modificadas com nanofluidos magnetorreológicos no citoplasma. Sofrem transição imediata de viscosidade para dureza de diamante sob impacto kinetic.
                </p>
            </div>

            <div class="panel-title" style="margin-top: 5px;">
                <span>MODULADORES DE CAMPO</span>
            </div>

            <div class="control-group">
                <div class="control-label">
                    <span>Pressão SAMS (Endurecimento):</span>
                    <span class="control-value" id="valParam1">100.0 MPa</span>
                </div>
                <input type="range" id="sliderParam1" min="1" max="100" value="50">
            </div>

            <div class="control-group">
                <div class="control-label">
                    <span>Densidade de Nanofluidos (MHD):</span>
                    <span class="control-value" id="valParam2">99.8%</span>
                </div>
                <input type="range" id="sliderParam2" min="1" max="100" value="85">
            </div>

            <button class="btn-trigger" id="btnMainTrigger" onclick="triggerPrimaryAction()">DISPARAR PROJÉTIL DE BALÍSTICA</button>
            <button class="btn-trigger danger" id="btnBigCrunch" onclick="triggerBigCrunch()" style="display:none;">SIMULAR BIG CRUNCH (FIM DO 4D)</button>
        </div>

        <!-- PAINEL CENTRAL: CANVAS VISUALIZADOR 2D -->
        <div class="canvas-area">
            <div class="canvas-tag" id="canvasTagText">VISOR DE LABORATÓRIO — TECIDO BIOMECÂNICO BIO-SAMS (CLIQUE NO CANVAS PARA IMPACTAR)</div>
            <canvas id="simCanvas"></canvas>
            <div class="canvas-hud" id="hudText">
                ESTADO DAS CÉLULAS: MACIAS / FLEXÍVEIS<br>
                RESISTÊNCIA KINETIC: 1.2 GPa<br>
                VISCOSIDADE CITOPLASMÁTICA: FLUIDO
            </div>
        </div>

        <!-- PAINEL DIREITO: MONITOR DE TELEMETRIA -->
        <div class="panel">
            <div class="panel-title">
                <span>MATRIZ DE DADOS SROS</span>
            </div>

            <div class="info-card">
                <h4>PROPRIEDADES DA MATÉRIA</h4>
                <div style="display:flex; flex-direction:column; gap:4px; font-size:0.68rem;">
                    <div style="display:flex; justify-content:space-between;">
                        <span>Densidade Atômica:</span>
                        <span id="statDensity" style="color:var(--neon-green)">1.45 g/cm³</span>
                    </div>
                    <div style="display:flex; justify-content:space-between;">
                        <span>Dobra Espacial ($\Lambda$):</span>
                        <span id="statWarp" style="color:var(--neon-cyan)">0.0000 rad</span>
                    </div>
                    <div style="display:flex; justify-content:space-between;">
                        <span>Persistência Dimensional:</span>
                        <span id="statPersist" style="color:var(--neon-gold)">3D / 4D Local</span>
                    </div>
                </div>
            </div>

            <div class="panel-title" style="margin-top: 10px;">
                <span>LOGS DE FUSÃO INTERDIMENSIONAL</span>
            </div>

            <div class="terminal" id="terminalLog">
                <div class="log-line green">> Bio-SAMS acoplado com nanofluidos magnetorreológicos.</div>
                <div class="log-line">> Aguardando testes de deformação cinética ou alteração de módulo.</div>
            </div>
        </div>
    </div>

    <script>
        const canvas = document.getElementById('simCanvas');
        const ctx = canvas.getContext('2d');

        // ELEMENTOS DO DOM
        const tabBio = document.getElementById('tabBio');
        const tabQuark = document.getElementById('tabQuark');
        const tabBrana = document.getElementById('tabBrana');

        const moduleDescTitle = document.getElementById('moduleDescTitle');
        const moduleDescText = document.getElementById('moduleDescText');
        const canvasTagText = document.getElementById('canvasTagText');
        const hudText = document.getElementById('hudText');

        const btnMainTrigger = document.getElementById('btnMainTrigger');
        const btnBigCrunch = document.getElementById('btnBigCrunch');

        const sliderParam1 = document.getElementById('sliderParam1');
        const sliderParam2 = document.getElementById('sliderParam2');
        const valParam1 = document.getElementById('valParam1');
        const valParam2 = document.getElementById('valParam2');

        const statDensity = document.getElementById('statDensity');
        const statWarp = document.getElementById('statWarp');
        const statPersist = document.getElementById('statPersist');
        const terminalLog = document.getElementById('terminalLog');

        // ESTADO INTERNO
        let currentModule = 'bio'; // 'bio', 'quark', 'brana'
        let isHardened = false;
        let hardnessTimer = 0;
        let projectiles = [];
        let particles = [];
        let isBigCrunchActive = false;
        let crunchScale = 1.0;

        // ESTRUTURAS DE SIMULAÇÃO
        let bioCells = [];

        function resizeCanvas() {
            canvas.width = canvas.parentElement.clientWidth;
            canvas.height = canvas.parentElement.clientHeight;
            initBioCells();
        }
        window.addEventListener('resize', resizeCanvas);

        function logMsg(msg, colorClass = 'green') {
            const entry = document.createElement('div');
            entry.className = `log-line ${colorClass}`;
            const time = new Date().toLocaleTimeString();
            entry.textContent = `[${time}] ${msg}`;
            terminalLog.appendChild(entry);
            terminalLog.scrollTop = terminalLog.scrollHeight;
        }

        // SLIDERS CONTROLS
        sliderParam1.addEventListener('input', (e) => {
            if (currentModule === 'bio') valParam1.textContent = (e.target.value * 2).toFixed(1) + ' MPa';
            else if (currentModule === 'quark') valParam1.textContent = (e.target.value * 100).toFixed(0) + ' M-Möbius';
            else valParam1.textContent = (e.target.value * 0.1).toFixed(1) + ' Yotta-TB';
        });

        sliderParam2.addEventListener('input', (e) => {
            valParam2.textContent = e.target.value + '.0%';
        });

        // INICIALIZAÇÃO DE CÉLULAS BIO-SAMS
        function initBioCells() {
            bioCells = [];
            const cols = 8;
            const rows = 6;
            const stepX = canvas.width / (cols + 1);
            const stepY = canvas.height / (rows + 1);

            for (let i = 0; i < cols; i++) {
                for (let j = 0; j < rows; j++) {
                    bioCells.push({
                        x: stepX * (i + 1),
                        y: stepY * (j + 1),
                        baseX: stepX * (i + 1),
                        baseY: stepY * (j + 1),
                        vx: 0, vy: 0,
                        radius: 22
                    });
                }
            }
        }

        // SELEÇÃO DE MÓDULO
        function selectModule(mod) {
            currentModule = mod;
            tabBio.className = 'tab-btn' + (mod === 'bio' ? ' active-bio' : '');
            tabQuark.className = 'tab-btn' + (mod === 'quark' ? ' active-quark' : '');
            tabBrana.className = 'tab-btn' + (mod === 'brana' ? ' active-brana' : '');

            projectiles = [];
            particles = [];
            isBigCrunchActive = false;
            crunchScale = 1.0;

            if (mod === 'bio') {
                moduleDescTitle.textContent = '1. BIOTECNOLOGIA BIO-SAMS';
                moduleDescText.innerHTML = 'Células biológicas com citoplasma enriquecido por nanofluidos magnetorreológicos. Endurecem instantaneamente como diamante mediante impacto kinetico.';
                canvasTagText.textContent = 'VISOR — TECIDO BIOMECÂNICO BIO-SAMS (CLIQUE PARA GERAR IMPACTO)';
                btnMainTrigger.textContent = 'DISPARAR PROJÉTIL DE BALÍSTICA';
                btnMainTrigger.style.display = 'block';
                btnBigCrunch.style.display = 'none';

                statDensity.textContent = '1.45 g/cm³';
                statDensity.style.color = 'var(--neon-green)';
                statWarp.textContent = '0.0000 rad';
                statPersist.textContent = '3D / 4D Local';
                logMsg('Módulo alterado: Tecido Biomecânico Vivo Bio-SAMS.', 'green');
            } else if (mod === 'quark') {
                moduleDescTitle.textContent = '2. MATÉRIA DE QUARK-GLUON ESTABILIZADA';
                moduleDescText.innerHTML = 'Liga exótica de alta densidade equivalente a estrelas de nêutrons. Curva a gravidade local para desviar qualquer projetil sem sofrer danos.';
                canvasTagText.textContent = 'VISOR — MATÉRIA DECAÍDA & DESVIO GRAVITACIONAL DE TRAJETÓRIAS';
                btnMainTrigger.textContent = 'LANCAR FEIXE BALÍSTICO / LASER';
                btnMainTrigger.style.display = 'block';
                btnBigCrunch.style.display = 'none';

                statDensity.textContent = '1.8e14 g/cm³';
                statDensity.style.color = 'var(--neon-purple)';
                statWarp.textContent = '3.1415 rad (Lensing)';
                statPersist.textContent = 'Métrica Local Trocada';
                logMsg('Módulo alterado: Matéria de Quark-Gluon Estabilizada.', 'purple');
            } else {
                moduleDescTitle.textContent = '3. CRISTAIS DE MEMÓRIA DE BRANA';
                moduleDescText.innerHTML = 'Dados gravados em dobras de Calabi-Yau na 6ª dimensão do Espaço de Hilbert. Imune à morte do universo convencional.';
                canvasTagText.textContent = 'VISOR — ESPAÇO CALABI-YAU 11D & CRISTAIS ETERNOS DE DADOS';
                btnMainTrigger.textContent = 'GRAVAR DADOS NA DOBRA 6D';
                btnMainTrigger.style.display = 'block';
                btnBigCrunch.style.display = 'block';

                statDensity.textContent = '0.00 g/cm³ (Vácuo)';
                statDensity.style.color = 'var(--neon-cyan)';
                statWarp.textContent = '11D Calabi-Yau';
                statPersist.textContent = 'Eterna / Oniversal';
                logMsg('Módulo alterado: Cristais de Memória de Brana (11D).', 'gold');
            }
        }

        // TRIGGER PRINCIPAL DE AÇÃO
        function triggerPrimaryAction() {
            if (currentModule === 'bio') {
                // Disparar projetil no Tecido Bio-SAMS
                projectiles.push({
                    x: 50,
                    y: canvas.height / 2 + (Math.random() * 80 - 40),
                    vx: 18,
                    vy: 0,
                    type: 'kinetic'
                });
                logMsg('Disparo kinetico disparado contra a matriz bio-sams!', 'green');
            } else if (currentModule === 'quark') {
                // Disparar Feixe de Energia / Projetil em direção à massa superdensa
                for (let i = -2; i <= 2; i++) {
                    projectiles.push({
                        x: 40,
                        y: canvas.height / 2 + (i * 35),
                        vx: 12,
                        vy: 0,
                        type: 'laser'
                    });
                }
                logMsg('Projéteis gravitacionalmente curvados pelo escudo de Quark-Gluon.', 'purple');
            } else {
                // Gravar Dados nos Cristais de Brana
                for (let i = 0; i < 20; i++) {
                    particles.push({
                        x: canvas.width / 2 + (Math.random() * 80 - 40),
                        y: canvas.height / 2 + (Math.random() * 80 - 40),
                        vx: (Math.random() - 0.5) * 4,
                        vy: (Math.random() - 0.5) * 4,
                        life: 100,
                        color: '#00f3ff'
                    });
                }
                logMsg('SROS: 10 yotta-terabytes gravados com sucesso nas dobras de Calabi-Yau!', 'gold');
            }
        }

        function triggerBigCrunch() {
            if (isBigCrunchActive) return;
            isBigCrunchActive = true;
            crunchScale = 1.0;
            logMsg('ALERTA: Simulação de Big Crunch iniciada! O espaço-tempo 4D está colapsando...', 'purple');
        }

        // CLIQUE NO CANVAS PARA GERAR IMPACTO LOCALIZADO
        canvas.addEventListener('click', (e) => {
            const rect = canvas.getBoundingClientRect();
            const clickX = e.clientX - rect.left;
            const clickY = e.clientY - rect.top;

            if (currentModule === 'bio') {
                projectiles.push({
                    x: 20,
                    y: clickY,
                    vx: 20,
                    vy: 0,
                    type: 'kinetic'
                });
            }
        });

        // DESENHO: MÓDULO 1 (BIO-SAMS)
        function drawBioModule() {
            const w = canvas.width;
            const h = canvas.height;

            if (isHardened) {
                hardnessTimer--;
                if (hardnessTimer <= 0) isHardened = false;
            }

            // Atualizar e desenhar projéteis
            for (let i = projectiles.length - 1; i >= 0; i--) {
                let p = projectiles[i];
                p.x += p.vx;

                // Colisão com o tecido no centro
                if (p.x >= w * 0.4 && p.x <= w * 0.6) {
                    isHardened = true;
                    hardnessTimer = 45; // Mantém duro por um tempo
                    p.vx = -p.vx * 0.5; // Repelido como repulsão de diamante
                    logMsg('IMPACTO DETECTADO! Transição de Fase: Nanofluidos endurecidos para Estrutura Diamante.', 'green');
                }

                ctx.fillStyle = '#ffcc00';
                ctx.shadowColor = '#ffcc00';
                ctx.shadowBlur = 10;
                ctx.beginPath();
                ctx.arc(p.x, p.y, 5, 0, Math.PI * 2);
                ctx.fill();
                ctx.shadowBlur = 0;

                if (p.x < 0 || p.x > w) projectiles.splice(i, 1);
            }

            // Desenhar Células e Nanofluidos Bio-SAMS
            bioCells.forEach(cell => {
                ctx.beginPath();
                ctx.arc(cell.x, cell.y, cell.radius, 0, Math.PI * 2);

                if (isHardened) {
                    // Estado Diamante
                    ctx.fillStyle = 'rgba(0, 255, 204, 0.8)';
                    ctx.strokeStyle = '#ffffff';
                    ctx.lineWidth = 3;
                    ctx.shadowColor = '#00ffcc';
                    ctx.shadowBlur = 20;
                } else {
                    // Estado Macio / Bio
                    ctx.fillStyle = 'rgba(0, 255, 102, 0.25)';
                    ctx.strokeStyle = '#00ff66';
                    ctx.lineWidth = 1.5;
                    ctx.shadowBlur = 0;
                }

                ctx.fill();
                ctx.stroke();

                // Desenhar Núcleo de Nanofluido Magnetorreológico
                ctx.beginPath();
                ctx.arc(cell.x, cell.y, cell.radius * 0.35, 0, Math.PI * 2);
                ctx.fillStyle = isHardened ? '#ffffff' : '#00b341';
                ctx.fill();
            });

            hudText.innerHTML = `
                ESTADO CELULAR: ${isHardened ? '<span style="color:#00ffcc;">DUREZA DIAMANTE (HARDENED)</span>' : '<span style="color:#00ff66;">MACIO / GEL FLEXÍVEL</span>'}<br>
                AMORTECIMENTO DINÂMICO: ${isHardened ? '100% (REPELINDO IMPACTO)' : 'ATIVO (SENSÍVEL)'}<br>
                NANOFLUIDOS SAMS: ALINHADOS MAGNETORREOLOGICAMENTE
            `;
        }

        // DESENHO: MÓDULO 2 (MATÉRIA DE QUARK-GLUON)
        function drawQuarkModule() {
            const w = canvas.width;
            const h = canvas.height;
            const cx = w / 2;
            const cy = h / 2;

            // 1. Grade de Curvatura Gravitacional (Lensing)
            ctx.strokeStyle = 'rgba(189, 0, 255, 0.15)';
            ctx.lineWidth = 1;
            const step = 30;
            for (let x = 0; x < w; x += step) {
                ctx.beginPath();
                for (let y = 0; y < h; y += step) {
                    let dx = x - cx;
                    let dy = y - cy;
                    let dist = Math.hypot(dx, dy);
                    let warp = Math.max(0, (180 - dist) * 0.25);
                    let wx = x - (dx / (dist + 1)) * warp;
                    let wy = y - (dy / (dist + 1)) * warp;

                    if (y === 0) ctx.moveTo(wx, wy);
                    else ctx.lineTo(wx, wy);
                }
                ctx.stroke();
            }

            // 2. Núcleo de Matéria Decaída Estabilizada (Massa de Estrela de Nêutrons)
            const time = Date.now() * 0.003;
            ctx.shadowColor = '#bd00ff';
            ctx.shadowBlur = 30;
            ctx.fillStyle = '#120024';
            ctx.strokeStyle = '#bd00ff';
            ctx.lineWidth = 3;

            ctx.beginPath();
            ctx.arc(cx, cy, 60, 0, Math.PI * 2);
            ctx.fill();
            ctx.stroke();

            // Anel Gravitacional Relativístico
            ctx.strokeStyle = '#ff00ab';
            ctx.beginPath();
            ctx.ellipse(cx, cy, 110, 35, time, 0, Math.PI * 2);
            ctx.stroke();

            // 3. Atualizar Projéteis com Desvio de Trajetória Gravitacional
            for (let i = projectiles.length - 1; i >= 0; i--) {
                let p = projectiles[i];
                let dx = cx - p.x;
                let dy = cy - p.y;
                let dist = Math.hypot(dx, dy);

                // Gravidade curvando o projetil/laser
                if (dist < 220) {
                    let force = (220 - dist) * 0.08;
                    p.vy += (dy / dist) * force;
                    p.vx += (dx / dist) * force * 0.2;
                }

                p.x += p.vx;
                p.y += p.vy;

                ctx.fillStyle = p.type === 'laser' ? '#ff0055' : '#00f3ff';
                ctx.shadowColor = ctx.fillStyle;
                ctx.shadowBlur = 10;
                ctx.beginPath();
                ctx.arc(p.x, p.y, 4, 0, Math.PI * 2);
                ctx.fill();

                if (p.x > w || p.y < 0 || p.y > h) projectiles.splice(i, 1);
            }

            hudText.innerHTML = `
                DENSIDADE DO NÚCLEO: <span style="color:#bd00ff;">1.8x10¹⁴ g/cm³ (QUARK-GLUON)</span><br>
                LENSING GRAVITACIONAL: DESVIANDO TRAJETÓRIAS BALÍSTICAS<br>
                DEFORMAÇÃO DA MALHA 4D: ATIVA
            `;
        }

        // DESENHO: MÓDULO 3 (CRISTAIS DE MEMÓRIA DE BRANA - CALABI-YAU)
        function drawBranaModule() {
            const w = canvas.width;
            const h = canvas.height;
            const cx = w / 2;
            const cy = h / 2;

            if (isBigCrunchActive) {
                crunchScale -= 0.005;
                if (crunchScale <= 0.05) {
                    crunchScale = 0.05; // O espaço 4D morre, mas o cristal 6D permanece
                }
            }

            ctx.save();
            ctx.translate(cx, cy);

            // Se Big Crunch, colapsar espaço ao redor
            if (isBigCrunchActive) {
                ctx.fillStyle = 'rgba(0,0,0,0.85)';
                ctx.fillRect(-cx, -cy, w, h);
            }

            // Desenhar Geometria de Calabi-Yau 11D (Projeção Harmônica)
            const time = Date.now() * 0.002;
            ctx.strokeStyle = isBigCrunchActive ? '#00f3ff' : 'rgba(0, 243, 255, 0.6)';
            ctx.lineWidth = 1.5;

            for (let i = 0; i < 6; i++) {
                ctx.beginPath();
                let angle = (i * Math.PI / 3) + time;
                let r = 70 * (isBigCrunchActive ? 1.0 : crunchScale);
                let x = Math.cos(angle) * r;
                let y = Math.sin(angle) * r;

                ctx.ellipse(x, y, 60, 25, angle, 0, Math.PI * 2);
                ctx.stroke();
            }

            // Cristal Eterno de Dados no Centro (Indestrutível)
            ctx.fillStyle = '#00f3ff';
            ctx.shadowColor = '#00f3ff';
            ctx.shadowBlur = 25;
            ctx.beginPath();
            ctx.arc(0, 0, 12, 0, Math.PI * 2);
            ctx.fill();

            ctx.restore();

            hudText.innerHTML = `
                ESPAÇO CALABI-YAU: <span style="color:#00f3ff;">6ª DIMENSÃO (ESPAÇO DE HILBERT)</span><br>
                UNIVERSO 4D: ${isBigCrunchActive ? '<span style="color:#ff0055;">COLAPSADO (BIG CRUNCH)</span>' : 'ESTÁVEL'}<br>
                INTEGRIDADE DOS DADOS DE BRANA: <span style="color:#00ff66;">100.0% INTACTO</span>
            `;
        }

        // LOOP PRINCIPAL DE RENDERIZAÇÃO
        function render() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Grade do Fundo
            ctx.strokeStyle = 'rgba(0, 243, 255, 0.03)';
            ctx.lineWidth = 1;
            for (let x = 0; x < canvas.width; x += 40) {
                ctx.beginPath(); ctx.moveTo(x, 0); ctx.lineTo(x, canvas.height); ctx.stroke();
            }

            if (currentModule === 'bio') drawBioModule();
            else if (currentModule === 'quark') drawQuarkModule();
            else drawBranaModule();

            requestAnimationFrame(render);
        }

        // INICIALIZAÇÃO
        resizeCanvas();
        render();
    </script>
</body>
</html>
