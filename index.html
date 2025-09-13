<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>给最爱的胡英茹宝宝</title>
    <style>
        :root{
            --bg:#05030b;
            --accent:#ff8fb1;
            --accent-2:#ffd2e6;
            --text:#f3eaf0;
        }
        html,body{
            height:100%;
            margin:0;
            background:var(--bg);
            color:var(--text);
            font-family:"Microsoft YaHei",system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
            overflow:hidden; /* 关闭浏览器默认滚动条 */
        }

        /* 布局：容器固定，高度100vh，每屏占满 */
        .wrap {
            position:relative;
            width:100%;
            height:100vh;
            overflow:hidden;
        }
        .sections {
            position:absolute;
            top:0; left:0;
            width:100%;
            height:100%;
            transition: transform 700ms cubic-bezier(.22,.9,.32,1);
            will-change: transform;
        }
        .section {
            width:100%;
            height:100vh;
            position:relative;
            display:flex;
            align-items:center;
            justify-content:center;
            flex-direction:column;
            box-sizing:border-box;
            padding:28px;
        }

        /* canvas 层级 */
        canvas#starfield, canvas#trail, canvas#fx {
            position:fixed; left:0; top:0;
            width:100%; height:100%;
            z-index:0;
            pointer-events:none;
        }

        /* UI */
        .ui {
            position:relative;
            z-index:6;
            pointer-events:auto;
            width:100%;
            height:100%;
            display:flex;
            align-items:center;
            justify-content:center;
            flex-direction:column;
            text-align:center;
            padding:24px;
        }
        .title {
            color:var(--accent);
            font-weight:700;
            font-size:clamp(26px, 4.2vw, 48px);
            text-shadow:0 0 18px rgba(255,140,177,0.18);
            user-select:none;
            margin-bottom:10px;
        }
        .subtitle {
            color:var(--accent-2);
            font-size:clamp(14px, 1.6vw, 18px);
            margin-bottom:18px;
        }

        /* 全屏和音乐按钮 */
        .top-right {
            position:fixed; right:18px; top:14px; z-index:9; display:flex; gap:8px; align-items:center;
        }
        .btn {
            background:linear-gradient(180deg, rgba(255,255,255,0.04), rgba(255,255,255,0.02));
            border:1px solid rgba(255,255,255,0.06);
            color:var(--text);
            padding:8px 12px;
            border-radius:12px;
            cursor:pointer;
            font-size:14px;
            box-shadow:0 8px 20px rgba(0,0,0,0.5);
        }
        .btn:active{ transform:translateY(1px); }

        /* 第一屏：爱心提示 */
        .hint {
            margin-top:12px;
            color:rgba(255,255,255,0.8);
            font-size:13px;
        }

        /* 时间轴（第二屏）*/
        .timeline {
            width:min(840px, 86%);
            max-width:920px;
            background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
            border-radius:14px;
            padding:26px;
            box-shadow:0 10px 40px rgba(4,2,8,0.6);
            border:1px solid rgba(255,255,255,0.03);
        }
        .timeline .tip { color:#d6c9d8; font-size:13px; text-align:left; margin-bottom:12px; }
        .tl-list { display:flex; flex-direction:column; gap:14px; }
        .tl-item {
            display:flex; gap:12px; align-items:flex-start; cursor:pointer;
            padding:12px; border-radius:10px;
            transition: background .18s, transform .12s;
        }
        .tl-item:hover { background:rgba(255,143,177,0.04); transform:translateY(-3px); }
        .tl-dot { width:14px;height:14px;border-radius:50%; background:var(--accent); box-shadow:0 0 12px rgba(255,140,177,0.6); margin-top:6px; flex:0 0 14px; }
        .tl-content { text-align:left; }
        .tl-date { color:var(--accent-2); font-weight:600; font-size:14px; }
        .tl-desc { color:#e7dfe8; font-size:15px; max-width:720px; word-break:break-word; }

        /* 弹窗 */
        .popup {
            position:fixed; left:50%; top:50%; transform:translate(-50%,-50%);
            z-index:11; display:none;
            min-width:260px; max-width:88%; padding:18px; border-radius:12px;
            background:linear-gradient(180deg, rgba(6,4,8,0.9), rgba(8,6,12,0.95));
            box-shadow:0 12px 40px rgba(0,0,0,0.6); border:1px solid rgba(255,255,255,0.04);
            color:var(--text); text-align:center;
        }
        .popup .text { font-size:clamp(14px,1.7vw,20px); line-height:1.6; color:#ffdff0; }
        .popup .close { margin-top:14px; }

        /* 第三屏 合照 */
        .photo-wrap { width:min(780px,88%); max-width:880px; border-radius:14px; padding:18px; background:rgba(255,255,255,0.02); box-shadow:0 12px 40px rgba(0,0,0,0.6); border:1px solid rgba(255,255,255,0.03); }
        .photo {
            width:100%; height:460px; max-height:62vh; border-radius:10px; object-fit:cover;
            display:block; margin:0 auto; box-shadow:0 18px 60px rgba(0,0,0,0.6);
            animation: breathe 4s ease-in-out infinite;
        }
        @keyframes breathe { 0%{ transform:scale(1); filter:brightness(0.96);} 50%{ transform:scale(1.02); filter:brightness(1.06);} 100%{ transform:scale(1); filter:brightness(0.96);} }

        /* 第四屏 情话墙 */
        .lovewall {
            width:100%; height:60vh; display:flex; align-items:center; justify-content:center; position:relative;
        }
        .phrase {
            position:relative; z-index:7; font-size:clamp(20px,3.4vw,30px); color:#ffe9f2; padding:12px 18px; border-radius:10px;
            background:linear-gradient(90deg, rgba(255,143,177,0.08), rgba(255,255,255,0.02));
            box-shadow:0 8px 30px rgba(255,143,177,0.06);
            max-width:88%; word-break:break-word;
        }
        .stars-container { position:absolute; left:0; top:0; width:100%; height:100%; z-index:5; pointer-events:auto; }

        /* 小提示（左下）*/
        .page-hint { position:fixed; left:18px; bottom:14px; z-index:9; color:#d7c8d8; font-size:13px; }

        /* 分页小点（右侧） */
        .nav-dots { position:fixed; right:18px; top:50%; transform:translateY(-50%); display:flex; flex-direction:column; gap:10px; z-index:9; }
        .nav-dots button {
            width:10px; height:10px; border-radius:50%; border:none; background:rgba(255,255,255,0.12); cursor:pointer;
        }
        .nav-dots button.active { background:var(--accent); box-shadow:0 0 8px rgba(255,140,177,0.6); }

        /* 手机适配 */
        @media (max-width:720px){
            .timeline{ padding:18px; }
            .photo{ height:48vh; }
        }
    </style>
</head>
<body>
<!-- 背景 canvas -->
<canvas id="starfield"></canvas>
<!-- 鼠标拖尾 -->
<canvas id="trail"></canvas>
<!-- FX canvas（心形粒子也在这里绘制） -->
<canvas id="fx"></canvas>

<div class="wrap" id="wrap">
    <div class="sections" id="sections">
        <!-- 第一屏：爱心 -->
        <section class="section" data-index="0" style="background:transparent;">
            <div class="ui">
                <div class="title" id="names">汪卓一 ❤️ 胡英茹</div>
            </div>
        </section>

        <!-- 第二屏：时间轴 -->
        <section class="section" data-index="1" style="background:transparent;">
            <div class="ui">
                <div class="title">我们的故事</div>
                <div class="timeline" role="list">
                    <div class="tip">✨ 下面的文字点点看呢</div>
                    <div class="tl-list">
                        <div class="tl-item" data-text="那一天，我们第一次相遇，命运就此开始改变。">
                            <div class="tl-dot"></div>
                            <div class="tl-content">
                                <div class="tl-date">2025-07-03</div>
                                <div class="tl-desc">初次见面</div>
                            </div>
                        </div>

                        <div class="tl-item" data-text="生日快乐，你微笑的样子我永远记得。">
                            <div class="tl-dot"></div>
                            <div class="tl-content">
                                <div class="tl-date">2025-07-18</div>
                                <div class="tl-desc">你的生日</div>
                            </div>
                        </div>

                        <div class="tl-item" data-text="想在和你再一次一起去旅行，收获了满满的美好回忆。">
                            <div class="tl-dot"></div>
                            <div class="tl-content">
                                <div class="tl-date">2025-08-03</div>
                                <div class="tl-desc">还好你来了</div>
                            </div>
                        </div>

                        <div class="tl-item" data-text="好想每天都和你在一起">
                            <div class="tl-dot"></div>
                            <div class="tl-content">
                                <div class="tl-date">2025-08-20</div>
                                <div class="tl-desc">你想我就来</div>
                            </div>
                        </div>

                        <div class="tl-item" data-text="与你相伴处处是欢喜">
                            <div class="tl-dot"></div>
                            <div class="tl-content">
                                <div class="tl-date">2025-08-29</div>
                                <div class="tl-desc">又可以和你一起玩啦</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 第三屏：合照 -->
        <section class="section" data-index="2" style="background:transparent;">
            <div class="ui">
                <div class="title">最喜欢的合照</div>
                <div class="photo-wrap" role="img" aria-label="我们的合照">
                    <img id="photoImg" class="photo" src="1.png" alt="我们的合照"
                         onerror="this.style.display='none'; this.parentElement.insertAdjacentHTML('beforeend','<div style=&quot;color:#d8c8d8;padding:30px;text-align:center;&quot;>未找到 photo.jpg， 请把合照放在同一目录并命名为 photo.jpg 或修改代码</div>')">
                </div>
            </div>
        </section>

        <!-- 第四屏：情话墙 -->
        <section class="section" data-index="3" style="background:transparent;">
            <div class="ui">
                <div class="title">爱你哦~多看一会还有呢</div>

                <div class="lovewall" id="lovewall">
                    <div class="phrase" id="phraseBox">每一句都是我对你的悄悄话……</div>
                    <div class="stars-container" id="starsContainer"></div>
                </div>
            </div>
        </section>
    </div>
</div>

<!-- 弹窗 -->
<div class="popup" id="popup">
    <div class="text" id="popupText"></div>
    <div style="text-align:center;"><button class="btn close" id="closePopup">知道了</button></div>
</div>

<!-- 操作控件 -->
<div class="top-right">
    <button class="btn" id="playBtn">播放音乐</button>
    <button class="btn" id="fullscreenBtn">进入全屏</button>
</div>

<!-- 页脚提示 -->
<div class="page-hint">上下翻页：鼠标滚轮 / ↑↓ 键 / 触摸滑动（移动设备）/ 双击看看呢~嘻嘻 </div>

<!-- 右侧小点导航 -->
<div class="nav-dots" id="navDots" aria-hidden="true">
    <button data-index="0" class="active"></button>
    <button data-index="1"></button>
    <button data-index="2"></button>
    <button data-index="3"></button>
</div>

<!-- 背景音乐 -->
<audio id="bgm" src="bgm.mp3" loop preload="auto"></audio>

<script>
    /* ===========================
       全局配置与工具
       =========================== */
    const sectionsEl = document.getElementById('sections');
    const totalSections = 4;
    let currentIndex = 0;
    let scrolling = false;
    const navDots = document.getElementById('navDots').children;

    function goTo(index){
        if(index < 0) index = 0;
        if(index >= totalSections) index = totalSections - 1;
        currentIndex = index;
        const y = - index * window.innerHeight;
        sectionsEl.style.transform = `translateY(${y}px)`;
        // 更新 nav dot
        for(let b of navDots) b.classList.remove('active');
        navDots[index].classList.add('active');
    }

    /* 禁止默认滚动并实现自定义翻页（鼠标滚轮）*/
    let wheelTimeout = null;
    window.addEventListener('wheel', (e)=>{
        e.preventDefault();
        if(wheelTimeout) return;
        wheelTimeout = setTimeout(()=> wheelTimeout = null, 300);
        if(e.deltaY > 0) goTo(currentIndex + 1);
        else goTo(currentIndex - 1);
    }, {passive:false});

    /* 键盘翻页 */
    window.addEventListener('keydown', (e)=>{
        if(e.key === 'ArrowDown' || e.key === 'PageDown') goTo(currentIndex + 1);
        if(e.key === 'ArrowUp' || e.key === 'PageUp') goTo(currentIndex - 1);
    });

    /* 触摸滑动翻页（移动设备）*/
    let touchStartY = 0;
    window.addEventListener('touchstart', (e)=> { touchStartY = e.touches[0].clientY; }, {passive:true});
    window.addEventListener('touchend', (e)=>{
        const dy = (e.changedTouches[0].clientY - touchStartY);
        if(dy < -40) goTo(currentIndex + 1);
        if(dy > 40) goTo(currentIndex - 1);
    }, {passive:true});

    /* 点击右侧小点跳转 */
    document.getElementById('navDots').addEventListener('click', (e)=>{
        const b = e.target.closest('button');
        if(!b) return;
        const idx = Number(b.getAttribute('data-index'));
        goTo(idx);
    });

    /* 窗口调整时保持位置 */
    window.addEventListener('resize', ()=> { goTo(currentIndex); });

    /* ===========================
       星辰与拖尾 & 爱心粒子
       =========================== */
    const starCanvas = document.getElementById('starfield');
    const trailCanvas = document.getElementById('trail');
    const fxCanvas = document.getElementById('fx');
    const starCtx = starCanvas.getContext('2d');
    const trailCtx = trailCanvas.getContext('2d');
    const fxCtx = fxCanvas.getContext('2d');

    function fitCanvas(canvas){
        const dpr = window.devicePixelRatio || 1;
        canvas.width = window.innerWidth * dpr;
        canvas.height = window.innerHeight * dpr;
        canvas.style.width = window.innerWidth + 'px';
        canvas.style.height = window.innerHeight + 'px';
        const ctx = canvas.getContext('2d');
        ctx.setTransform(dpr,0,0,dpr,0,0);
    }
    /* 初始调节 */
    fitCanvas(starCanvas); fitCanvas(trailCanvas); fitCanvas(fxCanvas);
    window.addEventListener('resize', ()=> { fitCanvas(starCanvas); fitCanvas(trailCanvas); fitCanvas(fxCanvas); });

    /* 星辰背景 */
    let stars = [];
    function generateStars(){
        stars = [];
        const count = Math.max(120, Math.floor(window.innerWidth / 6));
        for(let i=0;i<count;i++){
            stars.push({
                x: Math.random()*window.innerWidth,
                y: Math.random()*window.innerHeight,
                r: Math.random()*1.6 + 0.2,
                tw: Math.random()*Math.PI*2,
                twSpeed: (Math.random()*0.02+0.004),
                alphaBase: 0.3 + Math.random()*0.7
            });
        }
    }
    generateStars();

    /* 流星 */
    let meteors = [];
    function spawnMeteor(){
        if(Math.random() < 0.02){
            meteors.push({
                x: Math.random() * window.innerWidth * 0.8 + window.innerWidth*0.1,
                y: -20,
                vx: -4 - Math.random()*6,
                vy: 6 + Math.random()*6,
                life:0, maxLife: 40 + Math.floor(Math.random()*40)
            });
        }
    }

    /* 鼠标拖尾 */
    let trails = [];
    window.addEventListener('mousemove', (e)=>{
        // 鼠标拖尾点
        trails.push({x:e.clientX, y:e.clientY, life:0, maxLife:18 + Math.floor(Math.random()*10)});
        // 控制长度
        if(trails.length > 120) trails.splice(0, trails.length - 120);
    });

    /* 爱心粒子（绘制在 fxCanvas） */
    const particles = [];
    const PARTICLE_COUNT = 380;
    let forming = true; // 聚合或散开
    function heartXY(t, scale=16){
        const x = 16*Math.pow(Math.sin(t),3);
        const y = -(13*Math.cos(t) - 5*Math.cos(2*t) - 2*Math.cos(3*t) - Math.cos(4*t));
        return {x:x*scale, y:y*scale};
    }
    function initParticles(){
        particles.length = 0;
        for(let i=0;i<PARTICLE_COUNT;i++){
            const t = (i / PARTICLE_COUNT) * Math.PI*2;
            const pos = heartXY(t,25);
            particles.push({
                x: Math.random()*window.innerWidth,
                y: Math.random()*window.innerHeight,
                tx: window.innerWidth/2 + pos.x,
                ty: window.innerHeight/3 + pos.y+130,
                vx:0, vy:0,
                size: Math.random()*1.8 + 0.6,
                speed: Math.random()*0.08 + 0.02,
                wobble: Math.random()*6.28,
                color: `rgba(255,${100+Math.floor(Math.random()*120)},${150+Math.floor(Math.random()*80)},1)`
            });
        }
    }
    initParticles();

    /* 动画循环 */
    let frame = 0;
    function animate(){
        frame++;
        // 星辰背景
        starCtx.clearRect(0,0,window.innerWidth,window.innerHeight);
        starCtx.fillStyle = '#04020a';
        starCtx.fillRect(0,0,window.innerWidth,window.innerHeight);
        stars.forEach(s=>{
            s.tw += s.twSpeed;
            const a = 0.35 + 0.65 * (0.5 + 0.5*Math.sin(s.tw));
            starCtx.beginPath();
            starCtx.fillStyle = `rgba(255,255,255,${(s.alphaBase*a).toFixed(3)})`;
            starCtx.arc(s.x, s.y, s.r, 0, Math.PI*2);
            starCtx.fill();
            s.y += 0.02;
            if(s.y > window.innerHeight) s.y = 0;
        });
        // 流星
        if(frame % 6 === 0) spawnMeteor();
        for(let i=meteors.length-1;i>=0;i--){
            const m=meteors[i];
            m.x += m.vx; m.y += m.vy; m.life++;
            const alpha = Math.max(0, 1 - m.life/m.maxLife);
            const grd = starCtx.createLinearGradient(m.x, m.y, m.x - m.vx*8, m.y - m.vy*8);
            grd.addColorStop(0, `rgba(255,255,255,${alpha})`);
            grd.addColorStop(1, `rgba(255,255,255,0)`);
            starCtx.strokeStyle = grd; starCtx.lineWidth = 2.5;
            starCtx.beginPath(); starCtx.moveTo(m.x, m.y); starCtx.lineTo(m.x - m.vx*6, m.y - m.vy*6); starCtx.stroke();
            if(m.life > m.maxLife) meteors.splice(i,1);
        }

        // 鼠标拖尾
        trailCtx.clearRect(0,0,window.innerWidth,window.innerHeight);
        for(let i=trails.length-1;i>=0;i--){
            const t = trails[i];
            t.life++;
            const alpha = 1 - t.life / t.maxLife;
            trailCtx.beginPath();
            trailCtx.fillStyle = `rgba(255,200,230,${(alpha*0.9).toFixed(2)})`;
            trailCtx.arc(t.x, t.y, Math.max(1, 6 * alpha), 0, Math.PI*2);
            trailCtx.fill();
            if(t.life > t.maxLife) trails.splice(i,1);
        }

        // 爱心粒子绘制与行为
        fxCtx.clearRect(0,0,window.innerWidth,window.innerHeight);
        for(const p of particles){
            if(forming){
                // 向目标移动
                p.vx += (p.tx - p.x) * (p.speed*0.06);
                p.vy += (p.ty - p.y) * (p.speed*0.06);
                p.vx *= 0.88; p.vy *= 0.88;
                p.x += p.vx; p.y += p.vy;
            } else {
                // 散开漂浮
                p.x += (Math.random()-0.5) * 3 + Math.sin(frame*0.01 + p.wobble) * 0.6;
                p.y += (Math.random()-0.3) * 1.6;
                // 保持在屏内
                if(p.x < -40) p.x = window.innerWidth + 40;
                if(p.x > window.innerWidth + 40) p.x = -40;
                if(p.y > window.innerHeight + 40) p.y = -40;
            }
            const wob = Math.sin(p.wobble + frame*0.02) * 0.8;
            fxCtx.beginPath();
            // 更柔和的颜色
            fxCtx.fillStyle = p.color.replace(/,1\)/,`,${0.85 + Math.sin(frame*0.01 + p.wobble)*0.08})`);
            fxCtx.arc(p.x + wob, p.y + wob, p.size, 0, Math.PI*2);
            fxCtx.fill();
        }
        requestAnimationFrame(animate);
    }
    animate();

    /* 点击名字触发聚合/散开 和 显示一句情话 */
    const namesEl = document.getElementById('names');
    const phraseBox = document.getElementById('phraseBox');
    const phrases = [
        "每一颗星都是我对你的心意。", "想和你一起看遍所有星河。", "余生漫长，你是我唯一的光。",
        "你笑起来的样子，我想收藏。", "世界很大，我只想和你在一起。", "所有浪漫都不及你一个侧脸。"
    ];
    namesEl.addEventListener('click', ()=>{
        forming = true;
        spawnConfettiEffect(window.innerWidth/2, window.innerHeight/3, 60);
        // 随机一句情话显示在情话墙的中间（兼容多屏）
        phraseBox.textContent = phrases[Math.floor(Math.random()*phrases.length)];
    });

    /* 散开/聚合切换（双击空白处切换）*/
    window.addEventListener('dblclick', ()=> { forming = !forming; });

    /* 使用 particles 之外的小方片效果）*/
    let confettis = [];
    function spawnConfettiEffect(x,y,amount=40){
        for(let i=0;i<amount;i++){
            confettis.push({
                x, y,
                vx: (Math.random()-0.5)*8,
                vy: (Math.random()-2)*6,
                size: 6 + Math.random()*10,
                rot: Math.random()*360,
                life:0, maxLife: 60 + Math.floor(Math.random()*40),
                color: ['#ff8fb1','#ffd28f','#c6a0ff','#fff48f'][Math.floor(Math.random()*4)]
            });
        }
    }
    function drawConfetti(){
        for(let i=confettis.length-1;i>=0;i--){
            const c = confettis[i];
            c.x += c.vx; c.y += c.vy; c.vy += 0.28; c.rot += c.vx*0.06; c.life++;
            fxCtx.save();
            fxCtx.translate(c.x, c.y);
            fxCtx.rotate(c.rot * Math.PI / 180);
            fxCtx.fillStyle = c.color;
            fxCtx.fillRect(-c.size/2, -c.size/2, c.size, Math.max(4,c.size*0.6));
            fxCtx.restore();
            if(c.life > c.maxLife || c.y > window.innerHeight + 100) confettis.splice(i,1);
        }
    }
    /* 在主循环中绘制 confetti*/
    (function loopConfetti(){
        requestAnimationFrame(loopConfetti);
        drawConfetti();
    })();

    /* ===========================
       时间轴点击弹窗
       =========================== */
    const items = document.querySelectorAll('.tl-item');
    const popup = document.getElementById('popup');
    const popupText = document.getElementById('popupText');
    const closePopup = document.getElementById('closePopup');
    items.forEach(it=>{
        it.addEventListener('click', ()=>{
            const t = it.getAttribute('data-text') || '';
            popupText.textContent = t;
            popup.style.display = 'block';
        });
    });
    closePopup.addEventListener('click', ()=> popup.style.display = 'none');

    /* ===========================
       合照（第三屏）
       =========================== */
    const photoImg = document.getElementById('photoImg');

    /* ===========================
       情话墙（第四屏星星 + 自动切换）
       =========================== */
    const starsContainer = document.getElementById('starsContainer');
    const phrasesList = [
        "你是我看过最浪漫的意外。",
        "愿余生有你相伴，不必多言。",
        "我想把每个明天都交给你。",
        "只要你在，朝朝暮暮都值得期待。",
        "你笑起来的样子，胜过一切星光。",
        "牵你的手，走到世界尽头也心甘情愿。",
        "喜欢你，是我做过最确定的一件事。"
    ];
    let autoIndex = 0;
    function showPhrase(idx){
        idx = (idx + phrasesList.length) % phrasesList.length;
        autoIndex = idx;
        phraseBox.textContent = phrasesList[idx];
    }
    /* 自动轮播 */
    let autoTimer = setInterval(()=> { showPhrase(autoIndex + 1); }, 4200);

    /* 生成一些可点击星星（小 DOM 元素） */
    function createStarElements(count=30){
        starsContainer.innerHTML = '';
        for(let i=0;i<count;i++){
            const s = document.createElement('div');
            s.style.position='absolute';
            s.style.left = Math.random()*92 + '%';
            s.style.top = Math.random()*82 + '%';
            s.style.width = s.style.height = (6 + Math.random()*12) + 'px';
            s.style.borderRadius = '50%';
            s.style.background = 'rgba(255,255,255,0.9)';
            s.style.boxShadow = '0 0 10px rgba(255,200,230,0.5)';
            s.style.cursor = 'pointer';
            s.style.opacity = 0.85;
            const phraseIdx = Math.floor(Math.random()*phrasesList.length);
            s.dataset.phrase = phrasesList[phraseIdx];
            s.addEventListener('click', (e)=>{
                clearInterval(autoTimer);
                showPhrase(phrasesList.indexOf(e.currentTarget.dataset.phrase));
                // 重新启动轮播延迟
                setTimeout(()=> { autoTimer = setInterval(()=> { showPhrase(autoIndex + 1); }, 4200); }, 6000);
            });
            starsContainer.appendChild(s);
        }
    }
    createStarElements(36);

    /* ===========================
       背景音乐控制
       =========================== */
    const bgm = document.getElementById('bgm');
    const playBtn = document.getElementById('playBtn');
    let playing = false;
    playBtn.addEventListener('click', ()=>{
        if(!playing){
            bgm.play().catch(()=>{ alert('有点Bug不会改😭😭😭'); });
            playBtn.textContent = '暂停音乐';
            playing = true;
        } else {
            bgm.pause(); playBtn.textContent = '播放音乐'; playing = false;
        }
    });
    /* 尝试在首次交互时自动播放 */
    window.addEventListener('click', ()=> {
        if(!playing){
            bgm.play().then(()=>{ playing=true; playBtn.textContent='暂停音乐'; }).catch(()=>{/* ignore */});
        }
    }, {once:true});

    /* ===========================
       全屏按钮
       =========================== */
    const fsBtn = document.getElementById('fullscreenBtn');
    fsBtn.addEventListener('click', ()=>{
        if(!document.fullscreenElement){
            document.documentElement.requestFullscreen().catch(()=>{ alert('无法进入全屏（浏览器限制）'); });
            fsBtn.textContent='退出全屏';
        } else {
            document.exitFullscreen().catch(()=>{/* ignore */});
            fsBtn.textContent='进入全屏';
        }
    });
    window.addEventListener('click', (e)=> {
        // 点击页面中部时偶尔触发小彩带
        if(Math.random() > 0.88) spawnConfettiEffect(e.clientX, e.clientY, 28);
    });
</script>
</body>
</html>
