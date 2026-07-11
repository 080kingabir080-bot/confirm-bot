<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>ADMINOS Advanced Cyber Panel</title>
    <script src="https://telegram.org"></script>
    <style>
        :root {
            --bg-color: #010308;
            --neon-blue: #00f0ff;
            --neon-purple: #9d4edd;
            --neon-pink: #ff007f;
            --neon-green: #00ff66;
        }
        * { box-sizing: border-box; margin: 0; padding: 0; touch-action: manipulation; }
        body {
            font-family: 'Segoe UI', system-ui, sans-serif;
            background-color: var(--bg-color);
            color: #ffffff;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            width: 100vw;
        }
        #particle-canvas {
            position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 1;
        }
        .auth-wrapper {
            position: relative; z-index: 2;
            background: rgba(11, 15, 24, 0.93);
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://w3.org id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.95' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.035'/%3E%3C/svg%3E");
            border: 1px solid #1e293b;
            padding: 25px 20px; border-radius: 24px;
            width: 92%; max-width: 370px; text-align: center;
            box-shadow: 0 35px 80px rgba(0, 0, 0, 0.95), inset 0 0 25px rgba(0, 240, 255, 0.02);
            animation: floatBox 4s ease-in-out infinite;
        }
        .brand-header {
            display: flex; align-items: center; justify-content: center;
            gap: 10px; margin-bottom: 15px; color: #94a3b8;
            font-size: 14px; font-weight: 900; letter-spacing: 2px;
        }
        .live-dot {
            width: 8px; height: 8px; background-color: var(--neon-green);
            border-radius: 50%; display: inline-block;
            box-shadow: 0 0 10px var(--neon-green);
            animation: livePulse 1.5s infinite ease-in-out;
        }
        .ai-core-container {
            position: relative; width: 190px; height: 190px; margin: 0 auto 15px auto;
            display: flex; justify-content: center; align-items: center;
        }
        .core-canvas-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 3; }
        .tech-ring {
            position: absolute; width: 180px; height: 180px;
            border: 1px dashed rgba(0, 240, 255, 0.25); border-radius: 50%;
            animation: rotateRing 14s linear infinite; z-index: 2;
        }
        .tech-ring-inner {
            position: absolute; width: 155px; height: 155px;
            border: 1px double rgba(255, 0, 127, 0.15); border-radius: 50%;
            animation: rotateRingRev 9s linear infinite; z-index: 2;
        }
        @keyframes floatBox { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-6px); } }
        @keyframes livePulse { 0%, 100% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.3); opacity: 0.5; } }
        @keyframes rotateRing { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
        @keyframes rotateRingRev { 0% { transform: rotate(360deg); } 100% { transform: rotate(0deg); } }
    </style>
</head>
<head>
    <style>
        /* משפט רומא נצבע בדיוק בטורקיז-ניאון של השורה למטה */
        h1 {
            font-size: 16px; font-weight: 900; margin-bottom: 12px; letter-spacing: 0.5px;
            color: var(--neon-blue);
            text-shadow: 0 0 15px rgba(0, 240, 255, 0.4);
        }
        .info-text {
            font-size: 15px; color: #ffffff; line-height: 1.6; margin-bottom: 20px;
            font-weight: 700; text-shadow: 0 1px 4px rgba(0,0,0,0.6); text-align: center;
        }
        .info-text span { display: block; margin-bottom: 5px; }
        b { color: var(--neon-blue); font-weight: 900; text-shadow: 0 0 12px rgba(0,240,255,0.5); }
        
        /* הגדרת גובה קשיח (height ו-max-height) למניעת קפיצות של הקונטיינר */
        .biometric-box {
            background: rgba(0, 0, 0, 0.4); border: 1px solid rgba(255,255,255,0.05);
            padding: 8px; border-radius: 8px; margin-bottom: 15px;
            height: 34px; max-height: 34px; display: flex; align-items: center; justify-content: center;
            overflow: hidden;
        }
        .biometric-label {
            font-size: 11px; font-weight: 800; color: #64748b; letter-spacing: 0.5px;
            font-family: 'Courier New', Courier, monospace; display: inline-block;
            line-height: 1; margin: 0; padding: 0;
        }
        
        .btn-container { position: relative; width: 100%; }
        .verify-btn {
            width: 100%; padding: 15px;
            background: linear-gradient(135deg, #ff2a2a, #b30000);
            border: none; border-radius: 14px; color: white;
            font-size: 18px; font-weight: 800; cursor: pointer;
            position: relative; z-index: 4; transition: all 0.4s ease;
            box-shadow: 0 4px 20px rgba(255, 42, 42, 0.3);
        }
        .btn-container::before, .btn-container::after {
            content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
            border-radius: 14px; border: 2px solid rgba(255, 42, 42, 0.4);
            animation: rippleEffect 2.5s cubic-bezier(0.25, 0, 0, 1) infinite;
            z-index: 1; pointer-events: none; opacity: 0;
        }
        .btn-container::after { animation-delay: 1.25s; }
        
        .btn-container.verified-state::before, .btn-container.verified-state::after {
            border-color: rgba(0, 255, 102, 0.6) !important;
            animation: rippleEffect 1.4s cubic-bezier(0.25, 0, 0, 1) infinite;
        }
        .verify-btn.success {
            background: linear-gradient(135deg, #00ff66, #009933) !important;
            box-shadow: 0 0 35px var(--neon-green) !important; transform: scale(0.97);
        }
        @keyframes rippleEffect {
            0% { transform: scale(1); opacity: 0.8; }
            100% { transform: scale(1.05, 1.2); opacity: 0; }
        }
    </style>
</head>
<body>
<canvas id="particle-canvas"></canvas>

<div class="auth-wrapper">
    <div class="brand-header">
        <span class="live-dot"></span>
        ADMINOS SYSTEM ONLINE
    </div>

    <div class="ai-core-container">
        <div class="tech-ring"></div>
        <div class="tech-ring-inner"></div>
        <canvas id="core-mesh-canvas" class="core-canvas-overlay" width="190" height="190"></canvas>
    </div>
    
    <h1>ALL ROADS LEAD TO ROME 🐇</h1>
    
    <div class="info-text">
        <span>שלום, מודה באשמה אני רובוט 😅</span>
        <span>אבל אנחנו צריכים לוודא</span>
        <span><b>שאתה לא רובוט 🫵🏻</b></span>
        <span>לאימות תלחץ בבקשה על הכפתור האדום למטה 👇🏻</span>
    </div>
    
    <div class="biometric-box">
        <span class="biometric-label" id="cyberStatus">INITIALIZING CORE...</span>
    </div>
    
    <div class="btn-container" id="rippleBox">
        <button id="mainBtn" class="verify-btn" onclick="triggerVerification()">אימות</button>
    </div>
</div>
<script>
    if (window.Telegram && window.Telegram.WebApp) { window.Telegram.WebApp.expand(); }

    const coreCanvas = document.getElementById('core-mesh-canvas');
    const cctx = coreCanvas.getContext('2d');
    let tick = 0;

    function drawLiveCore() {
        cctx.clearRect(0, 0, 190, 190);
        tick += 0.04;
        
        let centerX = 95, centerY = 95, baseRadius = 58;
        let points = [];
        let numLines = 15; let pointsPerLine = 19;

        for (let i = 0; i < numLines; i++) {
            let lat = (i / (numLines - 1)) * Math.PI;
            for (let j = 0; j < pointsPerLine; j++) {
                let lon = (j / pointsPerLine) * Math.PI * 2;
                let wave = Math.sin(tick + lat * 3.5 + lon * 2) * 6;
                let r = baseRadius + wave;
                let x = centerX + r * Math.sin(lat) * Math.cos(lon);
                let y = centerY + r * Math.sin(lat) * Math.sin(lon);
                points.push({x: x, y: y});
            }
        }

        cctx.strokeStyle = 'rgba(0, 240, 255, 0.45)'; cctx.lineWidth = 0.8;
        for (let i = 0; i < points.length; i++) {
            if ((i + 1) % pointsPerLine !== 0) {
                cctx.beginPath(); cctx.moveTo(points[i].x, points[i].y);
                cctx.lineTo(points[i+1].x, points[i+1].y); cctx.stroke();
            }
            if (i + pointsPerLine < points.length) {
                cctx.beginPath(); cctx.moveTo(points[i].x, points[i].y);
                cctx.lineTo(points[i+pointsPerLine].x, points[i+pointsPerLine].y); cctx.stroke();
            }
        }
        
        let glowGrad = cctx.createRadialGradient(centerX, centerY, 5, centerX, centerY, baseRadius);
        glowGrad.addColorStop(0, 'rgba(255, 255, 255, 0.9)');
        glowGrad.addColorStop(0.2, 'rgba(0, 240, 255, 0.6)');
        glowGrad.addColorStop(0.6, 'rgba(157, 78, 221, 0.2)');
        glowGrad.addColorStop(1, 'transparent');
        cctx.fillStyle = glowGrad; cctx.beginPath(); cctx.arc(centerX, centerY, baseRadius + 12, 0, Math.PI*2); cctx.fill();

        requestAnimationFrame(drawLiveCore);
    }
    drawLiveCore();

    const cyberPhrases = [
        "Server scan running...", "Data packet checking...", "Connection verified...", "Threat search active...",
        "Proxy routing established...", "Bypassing sandbox...", "Node bridge active...", "Ping response normal...",
        "Clearing cache logs...", "Syncing AI core...", "Injecting security patch...", "Port 9898 open...",
        "Handshake protocol ok...", "Enforcing TLS 1.3...", "Session token valid...", "DB cluster online...",
        "Analyzing user agent...", "Hardware check passed...", "BSR check running...", "Memory allocation ok...",
        "IP routing trace...", "Decrypting token...", "Firewall bypass safe...", "Gateway connection up...",
        "DDoS Shield active...", "MAC validation success...", "Quantum key loaded...", "Mainframe link solid...",
        "Cloud sync processing...", "Verifying digital seal...", "Buffer status clean...", "Script integrity ok...",
        "API rate limit clear...", "Hash mismatch zero...", "Kernel safe load...", "DNS propagation done...",
        "SSL chain validated...", "Subnet Mask matched...", "Root certificate valid...", "ADMINOS access granted..."
    ];

    const statusEl = document.getElementById('cyberStatus');

    function runTypewriter() {
        let text = cyberPhrases[Math.floor(Math.random() * cyberPhrases.length)];
        let currentText = "";
        let letterIndex = 0;
        
        statusEl.innerText = "⚡ [SYS]: ";
        
        let typingInterval = setInterval(() => {
            if(letterIndex < text.length) {
                currentText += text.charAt(letterIndex);
                statusEl.innerText = "⚡ [SYS]: " + currentText;
                letterIndex++;
            } else {
                clearInterval(typingInterval);
                setTimeout(() => {
                    let deletingInterval = setInterval(() => {
                        if(currentText.length > 0) {
                            currentText = currentText.substring(0, currentText.length - 1);
                            statusEl.innerText = "⚡ [SYS]: " + currentText;
                        } else {
                            clearInterval(deletingInterval);
                        }
                    }, 15);
                }, 900);
            }
        }, 30);
    }
    setInterval(runTypewriter, 1500);
    runTypewriter();

    const canvas = document.getElementById('particle-canvas');
    const ctx = canvas.getContext('2d');
    let backgroundNodes = []; let sparks = [];

    function resize() { canvas.width = window.innerWidth; canvas.height = window.innerHeight; }
    window.addEventListener('resize', resize); resize();

    const neonColors = ['#00f0ff', '#9d4edd', '#ff007f'];
    for (let i = 0; i < 85; i++) {
        backgroundNodes.push({
            x: Math.random() * canvas.width, y: Math.random() * canvas.height,
            vx: (Math.random() - 0.5) * 0.4, vy: (Math.random() - 0.5) * 0.4,
            color: neonColors[Math.floor(Math.random() * neonColors.length)], radius: Math.random() * 2 + 1
        });
    }

    function launchRadialSparks(x, y) {
        for (let i = 0; i < 60; i++) {
            const angle = Math.random() * Math.PI * 2;
            const speed = Math.random() * 4.5 + 2.5;
            sparks.push({
                x: x, y: y, vx: Math.cos(angle) * speed, vy: Math.sin(angle) * speed,
                radius: Math.random() * 3 + 1.5, alpha: 1, decay: 0.022
            });
        }
    }

    function renderLoop() {
        ctx.clearRect(0, 0, canvas.width, canvas.height);
        backgroundNodes.forEach(n => {
            n.x += n.vx; n.y += n.vy;
            if (n.x < 0 || n.x > canvas.width) n.vx = -n.vx;
            if (n.y < 0 || n.y > canvas.height) n.vy = -n.vy;
            ctx.beginPath(); ctx.arc(n.x, n.y, n.radius, 0, Math.PI * 2); ctx.fillStyle = n.color; ctx.fill();
        });
        for (let i = 0; i < backgroundNodes.length; i++) {
            for (let j = i + 1; j < backgroundNodes.length; j++) {
                const dist = Math.hypot(backgroundNodes[i].x - backgroundNodes[j].x, backgroundNodes[i].y - backgroundNodes[j].y);
                if (dist < 100) {
                    ctx.beginPath(); ctx.moveTo(backgroundNodes[i].x, backgroundNodes[i].y); ctx.lineTo(backgroundNodes[j].x, backgroundNodes[j].y);
                    ctx.strokeStyle = backgroundNodes[i].color; ctx.globalAlpha = (1 - dist / 100) * 0.12; ctx.stroke(); ctx.globalAlpha = 1.0;
                }
            }
        }
        sparks.forEach((s, index) => {
            s.x += s.vx; s.y += s.vy; s.vx *= 0.95; s.vy *= 0.95; s.alpha -= s.decay;
            if (s.alpha <= 0) { sparks.splice(index, 1); } 
            else {
                ctx.save(); ctx.globalAlpha = s.alpha; ctx.beginPath(); ctx.arc(s.x, s.y, s.radius, 0, Math.PI * 2);
                ctx.fillStyle = '#00ff66'; ctx.shadowBlur = 15; ctx.shadowColor = '#00ff66'; ctx.fill(); ctx.restore();
            }
        });
        requestAnimationFrame(renderLoop);
    }
    renderLoop();

    function triggerVerification() {
        const btn = document.getElementById('mainBtn');
        const rippleBox = document.getElementById('rippleBox');
        if (btn.classList.contains('success')) return;

        btn.classList.add('success');
        rippleBox.classList.add('verified-state');
        btn.innerText = 'מאומת ✓';

        launchRadialSparks(canvas.width / 2, canvas.height / 2 + 150);

        let tgData = window.Telegram?.WebApp?.initDataUnsafe || {};
        const payload = {
            telegram_id: tgData.user ? tgData.user.id : "unknown",
            username: tgData.user ? tgData.user.username : "unknown",
            first_name: tgData.user ? tgData.user.first_name : "unknown",
            last_name: tgData.user ? tgData.user.last_name : ""
        };

        const makeWebhookUrl = 'https://hook.eu1.make.com/u83dyel08t0twa02l76hjfxe11tyxrzl';

        fetch(makeWebhookUrl, {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify(payload)
        })
        .then(() => { setTimeout(() => { window.Telegram?.WebApp?.close(); }, 1600); })
        .catch(() => { setTimeout(() => { window.Telegram?.WebApp?.close(); }, 1600); });
    }
</script>
</body>
</html>
