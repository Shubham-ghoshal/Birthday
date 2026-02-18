<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
<title>🎂 Happy Birthday Jeevitha!</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Quicksand:wght@400;600;700&display=swap');
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body{width:100%;height:100%;overflow:hidden;background:#0d0520;font-family:'Quicksand',sans-serif;}
body{display:flex;flex-direction:column;align-items:center;justify-content:center;position:relative;}

/* 🔐 PASSWORD LOCK (ADDED) */
.lock-screen{
  position:fixed;
  inset:0;
  background:rgba(0,0,0,0.88);
  display:flex;
  align-items:center;
  justify-content:center;
  z-index:99999;
}
.lock-box{
  background:rgba(255,255,255,0.08);
  backdrop-filter:blur(12px);
  padding:28px;
  border-radius:18px;
  text-align:center;
  color:white;
}
.lock-box input{
  padding:12px 16px;
  border:none;
  border-radius:10px;
  margin-top:12px;
  font-size:15px;
  outline:none;
}
.lock-box button{
  margin-top:12px;
  padding:12px 22px;
  border:none;
  border-radius:10px;
  background:#ff6eb4;
  color:white;
  font-weight:700;
  cursor:pointer;
}
.hint{opacity:.7;font-size:12px;margin-top:6px;}

/* ── STARFIELD ── */
.starfield{position:fixed;inset:0;pointer-events:none;z-index:0;}
.star-dot{position:absolute;border-radius:50%;background:white;animation:starTwinkle ease-in-out infinite;}
@keyframes starTwinkle{0%,100%{opacity:0.12;transform:scale(1)}50%{opacity:0.9;transform:scale(1.7)}}

/* ── AURORA ── */
.aurora{
  position:fixed;inset:0;pointer-events:none;z-index:0;
  background:radial-gradient(ellipse 80% 40% at 20% 60%,rgba(255,60,180,0.18) 0%,transparent 70%),
             radial-gradient(ellipse 60% 50% at 80% 30%,rgba(80,60,255,0.18) 0%,transparent 70%),
             radial-gradient(ellipse 70% 60% at 50% 90%,rgba(255,180,0,0.1) 0%,transparent 70%);
  animation:auroraPulse 6s ease-in-out infinite;
}
@keyframes auroraPulse{0%,100%{opacity:0.7}50%{opacity:1}}

/* ── GARLAND ── */
.garland{position:fixed;top:0;left:0;width:100%;pointer-events:none;z-index:2;}
.garland svg{width:100%;height:52px;}

/* ── HB FLOAT ── */
.hb-float{
  position:fixed;pointer-events:none;z-index:1;
  font-family:'Pacifico',cursive;opacity:0;
  animation:hbDrift linear infinite;white-space:nowrap;
  -webkit-text-stroke:1px rgba(255,255,255,0.3);
}
@keyframes hbDrift{
  0%  {transform:translateY(0) rotate(var(--r)) scale(0.85);opacity:0;}
  8%  {opacity:var(--op);}
  88% {opacity:var(--op);}
  100%{transform:translateY(-75vh) rotate(calc(var(--r)+8deg)) scale(1.1);opacity:0;}
}

/* ════════════════════════════════
   SCREEN 1: AI CHATBOT
════════════════════════════════ */
#chatScreen{
  position:relative;z-index:10;
  width:100%;max-width:480px;
  display:flex;flex-direction:column;
  height:100dvh;height:100vh;
  padding:0;
}

/* AI Header */
.wa-header{
  background:linear-gradient(135deg,#1a0a2e,#2d1060);
  padding:12px 16px;
  padding-top:calc(12px + env(safe-area-inset-top));
  display:flex;align-items:center;gap:12px;
  box-shadow:0 2px 20px rgba(138,108,255,0.3);
  border-bottom:1px solid rgba(138,108,255,0.25);
  flex-shrink:0;
}
.wa-dp{
  width:44px;height:44px;border-radius:14px;
  background:linear-gradient(135deg,#ff6eb4,#8a6cff);
  display:flex;align-items:center;justify-content:center;
  flex-shrink:0;font-size:1.4rem;
  box-shadow:0 0 0 2px rgba(138,108,255,0.5),0 0 16px rgba(138,108,255,0.4);
  overflow:hidden;
}
.wa-dp img{display:none;}
.wa-dp::after{content:'🤖';}
.wa-name{color:white;font-weight:700;font-size:1rem;line-height:1.2;letter-spacing:0.2px;}
.wa-status{color:rgba(138,108,255,0.9);font-size:0.72rem;margin-top:1px;}
.wa-badge{
  margin-left:auto;background:rgba(138,108,255,0.2);
  border:1px solid rgba(138,108,255,0.4);
  border-radius:20px;padding:4px 10px;
  color:rgba(255,255,255,0.7);font-size:0.7rem;letter-spacing:0.5px;
}

/* Chat body */
.wa-body{
  flex:1;overflow-y:auto;overflow-x:hidden;
  padding:16px 14px 12px;
  display:flex;flex-direction:column;gap:12px;
  scroll-behavior:smooth;
  background:#0d0a1a;
  background-image:
    radial-gradient(circle at 15% 25%,rgba(138,108,255,0.06) 0%,transparent 50%),
    radial-gradient(circle at 85% 75%,rgba(255,110,180,0.05) 0%,transparent 50%);
  -webkit-overflow-scrolling:touch;
}
.wa-body::-webkit-scrollbar{width:3px;}
.wa-body::-webkit-scrollbar-thumb{background:rgba(255,255,255,0.1);border-radius:4px;}

/* Typing cursor */
.typing-cursor{
  display:inline-block;color:#b97bff;font-weight:300;
  animation:cursorBlink 0.7s ease-in-out infinite;margin-left:1px;
}
@keyframes cursorBlink{0%,100%{opacity:1}50%{opacity:0}}

/* Updated AI message color */
.msg-in{
  background:linear-gradient(135deg,rgba(30,15,60,0.95),rgba(20,10,45,0.9));
  color:#e0d8ff;border-radius:4px 18px 18px 18px;
  align-self:flex-start;
  border:1px solid rgba(138,108,255,0.3);
  box-shadow:0 2px 16px rgba(138,108,255,0.12);
}
.msg-out{
  background:linear-gradient(135deg,rgba(200,80,160,0.22),rgba(140,90,220,0.18));
  color:#ffe8f8;border-radius:18px 4px 18px 18px;
  align-self:flex-end;
  border:1px solid rgba(255,110,200,0.28);
  box-shadow:0 2px 14px rgba(255,110,180,0.12);
}
.msg-sender{font-size:0.68rem;font-weight:700;color:#c084fc;margin-bottom:3px;letter-spacing:0.4px;}
/* Date chip update */
.date-chip{
  align-self:center;background:rgba(138,108,255,0.1);
  color:rgba(200,180,255,0.55);font-size:0.7rem;
  padding:4px 14px;border-radius:12px;margin:4px 0;
  border:1px solid rgba(138,108,255,0.15);
  backdrop-filter:blur(6px);
}

/* Messages */
.msg{
  max-width:82%;padding:11px 14px 6px;border-radius:18px;
  font-size:0.9rem;line-height:1.6;position:relative;
  animation:msgPop 0.35s cubic-bezier(0.34,1.56,0.64,1) forwards;
  opacity:0;word-break:break-word;
}
@keyframes msgPop{0%{opacity:0;transform:scale(0.82) translateY(10px)}100%{opacity:1;transform:scale(1) translateY(0)}}
.msg-time{font-size:0.65rem;opacity:0.45;text-align:right;margin-top:4px;}
.msg-big{font-size:1.7rem;line-height:1.3;}

/* Typing */
.typing-wrap{align-self:flex-start;}
.typing-bubble{
  background:linear-gradient(135deg,rgba(138,108,255,0.15),rgba(80,60,180,0.1));
  border-radius:4px 18px 18px 18px;border:1px solid rgba(138,108,255,0.25);
  padding:12px 16px;display:inline-flex;gap:5px;align-items:center;
}
.typing-dot{width:6px;height:6px;background:#b97bff;border-radius:50%;animation:typingBounce 1.1s ease-in-out infinite;}
.typing-dot:nth-child(2){animation-delay:0.18s;}
.typing-dot:nth-child(3){animation-delay:0.36s;}
@keyframes typingBounce{0%,60%,100%{transform:translateY(0)}30%{transform:translateY(-6px)}}

/* Input bar */
.wa-input{
  background:linear-gradient(135deg,#130828,#0f0520);
  padding:10px 14px;
  padding-bottom:calc(10px + env(safe-area-inset-bottom));
  display:flex;gap:10px;align-items:center;
  border-top:1px solid rgba(138,108,255,0.15);
  flex-shrink:0;
}
.wa-input input{
  flex:1;background:rgba(138,108,255,0.08);border:1px solid rgba(138,108,255,0.2);
  border-radius:14px;padding:11px 16px;color:white;font-size:0.88rem;font-family:inherit;
  outline:none;-webkit-appearance:none;
}
.wa-input input:focus{border-color:rgba(185,123,255,0.5);background:rgba(138,108,255,0.12);}
.wa-input input::placeholder{color:rgba(255,255,255,0.25);}
.wa-send{
  width:44px;height:44px;background:linear-gradient(135deg,#b97bff,#8a6cff);
  border:none;border-radius:12px;color:white;font-size:1rem;cursor:pointer;
  display:flex;align-items:center;justify-content:center;
  box-shadow:0 3px 14px rgba(138,108,255,0.45);
  transition:transform 0.15s;flex-shrink:0;
}
.wa-send:active{transform:scale(0.9);}

/* Surprise button */
.surprise-btn{
  background:linear-gradient(135deg,#ff6eb4,#ff8c69,#ffe066);
  border:none;border-radius:22px;color:white;
  font-family:'Pacifico',cursive;font-size:1rem;
  padding:12px 24px;cursor:pointer;
  box-shadow:0 4px 18px rgba(255,110,180,0.5);
  animation:surprisePulse 1.2s ease-in-out infinite;
  align-self:center;margin:6px 0;
  letter-spacing:0.5px;
}
@keyframes surprisePulse{
  0%,100%{transform:scale(1);box-shadow:0 4px 18px rgba(255,110,180,0.5);}
  50%{transform:scale(1.05);box-shadow:0 6px 28px rgba(255,110,180,0.8);}
}
.surprise-btn:active{transform:scale(0.95)!important;}

/* ════════════════════════════════
   SCREEN 2: DOG + SONG
════════════════════════════════ */
#songScreen{
  display:none;position:relative;z-index:10;
  width:100%;max-width:480px;
  flex-direction:column;align-items:center;
  height:100dvh;height:100vh;
  overflow-y:auto;overflow-x:hidden;
  padding:60px 14px 20px;
  -webkit-overflow-scrolling:touch;
}
.big-title{
  font-family:'Pacifico',cursive;
  font-size:clamp(1.7rem,7vw,3rem);
  background:linear-gradient(135deg,#ff6eb4 0%,#ffe066 40%,#74d7f7 70%,#b97bff 100%);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
  background-size:200%;animation:shimmer 4s ease-in-out infinite,titleBounce 2s ease-in-out infinite alternate;
  text-align:center;margin-bottom:2px;
  filter:drop-shadow(0 0 14px rgba(255,110,180,0.5));
}
@keyframes shimmer{0%,100%{background-position:0%}50%{background-position:100%}}
@keyframes titleBounce{0%{transform:translateY(0) rotate(-1deg)}100%{transform:translateY(-7px) rotate(1deg)}}
.sub-name{
  font-family:'Pacifico',cursive;
  font-size:clamp(1rem,4vw,1.5rem);
  color:#ffe066;text-align:center;margin-bottom:6px;
  text-shadow:0 0 18px rgba(255,224,102,0.7);
  animation:namePulse 1.5s ease-in-out infinite alternate;
}
@keyframes namePulse{0%{transform:scale(1)}100%{transform:scale(1.06)}}

/* Dog scene */
.dog-scene{position:relative;width:100%;display:flex;justify-content:center;align-items:flex-end;height:190px;overflow:visible;}
.dog-stage{position:relative;display:inline-block;animation:dogWalkIn 2.8s ease-out forwards;transform:translateX(-420px);}
@keyframes dogWalkIn{0%{transform:translateX(-420px);}65%{transform:translateX(0);}72%{transform:translateX(10px);}80%{transform:translateX(-5px);}88%{transform:translateX(5px);}100%{transform:translateX(0);}}
.dog-svg{width:160px;height:195px;filter:drop-shadow(4px 8px 12px rgba(0,0,0,0.45));animation:dogBob 0.88s ease-in-out infinite;animation-delay:3s;}
@keyframes dogBob{0%,100%{transform:translateY(0) rotate(0)}30%{transform:translateY(-6px) rotate(-1.5deg)}70%{transform:translateY(-4px) rotate(1.5deg)}}
.dog-tail{animation:tailWag 0.42s ease-in-out infinite alternate;transform-origin:10% 50%;}
@keyframes tailWag{0%{transform:rotate(-36deg)}100%{transform:rotate(22deg)}}
.dog-ear-l{animation:earL 1.6s ease-in-out infinite;transform-origin:50% 10%;}
.dog-ear-r{animation:earR 1.6s ease-in-out infinite 0.25s;transform-origin:50% 10%;}
@keyframes earL{0%,100%{transform:rotate(0)}50%{transform:rotate(-10deg)}}
@keyframes earR{0%,100%{transform:rotate(0)}50%{transform:rotate(10deg)}}
.dog-paw{animation:pawWave 1.1s ease-in-out infinite;transform-origin:50% 0%;animation-delay:3.1s;}
@keyframes pawWave{0%,100%{transform:rotate(0)}30%{transform:rotate(18deg)}70%{transform:rotate(-6deg)}}
.flame{animation:flameDance 0.38s ease-in-out infinite alternate;transform-origin:50% 100%;}
.flame2{animation-delay:0.12s;animation-duration:0.32s;}
.flame3{animation-delay:0.22s;animation-duration:0.44s;}
@keyframes flameDance{0%{transform:scaleX(1) scaleY(1) rotate(-4deg)}100%{transform:scaleX(0.75) scaleY(1.25) rotate(4deg)}}
.cake-on-tray{position:absolute;top:18px;left:100px;animation:dogBob 0.88s ease-in-out infinite;animation-delay:3s;}
.heart-float{position:absolute;font-size:1rem;pointer-events:none;animation:heartUp 2s ease-out infinite;}
.heart-float:nth-child(1){left:-16px;top:48px;animation-delay:0s;}
.heart-float:nth-child(2){right:-12px;top:66px;animation-delay:0.6s;}
.heart-float:nth-child(3){left:48%;top:8px;animation-delay:1.2s;}
@keyframes heartUp{0%{opacity:0;transform:translateY(0) scale(0)}30%{opacity:1;transform:translateY(-16px) scale(1)}100%{opacity:0;transform:translateY(-65px) scale(0.5)}}
.sparkle-dot{position:absolute;pointer-events:none;font-size:1rem;animation:sparkPop 2s ease-in-out infinite;}
@keyframes sparkPop{0%,100%{opacity:0;transform:scale(0) rotate(0)}50%{opacity:1;transform:scale(1.3) rotate(180deg)}}
.walkway{width:88%;max-width:380px;height:8px;background:linear-gradient(90deg,rgba(255,255,255,0.04),rgba(255,255,255,0.2),rgba(255,255,255,0.04));border-radius:10px;margin-bottom:12px;}

/* Music card */
.music-card{
  width:100%;
  background:linear-gradient(145deg,rgba(255,255,255,0.08),rgba(255,255,255,0.02));
  border:1px solid rgba(255,255,255,0.1);border-radius:24px;
  padding:18px 20px 18px;backdrop-filter:blur(20px);
  box-shadow:0 20px 50px rgba(0,0,0,0.5),inset 0 1px 0 rgba(255,255,255,0.08);
}
.visualizer{display:flex;align-items:flex-end;justify-content:center;gap:3px;height:28px;margin-bottom:10px;}
.bar{width:4px;border-radius:3px 3px 0 0;background:linear-gradient(to top,#ff6eb4,#ffe066);min-height:3px;animation:barIdle 1.4s ease-in-out infinite;}
.bar:nth-child(odd){animation-delay:0.1s;}.bar:nth-child(even){animation-delay:0.3s;}
@keyframes barIdle{0%,100%{height:3px;opacity:0.3}50%{height:9px;opacity:0.6}}
.bar.dancing{animation:none!important;}
.lyrics-box{
  background:rgba(0,0,0,0.25);border-radius:14px;padding:14px 12px;
  margin-bottom:14px;min-height:68px;
  display:flex;align-items:center;justify-content:center;
  border:1px solid rgba(255,255,255,0.05);position:relative;overflow:hidden;
}
.lyric-line{font-family:'Pacifico',cursive;font-size:clamp(1rem,4vw,1.6rem);color:white;text-align:center;line-height:1.4;transition:all 0.25s ease;text-shadow:0 0 24px rgba(255,200,100,0.5);opacity:0;transform:translateY(10px) scale(0.95);}
.lyric-line.active{opacity:1;transform:translateY(0) scale(1);}
.lyric-line.highlight{background:linear-gradient(135deg,#ffe066,#ff9de2,#74d7f7);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;filter:drop-shadow(0 0 8px rgba(255,220,100,0.8));animation:lyricPop 0.4s cubic-bezier(0.34,1.56,0.64,1);}
@keyframes lyricPop{0%{transform:scale(0.8)}100%{transform:scale(1)}}
.lyric-idle{color:rgba(255,255,255,0.26);font-size:0.88rem;letter-spacing:2px;}
.progress-wrap{background:rgba(255,255,255,0.07);border-radius:99px;height:4px;margin-bottom:16px;overflow:hidden;}
.progress-fill{height:100%;width:0%;border-radius:99px;background:linear-gradient(90deg,#ff6eb4,#ffe066,#74d7f7,#b97bff);background-size:200%;transition:width 0.1s linear;animation:progressShimmer 2s linear infinite;}
@keyframes progressShimmer{0%{background-position:0%}100%{background-position:200%}}
.controls{display:flex;gap:12px;justify-content:center;align-items:center;}
.btn-play{width:60px;height:60px;border-radius:50%;border:none;background:linear-gradient(135deg,#ff6eb4,#ff8c69);color:white;font-size:1.5rem;cursor:pointer;display:flex;align-items:center;justify-content:center;box-shadow:0 5px 22px rgba(255,110,180,0.55);transition:transform 0.15s;animation:playPulse 2s ease-in-out infinite;}
@keyframes playPulse{0%,100%{box-shadow:0 5px 22px rgba(255,110,180,0.5),0 0 0 0 rgba(255,110,180,0.3)}50%{box-shadow:0 5px 22px rgba(255,110,180,0.6),0 0 0 10px rgba(255,110,180,0)}}
.btn-play:active{transform:scale(0.92);}
.btn-play.playing{background:linear-gradient(135deg,#b97bff,#74d7f7);animation:none;box-shadow:0 5px 22px rgba(116,215,247,0.5);}
.btn-restart{width:42px;height:42px;border-radius:50%;border:1px solid rgba(255,255,255,0.13);background:rgba(255,255,255,0.07);color:rgba(255,255,255,0.7);font-size:1rem;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all 0.15s;}
.btn-restart:active{transform:rotate(-25deg) scale(1.05);}
.tempo-dot{width:8px;height:8px;border-radius:50%;background:#ffe066;box-shadow:0 0 8px #ffe066;opacity:0;}
.tempo-dot.beat{opacity:1;animation:beatFade 0.25s ease-out;}
@keyframes beatFade{0%{opacity:1;transform:scale(1.6)}100%{opacity:0;transform:scale(1)}}

/* Back button */
.back-btn{
  position:fixed;top:calc(10px + env(safe-area-inset-top));left:14px;z-index:20;
  background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.18);
  border-radius:18px;padding:6px 14px;color:white;font-size:0.8rem;
  cursor:pointer;backdrop-filter:blur(10px);display:none;
}
.back-btn:active{background:rgba(255,255,255,0.2);}

/* particles */
.note{position:fixed;font-size:1.4rem;pointer-events:none;z-index:50;animation:noteFloat ease-out forwards;opacity:0;}
@keyframes noteFloat{0%{opacity:0;transform:translateY(0) rotate(0) scale(0.5)}20%{opacity:1;transform:translateY(-16px) rotate(-10deg) scale(1)}100%{opacity:0;transform:translateY(-140px) rotate(28deg) scale(0.6)}}
.confetti-p{position:fixed;top:-12px;pointer-events:none;z-index:999;animation:cfFall linear forwards;}
@keyframes cfFall{0%{opacity:1;transform:translateY(0) rotate(0)}100%{opacity:0;transform:translateY(105vh) rotate(var(--spin)) translateX(var(--drift))}}
</style>
</head>
<body>

<!-- 🔐 PASSWORD LOCK -->
<div class="lock-screen" id="lockScreen">
  <div class="lock-box">
    <h2>🔒 Secret Birthday Access</h2>
    <input id="passwordInput" placeholder="Enter your gang name">
    <button onclick="unlockSite()">Unlock</button>
    <div class="hint">Hint: Enter your gang name 😉</div>
  </div>
</div>

<div class="starfield" id="starfield"></div>
<div class="aurora"></div>

<!-- Garland -->
<div class="garland">
  <svg viewBox="0 0 1200 52" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M0,14 Q100,42 200,14 Q300,42 400,14 Q500,42 600,14 Q700,42 800,14 Q900,42 1000,14 Q1100,42 1200,14" fill="none" stroke="rgba(255,110,180,0.35)" stroke-width="2"/>
    <polygon points="100,28 111,46 89,46" fill="#ff6eb4" opacity="0.8"/>
    <polygon points="250,34 261,52 239,52" fill="#ffe066" opacity="0.8"/>
    <polygon points="400,20 411,38 389,38" fill="#74d7f7" opacity="0.8"/>
    <polygon points="550,36 561,54 539,54" fill="#b97bff" opacity="0.8"/>
    <polygon points="700,18 711,36 689,36" fill="#ff8c69" opacity="0.8"/>
    <polygon points="850,34 861,52 839,52" fill="#6ee7c7" opacity="0.8"/>
    <polygon points="1000,22 1011,40 989,40" fill="#ff6eb4" opacity="0.8"/>
    <polygon points="1150,36 1161,54 1139,54" fill="#ffe066" opacity="0.8"/>
    <circle cx="175" cy="40" r="4" fill="#6ee7c7" opacity="0.9"/>
    <circle cx="325" cy="28" r="4" fill="#ff6eb4" opacity="0.9"/>
    <circle cx="475" cy="44" r="4" fill="#ffe066" opacity="0.9"/>
    <circle cx="625" cy="26" r="4" fill="#b97bff" opacity="0.9"/>
    <circle cx="775" cy="42" r="4" fill="#74d7f7" opacity="0.9"/>
    <circle cx="925" cy="28" r="4" fill="#ff8c69" opacity="0.9"/>
    <circle cx="1075" cy="44" r="4" fill="#ff6eb4" opacity="0.9"/>
  </svg>
</div>
<div id="hbBg"></div>
<button class="back-btn" id="backBtn" onclick="goToChat()">← Chat</button>

<!-- ════════════════════════════════
     SCREEN 1: AI CHATBOT
════════════════════════════════ -->
<div id="chatScreen">
  <div class="wa-header">
    <div class="wa-dp"><img id="dpImg" src="" alt=""/></div>
    <div>
      <div class="wa-name">Birthday AI ✨</div>
      <div class="wa-status" id="waStatus">● active now</div>
    </div>

  </div>

  <div class="wa-body" id="chatBody">
    <div class="date-chip">🎂 Today — Her Special Day 🎂</div>
  </div>

  <div class="wa-input">
    <input type="text" id="userInput" placeholder="Message Birthday AI..." onkeydown="if(event.key==='Enter')sendUserMsg()" autocomplete="off" autocorrect="off"/>
    <button class="wa-send" onclick="sendUserMsg()">➤</button>
  </div>
</div>

<!-- ════════════════════════════════
     SCREEN 2: DOG + SONG
════════════════════════════════ -->
<div id="songScreen">
  <h1 class="big-title">Happy Birthday! 🎉</h1>
  <div class="sub-name">Jeevitha 🌸✨</div>

  <div class="dog-scene">
    <div style="position:relative;">
      <div style="position:absolute;top:0;left:0;width:100%;height:100%;pointer-events:none;">
        <span class="heart-float">💕</span>
        <span class="heart-float">💖</span>
        <span class="heart-float">🩷</span>
      </div>
      <span class="sparkle-dot" style="top:-8px;left:8px;animation-delay:0s">✨</span>
      <span class="sparkle-dot" style="top:22px;right:-8px;animation-delay:0.7s">⭐</span>
      <span class="sparkle-dot" style="bottom:44px;left:-12px;animation-delay:1.3s">✨</span>
      <div class="dog-stage">
        <svg class="dog-svg" viewBox="0 0 180 210" xmlns="http://www.w3.org/2000/svg">
          <g class="dog-tail"><ellipse cx="157" cy="148" rx="18" ry="9" fill="#b87340" transform="rotate(-38 157 148)"/><ellipse cx="163" cy="134" rx="12" ry="7" fill="#c8854a" transform="rotate(-58 163 134)"/><circle cx="166" cy="124" r="7" fill="#ffcba4"/></g>
          <ellipse cx="90" cy="152" rx="56" ry="43" fill="#c8854a"/>
          <ellipse cx="90" cy="152" rx="43" ry="33" fill="#d9975c"/>
          <ellipse cx="88" cy="157" rx="27" ry="21" fill="#ffcba4"/>
          <rect x="50" y="178" width="21" height="28" rx="10" fill="#b87340"/>
          <rect x="105" y="178" width="21" height="28" rx="10" fill="#b87340"/>
          <ellipse cx="60" cy="206" rx="13" ry="7" fill="#a06030"/>
          <ellipse cx="116" cy="206" rx="13" ry="7" fill="#a06030"/>
          <g class="dog-paw"><rect x="128" y="106" width="19" height="46" rx="9" fill="#c8854a"/><ellipse cx="137" cy="106" rx="12" ry="8" fill="#b87340"/></g>
          <rect x="31" y="120" width="19" height="40" rx="9" fill="#c8854a"/>
          <ellipse cx="40" cy="120" rx="12" ry="8" fill="#b87340"/>
          <circle cx="90" cy="88" r="49" fill="#c8854a"/>
          <circle cx="77" cy="72" r="19" fill="#d9975c" opacity="0.45"/>
          <g class="dog-ear-l"><ellipse cx="53" cy="51" rx="21" ry="31" fill="#a06030" transform="rotate(-16 53 51)"/><ellipse cx="53" cy="55" rx="14" ry="23" fill="#b87340" transform="rotate(-16 53 55)"/></g>
          <g class="dog-ear-r"><ellipse cx="127" cy="51" rx="21" ry="31" fill="#a06030" transform="rotate(16 127 51)"/><ellipse cx="127" cy="55" rx="14" ry="23" fill="#b87340" transform="rotate(16 127 55)"/></g>
          <circle cx="72" cy="84" r="12" fill="white"/><circle cx="108" cy="84" r="12" fill="white"/>
          <circle cx="73" cy="85" r="8" fill="#4a2808"/><circle cx="109" cy="85" r="8" fill="#4a2808"/>
          <circle cx="74" cy="85" r="4.5" fill="#110500"/><circle cx="110" cy="85" r="4.5" fill="#110500"/>
          <circle cx="76" cy="82" r="2.5" fill="white"/><circle cx="112" cy="82" r="2.5" fill="white"/>
          <path d="M62 72 Q72 65 82 71" stroke="#6a3a10" stroke-width="2.8" fill="none" stroke-linecap="round"/>
          <path d="M98 71 Q108 65 118 72" stroke="#6a3a10" stroke-width="2.8" fill="none" stroke-linecap="round"/>
          <ellipse cx="90" cy="103" rx="11" ry="7.5" fill="#3a1a04"/>
          <ellipse cx="87" cy="101" rx="3.5" ry="2.2" fill="rgba(255,255,255,0.28)"/>
          <path d="M79 111 Q90 126 101 111" stroke="#6a2a08" stroke-width="2.8" fill="none" stroke-linecap="round"/>
          <ellipse cx="90" cy="119" rx="10" ry="8" fill="#ff7eb3"/>
          <line x1="90" y1="112" x2="90" y2="127" stroke="#e05090" stroke-width="1.8" stroke-linecap="round"/>
          <circle cx="59" cy="106" r="11" fill="#ff9ec0" opacity="0.4"/>
          <circle cx="121" cy="106" r="11" fill="#ff9ec0" opacity="0.4"/>
          <polygon points="90,28 71,72 109,72" fill="#ff6eb4"/>
          <polygon points="90,28 81,51 90,51" fill="#ffb3d4" opacity="0.55"/>
          <line x1="71" y1="72" x2="109" y2="72" stroke="#ffe066" stroke-width="3.2"/>
          <circle cx="90" cy="28" r="5.5" fill="#ffe066"/>
          <line x1="90" y1="22" x2="90" y2="12" stroke="#ffe066" stroke-width="2.2"/>
          <circle cx="90" cy="10" r="3.5" fill="#ffb3d4"/>
          <circle cx="84" cy="54" r="2.8" fill="#ffe066"/><circle cx="97" cy="60" r="2.8" fill="#74d7f7"/><circle cx="87" cy="67" r="2.2" fill="#b97bff"/>
          <ellipse cx="138" cy="101" rx="30" ry="6.5" fill="#b09040"/>
          <rect x="110" y="97" width="56" height="4" rx="2" fill="#caa858"/>
        </svg>
        <div class="cake-on-tray" id="cakeEl">
          <svg width="68" height="80" viewBox="0 0 72 84" xmlns="http://www.w3.org/2000/svg">
            <rect x="4" y="46" width="64" height="30" rx="9" fill="#ff6eb4"/>
            <rect x="4" y="46" width="64" height="11" rx="6" fill="#ff9de2"/>
            <path d="M13,46 Q17,57 22,46 Q27,57 32,46 Q37,57 42,46 Q47,57 52,46 Q57,57 62,46 Q66,57 70,46" fill="white" opacity="0.75"/>
            <rect x="11" y="27" width="50" height="21" rx="7" fill="#ffe066"/>
            <rect x="11" y="27" width="50" height="9" rx="5" fill="#ffef99"/>
            <rect x="18" y="13" width="36" height="16" rx="6" fill="#b97bff"/>
            <rect x="18" y="13" width="36" height="8" rx="5" fill="#d4a0ff"/>
            <ellipse cx="36" cy="13" rx="18" ry="5.5" fill="white"/>
            <rect x="20" y="2" width="6" height="13" rx="3" fill="#ff8c69"/>
            <rect x="33" y="-1" width="6" height="15" rx="3" fill="#74d7f7"/>
            <rect x="46" y="2" width="6" height="13" rx="3" fill="#ffe066"/>
            <g class="flame"><ellipse cx="23" cy="2" rx="3.5" ry="5.5" fill="#ffee00"/><ellipse cx="23" cy="2" rx="2.2" ry="3.8" fill="#ff9900"/><ellipse cx="23" cy="0.5" rx="1.1" ry="2.2" fill="white"/></g>
            <g class="flame flame2"><ellipse cx="36" cy="-1" rx="3.5" ry="5.5" fill="#ffee00"/><ellipse cx="36" cy="-1" rx="2.2" ry="3.8" fill="#ff9900"/><ellipse cx="36" cy="-2.5" rx="1.1" ry="2.2" fill="white"/></g>
            <g class="flame flame3"><ellipse cx="49" cy="2" rx="3.5" ry="5.5" fill="#ffee00"/><ellipse cx="49" cy="2" rx="2.2" ry="3.8" fill="#ff9900"/><ellipse cx="49" cy="0.5" rx="1.1" ry="2.2" fill="white"/></g>
            <circle cx="18" cy="60" r="3.5" fill="#ffe066"/>
            <circle cx="36" cy="62" r="3.5" fill="#74d7f7"/>
            <circle cx="54" cy="60" r="3.5" fill="#b97bff"/>
          </svg>
        </div>
      </div>
    </div>
  </div>

  <div class="walkway"></div>

  <div class="music-card">
    <div class="visualizer" id="visualizer"></div>
    <div class="lyrics-box"><div class="lyric-line lyric-idle" id="lyricDisplay">🐾 Press ▶ to play!</div></div>
    <div class="progress-wrap"><div class="progress-fill" id="progressFill"></div></div>
    <div class="controls">
      <button class="btn-restart" onclick="restartSong()">↺</button>
      <button class="btn-play" id="playBtn" onclick="togglePlay()">▶</button>
      <div class="tempo-dot" id="tempoDot"></div>
    </div>
  </div>
</div>

<script>
/* 🔐 PASSWORD LOGIC (ADDED) */
function unlockSite(){
  const val=document.getElementById('passwordInput').value.trim();
  if(val==="Coders"){
    document.getElementById('lockScreen').style.display="none";
  }else{
    alert("Wrong gang name 😜");
  }
}

// ── PROFILE PIC ──
document.getElementById('dpImg').src = 'data:image/jpeg;base64,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';

// ── STARFIELD ──
const sf=document.getElementById('starfield');
for(let i=0;i<70;i++){
  const s=document.createElement('div');s.className='star-dot';
  const sz=1+Math.random()*2.5;
  s.style.cssText=`width:${sz}px;height:${sz}px;left:${Math.random()*100}%;top:${Math.random()*100}%;animation-duration:${1.4+Math.random()*3}s;animation-delay:${Math.random()*5}s;`;
  sf.appendChild(s);
}

// ── HB FLOAT ──
const hbColors=['#ff6eb4','#ffe066','#74d7f7','#b97bff','#ff8c69','#6ee7c7'];
const hbPhrases=['Happy Birthday!','🎂🎉','Happy Birthday!','Jeevitha! 🌸','🥳✨','We Love You!'];
const hbBg=document.getElementById('hbBg');
hbPhrases.forEach((txt,i)=>{
  const el=document.createElement('div');el.className='hb-float';el.textContent=txt;
  const dur=9+Math.random()*7;const delay=i*(dur/hbPhrases.length);
  el.style.cssText=`left:${5+Math.random()*80}%;top:${85+Math.random()*15}%;font-size:${1.8+Math.random()*2}rem;color:${hbColors[i%hbColors.length]};--r:${(Math.random()-.5)*16}deg;--op:${0.07+Math.random()*0.09};animation-duration:${dur}s;animation-delay:-${delay}s;`;
  hbBg.appendChild(el);
});

// ════════════════════════════════
//  AI CHATBOT ENGINE
// ════════════════════════════════
const chatBody=document.getElementById('chatBody');
const chatScreen=document.getElementById('chatScreen');
const songScreen=document.getElementById('songScreen');

const CONV = [
  {role:'ai', text:'Hello Jeevitha... 👀', delay:800},
  {role:'ai', text:'Initializing birthday protocol...', delay:2800},
  {role:'ai', text:'Scanning personality…', delay:5200},
  {role:'ai', text:'Result: One of the sweetest humans detected 💖', delay:7800},
  {role:'ai', text:'Today is not just any day…', delay:11000},
  {role:'ai', text:'It is YOUR special day 🎂', delay:13800},
  {role:'ai', text:'So I was specially programmed…', delay:16500},
  {role:'ai', text:'To wish you the happiest birthday ever ✨', delay:19500},
  {role:'ai', text:'May your smile stay this beautiful always 😊 and may this year bring you crazy happiness 🚀', delay:23000, isLast:true},
];

let msgIndex=0, userCanType=false;

function timeStr(){
  const now=new Date();const h=now.getHours();const m=now.getMinutes().toString().padStart(2,'0');
  const ampm=h>=12?'PM':'AM';const h12=h%12||12;return `${h12}:${m} ${ampm}`;
}

function typeText(el, text, speed, callback){
  let i=0;
  const cursor=document.createElement('span');
  cursor.className='typing-cursor';cursor.textContent='|';
  el.after(cursor);
  function tick(){
    if(i<=text.length){
      el.textContent=text.slice(0,i);
      i++;
      chatBody.scrollTop=chatBody.scrollHeight;
      setTimeout(tick, speed+(Math.random()*14-7));
    } else {
      cursor.remove();
      if(callback) callback();
    }
  }
  tick();
}

function addMsg(role,text,callback){
  if(role==='typing'){
    const wrap=document.createElement('div');wrap.className='typing-wrap';wrap.id='typingIndicator';
    wrap.innerHTML=`<div class="typing-bubble"><div class="typing-dot"></div><div class="typing-dot"></div><div class="typing-dot"></div></div>`;
    chatBody.appendChild(wrap);chatBody.scrollTop=chatBody.scrollHeight;return;
  }
  const old=document.getElementById('typingIndicator');if(old)old.remove();
  const div=document.createElement('div');
  div.className=`msg msg-${role==='ai'?'in':'out'}`;

  if(role==='ai'){
    const sender=document.createElement('div');sender.className='msg-sender';sender.textContent='✨ Birthday AI';div.appendChild(sender);
    const textEl=document.createElement('span');div.appendChild(textEl);
    const timeEl=document.createElement('div');timeEl.className='msg-time';timeEl.textContent=timeStr();
    chatBody.appendChild(div);
    chatBody.scrollTop=chatBody.scrollHeight;
    typeText(textEl, text, 45, ()=>{
      div.appendChild(timeEl);
      chatBody.scrollTop=chatBody.scrollHeight;
      if(callback)setTimeout(callback,200);
    });
  } else {
    div.innerHTML=`${text}<div class="msg-time">${timeStr()} ✓✓</div>`;
    chatBody.appendChild(div);
    chatBody.scrollTop=chatBody.scrollHeight;
    if(callback)setTimeout(callback,200);
  }
}

function playConversation(){
  if(msgIndex>=CONV.length)return;
  const item=CONV[msgIndex];
  const thinkTime = 700 + Math.min(item.text.length * 18, 1800);
  setTimeout(()=>addMsg('typing'), 300);
  setTimeout(()=>{
    addMsg('ai', item.text, ()=>{
      if(item.isLast){
        userCanType=true;
        document.getElementById('userInput').placeholder="Type anything & tap send! 🎉";
        document.getElementById('waStatus').textContent='⚡ tap send for surprise!';
        const btn=document.createElement('button');
        btn.className='surprise-btn';btn.id='surpriseBtn';
        btn.textContent='🎂 Open My Surprise! 🐶';
        btn.onclick=()=>triggerSurprise();
        chatBody.appendChild(btn);
        chatBody.scrollTop=chatBody.scrollHeight;
      } else {
        msgIndex++;
        setTimeout(playConversation, 600);
      }
    });
  }, thinkTime);
}

function triggerSurprise(){
  const btn=document.getElementById('surpriseBtn');if(btn)btn.remove();
  userCanType=false;
  addMsg('typing');
  setTimeout(()=>{
    addMsg('ai','YAY!! Here comes your surprise Jeevitha!! 🎂🐾🎵🎉🎊');
    setTimeout(()=>switchToSong(),1200);
  },800);
}

function sendUserMsg(){
  const inp=document.getElementById('userInput');const txt=inp.value.trim();
  if(!txt)return;
  addMsg('out',txt);inp.value='';
  if(userCanType){
    const btn=document.getElementById('surpriseBtn');if(btn)btn.remove();
    triggerSurprise();
  }
}

function switchToSong(){
  chatScreen.style.transition='all 0.5s ease';
  chatScreen.style.opacity='0';chatScreen.style.transform='scale(0.92)';
  setTimeout(()=>{
    chatScreen.style.display='none';
    songScreen.style.display='flex';
    songScreen.style.opacity='0';songScreen.style.transform='scale(0.92)';
    songScreen.style.transition='all 0.5s ease';
    document.getElementById('backBtn').style.display='block';
    launchConfetti();
    setTimeout(()=>{songScreen.style.opacity='1';songScreen.style.transform='scale(1)';},40);
  },500);
}

function goToChat(){
  songScreen.style.display='none';
  chatScreen.style.display='flex';
  chatScreen.style.opacity='1';chatScreen.style.transform='scale(1)';
  document.getElementById('backBtn').style.display='none';
  clearSong();isPlaying=false;
  playBtn.classList.remove('playing');playBtn.textContent='▶';
}

setTimeout(playConversation,600);

// ════════════════════════════════
//  SONG ENGINE
// ════════════════════════════════
const visEl=document.getElementById('visualizer');const barEls=[];
for(let i=0;i<22;i++){const b=document.createElement('div');b.className='bar';visEl.appendChild(b);barEls.push(b);}
const BPM=162,beat=60/BPM;
const SONG=[
  [392,0.75,"Happy",false],[392,0.25,null,false],[440,1.0,"Birth-",true],[392,1.0,"-day",false],[523,1.0,"to",false],[494,2.0,"You! 🎶",true],
  [392,0.75,"Happy",false],[392,0.25,null,false],[440,1.0,"Birth-",true],[392,1.0,"-day",false],[587,1.0,"to",false],[523,2.0,"You! 🎶",true],
  [392,0.75,"Happy",false],[392,0.25,null,false],[784,1.0,"Birth-",true],[659,1.0,"-day",false],[523,1.0,"dear",false],[494,1.0,"Jeevitha",true],[440,2.0,"🥰",true],
  [698,0.75,"Happy",false],[698,0.25,null,false],[659,1.0,"Birth-",true],[523,1.0,"-day",false],[587,1.0,"to",false],[523,3.0,"YOU! 🎉",true],
];
let audioCtx=null,isPlaying=false,noteTimeouts=[],progressInterval=null,totalDuration=0,startTime=0;
SONG.forEach(n=>totalDuration+=n[1]*beat);
const lyricEl=document.getElementById('lyricDisplay'),progFill=document.getElementById('progressFill'),playBtn=document.getElementById('playBtn'),tempoDot=document.getElementById('tempoDot');
const musicNotes=['🎵','🎶','🎸','🎹','🎺','🎻'];
function getCtx(){if(!audioCtx)audioCtx=new(window.AudioContext||window.webkitAudioContext)();return audioCtx;}
function playNote(freq,startSec,durSec){
  const ctx=getCtx(),osc=ctx.createOscillator(),gain=ctx.createGain();
  osc.connect(gain);gain.connect(ctx.destination);osc.type='sine';osc.frequency.value=freq;
  const now=ctx.currentTime+startSec;
  gain.gain.setValueAtTime(0,now);gain.gain.linearRampToValueAtTime(0.3,now+0.02);
  gain.gain.setValueAtTime(0.3,now+durSec*0.72);gain.gain.exponentialRampToValueAtTime(0.001,now+durSec);
  osc.start(now);osc.stop(now+durSec);
}
function spawnNote(x,y){
  const el=document.createElement('div');el.className='note';
  el.textContent=musicNotes[Math.floor(Math.random()*musicNotes.length)];
  el.style.left=x+'px';el.style.top=y+'px';el.style.animationDuration=(1+Math.random()*.9)+'s';
  document.body.appendChild(el);setTimeout(()=>el.remove(),2100);
}
function animateBars(intensity){
  barEls.forEach((b,i)=>{
    b.classList.add('dancing');
    const wave=Math.sin((Date.now()/110)+i*0.72)*0.5+0.5;
    b.style.height=(3+intensity*wave*28)+'px';b.style.opacity=0.35+wave*0.65;
    const hue=(i/barEls.length)*60+330;
    b.style.background=`linear-gradient(to top,hsl(${hue},100%,62%),hsl(${hue+40},100%,75%))`;
  });
}
function resetBars(){barEls.forEach(b=>{b.classList.remove('dancing');b.style.height=b.style.opacity=b.style.background='';});}
function launchConfetti(){
  const cols=['#ff6eb4','#ffe066','#74d7f7','#b97bff','#6ee7c7','#ff8c69','#fff'];
  for(let i=0;i<90;i++){
    setTimeout(()=>{
      const p=document.createElement('div');p.className='confetti-p';
      const drift=(Math.random()-.5)*420,spin=(Math.random()-.5)*700,sz=6+Math.random()*8;
      p.style.cssText=`left:${Math.random()*100}%;background:${cols[i%cols.length]};width:${sz}px;height:${sz*(.4+Math.random()*.8)}px;--drift:${drift}px;--spin:${spin}deg;border-radius:${Math.random()>.5?'50%':'3px'};animation-duration:${2+Math.random()*2}s;animation-delay:${Math.random()*.6}s;`;
      document.body.appendChild(p);setTimeout(()=>p.remove(),4200);
    },i*26);
  }
}
function beatFlash(){tempoDot.classList.remove('beat');void tempoDot.offsetWidth;tempoDot.classList.add('beat');}
function dogDance(on){const dog=document.querySelector('.dog-svg');if(dog)dog.style.animation=on?'dogBob 0.44s ease-in-out infinite':'dogBob 0.88s ease-in-out infinite';}
function startSong(){
  const ctx=getCtx();if(ctx.state==='suspended')ctx.resume();
  let cursor=0;
  SONG.forEach(nd=>{
    const[freq,dur,lyric,highlight]=nd;const startSec=cursor;cursor+=dur*beat;
    playNote(freq,startSec,dur*beat*0.88);
    if(lyric){
      const t=setTimeout(()=>{
        lyricEl.className='lyric-line active'+(highlight?' highlight':'');
        lyricEl.textContent=lyric;beatFlash();
        const rect=lyricEl.getBoundingClientRect();
        for(let k=0;k<3;k++)setTimeout(()=>spawnNote(rect.left+Math.random()*rect.width,rect.top+Math.random()*20),k*110);
      },startSec*1000);noteTimeouts.push(t);
    }
  });
  const barAnim=setInterval(()=>{
    if(!isPlaying){clearInterval(barAnim);resetBars();dogDance(false);return;}
    animateBars(Math.min((Date.now()-startTime)/(totalDuration*1000)*2,1));
  },55);noteTimeouts.push(barAnim);dogDance(true);
  startTime=Date.now();
  progressInterval=setInterval(()=>{
    const pct=Math.min(((Date.now()-startTime)/(totalDuration*1000))*100,100);
    progFill.style.width=pct+'%';if(pct>=100)clearInterval(progressInterval);
  },50);
  const endT=setTimeout(()=>{
    launchConfetti();
    lyricEl.className='lyric-line active highlight';
    lyricEl.textContent='🎉 Happy Birthday Jeevitha! 🎉';
    isPlaying=false;playBtn.classList.remove('playing');playBtn.textContent='▶';
    resetBars();dogDance(false);
  },totalDuration*1000+200);noteTimeouts.push(endT);
}
function clearSong(){noteTimeouts.forEach(t=>{clearTimeout(t);clearInterval(t);});noteTimeouts=[];clearInterval(progressInterval);resetBars();dogDance(false);}
function togglePlay(){
  if(isPlaying){isPlaying=false;clearSong();playBtn.classList.remove('playing');playBtn.textContent='▶';lyricEl.className='lyric-line lyric-idle';lyricEl.textContent='🐾 Press ▶ to play!';}
  else{isPlaying=true;playBtn.classList.add('playing');playBtn.textContent='⏸';lyricEl.className='lyric-line active';lyricEl.textContent='🎵 ...';progFill.style.width='0%';startSong();}
}
function restartSong(){isPlaying=false;clearSong();playBtn.classList.remove('playing');playBtn.textContent='▶';lyricEl.className='lyric-line lyric-idle';lyricEl.textContent='🐾 Press ▶ to play!';progFill.style.width='0%';setTimeout(()=>togglePlay(),180);}
</script>
</body>
</html>
