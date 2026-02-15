<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Missão: Amor Infinito</title>
<style>
body {
    margin: 0;
    font-family: 'Courier New', monospace;
    background: black;
    color: #00ff88;
    text-align: center;
    overflow-x: hidden;
}

.screen { display: none; padding: 40px; }
.active { display: block; }

button {
    padding: 12px 20px;
    margin: 10px;
    background: #00ff88;
    border: none;
    cursor: pointer;
    font-weight: bold;
}

.progress-bar {
    width: 80%;
    height: 30px;
    border: 2px solid #00ff88;
    margin: 20px auto;
}

.progress { height: 100%; width: 0%; background: #00ff88; }

/* ===== BATALHA ===== */
.battle-area {
    position: relative;
    height: 220px;
    margin-top: 20px;
}

.dragon {
    position: absolute;
    right: 20%;
    font-size: 90px;
    cursor: pointer;
    animation: dragonMove 2s infinite alternate ease-in-out;
}

@keyframes dragonMove {
    from { transform: translateY(0px); }
    to { transform: translateY(-20px); }
}

.knight {
    position: absolute;
    left: 20%;
    font-size: 80px;
}

.attack {
    animation: knightAttack 0.3s ease;
}

@keyframes knightAttack {
    0% { transform: translateX(0); }
    50% { transform: translateX(30px); }
    100% { transform: translateX(0); }
}

.dragon-death {
    animation: dragonDeath 1s forwards;
}

@keyframes dragonDeath {
    0% { transform: scale(1) rotate(0deg); opacity: 1; }
    100% { transform: scale(0) rotate(90deg); opacity: 0; }
}

.explosion {
    position: absolute;
    font-size: 30px;
    animation: explode 0.8s forwards;
}

@keyframes explode {
    from { transform: scale(0.5); opacity: 1; }
    to { transform: scale(2); opacity: 0; }
}

.shake {
    animation: shakeScreen 0.5s;
}

@keyframes shakeScreen {
    0% { transform: translate(0,0); }
    25% { transform: translate(-10px,5px); }
    50% { transform: translate(10px,-5px); }
    75% { transform: translate(-5px,5px); }
    100% { transform: translate(0,0); }
}

.victory-screen {
    position: fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:black;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    color:#00ff88;
    font-size:30px;
    z-index:999;
}

.floating {
    position: absolute;
    font-size: 20px;
    animation: floatUp 4s linear infinite;
}

@keyframes floatUp {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-600px); opacity: 0; }
}
</style>
</head>
<body>

<div id="loading" class="screen active">
    <h1>Loading...</h1>
    <div class="progress-bar">
        <div class="progress" id="progress"></div>
    </div>
</div>

<div id="menu" class="screen">
    <h1>🎮 Missão: Amor Infinito 🎮</h1>
    <button onclick="showScreen('rpg')">🧙 RPG do Amor</button>
    <button onclick="showScreen('achievement')">🏆 Conquistas</button>
    <button onclick="showScreen('final')">💍 Missão Final</button>
</div>

<div id="rpg" class="screen">
    <h2>Ficha do Jogador</h2>
    <input type="text" id="playerName" placeholder="Digite seu nome de jogador" />
    <button onclick="saveName()">Confirmar Nome</button>
    <div id="playerCard" style="margin-top:20px; display:none;">
        <p>Nome: <span id="displayName"></span></p>
        <p>Classe: Conquistador Lendário</p>
        <p>HP: 100 ❤️</p>
        <button onclick="startDragonFight()">🐉 Lutar contra o Dragão</button>
    </div>

    <div id="dragonGame" style="margin-top:30px; display:none;">
        <h3>⚔️ Batalha contra o Dragão</h3>
        <p id="dragonHP">50</p>
        <div class="battle-area">
            <div class="knight" id="knight">🛡️</div>
            <div class="dragon" id="dragon" onclick="attackDragon()">🐉</div>
        </div>
    </div>

    <button onclick="showScreen('menu')">Voltar</button>
</div>

<div id="achievement" class="screen">
    <h2>🏆 Achievements</h2>
    <p>✔ Primeiro Beijo</p>
    <p>✔ Primeira Risada</p>
    <p id="nameAchievement">🔒 Amor Lendário</p>
    <button onclick="showScreen('menu')">Voltar</button>
</div>

<div id="final" class="screen">
    <h2>💍 Missão Final</h2>
    <p>Você aceita ser meu player 2 para sempre?</p>
    <button>SIM ❤️</button>
    <button id="noBtn">NÃO 😈</button>
    <button onclick="showScreen('menu')">Voltar</button>
</div>

<script>

// LOADING
let progress = 0;
let interval = setInterval(() => {
    progress += 5;
    document.getElementById('progress').style.width = progress + '%';
    if(progress >= 100) {
        clearInterval(interval);
        showScreen('menu');
    }
}, 200);

function showScreen(id) {
    document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
}

// RPG
let dragonLife = 50;
let combo = 0;
let phase = 1;

function saveName() {
    const name = document.getElementById('playerName').value;
    if(name.trim() !== '') {
        document.getElementById('displayName').innerText = name;
        document.getElementById('playerCard').style.display = 'block';
        document.getElementById('nameAchievement').innerText = '✔ ' + name + ' conquistou o Amor Supremo ❤️';
    }
}

function startDragonFight() {
    dragonLife = phase === 1 ? 50 : 80;
    combo = 0;
    document.getElementById('dragonHP').innerText = dragonLife;
    document.getElementById('dragonGame').style.display = 'block';
}

function attackDragon() {
    const knight = document.getElementById('knight');
    const dragon = document.getElementById('dragon');

    if(dragonLife > 0) {
        knight.classList.add('attack');
        setTimeout(() => knight.classList.remove('attack'), 300);

        dragonLife--;
        combo++;

        document.getElementById('dragonHP').innerText = dragonLife + ' | Combo: ' + combo;
    }

    if(dragonLife <= 0) {
        dragon.classList.add('dragon-death');
        document.body.classList.add('shake');

        const battleArea = document.querySelector('.battle-area');
        for(let i=0;i<8;i++){
            const boom = document.createElement('div');
            boom.classList.add('explosion');
            boom.innerText = '💥';
            boom.style.left = (Math.random()*200 + 200) + 'px';
            boom.style.top = (Math.random()*100 + 50) + 'px';
            battleArea.appendChild(boom);
            setTimeout(()=> boom.remove(),800);
        }

        setTimeout(() => {
            document.body.classList.remove('shake');
            showVictory();
        }, 1000);
    }
}

function showVictory() {
    const victory = document.createElement('div');
    victory.classList.add('victory-screen');
    victory.innerHTML = '🏆 VITÓRIA ÉPICA 🏆<br><br>Combo Final: ' + combo +
    '<br><br><button onclick="startPhaseTwo()">Fase 2 🔥</button>';
    document.body.appendChild(victory);
}

function startPhaseTwo() {
    document.querySelector('.victory-screen').remove();
    phase = 2;
    dragonLife = 80;
    combo = 0;
    document.getElementById('dragon').innerText = '🐲';
    document.getElementById('dragonGame').style.display = 'block';
    document.getElementById('dragonHP').innerText = dragonLife;
}

// BOTÃO QUE FOGE
// ===== PEDIDO FINAL CINEMATOGRÁFICO =====

// botão SIM
const finalScreen = document.getElementById('final');
const simBtn = finalScreen.querySelector('button');
const noBtn = document.getElementById('noBtn');

// BOTÃO NÃO FOGE
noBtn.addEventListener('mouseover', () => {
    noBtn.style.position = 'absolute';
    noBtn.style.left = Math.random() * (window.innerWidth - 100) + 'px';
    noBtn.style.top = Math.random() * (window.innerHeight - 50) + 'px';
});

// BOTÃO SIM ATIVA FINAL
simBtn.addEventListener('click', () => {

    const playerName = document.getElementById('displayName').innerText || "Meu Amor";

    const loveScreen = document.createElement('div');
    loveScreen.classList.add('victory-screen');
    loveScreen.style.background = 'radial-gradient(circle at center, #1a001f, black)';
    loveScreen.innerHTML = `
        <div style="animation: floatText 3s ease-in-out infinite;">
            <h1 style="font-size:40px; color:#ff4da6;">💖 ELE DISSE SIM 💖</h1>
            <p style="max-width:600px; margin:20px auto; font-size:20px;">
            ${playerName}, desde o primeiro momento você virou meu parceiro favorito 💕<br><br>
            Meu Player 2 eterno, meu companheiro de todas as fases da vida.<br><br>
            Que a gente enfrente todos os chefões juntos,
            suba de nível no amor todos os dias
            e nunca aperte "Game Over" na nossa história. 🎮❤️<br><br>
            Te escolho hoje e em todas as próximas fases.
            </p>
        </div>
    `;

    document.body.appendChild(loveScreen);

    createLoveHearts();
});

function createLoveHearts() {
    for(let i = 0; i < 60; i++) {
        const heart = document.createElement('div');
        heart.classList.add('floating');
        heart.innerText = '💖';
        heart.style.left = Math.random() * window.innerWidth + 'px';
        heart.style.top = window.innerHeight + 'px';
        heart.style.fontSize = (20 + Math.random() * 30) + 'px';
        heart.style.animationDuration = (3 + Math.random() * 3) + 's';
        document.body.appendChild(heart);
        setTimeout(() => heart.remove(), 5000);
    }
}


// CORAÇÕES
setInterval(() => {
    const heart = document.createElement('div');
    heart.classList.add('floating');
    heart.innerText = '❤️';
    heart.style.left = Math.random() * window.innerWidth + 'px';
    heart.style.top = window.innerHeight + 'px';
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 4000);
}, 600);

</script>

</body>
</html>
