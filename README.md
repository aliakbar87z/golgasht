[ghorekeshie2.html](https://github.com/user-attachments/files/28667807/ghorekeshie2.html)
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قرعه‌کشیه | با مدیریت خانم قیصری</title>
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazir-font@v33.1.0/dist/font-face.css" rel="stylesheet" type="text/css" />
    <style>
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body {
            font-family: 'Vazir', 'Tahoma', 'Segoe UI', sans-serif;
            background: #1a0b2e;
            display: flex; justify-content: center; align-items: center;
            min-height: 100vh; padding: 20px; overflow-x: hidden; position: relative;
        }
        body::before {
            content: ""; position: fixed; top: 0; left: 0;
            width: 100%; height: 100%;
            background: linear-gradient(45deg, #ff006e, #8338ec, #3a86ff, #ffbe0b, #fb5607);
            background-size: 400% 400%; animation: gradientShift 12s ease infinite; z-index: -3;
        }
        @keyframes gradientShift { 0% { background-position: 0% 50%; } 50% { background-position: 100% 50%; } 100% { background-position: 0% 50%; } }
        .particles { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: -2; }
        .particle { position: absolute; background: rgba(255,255,255,0.7); border-radius: 50%; box-shadow: 0 0 20px rgba(255,255,255,0.8), 0 0 40px rgba(255,200,0,0.5); animation: floatUp linear infinite; bottom: -50px; }
        @keyframes floatUp { 0% { transform: translateY(0) rotate(0deg) scale(0); opacity: 0; } 10% { opacity: 1; } 90% { opacity: 1; } 100% { transform: translateY(-110vh) rotate(720deg) scale(1.5); opacity: 0; } }
        .stickers-container { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: -1; }
        .sticker { position: absolute; font-size: 36px; animation: dance 3s ease-in-out infinite; opacity: 0.8; text-shadow: 0 0 10px rgba(255,255,255,0.7); user-select: none; }
        @keyframes dance { 0% { transform: translateY(0) rotate(0deg) scale(1); } 25% { transform: translateY(-20px) rotate(10deg) scale(1.15); } 50% { transform: translateY(0) rotate(0deg) scale(1); } 75% { transform: translateY(-20px) rotate(-10deg) scale(1.15); } 100% { transform: translateY(0) rotate(0deg) scale(1); } }

        .gate, .main-app { background: rgba(255,255,255,0.15); backdrop-filter: blur(20px); border-radius: 30px; box-shadow: 0 25px 50px rgba(0,0,0,0.4), inset 0 0 20px rgba(255,255,255,0.2); max-width: 600px; width: 100%; padding: 30px 20px; text-align: center; border: 1px solid rgba(255,255,255,0.3); color: #fff; position: relative; z-index: 1; }
        .manager-header { position: absolute; top: -40px; left: 50%; transform: translateX(-50%); background: linear-gradient(to right, #ffd700, #ffaa00); color: #1a0b2e; padding: 8px 35px; border-radius: 50px; font-weight: 900; font-size: 1.1em; letter-spacing: 2px; box-shadow: 0 10px 25px rgba(255,215,0,0.5); white-space: nowrap; border: 2px solid #fff; display: flex; align-items: center; justify-content: center; overflow: hidden; text-shadow: 0 0 5px rgba(255,255,255,0.8); }
        .typewriter-text { display: inline-block; white-space: nowrap; overflow: hidden; animation: typing 4s steps(30, end), blink-caret 0.7s step-end infinite; border-left: 3px solid #1a0b2e; }
        @keyframes typing { from { width: 0; } to { width: 100%; } }
        @keyframes blink-caret { from, to { border-color: transparent; } 50% { border-color: #1a0b2e; } }

        .warning-card { background: rgba(0,0,0,0.25); backdrop-filter: blur(12px); border: 1px solid rgba(255,215,0,0.5); border-radius: 20px; padding: 18px 15px; margin: 10px 0 5px 0; display: flex; flex-direction: column; align-items: center; gap: 10px; animation: fadeInUp 0.9s ease-out; position: relative; overflow: hidden; box-shadow: 0 0 30px rgba(255,215,0,0.3); }
        .warning-card::before { content: ""; position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent); background-size: 200% 100%; animation: shimmer 2.5s infinite; pointer-events: none; }
        @keyframes shimmer { 0% { background-position: -200% 0; } 100% { background-position: 200% 0; } }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(25px); } to { opacity: 1; transform: translateY(0); } }
        .warning-icon { font-size: 28px; animation: pulse 2s infinite; color: #ffd700; filter: drop-shadow(0 0 10px #ffaa00); }
        @keyframes pulse { 0% { transform: scale(1); opacity: 0.9; } 50% { transform: scale(1.25); opacity: 1; } 100% { transform: scale(1); opacity: 0.9; } }
        .warning-text { font-size: 14px; line-height: 2; text-align: justify; color: #fff; text-shadow: 0 0 8px rgba(0,0,0,0.5); }
        .warning-text strong { color: #ffd700; font-weight: 900; }

        .gate h2 { color: #fff; margin-bottom: 8px; margin-top: 25px; }
        .channels { display: flex; flex-direction: column; gap: 15px; margin-bottom: 30px; }
        .channel-btn { display: flex; align-items: center; justify-content: space-between; background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.4); border-radius: 16px; padding: 15px; text-decoration: none; color: #fff; font-weight: bold; transition: 0.3s; }
        .channel-btn:hover { background: rgba(255,255,255,0.35); border-color: #ffd700; transform: scale(1.02); }
        .channel-name { font-size: 16px; }
        .join-badge { background: #ffd700; color: #1a0b2e; padding: 6px 12px; border-radius: 20px; font-size: 14px; font-weight: bold; }

        .input-group { display: flex; flex-direction: column; gap: 10px; background: rgba(255,255,255,0.1); backdrop-filter: blur(10px); border-radius: 12px; padding: 15px; margin: 10px 0; border: 1px solid rgba(255,215,0,0.3); }
        .input-group label { font-size: 14px; color: #ffd700; }
        .input-group input, .input-group textarea { width: 100%; padding: 12px; border-radius: 8px; border: none; background: rgba(255,255,255,0.2); color: #fff; font-family: inherit; font-size: 14px; text-align: center; }
        .input-row { display: flex; gap: 10px; }
        .input-row input { flex: 1; padding: 12px; border-radius: 8px; border: none; background: rgba(255,255,255,0.2); color: #fff; font-family: inherit; font-size: 16px; text-align: center; }
        .input-row button { background: #ffaa00; color: #1a0b2e; border: none; border-radius: 8px; padding: 12px 18px; font-weight: bold; cursor: pointer; }

        .code-input-group { display: flex; flex-direction: column; gap: 8px; background: rgba(255,255,255,0.1); backdrop-filter: blur(10px); border-radius: 12px; padding: 12px; margin: 15px 0; border: 1px solid rgba(255,215,0,0.3); }
        .code-input-group label { font-size: 14px; color: #ffd700; }
        #verifyCode { width: 100%; padding: 12px; border-radius: 8px; border: none; background: rgba(255,255,255,0.2); color: #fff; font-family: inherit; font-size: 16px; text-align: center; letter-spacing: 3px; }

        .confirm-btn { background: linear-gradient(to right, #ffd700, #ffaa00); color: #1a0b2e; border: none; border-radius: 16px; padding: 18px; font-size: 18px; font-weight: bold; width: 100%; cursor: pointer; transition: 0.3s; box-shadow: 0 10px 20px rgba(255,215,0,0.4); }
        .confirm-btn:hover { background: linear-gradient(to right, #ffe55c, #ffb703); transform: translateY(-3px); }
        .hidden { display: none !important; }

        .header { background: rgba(255,255,255,0.1); backdrop-filter: blur(10px); color: #ffd700; padding: 22px 18px; text-align: center; font-size: 1.7em; font-weight: 900; letter-spacing: 1px; border-radius: 20px; margin: 0 0 20px 0; text-shadow: 2px 2px 0 rgba(0,0,0,0.5); border: 1px solid rgba(255,255,255,0.2); }
        .header .sub { font-size: 0.6em; color: #eee; font-weight: normal; text-shadow: none; }
        .content { display: flex; flex-direction: column; gap: 15px; text-align: right; color: #fff; }

        .names-display { background: rgba(0,0,0,0.3); border: 1px solid rgba(255,255,255,0.3); border-radius: 14px; padding: 15px; font-size: 14px; line-height: 2.2; max-height: 200px; overflow-y: auto; text-align: right; direction: rtl; color: #ddd; word-break: break-word; }
        .file-zone { display: flex; gap: 10px; flex-wrap: wrap; align-items: center; }
        .file-label { background: rgba(255,255,255,0.2); color: white; padding: 10px 18px; border-radius: 12px; font-size: 14px; cursor: pointer; transition: 0.2s; backdrop-filter: blur(5px); border: 1px solid rgba(255,255,255,0.3); }
        .file-label:hover { background: rgba(255,255,255,0.4); }
        #fileInput, .member-file-input { display: none; }
        .names-area { width: 100%; height: 100px; border: 2px dashed rgba(255,255,255,0.5); border-radius: 14px; padding: 12px; font-family: inherit; font-size: 13px; resize: vertical; direction: ltr; text-align: left; background: rgba(0,0,0,0.3); color: #fff; }
        .datetime-box { display: flex; flex-wrap: wrap; align-items: center; gap: 8px; background: rgba(255,255,255,0.1); padding: 12px; border-radius: 12px; backdrop-filter: blur(5px); }
        .datetime-box label { font-weight: bold; font-size: 14px; }
        .datetime-box input { flex: 1; padding: 10px; border: 2px solid rgba(255,255,255,0.4); border-radius: 10px; font-family: inherit; background: rgba(0,0,0,0.5); color: #fff; }
        .countdown { background: rgba(255,215,0,0.2); color: #ffd700; padding: 12px; border-radius: 14px; text-align: center; font-size: 1.5em; font-weight: bold; backdrop-filter: blur(5px); }
        .buttons { display: flex; gap: 8px; flex-wrap: wrap; }
        .btn { flex: 1 1 auto; padding: 12px 15px; border: none; border-radius: 12px; font-size: 15px; font-weight: bold; cursor: pointer; transition: 0.2s; text-align: center; backdrop-filter: blur(5px); }
        .btn-primary { background: linear-gradient(to right, #ffd700, #ffaa00); color: #1a0b2e; }
        .btn-primary:hover { background: linear-gradient(to right, #ffe55c, #ffb703); }
        .btn-secondary { background: rgba(255,255,255,0.2); color: #fff; border: 1px solid rgba(255,255,255,0.3); }
        .btn-secondary:hover { background: rgba(255,255,255,0.4); }
        .btn-danger { background: #e74c3c; color: white; }
        .btn-danger:hover { background: #c0392b; }
        .admin-btn { background: transparent; border: 1px dashed rgba(255,255,255,0.5); color: rgba(255,255,255,0.6); font-size: 13px; padding: 8px 15px; border-radius: 20px; cursor: pointer; margin-top: 5px; transition: 0.3s; }
        .admin-btn:hover { background: rgba(255,255,255,0.2); color: #fff; }
        .winner-card { background: rgba(255,215,0,0.15); border: 2px solid #ffd700; border-radius: 20px; padding: 25px; text-align: center; font-size: 1.8em; font-weight: 900; color: #ffd700; min-height: 80px; display: flex; align-items: center; justify-content: center; transition: 0.3s; word-break: break-word; backdrop-filter: blur(10px); text-shadow: 0 0 15px #ffaa00; }
        @keyframes winPop { 0% { transform: scale(0.7); opacity: 0; } 60% { transform: scale(1.1); } 100% { transform: scale(1); opacity: 1; } }
        .winner-animate { animation: winPop 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
        .rolling-names { font-size: 1.5em; font-weight: bold; animation: rollNames 0.1s infinite; }
        @keyframes rollNames { 0% { opacity: 0.3; transform: translateY(-5px); } 50% { opacity: 1; transform: translateY(5px); } 100% { opacity: 0.3; transform: translateY(-5px); } }
        .stats-table { width: 100%; border-collapse: collapse; background: rgba(0,0,0,0.3); border-radius: 10px; overflow: hidden; font-size: 13px; }
        .stats-table th { background: rgba(255,215,0,0.3); padding: 8px; color: #fff; }
        .stats-table td { padding: 8px; border-bottom: 1px solid rgba(255,255,255,0.1); color: #ddd; }
        .info-text { font-size: 13px; color: #ffd700; margin-top: 5px; font-weight: bold; }
        .alert-box { background: rgba(255, 193, 7, 0.2); border: 1px solid #ffc107; border-radius: 12px; padding: 15px; margin-top: 10px; color: #ffc107; font-weight: bold; animation: fadeInUp 0.5s; }
        .channel-lists { background: rgba(255,255,255,0.05); border-radius: 12px; padding: 10px; margin-top: 10px; }
        .channel-lists label { color: #ffd700; font-size: 13px; display: block; margin-bottom: 3px; }
        .members-section { background: #ff9800; border: 2px solid #fff; border-radius: 16px; padding: 15px; margin: 15px 0; box-shadow: 0 0 20px #ff9800; }
        .members-section h3 { color: #fff; font-size: 1.3em; margin-bottom: 10px; text-shadow: 1px 1px 2px #000; }
    </style>
</head>
<body>
<div class="stickers-container" id="stickersContainer"></div>
<div class="particles" id="particlesContainer"></div>

<div id="gatePage" class="gate">
    <div class="manager-header"><span class="typewriter-text">✨ با مدیریت خانم قیصری ✨</span></div>
    <h2>🔐 ورود به قرعه‌کشی</h2>
    <div class="warning-card"><div class="warning-icon">⚠️</div><div class="warning-text"><strong>توجه:</strong> شرکت در این قرعه‌کشی <strong>منوط به عضویت در هر سه کانال</strong> می‌باشد. کد ورود <strong>فقط در کانال‌های زیر منتشر می‌شود</strong>. پس از عضویت، کد را دریافت کرده و در کادر پایین وارد کنید.</div></div>
    <div class="channels">
        <a href="https://eitaa.com/Lavazemtahreirgoldasht" target="_blank" class="channel-btn"><span class="channel-name">📚 نوشت‌افزار گلدشت</span><span class="join-badge">عضویت</span></a>
        <a href="https://eitaa.com/hambaziiii" target="_blank" class="channel-btn"><span class="channel-name">🧸 اسباب‌بازی گلدشت</span><span class="join-badge">عضویت</span></a>
        <a href="https://eitaa.com/Gallerymahak402" target="_blank" class="channel-btn"><span class="channel-name">🖼 گالری ماهک</span><span class="join-badge">عضویت</span></a>
    </div>
    <div class="input-group"><label>👤 نام و نام خانوادگی (اختیاری):</label><input type="text" id="fullName" placeholder="مثال: علی اکبری"></div>
    <div class="input-group"><label>📱 شماره موبایل:</label><div class="input-row"><input type="tel" id="phoneNumber" placeholder="مثال: ۰۹۱۲۳۴۵۶۷۸۹"><button onclick="showCodeMessage()">دریافت کد</button></div><div id="channelCodeMessage"></div></div>
    <div class="code-input-group"><label>🔑 کد ورود (از کانال‌ها دریافت کنید):</label><input type="text" id="verifyCode" placeholder="کد عضویت"></div>
    <p class="info-text">📌 اطلاعات شما تنها برای احراز هویت و آمار مدیریت ذخیره می‌شود.</p>
    <button class="confirm-btn" onclick="enterApp()">✅ ورود به قرعه‌کشی</button>
</div>

<div id="mainApp" class="main-app hidden">
    <div class="manager-header"><span class="typewriter-text">✨ با مدیریت خانم قیصری ✨</span></div>
    <div class="header">🎯 قرعه‌کشیه<span class="sub">نوشت‌افزار گلدشت | اسباب‌بازی گلدشت | گالری ماهک</span></div>
    <div class="content">
        <div id="publicView">
            <div class="names-display" id="publicNamesList">هنوز شماره‌ای وارد نشده است.</div>
            <div class="countdown" id="countdownDisplay">⏳ هنوز تنظیم نشده</div>
            <div class="winner-card" id="winnerDisplay">🎁 برنده اینجا نمایش داده می‌شود</div>
            <button class="admin-btn" onclick="promptAdminPassword()">🔑 ورود مدیر</button>
        </div>
        <div id="adminView" class="hidden">
            <div style="display:flex; gap:10px; align-items:center; margin-bottom:5px;"><label style="font-size:14px;">🎟 حالت امتیازی (شماره - تعداد):</label><input type="checkbox" id="weightedMode" onchange="toggleWeightedMode()"></div>
            <div class="file-zone"><label for="fileInput" class="file-label">📁 آپلود فایل شماره‌ها (txt)</label><input type="file" id="fileInput" accept=".txt, .csv"><button class="btn btn-secondary" onclick="clearNames()">🗑 پاک کردن لیست</button></div>
            <textarea id="namesList" class="names-area" placeholder="هر خط یک شماره (در حالت امتیازی: شماره - تعداد)"></textarea>
            <div class="datetime-box"><label>⏰ زمان قرعه‌کشی خودکار:</label><input type="datetime-local" id="drawTime"><button class="btn btn-primary" onclick="saveSettings()">💾 ذخیره زمان</button></div>
            <div style="display:flex; gap:10px; align-items:center; background:rgba(255,255,255,0.1); padding:10px; border-radius:10px;"><label style="font-size:14px;">🔐 کد عضویت (در کانال‌ها اعلام شود):</label><input type="text" id="memberCodeInput" style="flex:1; padding:8px; background:rgba(0,0,0,0.5); color:#fff; border:1px solid #ffd700; border-radius:8px;"><button class="btn btn-primary" onclick="updateMemberCode()" style="flex:0;">ذخیره کد</button></div>
            <p style="color:#ffd700; font-size:12px; margin-top:5px;">📌 کد پیش‌فرض GOLDASHT است. برای تغییر برای همه، فایل را دوباره آپلود کنید.</p>
            <div style="background:rgba(255,255,255,0.1); border-radius:12px; padding:15px;">
                <div style="display:flex; align-items:center; gap:10px; margin-bottom:10px;"><label style="color:#ffd700;">✅ بررسی خودکار عضویت در کانال‌ها:</label><input type="checkbox" id="autoVerifyCheck" onchange="toggleAutoVerify()"></div>
                <div style="display:flex; align-items:center; gap:10px; margin-bottom:10px;"><label style="color:#ffd700;">⚡ تأیید خودکار برنده (در صورت عضویت در سه کانال):</label><input type="checkbox" id="autoApproveCheck" onchange="toggleAutoApprove()"></div>
            </div>

            <div class="members-section">
                <h3>📋 اعضای کانال‌ها</h3>
                <div style="background:rgba(0,0,0,0.2); border-radius:8px; padding:8px; margin-top:5px;"><label style="color:#fff; font-weight:bold;">📚 نوشت‌افزار گلدشت</label><textarea id="ch1Members" class="names-area" style="background:#fff; color:#000;" placeholder="شماره‌ها..."></textarea></div>
                <div style="background:rgba(0,0,0,0.2); border-radius:8px; padding:8px; margin-top:5px;"><label style="color:#fff; font-weight:bold;">🧸 اسباب‌بازی گلدشت</label><textarea id="ch2Members" class="names-area" style="background:#fff; color:#000;" placeholder="شماره‌ها..."></textarea></div>
                <div style="background:rgba(0,0,0,0.2); border-radius:8px; padding:8px; margin-top:5px;"><label style="color:#fff; font-weight:bold;">🖼 گالری ماهک</label><textarea id="ch3Members" class="names-area" style="background:#fff; color:#000;" placeholder="شماره‌ها..."></textarea></div>
            </div>

            <div id="approvalBox" class="alert-box hidden">⚠️ برنده انتخاب شد: <span id="pendingWinnerNumber"></span><br><span id="membershipStatus"></span><div class="buttons" style="margin-top:10px;"><button class="btn btn-primary" onclick="approveWinner()">✅ تأیید نهایی</button><button class="btn btn-danger" onclick="rejectWinner()">❌ رد و انتخاب دوباره</button></div></div>
            <div style="background:rgba(255,255,255,0.1); border-radius:12px; padding:15px; margin-top:10px;"><h3 style="color:#ffd700; margin-bottom:10px;">📊 آمار مراجعه‌کنندگان</h3><div id="userStats" style="max-height:300px; overflow-y:auto;"><p style="color:#aaa;">هنوز کسی وارد نشده است.</p></div><div style="margin-top:10px; font-size:14px; color:#ffd700;" id="totalUsers"></div></div>
            <div class="buttons"><button class="btn btn-primary" onclick="manualDraw()">🎲 قرعه‌کشی دستی</button><button class="btn btn-secondary" onclick="resetAll()">🔄 بازنشانی کامل</button></div>
            <button class="admin-btn" onclick="exitAdmin()">🚪 خروج از مدیریت</button>
        </div>
    </div>
</div>

<script>
    const DEFAULT_MEMBER_CODE = "GOLDASHT";
    const ADMIN_PASSWORD = "ali.akbar.87.z";
    const MEMBER_CODE_KEY = 'member_code', STORAGE_KEY = 'ghorekeshie_golgasht', USERS_KEY = 'gate_visitors', WINNERS_HISTORY_KEY = 'confirmed_winners', CH1_KEY = 'ch1_members', CH2_KEY = 'ch2_members', CH3_KEY = 'ch3_members', AUTO_VERIFY_KEY = 'auto_verify', AUTO_APPROVE_KEY = 'auto_approve';
    function getMemberCode(){return localStorage.getItem(MEMBER_CODE_KEY)||DEFAULT_MEMBER_CODE}
    function setMemberCode(code){localStorage.setItem(MEMBER_CODE_KEY,code)}
    function createParticles(){const c=document.getElementById('particlesContainer');for(let i=0;i<40;i++){const p=document.createElement('div');p.className='particle';const s=Math.random()*8+4;p.style.width=s+'px';p.style.height=s+'px';p.style.left=Math.random()*100+'%';p.style.animationDuration=(Math.random()*10+8)+'s';p.style.animationDelay=Math.random()*10+'s';p.style.backgroundColor=`rgba(255,255,255,${Math.random()*0.6+0.2})`;c.appendChild(p)}}
    function createStickers(){const emojis=['✏️','📎','📚','🖍️','🎨','📐','✂️','🖊️','🧸','🎮','🪀','🎲','🧩','🪁','🎯','🎪','💍','👑','👜','👓','🎀','💎','⌚','🌟'];const c=document.getElementById('stickersContainer');for(let i=0;i<25;i++){const s=document.createElement('div');s.className='sticker';s.textContent=emojis[Math.floor(Math.random()*emojis.length)];s.style.left=Math.random()*100+'%';s.style.top=Math.random()*100+'%';s.style.fontSize=(Math.random()*20+25)+'px';s.style.animationDuration=(Math.random()*3+2.5)+'s';s.style.animationDelay=Math.random()*5+'s';s.style.opacity=Math.random()*0.4+0.5;c.appendChild(s)}}
    createParticles();createStickers();
    function getChannelSource(){const params=new URLSearchParams(window.location.search);const ch=params.get('ch');if(ch==='1')return 1;if(ch==='2')return 2;if(ch==='3')return 3;return null}
    function getVisitors(){return JSON.parse(localStorage.getItem(USERS_KEY)||'[]')}
    function addVisitor(name,phone,channelSource=null){const visitors=getVisitors();if(!visitors.find(v=>v.phone===phone)){visitors.push({name:name||'ناشناس',phone,time:new Date().toLocaleString('fa-IR'),source:channelSource});localStorage.setItem(USERS_KEY,JSON.stringify(visitors))}}
    function updateVisitorStats(){const visitors=getVisitors();document.getElementById('totalUsers').textContent=`👥 تعداد کل مراجعه‌کنندگان: ${visitors.length} نفر`;const container=document.getElementById('userStats');if(visitors.length===0){container.innerHTML='<p style="color:#aaa;">هنوز کسی وارد نشده است.</p>';return}let html=`<table class="stats-table"><thead><tr><th>#</th><th>نام</th><th>شماره</th><th>زمان</th><th>کانال</th></tr></thead><tbody>`;visitors.forEach((v,idx)=>{const chName=v.source===1?'نوشت‌افزار':v.source===2?'اسباب‌بازی':v.source===3?'گالری ماهک':'نامشخص';html+=`<tr><td>${idx+1}</td><td>${v.name}</td><td>${v.phone}</td><td>${v.time}</td><td>${chName}</td></tr>`});html+='</tbody></table>';container.innerHTML=html}
    function showCodeMessage(){const phone=document.getElementById('phoneNumber').value.trim();if(phone.length<10){alert('لطفاً یک شماره موبایل معتبر وارد کنید.');return}document.getElementById('channelCodeMessage').innerHTML='📢 کد ورود <strong>فقط در کانال‌های ما</strong> منتشر شده است.<br>لطفاً عضو شوید و کد را از پست سنجاق‌شده بردارید.'}
    function addMemberToChannel(ch,phone){const members=getChannelMembers(ch);if(!members.includes(phone)){members.push(phone);setChannelMembers(ch,members);return true}return false}
    function enterApp(){const fullName=document.getElementById('fullName').value.trim();const phone=document.getElementById('phoneNumber').value.trim();const code=document.getElementById('verifyCode').value.trim();const source=getChannelSource();if(!source){alert('⛔ لطفاً از لینک مخصوص کانال خود استفاده کنید (لینکی که توسط ادمین در کانال قرار داده شده است).');return}if(phone.length<10){alert('❌ لطفاً شماره موبایل معتبر وارد کنید.');return}if(code!==getMemberCode()){alert('❌ کد وارد شده اشتباه است. لطفاً در کانال‌ها عضو شوید و کد صحیح را دریافت کنید.');return}const added=addMemberToChannel(source,phone);if(!added){alert('⚠️ این شماره موبایل قبلاً در همین کانال ثبت شده است.');return}addVisitor(fullName,phone,source);document.getElementById('gatePage').classList.add('hidden');document.getElementById('mainApp').classList.remove('hidden');loadAllData()}
    function getSettings(){return JSON.parse(localStorage.getItem(STORAGE_KEY)||'{"numbers":"","drawTime":"","winner":"","weighted":false,"pendingWinner":""}')}
    function setSettings(obj){localStorage.setItem(STORAGE_KEY,JSON.stringify(obj))}
    function getChannelMembers(ch){const key=ch===1?CH1_KEY:(ch===2?CH2_KEY:CH3_KEY);return(localStorage.getItem(key)||'').split(/[\r\n]+/).map(n=>n.trim()).filter(n=>n)}
    function setChannelMembers(ch,numbers){const key=ch===1?CH1_KEY:(ch===2?CH2_KEY:CH3_KEY);localStorage.setItem(key,Array.from(new Set(numbers)).join('\n'))}
    function isAutoVerifyEnabled(){return localStorage.getItem(AUTO_VERIFY_KEY)==='true'}
    function isAutoApproveEnabled(){return localStorage.getItem(AUTO_APPROVE_KEY)==='true'}
    function checkAllThreeChannels(number){return getChannelMembers(1).includes(number)&&getChannelMembers(2).includes(number)&&getChannelMembers(3).includes(number)}
    const namesEl=document.getElementById('namesList');const drawTimeEl=document.getElementById('drawTime');const countdownEl=document.getElementById('countdownDisplay');const winnerEl=document.getElementById('winnerDisplay');const publicNamesEl=document.getElementById('publicNamesList');const fileInput=document.getElementById('fileInput');const weightedCheck=document.getElementById('weightedMode');const memberCodeInput=document.getElementById('memberCodeInput');const ch1El=document.getElementById('ch1Members');const ch2El=document.getElementById('ch2Members');const ch3El=document.getElementById('ch3Members');const autoVerifyCheck=document.getElementById('autoVerifyCheck');const autoApproveCheck=document.getElementById('autoApproveCheck');const approvalBox=document.getElementById('approvalBox');const pendingWinnerSpan=document.getElementById('pendingWinnerNumber');const membershipStatus=document.getElementById('membershipStatus');let autoTimer=null;
    function toggleWeightedMode(){const s=getSettings();s.weighted=weightedCheck.checked;setSettings(s)}
    function toggleAutoVerify(){localStorage.setItem(AUTO_VERIFY_KEY,autoVerifyCheck.checked)}
    function toggleAutoApprove(){localStorage.setItem(AUTO_APPROVE_KEY,autoApproveCheck.checked)}
    function parseNumbersForDraw(){const raw=namesEl.value.split(/[\r\n]+/).map(l=>l.trim()).filter(l=>l);const weighted=weightedCheck.checked;let entries=[];raw.forEach(line=>{let num=line,count=1;if(weighted&&line.includes('-')){const parts=line.split('-').map(p=>p.trim());num=parts[0];count=parseInt(parts[1])||1}for(let i=0;i<count;i++)entries.push(num)});return entries}
    function updatePublicNamesDisplay(){const numbers=namesEl.value.split(/[\r\n]+/).filter(l=>l.trim());publicNamesEl.textContent=numbers.length?numbers.join('، '):'هنوز شماره‌ای وارد نشده است.'}
    function loadAllData(){const s=getSettings();namesEl.value=s.numbers||'';drawTimeEl.value=s.drawTime||'';weightedCheck.checked=s.weighted||false;memberCodeInput.value=getMemberCode();ch1El.value=getChannelMembers(1).join('\n');ch2El.value=getChannelMembers(2).join('\n');ch3El.value=getChannelMembers(3).join('\n');autoVerifyCheck.checked=isAutoVerifyEnabled();autoApproveCheck.checked=isAutoApproveEnabled();if(s.winner)winnerEl.textContent='🎉 '+s.winner+' 🎉';else winnerEl.textContent='🎁 برنده اینجا نمایش داده می‌شود';updatePublicNamesDisplay();updateCountdown();updateVisitorStats();if(s.pendingWinner)showApprovalBox(s.pendingWinner);else approvalBox.classList.add('hidden')}
    function saveAllChannelData(){setChannelMembers(1,ch1El.value.split(/[\r\n]+/).filter(n=>n.trim()));setChannelMembers(2,ch2El.value.split(/[\r\n]+/).filter(n=>n.trim()));setChannelMembers(3,ch3El.value.split(/[\r\n]+/).filter(n=>n.trim()))}
    function saveNamesToStorage(){const s=getSettings();s.numbers=namesEl.value;s.weighted=weightedCheck.checked;setSettings(s);updatePublicNamesDisplay();saveAllChannelData()}
    function saveSettings(){saveNamesToStorage();const s=getSettings();s.drawTime=drawTimeEl.value;setSettings(s);updateCountdown();alert('✅ زمان قرعه‌کشی ذخیره شد.')}
    fileInput.addEventListener('change',function(e){const file=e.target.files[0];if(!file)return;const reader=new FileReader();reader.onload=function(ev){const lines=ev.target.result.split(/[\r\n]+/).map(l=>l.trim()).filter(l=>l);const cur=namesEl.value.trim();const curList=cur?cur.split(/[\r\n]+/).filter(l=>l.trim()):[];namesEl.value=[...new Set([...curList,...lines])].join('\n');saveNamesToStorage()};reader.readAsText(file,'UTF-8')});
    namesEl.addEventListener('input',saveNamesToStorage);ch1El.addEventListener('input',saveNamesToStorage);ch2El.addEventListener('input',saveNamesToStorage);ch3El.addEventListener('input',saveNamesToStorage);weightedCheck.addEventListener('change',saveNamesToStorage);
    function clearNames(){if(confirm('همه شماره‌های قرعه‌کشی پاک شوند؟')){namesEl.value='';saveNamesToStorage()}}
    const ones=['','یک','دو','سه','چهار','پنج','شش','هفت','هشت','نه'];const tens=['','','بیست','سی','چهل','پنجاه','شصت','هفتاد','هشتاد','نود'];const teens=['ده','یازده','دوازده','سیزده','چهارده','پانزده','شانزده','هفده','هجده','نوزده'];const hundreds=['','صد','دویست','سیصد','چهارصد','پانصد','ششصد','هفتصد','هشتصد','نهصد'];
    function numberToWords(num){if(num===0)return'صفر';let result='';let n=parseInt(num);if(n>=1000){const thousands=Math.floor(n/1000);if(thousands===1)result+='هزار';else result+=ones[thousands]+' هزار';n%=1000;if(n>0)result+=' و '}if(n>=100){result+=hundreds[Math.floor(n/100)];n%=100;if(n>0)result+=' و '}if(n>=10&&n<20){result+=teens[n-10];return result.trim()}if(n>=10){result+=tens[Math.floor(n/10)];n%=10;if(n>0)result+=' و '}if(n>0)result+=ones[n];return result.trim().replace(/\s+و\s*$/,'')}
    function speakPhoneNumber(phoneStr){const digits=phoneStr.replace(/\D/g,'');if(digits.length!==11)return;const firstPart=digits.substring(0,4);let firstWords='';if(firstPart.startsWith('0')){firstWords='صفر، ';firstWords+=numberToWords(parseInt(firstPart.substring(1,4)))}else firstWords=numberToWords(parseInt(firstPart));const lastWords=numberToWords(parseInt(digits.substring(7,11)));const fullPhrase=firstWords+' ... '+lastWords;const utterance=new SpeechSynthesisUtterance(fullPhrase);utterance.lang='fa-IR';utterance.rate=0.8;utterance.pitch=1.0;const voices=window.speechSynthesis.getVoices();const persianVoice=voices.find(v=>v.lang==='fa-IR'||v.lang==='fa');if(persianVoice)utterance.voice=persianVoice;window.speechSynthesis.speak(utterance)}
    function playCelebrationSound(){try{const audioCtx=new(window.AudioContext||window.webkitAudioContext)();const notes=[523.25,659.25,783.99,1046.50];notes.forEach((freq,i)=>{const osc=audioCtx.createOscillator();const gain=audioCtx.createGain();osc.type='square';osc.frequency.value=freq;gain.gain.setValueAtTime(0.3,audioCtx.currentTime+i*0.2);gain.gain.exponentialRampToValueAtTime(0.001,audioCtx.currentTime+i*0.2+0.4);osc.connect(gain);gain.connect(audioCtx.destination);osc.start(audioCtx.currentTime+i*0.2);osc.stop(audioCtx.currentTime+i*0.2+0.4)})}catch(e){}}
    function showApprovalBox(number){pendingWinnerSpan.textContent=number;if(isAutoVerifyEnabled()){if(checkAllThreeChannels(number))membershipStatus.textContent='✅ این شماره در هر سه کانال عضویت دارد.';else membershipStatus.textContent='❌ این شماره در یکی از کانال‌ها (یا بیشتر) عضویت ندارد.'}else membershipStatus.textContent='';approvalBox.classList.remove('hidden')}
    function approveWinner(){const s=getSettings();const winner=s.pendingWinner;if(!winner)return;const history=JSON.parse(localStorage.getItem(WINNERS_HISTORY_KEY)||'[]');history.push({number:winner,time:new Date().toLocaleString('fa-IR')});localStorage.setItem(WINNERS_HISTORY_KEY,JSON.stringify(history));s.winner=winner;s.pendingWinner='';setSettings(s);winnerEl.textContent='🎉 '+winner+' 🎉';approvalBox.classList.add('hidden')}
    function rejectWinner(){const s=getSettings();s.pendingWinner='';setSettings(s);winnerEl.textContent='🎁 برنده اینجا نمایش داده می‌شود';approvalBox.classList.add('hidden');drawWinner(false)}
    function drawWinner(skipApproval=false){const entries=parseNumbersForDraw();if(entries.length===0){winnerEl.textContent='⚠️ لیست خالی است!';return}winnerEl.textContent='🎰 در حال قرعه‌کشی...';winnerEl.classList.add('rolling-names');let counter=0;const interval=setInterval(()=>{const rand=entries[Math.floor(Math.random()*entries.length)];winnerEl.textContent=rand;counter++;if(counter>=15){clearInterval(interval);let winner=entries[Math.floor(Math.random()*entries.length)];const s=getSettings();if(isAutoVerifyEnabled()&&isAutoApproveEnabled()){let attempts=0;while(!checkAllThreeChannels(winner)&&attempts<50){winner=entries[Math.floor(Math.random()*entries.length)];attempts++}if(!checkAllThreeChannels(winner)){winnerEl.textContent='⚠️ هیچ شماره‌ای که در هر سه کانال باشد یافت نشد!';winnerEl.classList.remove('rolling-names');return}const history=JSON.parse(localStorage.getItem(WINNERS_HISTORY_KEY)||'[]');history.push({number:winner,time:new Date().toLocaleString('fa-IR')});localStorage.setItem(WINNERS_HISTORY_KEY,JSON.stringify(history));s.winner=winner;s.pendingWinner='';setSettings(s);winnerEl.textContent='🎉 '+winner+' 🎉';winnerEl.classList.remove('rolling-names');winnerEl.classList.add('winner-animate');setTimeout(()=>winnerEl.classList.remove('winner-animate'),700);playCelebrationSound();speakPhoneNumber(winner);return}if(isAutoVerifyEnabled()&&!isAutoApproveEnabled()){let attempts=0;while(!checkAllThreeChannels(winner)&&attempts<50){winner=entries[Math.floor(Math.random()*entries.length)];attempts++}if(!checkAllThreeChannels(winner)){winnerEl.textContent='⚠️ هیچ شماره‌ای که در هر سه کانال باشد یافت نشد!';winnerEl.classList.remove('rolling-names');return}}winnerEl.textContent='🎉 '+winner+' 🎉';winnerEl.classList.remove('rolling-names');winnerEl.classList.add('winner-animate');setTimeout(()=>winnerEl.classList.remove('winner-animate'),700);s.pendingWinner=winner;s.winner='';setSettings(s);showApprovalBox(winner);playCelebrationSound();speakPhoneNumber(winner)}},100)}
    function manualDraw(){drawWinner(false)}
    function updateCountdown(){if(autoTimer)clearInterval(autoTimer);const dt=drawTimeEl.value;if(!dt){countdownEl.textContent='⏳ زمان تنظیم نشده';return}const drawDate=new Date(dt);function tick(){const diff=drawDate-new Date();if(diff<=0){countdownEl.textContent='🎯 زمان قرعه‌کشی فرا رسید!';const s=getSettings();if(!s.winner&&!s.pendingWinner)drawWinner(false);clearInterval(autoTimer);autoTimer=null;return}const ts=Math.floor(diff/1000);const d=Math.floor(ts/86400),h=Math.floor((ts%86400)/3600),m=Math.floor((ts%3600)/60),sec=ts%60;let txt='⏳ ';if(d>0)txt+=d+' روز ';txt+=`${h.toString().padStart(2,'0')}:${m.toString().padStart(2,'0')}:${sec.toString().padStart(2,'0')} مانده`;countdownEl.textContent=txt}tick();autoTimer=setInterval(tick,1000)}
    drawTimeEl.addEventListener('change',saveSettings);
    function resetAll(){if(confirm('همه تنظیمات، شماره‌ها، اعضای کانال‌ها و مراجعه‌کنندگان پاک شوند؟')){namesEl.value='';drawTimeEl.value='';ch1El.value='';ch2El.value='';ch3El.value='';setSettings({numbers:'',drawTime:'',winner:'',weighted:false,pendingWinner:''});localStorage.removeItem(USERS_KEY);localStorage.removeItem(WINNERS_HISTORY_KEY);localStorage.removeItem(CH1_KEY);localStorage.removeItem(CH2_KEY);localStorage.removeItem(CH3_KEY);localStorage.removeItem(AUTO_VERIFY_KEY);localStorage.removeItem(AUTO_APPROVE_KEY);winnerEl.textContent='🎁 برنده اینجا نمایش داده می‌شود';updatePublicNamesDisplay();updateCountdown();updateVisitorStats();weightedCheck.checked=false;autoVerifyCheck.checked=false;autoApproveCheck.checked=false;approvalBox.classList.add('hidden')}}
    function updateMemberCode(){const newCode=memberCodeInput.value.trim();if(!newCode){alert('کد نمی‌تواند خالی باشد.');return}setMemberCode(newCode);alert('✅ کد جدید ذخیره شد. این کد فقط برای مرورگر شما اعمال می‌شود.\nبرای تغییر کد برای همه کاربران، فایل HTML را با کد جدید دوباره روی GitHub Pages آپلود کنید.')}
    function promptAdminPassword(){const pw=prompt('لطفاً رمز مدیریت را وارد کنید:');if(pw===ADMIN_PASSWORD){document.getElementById('publicView').classList.add('hidden');document.getElementById('adminView').classList.remove('hidden');loadAllData()}else if(pw!==null)alert('❌ رمز اشتباه است!')}
    function exitAdmin(){document.getElementById('adminView').classList.add('hidden');document.getElementById('publicView').classList.remove('hidden');saveNamesToStorage();loadAllData()}
    window.addEventListener('load',()=>{document.getElementById('fullName').value='';document.getElementById('phoneNumber').value='';document.getElementById('channelCodeMessage').innerHTML='';document.getElementById('verifyCode').value=''});
</script>
</body>
</html>
