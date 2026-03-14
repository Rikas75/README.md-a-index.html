<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no,viewport-fit=cover">
  <meta name="theme-color"                    content="#0d0d0d">
  <meta name="apple-mobile-web-app-capable"   content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title"     content="USALA">
  <meta name="description"                    content="USALA Suite — Finanzas Personales">
  <title>USALA Suite</title>

  <!-- PWA -->
  <link rel="apple-touch-icon" href="img/icon-192.png">

  <!-- Fuente -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;700;800;900&display=swap" rel="stylesheet">

  <!-- Estilos -->
<style>
:root {
  --bg:      #eef6f0;
  --bg2:     #e4f0e8;
  --card:    rgba(255,255,255,0.75);
  --card2:   rgba(255,255,255,0.50);
  --text:    #142a1c;
  --txt:     #142a1c;
  --dim:     rgba(30,80,50,0.50);
  --accent:  #1a8c4e;
  --accent2: #22b060;
  --danger:  #e03535;
  --gold:    #c07a10;
  --blue:    #2196f3;
  --border:  rgba(30,140,80,0.14);
  --nav:     rgba(10,40,20,0.90);
  --navtext: #ffffff;
  --shadow:  0 4px 24px rgba(30,140,80,0.12);
  --radius:  18px;
  --inp:     rgba(255,255,255,0.65);
  --orb1:    rgba(43,192,112,0.18);
  --orb2:    rgba(20,160,80,0.12);
  --orb3:    rgba(100,220,160,0.10);
  --glow:    rgba(26,140,78,0.30);
}
[data-theme="dark"] {
  --bg:      #1e2228;
  --bg2:     #252c34;
  --card:    rgba(255,255,255,0.07);
  --card2:   rgba(255,255,255,0.04);
  --text:    #e8edf2;
  --dim:     rgba(200,215,230,0.45);
  --accent:  #3dbf7a;
  --accent2: #52d48e;
  --danger:  #ff6057;
  --gold:    #ffb340;
  --border:  rgba(255,255,255,0.10);
  --nav:     rgba(18,22,28,0.95);
  --navtext: #e8edf2;
  --inp:     rgba(255,255,255,0.07);
  --orb1:    rgba(60,190,120,0.14);
  --orb2:    rgba(40,100,180,0.10);
  --orb3:    rgba(80,200,140,0.08);
  --glow:    rgba(61,191,122,0.30);
  --blue:    #2196f3;
  --txt:     #e8edf2;
}
[data-theme="gold"] {
  --bg:      #fdf6e8;
  --bg2:     #f8edda;
  --card:    rgba(255,255,255,0.78);
  --card2:   rgba(255,255,255,0.55);
  --text:    #2a1a00;
  --dim:     rgba(100,60,0,0.50);
  --accent:  #b86e00;
  --accent2: #d48a10;
  --danger:  #cc2a2a;
  --gold:    #c07a10;
  --border:  rgba(180,110,0,0.16);
  --nav:     rgba(40,20,0,0.92);
  --navtext: #fdf6e8;
  --inp:     rgba(255,255,255,0.65);
  --orb1:    rgba(220,160,40,0.18);
  --orb2:    rgba(180,100,0,0.12);
  --orb3:    rgba(255,200,80,0.10);
  --glow:    rgba(180,110,0,0.28);
  --blue:    #2196f3;
  --txt:     #2a1a00;
}
[data-theme="ocean"] {
  --bg:      #eaf4fc;
  --bg2:     #deeef8;
  --card:    rgba(255,255,255,0.78);
  --card2:   rgba(255,255,255,0.55);
  --text:    #0a2540;
  --dim:     rgba(10,60,120,0.48);
  --accent:  #0070cc;
  --accent2: #1a90e8;
  --danger:  #d42a2a;
  --gold:    #c07a10;
  --border:  rgba(0,100,200,0.14);
  --nav:     rgba(5,25,60,0.92);
  --navtext: #eaf4fc;
  --inp:     rgba(255,255,255,0.65);
  --orb1:    rgba(0,130,230,0.16);
  --orb2:    rgba(0,80,180,0.10);
  --orb3:    rgba(80,180,255,0.10);
  --glow:    rgba(0,112,204,0.28);
  --blue:    #2196f3;
  --txt:     #0a2540;
}
[data-theme="rose"] {
  --bg:      #fdf0f4;
  --bg2:     #f8e6ed;
  --card:    rgba(255,255,255,0.78);
  --card2:   rgba(255,255,255,0.55);
  --text:    #2a0a18;
  --dim:     rgba(120,20,60,0.48);
  --accent:  #c0204a;
  --accent2: #dc3a64;
  --danger:  #c02020;
  --gold:    #b07010;
  --border:  rgba(200,30,80,0.14);
  --nav:     rgba(40,0,20,0.92);
  --navtext: #fdf0f4;
  --inp:     rgba(255,255,255,0.65);
  --orb1:    rgba(220,60,110,0.14);
  --orb2:    rgba(160,20,70,0.10);
  --orb3:    rgba(255,120,160,0.10);
  --glow:    rgba(192,32,74,0.26);
  --blue:    #2196f3;
  --txt:     #2a0a18;
}
* {margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body {
  height:100%;font-family:Outfit,sans-serif;
  background:var(--bg);color:var(--text);overflow:hidden;
}
body.login-active {overflow:hidden;}
.screen {display:none;position:fixed;inset:0;}
.screen.active {display:flex;flex-direction:column;}
.screen::before {
  content:'';position:absolute;inset:0;pointer-events:none;z-index:0;
  background:
    radial-gradient(ellipse 70% 60% at 10% 10%, var(--orb1) 0%, transparent 55%),
    radial-gradient(ellipse 60% 70% at 90% 80%, var(--orb2) 0%, transparent 55%),
    radial-gradient(ellipse 50% 50% at 70% 5%,  var(--orb3) 0%, transparent 50%);
  animation: bgPulse 12s ease-in-out infinite alternate;
}
@keyframes bgPulse {
  0%{opacity:0.7;transform:scale(1);}
  100%{opacity:1;transform:scale(1.05);}
}
.screen::after {
  content:'';position:absolute;inset:0;pointer-events:none;z-index:0;
  background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.035'/%3E%3C/svg%3E");
  background-size:180px;opacity:0.6;
}
#accessScreen {
  align-items:stretch;justify-content:center;
  background: linear-gradient(145deg,#0a1628 0%,#0d2137 40%,#0a2818 70%,#071a10 100%) !important;
  overflow:hidden;
  position:fixed;inset:0;
}
.lg-scroll-outer {
  position:relative;z-index:1;
  flex:1;width:100%;
  overflow-y:auto;
  overflow-x:hidden;
  -webkit-overflow-scrolling:touch;
  display:flex;flex-direction:column;align-items:center;
}
.lg-scroll-outer::-webkit-scrollbar {display:none;}
.lg-scroll-outer {-ms-overflow-style:none;scrollbar-width:none;}
#accessScreen::before {
  content:'';position:absolute;inset:0;pointer-events:none;
  background:
    radial-gradient(ellipse 60% 50% at 20% 20%, rgba(30,180,100,0.18) 0%, transparent 60%),
    radial-gradient(ellipse 50% 60% at 80% 70%, rgba(45,100,255,0.14) 0%, transparent 60%),
    radial-gradient(ellipse 40% 40% at 60% 10%, rgba(100,220,160,0.10) 0%, transparent 50%);
  animation: lgBgPulse 8s ease-in-out infinite alternate;
}
@keyframes lgBgPulse {
  0%{opacity:0.7;transform:scale(1);}
  100%{opacity:1;transform:scale(1.04);}
}
#accessScreen::after {
  content:'';position:absolute;inset:0;pointer-events:none;
  background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
  background-size:180px;opacity:0.5;
}
.lg-wrap {
  width:100%;max-width:400px;margin:0 auto;
  padding:48px 20px 80px;
  display:flex;flex-direction:column;align-items:center;
  position:relative;z-index:1;
  min-height:100vh;
  animation:lgFadeUp 0.6s cubic-bezier(0.16,1,0.3,1) both;
}
@keyframes lgFadeUp {
  from{opacity:0;transform:translateY(28px);}
  to{opacity:1;transform:translateY(0);}
}
.lg-logo {
  font-size:3rem;font-weight:900;letter-spacing:-0.06em;
  background:linear-gradient(135deg,#fff 0%,rgba(180,255,220,0.9) 60%,rgba(120,200,180,0.7) 100%);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
  background-clip:text;line-height:1;text-align:center;
  filter:drop-shadow(0 2px 24px rgba(60,200,120,0.3));
}
.lg-sub {
  font-size:0.62rem;font-weight:600;letter-spacing:0.28em;text-transform:uppercase;
  color:rgba(255,255,255,0.35);margin-top:6px;margin-bottom:36px;text-align:center;
}
.lg-card {
  width:100%;
  background:rgba(255,255,255,0.06);
  backdrop-filter:blur(24px) saturate(180%);
  -webkit-backdrop-filter:blur(24px) saturate(180%);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:24px;
  padding:22px 20px 22px;
  margin-bottom:14px;
  box-shadow:0 8px 40px rgba(0,0,0,0.35), 0 1px 0 rgba(255,255,255,0.1) inset;
  animation:lgFadeUp 0.6s cubic-bezier(0.16,1,0.3,1) 0.08s both;
}
.lg-avatar {
  width:76px;height:76px;border-radius:50%;
  background:linear-gradient(135deg,rgba(60,200,120,0.8),rgba(30,120,80,0.9));
  display:flex;align-items:center;justify-content:center;
  font-size:2rem;font-weight:900;color:#fff;
  margin:0 auto 14px;
  border:1.5px solid rgba(255,255,255,0.2);
  box-shadow:0 8px 32px rgba(0,0,0,0.3),0 0 0 6px rgba(60,200,120,0.12);
}
.lg-greeting {
  font-size:0.62rem;font-weight:600;letter-spacing:0.16em;text-transform:uppercase;
  color:rgba(255,255,255,0.4);text-align:center;margin-bottom:5px;
}
.lg-name {
  font-size:1.5rem;font-weight:800;color:#fff;
  text-align:center;margin-bottom:22px;letter-spacing:-0.02em;
}
.lg-section-title {
  font-size:0.68rem;font-weight:600;letter-spacing:0.08em;text-transform:uppercase;
  color:rgba(255,255,255,0.35);margin-bottom:8px;
}
.lg-err {
  display:none;padding:10px 14px;
  background:rgba(255,60,60,0.12);border:1px solid rgba(255,80,80,0.25);
  border-radius:12px;font-size:0.78rem;color:#ff8a80;
  margin-bottom:14px;text-align:center;
  animation:lgShake 0.35s ease;
}
@keyframes lgShake {
  0%,100%{transform:translateX(0);}
  20%{transform:translateX(-6px);}
  40%{transform:translateX(6px);}
  60%{transform:translateX(-4px);}
  80%{transform:translateX(4px);}
}
.lg-inp {
  width:100%;padding:15px 16px;
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:14px;
  font-family:Outfit,sans-serif;font-size:0.95rem;color:#fff;
  outline:none;box-sizing:border-box;
  transition:border-color 0.2s,background 0.2s;
  margin-bottom:12px;
}
.lg-inp::placeholder {color:rgba(255,255,255,0.3);}
.lg-inp:focus {
  border-color:rgba(60,200,120,0.6);
  background:rgba(255,255,255,0.1);
}
.lg-code-inp {
  width:100%;padding:16px;
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:14px;
  font-family:JetBrains Mono,monospace;font-size:1.15rem;font-weight:700;
  color:#fff;letter-spacing:0.14em;text-align:center;text-transform:uppercase;
  outline:none;box-sizing:border-box;
  transition:border-color 0.2s,background 0.2s;
  margin-bottom:14px;
}
.lg-code-inp::placeholder {color:rgba(255,255,255,0.25);font-family:Outfit,sans-serif;letter-spacing:0.02em;font-size:0.9rem;}
.lg-code-inp:focus {border-color:rgba(60,200,120,0.6);background:rgba(255,255,255,0.1);}
.lg-btn {
  width:100%;padding:16px;
  background:linear-gradient(135deg,#2bc070,#1a9a55);
  color:#fff;border:none;border-radius:16px;
  font-family:Outfit,sans-serif;font-size:1rem;font-weight:700;
  cursor:pointer;letter-spacing:0.01em;
  box-shadow:0 4px 24px rgba(43,192,112,0.35),0 1px 0 rgba(255,255,255,0.15) inset;
  transition:transform 0.12s,box-shadow 0.12s,opacity 0.12s;
  position:relative;overflow:hidden;
}
.lg-btn::after {
  content:'';position:absolute;inset:0;
  background:linear-gradient(to bottom,rgba(255,255,255,0.12),transparent);
  pointer-events:none;
}
.lg-btn:active {transform:scale(0.97);opacity:0.9;box-shadow:0 2px 12px rgba(43,192,112,0.25);}
.lg-btn-ghost {
  width:100%;padding:14px;
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.1);
  border-radius:14px;
  font-family:Outfit,sans-serif;font-size:0.85rem;color:rgba(255,255,255,0.55);
  cursor:pointer;transition:background 0.15s,border-color 0.15s;margin-top:10px;
}
.lg-btn-ghost:active {background:rgba(255,255,255,0.1);}
.lg-link {
  font-size:0.8rem;color:rgba(100,220,160,0.8);
  cursor:pointer;font-weight:600;text-align:center;
  margin-top:16px;display:block;letter-spacing:0.01em;
  transition:color 0.15s;
}
.lg-link:active {color:#fff;}
.nip-dots {display:flex;gap:14px;justify-content:center;margin:6px 0 16px;}
.nip-dot {
  width:14px;height:14px;border-radius:50%;
  border:2px solid rgba(255,255,255,0.2);
  background:transparent;
  transition:all 0.2s cubic-bezier(0.34,1.56,0.64,1);
}
.nip-dot.on {
  background:linear-gradient(135deg,#2bc070,#1a9a55);
  border-color:transparent;
  box-shadow:0 0 12px rgba(43,192,112,0.6);
  transform:scale(1.2);
}
.numpad {display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-top:4px;}
.nk {
  padding:15px 10px;border:none;
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.08);
  color:#fff;
  font-family:Outfit,sans-serif;font-size:1.25rem;font-weight:500;
  border-radius:14px;cursor:pointer;
  transition:background 0.1s,transform 0.08s,border-color 0.1s;
  -webkit-tap-highlight-color:transparent;
  touch-action:manipulation;
  position:relative;overflow:hidden;
  min-height:52px;
}
.nk::after {content:'';position:absolute;inset:0;background:linear-gradient(to bottom,rgba(255,255,255,0.06),transparent);pointer-events:none;}
.nk:active {background:rgba(43,192,112,0.25);border-color:rgba(43,192,112,0.4);transform:scale(0.93);}
.nk-del {font-size:1.1rem;color:rgba(255,255,255,0.5);}
.nk-blank {background:transparent!important;border:none!important;pointer-events:none;}
.lg-modal-backdrop {display:none;position:fixed;inset:0;background:rgba(0,0,0,0.6);backdrop-filter:blur(8px);z-index:500;align-items:flex-end;justify-content:center;}
.lg-modal-backdrop.open {display:flex;}
.lg-modal-box {
  background:rgba(15,28,20,0.95);
  backdrop-filter:blur(32px);
  border:1px solid rgba(255,255,255,0.1);
  border-radius:28px 28px 0 0;
  padding:28px 24px 48px;
  width:100%;max-width:480px;
  box-shadow:0 -8px 40px rgba(0,0,0,0.5);
}
.lg-modal-handle {width:36px;height:4px;background:rgba(255,255,255,0.2);border-radius:2px;margin:0 auto 24px;}
.lg-dashed-btn {
  width:100%;padding:16px;
  border:1.5px dashed rgba(60,200,120,0.4);
  background:rgba(60,200,120,0.05);
  color:rgba(100,220,160,0.9);
  border-radius:16px;
  font-family:Outfit,sans-serif;font-size:0.9rem;font-weight:700;
  cursor:pointer;transition:background 0.15s,border-color 0.15s;margin-top:8px;
}
.lg-dashed-btn:active {background:rgba(60,200,120,0.1);border-color:rgba(60,200,120,0.6);}
.lg-textarea {
  width:100%;padding:14px 16px;
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:14px;
  font-family:Outfit,sans-serif;font-size:0.88rem;color:#fff;
  outline:none;resize:none;box-sizing:border-box;margin-bottom:12px;
  transition:border-color 0.2s;
}
.lg-textarea::placeholder {color:rgba(255,255,255,0.28);}
.lg-textarea:focus {border-color:rgba(60,200,120,0.6);}
.lg-divider {display:flex;align-items:center;gap:12px;margin:18px 0 14px;}
.lg-divider::before,.lg-divider::after {content:'';flex:1;height:1px;background:rgba(255,255,255,0.1);}
.lg-divider span {font-size:0.68rem;color:rgba(255,255,255,0.3);font-weight:600;letter-spacing:0.06em;white-space:nowrap;}
#themePicker {align-items:center;justify-content:center;padding:32px 24px;}
.theme-card {padding:20px 16px;border-radius:16px;cursor:pointer;border:2px solid transparent;transition:all 0.2s;text-align:left;}
.theme-card:active {transform:scale(0.97);}
.theme-card.selected {border-color:currentColor;}
#dashboard {display:none;flex-direction:column;}
#dashboard.active {display:flex;}
#dashboard > * {position:relative;z-index:1;}
.topbar {
  display:flex;align-items:center;padding:14px 16px 10px;gap:10px;
  background:rgba(255,255,255,0.55);
  backdrop-filter:blur(20px) saturate(160%);
  -webkit-backdrop-filter:blur(20px) saturate(160%);
  border-bottom:1px solid var(--border);
  position:relative;z-index:2;
}
[data-theme="dark"] .topbar {background:rgba(0,0,0,0.25);}
.top-logo {
  font-size:1.05rem;font-weight:900;flex:1;letter-spacing:-0.03em;
  color:var(--accent);
}
.top-ver {
  font-size:0.55rem;font-weight:800;margin-left:5px;
  color:var(--bg);background:var(--accent);
  padding:2px 7px;border-radius:8px;vertical-align:middle;letter-spacing:0.04em;
}
.top-icon {
  width:36px;height:36px;border-radius:50%;
  background:rgba(255,255,255,0.70);
  border:1px solid var(--border);
  backdrop-filter:blur(8px);
  cursor:pointer;font-size:1rem;
  display:flex;align-items:center;justify-content:center;
  color:var(--text);transition:background 0.15s;
}
[data-theme="dark"] .top-icon {background:rgba(255,255,255,0.08);}
.top-icon:active {background:rgba(255,255,255,0.9);}
.content {flex:1;overflow-y:auto;padding:0 16px 90px;position:relative;z-index:1;}
.content > * {animation:pageEnter 0.4s cubic-bezier(0.16,1,0.3,1) both;}
.bot-nav {
  position:fixed;bottom:0;left:0;right:0;
  background:rgba(255,255,255,0.75);
  backdrop-filter:blur(24px) saturate(180%);
  -webkit-backdrop-filter:blur(24px) saturate(180%);
  display:flex;
  border-top:1px solid var(--border);
  z-index:50;
  padding-bottom:env(safe-area-inset-bottom);
}
[data-theme="dark"] .bot-nav {background:rgba(18,22,28,0.92);}
[data-theme="gold"] .bot-nav {background:rgba(250,240,220,0.88);}
[data-theme="ocean"] .bot-nav {background:rgba(230,245,255,0.88);}
[data-theme="rose"] .bot-nav {background:rgba(250,238,245,0.88);}
.nb {
  flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;
  padding:10px 2px 8px;border:none;background:none;
  color:var(--text);opacity:0.40;cursor:pointer;
  font-family:Outfit,sans-serif;transition:opacity 0.18s,transform 0.15s;
}
[data-theme="dark"] .nb {color:var(--navtext);}
.nb.active {opacity:1;}
.nb.active .nb-ico {transform:scale(1.12);}
.nb-ico {font-size:1.15rem;margin-bottom:2px;transition:transform 0.15s;}
.nb-lbl {font-size:0.44rem;font-weight:700;letter-spacing:0.05em;text-transform:uppercase;}
.card {
  background:var(--card);
  backdrop-filter:blur(20px) saturate(160%);
  -webkit-backdrop-filter:blur(20px) saturate(160%);
  border:1px solid var(--border);
  border-radius:var(--radius);padding:18px;margin-bottom:12px;
  box-shadow:0 4px 24px rgba(0,0,0,0.25), 0 1px 0 rgba(255,255,255,0.07) inset;
}
.card-title {
  font-size:0.65rem;font-weight:700;letter-spacing:0.12em;text-transform:uppercase;
  color:var(--dim);margin-bottom:14px;
}
.stat-grid {display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px;}
.stat-card {
  background:var(--card);
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:16px;padding:16px;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
  cursor:pointer;transition:transform 0.15s,box-shadow 0.15s;
}
.stat-card:active {transform:scale(0.97);}
.stat-card.full {grid-column:1/-1;}
.stat-label {
  font-size:0.62rem;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;
  color:var(--dim);margin-bottom:6px;
}
.stat-val {font-size:1.2rem;font-weight:800;color:var(--accent);}
.stat-val.red {color:var(--danger);}
.stat-val.gold {color:var(--gold);}
.tx-item {
  display:flex;align-items:center;gap:12px;padding:13px 0;
  border-bottom:1px solid rgba(255,255,255,0.06);
  transition:opacity 0.15s;
}
.tx-item:last-child {border-bottom:none;}
.tx-ico {
  width:40px;height:40px;border-radius:14px;
  background:var(--inp);
  border:1px solid var(--border);
  backdrop-filter:blur(8px);
  display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0;
}
.tx-info {flex:1;min-width:0;}
.tx-name {font-weight:600;font-size:0.88rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--text);}
.tx-date {font-size:0.67rem;color:var(--dim);margin-top:2px;}
.tx-right {display:flex;align-items:center;gap:6px;flex-shrink:0;}
.tx-amt {font-weight:800;font-size:0.9rem;font-family:JetBrains Mono,monospace;}
.ing {color:var(--accent2);}
.gas {color:var(--danger);}
.ic-btn {background:none;border:none;cursor:pointer;font-size:0.95rem;padding:4px;opacity:0.5;color:var(--text);}
.ic-btn:active {opacity:1;}
.mod-list {display:flex;flex-direction:column;gap:8px;}
.mod-item {
  display:flex;align-items:center;gap:14px;padding:15px 16px;
  background:var(--card);
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:18px;cursor:pointer;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
  transition:transform 0.15s,opacity 0.15s;
}
.mod-item:active {transform:scale(0.98);opacity:0.9;}
.mod-icon {
  font-size:1.4rem;width:44px;height:44px;
  background:linear-gradient(135deg,var(--inp),rgba(255,255,255,0.04));
  border:1px solid var(--border);
  border-radius:13px;display:flex;align-items:center;justify-content:center;flex-shrink:0;
}
.mod-label {font-weight:700;font-size:0.9rem;color:var(--text);}
.mod-sub {font-size:0.7rem;color:var(--dim);margin-top:2px;}
.mod-arrow {margin-left:auto;color:var(--dim);font-size:0.9rem;opacity:0.5;}
.inp {
  width:100%;padding:13px 14px;
  background:var(--inp);
  backdrop-filter:blur(8px);
  border:1px solid var(--border);
  border-radius:13px;
  font-family:Outfit,sans-serif;font-size:0.92rem;color:var(--text);
  outline:none;box-sizing:border-box;
  transition:border-color 0.2s,background 0.2s;
}
.inp::placeholder {color:var(--dim);}
.inp:focus {border-color:var(--accent);background:rgba(255,255,255,0.1);}
textarea.inp {resize:vertical;}
.form-row {display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.btn-sec {
  width:100%;padding:14px;
  background:var(--inp);
  border:1px solid var(--border);
  border-radius:13px;
  font-family:Outfit,sans-serif;font-size:0.88rem;font-weight:700;
  color:var(--accent);cursor:pointer;margin-bottom:8px;
  backdrop-filter:blur(8px);
  transition:background 0.15s;
}
.btn-sec:active {background:rgba(255,255,255,0.1);}
.btn-main {
  width:100%;padding:14px;
  background:var(--accent);
  border:none;
  border-radius:13px;
  font-family:Outfit,sans-serif;font-size:0.88rem;font-weight:700;
  color:#fff;cursor:pointer;margin-bottom:8px;
  box-shadow:0 2px 12px var(--glow);
  transition:background 0.15s,transform 0.1s;
}
.btn-main:active { transform:scale(0.98); background:var(--accent2); }

.back-btn {background:none;border:none;font-size:1.4rem;cursor:pointer;color:var(--text);padding:0 10px 0 0;line-height:1;opacity:0.8;}
.page-header {display:flex;align-items:center;margin-bottom:20px;padding-top:4px;}
.page-title {font-size:1.05rem;font-weight:800;color:var(--text);}
.prog-wrap {background:rgba(255,255,255,0.07);border:1px solid var(--border);border-radius:8px;height:7px;overflow:hidden;margin:8px 0;}
.prog-bar {height:100%;background:linear-gradient(90deg,var(--accent),var(--accent2));border-radius:8px;transition:width 0.5s cubic-bezier(0.4,0,0.2,1);}
.cred-item {
  background:var(--card);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:18px;padding:16px;margin-bottom:10px;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
}
.cred-top {display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:10px;}
.cred-persona {font-weight:800;font-size:0.92rem;color:var(--text);}
.cred-desc {font-size:0.7rem;color:var(--dim);margin-top:2px;}
.cred-badge {font-size:0.63rem;padding:4px 10px;border-radius:20px;font-weight:700;letter-spacing:0.03em;}
.badge-pend {background:rgba(255,152,0,0.15);color:#ffb340;border:1px solid rgba(255,152,0,0.2);}
.badge-pagado {background:rgba(43,192,112,0.15);color:var(--accent2);border:1px solid rgba(43,192,112,0.2);}
.badge-vencido {background:rgba(255,95,87,0.15);color:var(--danger);border:1px solid rgba(255,95,87,0.2);}
.cred-btns {display:flex;gap:6px;margin-top:10px;}
.cred-btn {
  flex:1;padding:9px 6px;border-radius:12px;
  border:1px solid var(--border);background:var(--inp);
  backdrop-filter:blur(8px);
  font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;
  cursor:pointer;color:var(--accent);transition:background 0.15s;
}
.cred-btn:active {background:rgba(255,255,255,0.1);}
.cred-btn.danger {color:var(--danger);border-color:rgba(255,95,87,0.2);}
.cred-btn.success {color:var(--accent2);border-color:rgba(43,192,112,0.2);}
.modal {display:none;position:fixed;inset:0;z-index:100;background:rgba(0,0,0,0.55);backdrop-filter:blur(8px);align-items:flex-end;}
.modal.open {display:flex;}
.modal-box {
  background:rgba(245,250,247,0.96);
  backdrop-filter:blur(32px) saturate(180%);
  -webkit-backdrop-filter:blur(32px) saturate(180%);
  border:1px solid var(--border);
  border-top:1px solid rgba(255,255,255,0.8);
  border-radius:28px 28px 0 0;
  padding:20px 20px 36px;
  width:100%;max-height:90vh;overflow-y:auto;
  box-shadow:0 -8px 40px rgba(0,0,0,0.18);
  color:var(--text);
}
[data-theme="dark"] .modal-box {background:rgba(28,34,42,0.96);border-top-color:rgba(255,255,255,0.08);}
[data-theme="gold"] .modal-box {background:rgba(253,248,235,0.96);}
[data-theme="ocean"] .modal-box {background:rgba(237,248,254,0.96);}
[data-theme="rose"] .modal-box {background:rgba(253,242,247,0.96);}
.modal-box::before {content:'';display:block;width:36px;height:4px;background:rgba(255,255,255,0.2);border-radius:2px;margin:0 auto 18px;}
.modal-header {display:flex;justify-content:space-between;align-items:center;margin-bottom:18px;}
.modal-title {font-size:1rem;font-weight:800;color:var(--text);}
.modal-close {
  background:rgba(255,255,255,0.1);border:none;
  width:32px;height:32px;border-radius:50%;
  font-size:1.1rem;cursor:pointer;color:var(--dim);
  display:flex;align-items:center;justify-content:center;
  transition:background 0.15s;
}
.modal-close:active {background:rgba(255,255,255,0.2);}
.tipo-selector {display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:16px;}
.tipo-opt {
  padding:12px;border-radius:14px;
  border:1px solid var(--border);background:var(--inp);
  text-align:center;cursor:pointer;font-weight:700;font-size:0.88rem;
  color:var(--dim);transition:all 0.15s;
}
.tipo-opt.selected {border-color:var(--accent);background:rgba(43,192,112,0.1);color:var(--accent);}
.toast {
  position:fixed;top:20px;left:50%;transform:translateX(-50%);
  background:rgba(30,50,35,0.9);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid rgba(43,192,112,0.25);
  color:#fff;padding:10px 20px;border-radius:22px;font-size:0.82rem;font-weight:600;
  z-index:999;white-space:nowrap;
  box-shadow:0 8px 28px rgba(0,0,0,0.4);
  animation:toastIn 0.3s cubic-bezier(0.16,1,0.3,1);
}
@keyframes toastIn {from{opacity:0;transform:translateX(-50%) translateY(-10px);}to{opacity:1;transform:translateX(-50%) translateY(0);}}
.hero-card {
  border-radius:28px;
  background:linear-gradient(145deg,var(--accent) 0%,var(--accent2) 100%);
  padding:24px 22px 20px;
  margin-bottom:16px;
  position:relative;overflow:hidden;
  box-shadow:0 12px 40px var(--glow);
}
.hero-card::before {
  content:'';position:absolute;
  top:-40px;right:-40px;
  width:160px;height:160px;
  border-radius:50%;
  background:rgba(255,255,255,0.1);
}
.hero-card::after {
  content:'';position:absolute;
  bottom:-30px;right:30px;
  width:100px;height:100px;
  border-radius:50%;
  background:rgba(255,255,255,0.06);
}
.hero-label {font-size:0.62rem;font-weight:700;letter-spacing:0.14em;text-transform:uppercase;color:rgba(255,255,255,0.7);margin-bottom:6px;}
.hero-amount {font-size:2.4rem;font-weight:900;color:#fff;letter-spacing:-0.04em;line-height:1;margin-bottom:4px;font-family:Outfit,sans-serif;}
.hero-sub {font-size:0.75rem;color:rgba(255,255,255,0.65);margin-bottom:20px;}
.hero-pills {display:flex;gap:8px;flex-wrap:wrap;position:relative;z-index:1;}
.hero-pill {
  display:flex;align-items:center;gap:5px;
  background:rgba(0,0,0,0.2);
  border:1px solid rgba(255,255,255,0.15);
  backdrop-filter:blur(8px);
  border-radius:20px;padding:6px 12px;
  font-size:0.72rem;font-weight:700;color:#fff;
  cursor:pointer;transition:background 0.15s;
}
.hero-pill:active {background:rgba(0,0,0,0.35);}
.hero-pill-ico {font-size:0.9rem;}
.quick-grid {display:grid;grid-template-columns:repeat(5,1fr);gap:8px;margin-bottom:16px;}
.quick-item {
  display:flex;flex-direction:column;align-items:center;gap:7px;
  cursor:pointer;transition:transform 0.15s;
}
.quick-item:active {transform:scale(0.93);}
.quick-ico {
  width:54px;height:54px;border-radius:18px;
  background:var(--card);
  backdrop-filter:blur(20px);
  border:1px solid var(--border);
  display:flex;align-items:center;justify-content:center;
  font-size:1.4rem;
  box-shadow:0 4px 16px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.07) inset;
}
.quick-lbl {font-size:0.58rem;font-weight:700;color:var(--dim);text-align:center;letter-spacing:0.02em;line-height:1.2;}
.sec-title {
  font-size:0.62rem;font-weight:800;letter-spacing:0.12em;text-transform:uppercase;
  color:var(--dim);margin:20px 0 10px;display:flex;align-items:center;gap:8px;
}
.sec-title::after {content:'';flex:1;height:1px;background:var(--border);}
.insight-row {display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:10px;}
.insight-card {
  background:var(--card);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:20px;padding:16px 14px;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
  cursor:pointer;transition:transform 0.15s;position:relative;overflow:hidden;
}
.insight-card:active {transform:scale(0.97);}
.insight-card.full {grid-column:1/-1;}
.insight-card.accent {
  background:linear-gradient(135deg,rgba(43,192,112,0.15),rgba(43,192,112,0.06));
  border-color:rgba(43,192,112,0.25);
}
.insight-card.danger {
  background:linear-gradient(135deg,rgba(255,95,87,0.12),rgba(255,95,87,0.04));
  border-color:rgba(255,95,87,0.2);
}
.insight-card.gold {
  background:linear-gradient(135deg,rgba(255,179,64,0.12),rgba(255,179,64,0.04));
  border-color:rgba(255,179,64,0.2);
}
.insight-ico {font-size:1.3rem;margin-bottom:10px;display:block;}
.insight-label {font-size:0.6rem;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:var(--dim);margin-bottom:4px;}
.insight-val {font-size:1.1rem;font-weight:900;color:var(--text);font-family:Outfit,sans-serif;line-height:1.1;}
.insight-trend {font-size:0.65rem;font-weight:600;margin-top:5px;display:flex;align-items:center;gap:3px;}
.insight-badge-abs {
  position:absolute;top:12px;right:12px;
  background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.08);
  border-radius:20px;padding:3px 8px;
  font-size:0.6rem;font-weight:700;color:var(--dim);
}
.tx-feed-header {display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;}
.tx-feed-title {font-size:0.9rem;font-weight:800;color:var(--text);}
.tx-feed-link {font-size:0.72rem;color:var(--accent);font-weight:600;cursor:pointer;}
.cuenta-card {
  background:var(--card);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:20px;padding:18px;margin-bottom:10px;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
}
.cuenta-card-header {display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:14px;}
.cuenta-card-ico {
  width:44px;height:44px;border-radius:14px;
  display:flex;align-items:center;justify-content:center;font-size:1.3rem;
  border:1px solid var(--border);
}
.cuenta-card-badge {font-size:0.62rem;font-weight:700;padding:4px 10px;border-radius:20px;letter-spacing:0.04em;}
.cuenta-saldo {font-size:1.8rem;font-weight:900;color:var(--text);letter-spacing:-0.03em;margin-bottom:4px;}
.cuenta-label {font-size:0.68rem;color:var(--dim);font-weight:600;}
.cuenta-actions {display:flex;gap:7px;margin-top:14px;}
.cuenta-btn {
  flex:1;padding:10px 6px;border-radius:12px;
  background:var(--inp);border:1px solid var(--border);
  font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;
  color:var(--text);cursor:pointer;transition:background 0.15s;
  backdrop-filter:blur(8px);
}
.cuenta-btn:active {background:rgba(255,255,255,0.15);}
.cuenta-btn.primary {background:var(--accent);border-color:var(--accent);color:#fff;box-shadow:0 2px 12px var(--glow);}
.cuenta-btn.primary:active {filter:brightness(0.9);}
.bar-chart {display:flex;align-items:flex-end;gap:6px;height:90px;margin:12px 0;}
.bar-col {flex:1;display:flex;flex-direction:column;align-items:center;gap:5px;}
.bar-fill {
  width:100%;border-radius:8px 8px 4px 4px;
  background:var(--accent);min-height:4px;
  transition:height 0.6s cubic-bezier(0.16,1,0.3,1);
  position:relative;overflow:hidden;
}
.bar-fill::after {content:'';position:absolute;inset:0;background:linear-gradient(to bottom,rgba(255,255,255,0.15),transparent);}
.bar-fill.danger {background:var(--danger);}
.bar-lbl {font-size:0.55rem;color:var(--dim);font-weight:600;text-align:center;}
.profile-header {
  background:var(--card);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid var(--border);
  border-radius:24px;padding:20px;margin-bottom:16px;
  display:flex;align-items:center;gap:14px;
  box-shadow:0 4px 20px rgba(0,0,0,0.2),0 1px 0 rgba(255,255,255,0.06) inset;
}
.profile-avatar {
  width:56px;height:56px;border-radius:18px;flex-shrink:0;
  background:linear-gradient(135deg,var(--accent),var(--accent2));
  display:flex;align-items:center;justify-content:center;
  font-size:1.5rem;font-weight:900;color:#fff;
  box-shadow:0 4px 16px var(--glow);
  border:1.5px solid rgba(255,255,255,0.2);
}
.profile-name {font-size:1rem;font-weight:800;color:var(--text);margin-bottom:2px;}
.profile-role {font-size:0.68rem;color:var(--dim);font-weight:600;}
.profile-badge {
  margin-left:auto;padding:5px 12px;border-radius:20px;font-size:0.62rem;font-weight:800;
  letter-spacing:0.06em;text-transform:uppercase;
  background:rgba(43,192,112,0.15);color:var(--accent2);
  border:1px solid rgba(43,192,112,0.2);
}
.mod-section {margin-bottom:20px;}
.mod-section-title {
  font-size:0.6rem;font-weight:800;letter-spacing:0.14em;text-transform:uppercase;
  color:var(--dim);margin-bottom:8px;padding-left:2px;
}
.noticia-banner {
  background:linear-gradient(135deg,rgba(43,192,112,0.15),rgba(43,192,112,0.06));
  border:1px solid rgba(43,192,112,0.25);
  backdrop-filter:blur(12px);
  border-radius:20px;padding:14px 16px;margin-bottom:14px;cursor:pointer;
  box-shadow:0 4px 16px rgba(43,192,112,0.1);
  transition:transform 0.15s;
}
.noticia-banner:active {transform:scale(0.98);}
@keyframes gradShift {0%{background-position:0% 50%;}50%{background-position:100% 50%;}100%{background-position:0% 50%;}}
@keyframes float1 {0%,100%{transform:translateY(0) scale(1);}50%{transform:translateY(-12px) scale(1.05);}}
@keyframes float2 {0%,100%{transform:translateY(0) rotate(0deg);}50%{transform:translateY(-8px) rotate(8deg);}}
@keyframes popIn {0%{transform:scale(0) rotate(-15deg);opacity:0;}70%{transform:scale(1.2) rotate(5deg);}100%{transform:scale(1) rotate(0deg);opacity:1;}}
@keyframes slideUp {from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
@keyframes fadeIn {from{opacity:0;}to{opacity:1;}}
@keyframes pageEnter {from{opacity:0;transform:translateY(12px);}to{opacity:1;transform:translateY(0);}}
.pp-overlay {
  position:fixed;inset:0;
  background:rgba(0,0,0,0.55);backdrop-filter:blur(8px);
  z-index:8000;display:flex;align-items:flex-end;justify-content:center;
  animation:fadeIn 0.18s;
}
.pp-panel {
  background:rgba(245,250,247,0.97);
  backdrop-filter:blur(32px) saturate(180%);
  -webkit-backdrop-filter:blur(32px) saturate(180%);
  border:1px solid var(--border);
  border-top:1px solid rgba(255,255,255,0.8);
  border-radius:28px 28px 0 0;
  width:100%;max-width:520px;max-height:90vh;
  display:flex;flex-direction:column;
  animation:slideUp 0.28s cubic-bezier(.4,0,.2,1);
  box-shadow:0 -8px 40px rgba(0,0,0,0.15);
}
[data-theme="dark"] .pp-panel {background:rgba(28,34,42,0.97);}
[data-theme="gold"] .pp-panel {background:rgba(253,248,235,0.97);}
[data-theme="ocean"] .pp-panel {background:rgba(237,248,254,0.97);}
[data-theme="rose"] .pp-panel {background:rgba(253,242,247,0.97);}
.pp-handle {width:36px;height:4px;background:rgba(255,255,255,0.2);border-radius:99px;margin:12px auto 0;}
.pp-head {padding:16px 18px 0;}
.pp-title {font-size:1.05rem;font-weight:900;margin-bottom:2px;color:var(--text);}
.pp-subtitle {font-size:0.72rem;color:var(--dim);margin-bottom:12px;}
.pp-tab {
  padding:6px 14px;border-radius:20px;
  border:1px solid var(--border);background:var(--inp);
  font-family:Outfit,sans-serif;font-size:0.76rem;font-weight:700;
  cursor:pointer;white-space:nowrap;color:var(--dim);transition:all 0.15s;
}
.pp-tab.active {background:var(--accent);border-color:var(--accent);color:#fff;}
.pp-body {flex:1;overflow-y:auto;padding:0 18px 32px;}
.pp-empty {text-align:center;padding:32px 20px;color:var(--dim);font-size:0.82rem;}
.pp-item {display:flex;align-items:center;gap:12px;padding:13px 0;border-bottom:1px solid rgba(255,255,255,0.06);}
.pp-item:last-child {border-bottom:none;}
.pp-ico {width:40px;height:40px;border-radius:13px;background:var(--inp);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0;}
.pp-info {flex:1;min-width:0;}
.pp-name {font-weight:700;font-size:0.88rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--text);}
.pp-when {font-size:0.68rem;color:var(--dim);margin-top:2px;}
.pp-amt {font-weight:900;font-size:0.92rem;font-family:JetBrains Mono,monospace;flex-shrink:0;}
.pp-section-title {font-size:0.62rem;font-weight:800;text-transform:uppercase;letter-spacing:0.09em;color:var(--dim);padding:12px 0 6px;}
.pp-btn-abrir {
  display:flex;flex-direction:column;align-items:center;justify-content:center;
  background:var(--card);border:1px solid var(--border);
  backdrop-filter:blur(12px);
  border-radius:16px;padding:14px 10px;cursor:pointer;gap:2px;transition:all 0.15s;
}
.pp-btn-abrir:active {transform:scale(0.96);}
.lock-screen {
  position:fixed;inset:0;z-index:99999;
  display:flex;flex-direction:column;align-items:center;justify-content:center;
  background:linear-gradient(145deg,var(--bg) 0%,var(--bg2) 100%);
  animation:fadeIn 0.3s;
}
.lock-screen::before {
  content:'';position:absolute;inset:0;pointer-events:none;
  background:
    radial-gradient(ellipse 60% 50% at 20% 20%, var(--orb1) 0%, transparent 60%),
    radial-gradient(ellipse 50% 60% at 80% 75%, var(--orb2) 0%, transparent 60%);
}
.lock-card {
  background:rgba(255,255,255,0.07);
  backdrop-filter:blur(32px) saturate(180%);
  -webkit-backdrop-filter:blur(32px) saturate(180%);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:28px;padding:32px 28px;
  width:90%;max-width:340px;
  box-shadow:0 16px 48px rgba(0,0,0,0.4),0 1px 0 rgba(255,255,255,0.1) inset;
  text-align:center;position:relative;z-index:1;
}
.lock-avatar {
  width:76px;height:76px;border-radius:50%;
  background:linear-gradient(135deg,var(--accent),var(--accent2));
  display:flex;align-items:center;justify-content:center;font-size:2rem;
  margin:0 auto 14px;
  border:1.5px solid rgba(255,255,255,0.2);
  box-shadow:0 8px 32px var(--glow);
}
.lock-nombre {font-size:1.1rem;font-weight:900;margin-bottom:4px;color:var(--text);}
.lock-sub {font-size:0.75rem;color:var(--dim);margin-bottom:22px;}
.lock-dots {display:flex;justify-content:center;gap:14px;margin-bottom:20px;}
.lock-dot {
  width:15px;height:15px;border-radius:50%;
  border:2px solid rgba(255,255,255,0.2);background:transparent;
  transition:all 0.2s cubic-bezier(0.34,1.56,0.64,1);
}
.lock-dot.filled {
  background:linear-gradient(135deg,var(--accent),var(--accent2));
  border-color:transparent;
  box-shadow:0 0 10px var(--glow);transform:scale(1.2);
}
.lock-dot.error {background:var(--danger);border-color:transparent;}
.lock-pad {display:grid;grid-template-columns:repeat(3,1fr);gap:10px;max-width:240px;margin:0 auto;}
.lock-key {
  height:52px;border-radius:14px;
  border:1px solid rgba(255,255,255,0.08);
  background:rgba(255,255,255,0.07);
  backdrop-filter:blur(8px);
  font-family:Outfit,sans-serif;font-size:1.2rem;font-weight:500;
  cursor:pointer;color:var(--text);transition:all 0.1s;
  touch-action:manipulation;
}
.lock-key:active {transform:scale(0.92);background:rgba(43,192,112,0.25);color:#fff;}
.lock-key.del {font-size:1rem;color:var(--dim);}
.lock-timeout-badge {
  display:inline-block;font-size:0.65rem;font-weight:800;
  padding:4px 12px;border-radius:20px;
  background:rgba(255,255,255,0.1);border:1px solid var(--border);
  color:var(--dim);margin-bottom:16px;letter-spacing:0.04em;
}
.ayuda-chip {
  flex-shrink:0;border:1px solid var(--border);border-radius:22px;
  padding:7px 15px;font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;
  background:var(--inp);backdrop-filter:blur(8px);
  color:var(--dim);cursor:pointer;transition:all 0.15s;
}
.ayuda-chip.active,.ayuda-chip:active {
  background:var(--accent);color:#fff;border-color:var(--accent);
  box-shadow:0 2px 12px var(--glow);
}
.cat-add-btn {
  display:inline-flex;align-items:center;gap:4px;padding:6px 12px;
  border-radius:20px;border:1px dashed var(--accent);
  background:rgba(43,192,112,0.05);color:var(--accent);
  font-family:Outfit,sans-serif;font-size:0.74rem;font-weight:700;
  cursor:pointer;margin-top:5px;transition:all 0.18s;
}
.cat-add-btn:active {background:rgba(43,192,112,0.15);}
.cat-modal-overlay {position:fixed;inset:0;background:rgba(0,0,0,0.55);backdrop-filter:blur(8px);z-index:10000;display:flex;align-items:flex-end;justify-content:center;animation:fadeIn 0.15s;}
.cat-modal-box {
  background:rgba(245,250,247,0.97);
  backdrop-filter:blur(32px) saturate(180%);
  -webkit-backdrop-filter:blur(32px) saturate(180%);
  border:1px solid var(--border);border-top:1px solid rgba(255,255,255,0.8);
  border-radius:28px 28px 0 0;padding:20px 18px 36px;
  width:100%;max-width:480px;
  animation:slideUp 0.25s cubic-bezier(.4,0,.2,1);
  box-shadow:0 -8px 40px rgba(0,0,0,0.15);
  color:var(--text);
}
[data-theme="dark"] .cat-modal-box {background:rgba(28,34,42,0.97);}
[data-theme="gold"] .cat-modal-box {background:rgba(253,248,235,0.97);}
[data-theme="ocean"] .cat-modal-box {background:rgba(237,248,254,0.97);}
[data-theme="rose"] .cat-modal-box {background:rgba(253,242,247,0.97);}
.cat-modal-title {font-size:1rem;font-weight:900;margin-bottom:4px;color:var(--text);}
.cat-modal-sub {font-size:0.75rem;color:var(--dim);margin-bottom:14px;}
.cat-chips-wrap {display:flex;flex-wrap:wrap;gap:6px;margin-bottom:14px;max-height:160px;overflow-y:auto;}
.cat-chip {
  display:inline-flex;align-items:center;gap:5px;padding:5px 12px;
  border-radius:20px;border:1px solid var(--border);
  background:var(--inp);font-size:0.78rem;font-weight:600;color:var(--text);
}
.cat-chip .del-chip {background:none;border:none;cursor:pointer;color:var(--dim);font-size:0.8rem;padding:0;line-height:1;}
.cat-chip .del-chip:active {color:var(--danger);}
.cat-new-row {display:flex;gap:8px;align-items:center;}
.cat-new-inp {
  flex:1;padding:10px 12px;border-radius:12px;
  border:1px solid var(--border);background:var(--inp);
  backdrop-filter:blur(8px);color:var(--text);
  font-family:Outfit,sans-serif;font-size:0.85rem;outline:none;
}
.cat-new-inp:focus {border-color:var(--accent);}
.cat-save-btn {
  padding:10px 16px;border-radius:12px;border:none;
  background:var(--accent);color:#fff;
  font-family:Outfit,sans-serif;font-weight:700;font-size:0.85rem;
  cursor:pointer;white-space:nowrap;
  box-shadow:0 2px 12px var(--glow);
}
.undo-bar {
  position:fixed;bottom:86px;left:10px;right:10px;
  background:rgba(20,50,30,0.95);
  backdrop-filter:blur(24px) saturate(180%);
  -webkit-backdrop-filter:blur(24px) saturate(180%);
  border:1px solid rgba(255,255,255,0.15);
  color:#fff;padding:14px 16px;border-radius:18px;
  font-size:0.84rem;font-weight:600;
  z-index:9999;display:flex;flex-direction:column;gap:8px;
  box-shadow:0 8px 32px rgba(0,0,0,0.35);
  animation:undoSlideIn 0.25s cubic-bezier(.4,0,.2,1);
}
[data-theme="dark"] .undo-bar {background:rgba(18,24,32,0.97);}
[data-theme="gold"] .undo-bar {background:rgba(40,20,0,0.96);}
[data-theme="ocean"] .undo-bar {background:rgba(5,25,60,0.96);}
[data-theme="rose"] .undo-bar {background:rgba(40,0,20,0.96);}
.undo-btn {
  background:var(--accent);border:none;color:#fff;
  padding:7px 16px;border-radius:10px;
  font-family:Outfit,sans-serif;font-weight:700;cursor:pointer;font-size:0.8rem;
  box-shadow:0 2px 12px var(--glow);
}
.undo-prog {position:absolute;bottom:0;left:0;height:3px;background:var(--accent);border-radius:0 0 18px 18px;transition:width 7s linear;width:100%;opacity:0.7;}
.danger-zone {
  border:1px solid rgba(255,95,87,0.2);
  background:rgba(255,95,87,0.04);
  backdrop-filter:blur(8px);
  border-radius:16px;padding:16px;margin-top:12px;
}
.danger-title {font-size:0.75rem;font-weight:700;color:var(--danger);margin-bottom:12px;letter-spacing:0.06em;text-transform:uppercase;}
.danger-btn {
  width:100%;padding:12px;
  background:rgba(255,95,87,0.08);border:1px solid rgba(255,95,87,0.18);
  border-radius:12px;color:var(--danger);
  font-family:Outfit,sans-serif;font-size:0.82rem;font-weight:600;
  cursor:pointer;margin-bottom:8px;text-align:left;
  transition:background 0.15s;
}
.danger-btn:active {background:rgba(255,95,87,0.16);}
.danger-btn:last-child {margin-bottom:0;}
.chip {
  display:inline-flex;align-items:center;gap:4px;padding:4px 10px;
  border-radius:20px;font-size:0.68rem;font-weight:700;
  backdrop-filter:blur(8px);border:1px solid rgba(255,255,255,0.08);
}
.set-item {
  display:flex;align-items:center;justify-content:space-between;
  padding:15px 0;border-bottom:1px solid rgba(255,255,255,0.06);
  transition:opacity 0.15s;
}
.set-item:last-child {border-bottom:none;}
.set-item:active {opacity:0.75;}
.set-label {font-weight:600;font-size:0.88rem;color:var(--text);}
.set-sub {font-size:0.7rem;color:var(--dim);margin-top:2px;}
.set-arrow {color:var(--dim);font-size:0.85rem;opacity:0.5;}
.pres-item {display:flex;align-items:center;gap:10px;padding:13px 0;border-bottom:1px solid rgba(255,255,255,0.06);}
.pres-item:last-child {border-bottom:none;}
.ck {padding:16px 6px;border:none;background:rgba(255,255,255,0.08);color:#fff;font-family:Outfit,sans-serif;font-size:1.15rem;font-weight:600;cursor:pointer;transition:background 0.1s,transform 0.08s;-webkit-tap-highlight-color:transparent;border-radius:4px;}
.ck:active {background:rgba(255,255,255,0.22);transform:scale(0.93);}
.ck-fn {background:rgba(160,174,200,0.15);color:#a0aec8;font-size:0.95rem;font-weight:700;}
.ck-fn:active {background:rgba(160,174,200,0.3);}
.ck-op {background:rgba(255,159,10,0.18);color:#ffb347;font-size:1.2rem;font-weight:700;}
.ck-op:active {background:rgba(255,159,10,0.4);}
.ck-eq {background:linear-gradient(135deg,#ff9f0a,#ff6b00);color:#fff;font-size:1.25rem;font-weight:800;border-radius:4px;}
.ck-eq:active {filter:brightness(0.85);}
.ck-del {background:rgba(255,80,80,0.15);color:#ff6b6b;font-size:1rem;}
.ck-del:active {background:rgba(255,80,80,0.35);}
50% {transform:scaleY(1.8);}
}
.page-header + .sec-title { margin-top: 0; }
@media (hover: hover) {
  .insight-card:hover { transform: translateY(-2px); box-shadow: 0 8px 32px rgba(0,0,0,0.3); }
  .mod-item:hover { transform: translateY(-1px); }
  .quick-item:hover .quick-ico { transform: scale(1.06); }
}
#themePicker .content-wrap { width: 100%; max-width: 400px; }
#calcWidget {
  border-radius: 24px !important;
}
.pp-tabs::-webkit-scrollbar { display: none; }
.pp-tabs { -ms-overflow-style: none; scrollbar-width: none; }
.cred-item { transition: transform 0.15s, opacity 0.15s; }
.cred-item:active { transform: scale(0.99); opacity: 0.9; }
.hero-pill + .hero-pill { }
.top-ver {
  font-size: 0.5rem !important;
  padding: 2px 6px !important;
  border-radius: 6px !important;
  letter-spacing: 0.06em !important;
}
.mod-item:last-child { }
.toast { top: env(safe-area-inset-top, 20px); margin-top: 8px; }
.consejero-card {
  border-radius:24px;
  background:var(--card);
  backdrop-filter:blur(20px) saturate(160%);
  -webkit-backdrop-filter:blur(20px) saturate(160%);
  border:1px solid var(--border);
  padding:16px;
  margin-bottom:14px;
  display:flex;align-items:flex-start;gap:14px;
  position:relative;overflow:hidden;
  box-shadow:0 4px 24px rgba(0,0,0,0.12);
  cursor:pointer;
  transition:transform 0.15s;
}
.consejero-card:active {transform:scale(0.98);}
.consejero-avatar svg {width:64px;height:64px;}
.consejero-body {flex:1;min-width:0;}
.consejero-titulo {
  font-size:0.7rem;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;
  color:var(--accent);margin-bottom:3px;
}
.consejero-estado {
  font-size:1rem;font-weight:800;color:var(--text);
  margin-bottom:5px;line-height:1.2;
}
.consejero-msg {
  font-size:0.8rem;color:var(--dim);line-height:1.45;
}
.consejero-chips {
  display:flex;flex-wrap:wrap;gap:6px;margin-top:10px;
}
.consejero-chip {
  font-size:0.7rem;font-weight:700;padding:4px 10px;border-radius:20px;
  display:flex;align-items:center;gap:4px;
}
.chip-verde {background:rgba(43,192,112,0.15);color:#1a8c4e;}
.chip-rojo {background:rgba(255,95,87,0.12);color:#cc2a2a;}
.chip-gold {background:rgba(192,122,16,0.12);color:#c07a10;}
.chip-azul {background:rgba(0,112,204,0.12);color:#0070cc;}
.salud-bar-wrap {
  height:6px;border-radius:3px;
  background:rgba(0,0,0,0.08);
  margin-top:10px;overflow:hidden;
}
.salud-bar-fill {
  height:100%;border-radius:3px;
  transition:width 1s cubic-bezier(0.16,1,0.3,1);
}
@keyframes consejeroFloat {
  0%{transform:translateY(0);}
  50%{transform:translateY(-4px);}
  100%{transform:translateY(0);}
}
.consejero-avatar {animation:consejeroFloat 3s ease-in-out infinite;}
.carrito-cat-grid {
  display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:16px;
}
.carrito-cat-btn {
  border-radius:14px;padding:10px 6px;border:2px solid transparent;
  background:var(--card);backdrop-filter:blur(12px);
  display:flex;flex-direction:column;align-items:center;gap:4px;
  cursor:pointer;transition:all 0.18s;font-family:Outfit,sans-serif;
  box-shadow:0 2px 10px rgba(0,0,0,0.08);
}
.carrito-cat-btn.activa {
  border-color:var(--accent);
  background:rgba(var(--accent-rgb,43,192,112),0.12);
}
.carrito-cat-ico {font-size:1.4rem;}
.carrito-cat-lbl {font-size:0.65rem;font-weight:700;color:var(--text);text-align:center;}
.carrito-item {
  display:flex;align-items:center;gap:10px;
  padding:12px 14px;border-radius:16px;
  background:var(--card);border:1px solid var(--border);
  margin-bottom:8px;transition:all 0.2s;
  box-shadow:0 2px 8px rgba(0,0,0,0.06);
  position:relative;overflow:hidden;
}
.carrito-item.comprado {opacity:0.55;}
.carrito-item.comprado .ci-nombre {text-decoration:line-through;}
.ci-check {
  width:26px;height:26px;border-radius:50%;border:2px solid var(--border);
  display:flex;align-items:center;justify-content:center;
  cursor:pointer;flex-shrink:0;transition:all 0.2s;font-size:0.9rem;
}
.ci-check.on {background:var(--accent);border-color:var(--accent);color:#fff;}
.ci-body {flex:1;min-width:0;}
.ci-nombre {font-size:0.88rem;font-weight:700;color:var(--text);white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.ci-meta {font-size:0.68rem;color:var(--dim);margin-top:1px;}
.ci-precio-hist {font-size:0.65rem;color:var(--accent);font-weight:600;margin-top:2px;}
.ci-right {display:flex;flex-direction:column;align-items:flex-end;gap:4px;flex-shrink:0;}
.ci-precio {font-size:0.9rem;font-weight:800;color:var(--text);}
.ci-qty {
  display:flex;align-items:center;gap:6px;
  background:var(--inp);border-radius:20px;padding:3px 10px;
}
.ci-qty button {background:none;border:none;font-size:1rem;cursor:pointer;color:var(--text);padding:0 2px;font-family:Outfit,sans-serif;}
.ci-qty span {font-size:0.8rem;font-weight:700;color:var(--text);min-width:16px;text-align:center;}
.carrito-total-bar {
  position:sticky;bottom:72px;
  background:var(--card);backdrop-filter:blur(20px);
  border:1px solid var(--border);border-radius:20px;
  padding:12px 16px;margin:10px 0;
  display:flex;justify-content:space-between;align-items:center;
  box-shadow:0 4px 20px rgba(0,0,0,0.15);
  z-index:10;transition:all 0.25s;
}
.carrito-total-bar.collapsed {
  padding:7px 14px;opacity:0.75;
}
.carrito-total-bar.collapsed .ctb-detalle {display:none;}
.hist-precio-row {
  display:flex;justify-content:space-between;align-items:center;
  padding:8px 0;border-bottom:1px solid var(--border);font-size:0.8rem;
}
.hist-precio-tienda {font-weight:700;color:var(--text);}
.hist-precio-val {font-weight:800;color:var(--accent);}
.hist-precio-fecha {font-size:0.65rem;color:var(--dim);}
</style>
</head>
<body>

<!-- ══ ACCESS SCREEN ══ -->
<div class="screen active" id="accessScreen">
<div class="lg-scroll-outer">
<div class="lg-wrap">

  <!-- Logo -->
  <div style="text-align:center;width:100%;">
    <div class="lg-logo">USALA</div>
    <div class="lg-sub">Finanzas Personales</div>
  </div>

  <!-- ── PANEL: Sesión recordada ── -->
  <div class="lg-card" id="panelSesion" style="display:none;">
    <div class="lg-avatar" id="sesionAvatar">👤</div>
    <div class="lg-greeting">Bienvenid@ de vuelta</div>
    <div class="lg-name" id="sesionNombre"></div>

    <!-- Con NIP -->
    <div id="nipZona" style="display:none;">
      <div style="font-size:0.75rem;color:rgba(255,255,255,0.45);text-align:center;margin-bottom:16px;letter-spacing:0.02em;">Ingresa tu NIP para continuar</div>
      <div class="nip-dots">
        <div class="nip-dot" id="nd1"></div>
        <div class="nip-dot" id="nd2"></div>
        <div class="nip-dot" id="nd3"></div>
        <div class="nip-dot" id="nd4"></div>
      </div>
      <div id="nipErr" style="display:none;font-size:0.75rem;color:#ff8a80;text-align:center;margin-bottom:12px;animation:lgShake 0.35s ease;">NIP incorrecto — intenta de nuevo</div>
      <div class="numpad" id="numpadNip">
        <button class="nk" onclick="nkPress(1)">1</button>
        <button class="nk" onclick="nkPress(2)">2</button>
        <button class="nk" onclick="nkPress(3)">3</button>
        <button class="nk" onclick="nkPress(4)">4</button>
        <button class="nk" onclick="nkPress(5)">5</button>
        <button class="nk" onclick="nkPress(6)">6</button>
        <button class="nk" onclick="nkPress(7)">7</button>
        <button class="nk" onclick="nkPress(8)">8</button>
        <button class="nk" onclick="nkPress(9)">9</button>
        <div class="nk nk-blank"></div>
        <button class="nk" onclick="nkPress(0)">0</button>
        <button class="nk nk-del" onclick="nkDel()">⌫</button>
      </div>
    </div>

    <!-- Sin NIP -->
    <div id="sinNipZona">
      <button class="lg-btn" onclick="entrarSesionGuardada()">Continuar →</button>
    </div>

    <button class="lg-btn-ghost" onclick="mostrarPanelCodigo(true)">No soy yo — usar otro código</button>
    <span class="lg-link" onclick="abrirAdminModal()">🔐 Acceso administrador</span>
  </div>

  <!-- ── PANEL: Código ── -->
  <div class="lg-card" id="panelCodigo" style="display:none;">

    <!-- Saludo cuando el código ya está registrado -->
    <div id="accSaludo" style="display:none;text-align:center;margin-bottom:20px;">
      <div class="lg-avatar" id="accSaludoAvatar" style="margin-bottom:10px;">👤</div>
      <div class="lg-greeting">¡Hola de nuevo!</div>
      <div class="lg-name" id="accSaludoNombre" style="margin-bottom:0;"></div>
    </div>

    <!-- Título cuando es primera vez -->
    <div id="accTituloZona" style="margin-bottom:20px;">
      <div style="font-size:1.15rem;font-weight:800;color:#fff;margin-bottom:4px;letter-spacing:-0.02em;" id="accTitulo">Ingresa tu código</div>
      <div style="font-size:0.78rem;color:rgba(255,255,255,0.4);" id="accSubtitulo">El administrador te lo compartió</div>
    </div>

    <div id="accessErr" class="lg-err"></div>

    <!-- Nombre (solo primera vez) -->
    <div id="accNombreRow">
      <div class="lg-section-title">Tu nombre</div>
      <input class="lg-inp" id="accNombre" placeholder="¿Cómo te llamas?" autocomplete="off">
    </div>

    <div class="lg-section-title">Código de acceso</div>
    <input class="lg-code-inp" id="accCodigo" placeholder="Ej: MARI-WTFX"
      autocomplete="off" autocapitalize="characters" spellcheck="false"
      oninput="this.value=this.value.toUpperCase();accCodigoLookup(this.value)"
      onkeydown="if(event.key==='Enter')verificarCodigo()">

    <!-- Contraseña personal (aparece si el usuario ya tiene una) -->
    <div id="accPassRow" style="display:none;">
      <div class="lg-section-title">Tu contraseña</div>
      <div style="position:relative;">
        <input class="lg-inp" id="accPassword" type="password" placeholder="Tu contraseña personal"
          autocomplete="current-password"
          onkeydown="if(event.key==='Enter')verificarCodigo()">
        <button onclick="toggleAccPass()" type="button"
          style="position:absolute;right:12px;top:50%;transform:translateY(-50%);background:none;border:none;cursor:pointer;font-size:1rem;color:rgba(255,255,255,0.4);"
          id="accPassEye">👁</button>
      </div>
      <div id="accPassOlvide" style="font-size:0.7rem;color:rgba(255,255,255,0.3);text-decoration:underline;cursor:pointer;margin-top:6px;text-align:right;" onclick="olvidarContraseña()">¿Olvidaste tu contraseña?</div>
    </div>

    <!-- Crear contraseña (primera vez) -->
    <div id="accCrearPassRow" style="display:none;">
      <div class="lg-section-title" style="color:rgba(43,192,112,0.9);">🔐 Crea tu contraseña personal</div>
      <div style="font-size:0.72rem;color:rgba(255,255,255,0.35);margin-bottom:10px;">Opcional — te permitirá entrar desde cualquier dispositivo de forma segura</div>
      <div style="position:relative;">
        <input class="lg-inp" id="accNuevaPass" type="password"
          placeholder="Mínimo 8 caracteres, mayúscula, símbolo..."
          oninput="renderPasswordStrength(this.value,'passStrengthBox')">
        <button onclick="toggleAccNuevaPass()" type="button"
          style="position:absolute;right:12px;top:50%;transform:translateY(-50%);background:none;border:none;cursor:pointer;font-size:1rem;color:rgba(255,255,255,0.4);">👁</button>
      </div>
      <!-- Indicador visual de fortaleza (6 reglas) -->
      <div id="passStrengthBox"></div>
      <button class="lg-btn-ghost" onclick="saltarCrearPass()" style="margin-top:8px;font-size:0.82rem;">Por ahora no →</button>
    </div>

    <button class="lg-btn" onclick="verificarCodigo()">Entrar →</button>

    <div class="lg-divider"><span>¿Sin código?</span></div>
    <button class="lg-dashed-btn" onclick="mostrarPanelSolicitud()">📩 Solicitar acceso</button>
    <span class="lg-link" onclick="abrirAdminModal()">🔐 Acceso administrador</span>
  </div>

  <!-- ── PANEL: Solicitar acceso ── -->
  <div class="lg-card" id="panelSolicitud" style="display:none;">
    <div style="font-size:1.1rem;font-weight:800;color:#fff;margin-bottom:4px;letter-spacing:-0.02em;">📩 Solicitar acceso</div>
    <div style="font-size:0.78rem;color:rgba(255,255,255,0.4);margin-bottom:20px;">El admin recibirá tu solicitud y te enviará un código</div>
    <div id="solicitudMsg" class="lg-err"></div>
    <div class="lg-section-title">Nombre completo</div>
    <input class="lg-inp" id="solNombre" placeholder="¿Cómo te llamas?" autocomplete="off">
    <div class="lg-section-title">¿Para qué usarás USALA?</div>
    <textarea class="lg-textarea" id="solMotivo" placeholder="Ej: Llevar control de mis gastos..." style="height:76px;"></textarea>
    <div class="lg-section-title">Tu WhatsApp o email</div>
    <input class="lg-inp" id="solContacto" type="text" inputmode="tel"
      placeholder="55 1234 5678 o correo@email.com"
      oninput="formatearContacto(this)">
    <div id="solContactoHint" style="font-size:0.68rem;color:rgba(100,220,160,0.8);margin:-6px 0 10px;display:none;"></div>
    <button class="lg-btn" onclick="enviarSolicitud()" style="margin-top:4px;">📩 Enviar solicitud</button>
    <button class="lg-btn-ghost" onclick="mostrarPanelCodigo()">← Ya tengo un código</button>
  </div>

  <!-- ── PANEL: Solicitud enviada ── -->
  <div class="lg-card" id="panelEnviada" style="display:none;text-align:center;">
    <div style="font-size:3rem;margin-bottom:12px;filter:drop-shadow(0 4px 16px rgba(43,192,112,0.4));">📩</div>
    <div style="font-size:1.1rem;font-weight:800;color:#fff;margin-bottom:6px;">¡Solicitud lista!</div>
    <div style="font-size:0.78rem;color:rgba(255,255,255,0.4);margin-bottom:22px;line-height:1.6;">Envíala al administrador para que te dé acceso</div>
    <a id="_solWaBtn" href="#" target="_blank"
      style="display:flex;align-items:center;justify-content:center;gap:10px;width:100%;padding:15px;background:linear-gradient(135deg,#25D366,#1da855);color:#fff;border:none;border-radius:16px;font-family:Outfit,sans-serif;font-size:0.92rem;font-weight:700;cursor:pointer;margin-bottom:10px;text-decoration:none;box-shadow:0 4px 20px rgba(37,211,102,0.3);">
      📲 Enviar por WhatsApp
    </a>
    <button id="_solCopyBtn"
      style="width:100%;padding:14px;background:rgba(255,255,255,0.07);color:rgba(255,255,255,0.7);border:1px solid rgba(255,255,255,0.12);border-radius:14px;font-family:Outfit,sans-serif;font-size:0.88rem;font-weight:600;cursor:pointer;margin-bottom:18px;">
      📋 Copiar mensaje
    </button>
    <input type="hidden" id="_solPayload" value="">
    <div style="font-size:0.72rem;color:rgba(255,255,255,0.3);margin-bottom:16px;line-height:1.5;">El admin pegará el mensaje en la app para registrarte.</div>
    <button class="lg-btn-ghost" onclick="mostrarPanelCodigo()">← Volver al login</button>
  </div>

</div>
</div>

<!-- ══ ADMIN MODAL ══ -->
<div class="lg-modal-backdrop" id="adminModal">
  <div style="position:absolute;inset:0;" onclick="cerrarAdminModal()"></div>
  <div class="lg-modal-box" style="position:relative;">
    <div class="lg-modal-handle"></div>
    <div style="text-align:center;font-size:2.2rem;margin-bottom:8px;filter:drop-shadow(0 4px 16px rgba(43,192,112,0.3));">🔐</div>
    <div style="font-size:1.05rem;font-weight:800;text-align:center;color:#fff;margin-bottom:18px;letter-spacing:-0.02em;">Acceso Administrador</div>
    <div id="adminErr" class="lg-err"></div>
    <div class="lg-section-title">Contraseña</div>
    <input class="lg-inp" id="adminPass" type="password" placeholder="Contraseña de administrador"
      onkeydown="if(event.key==='Enter')verificarAdmin()">
    <button class="lg-btn" onclick="verificarAdmin()" style="margin-top:6px;">Entrar como Admin →</button>
    <div style="text-align:center;font-size:0.7rem;color:rgba(255,255,255,0.25);margin-top:14px;">¿Primera vez? Usa la clave que te fue asignada</div>
    <button onclick="recuperarAdmin()" style="width:100%;margin-top:8px;padding:10px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.7rem;color:rgba(255,255,255,0.3);text-decoration:underline;cursor:pointer;">¿Olvidaste tu contraseña? Restablecer</button>
  </div>
</div>
</div><!-- /lg-scroll-outer -->

<!-- ══ DASHBOARD ══ -->
<div class="screen" id="dashboard">
  <div class="topbar">
    <!-- Logo + título tab activo -->
    <div style="display:flex;flex-direction:column;justify-content:center;flex:1;min-width:0;">
      <div class="top-logo">USALA <span class="top-ver" id="verBadge"></span></div>
      <div id="topUserName" style="font-size:0.65rem;font-weight:600;color:var(--dim);overflow:hidden;text-overflow:ellipsis;white-space:nowrap;margin-top:1px;"></div>
    </div>
    <!-- Acciones derechas -->
    <div style="display:flex;align-items:center;gap:6px;">
      <button class="top-icon" id="btnSolicitudes" onclick="goTab('mas',document.querySelectorAll('.nb')[4]);setTimeout(function(){goSub('codigos');},50);" title="Solicitudes" style="display:none;position:relative;">
        📩
        <span id="badgeSolicitudes" style="position:absolute;top:2px;right:2px;background:#ff3b30;color:#fff;font-size:0.45rem;font-weight:800;width:14px;height:14px;border-radius:50%;display:flex;align-items:center;justify-content:center;"></span>
      </button>
      <button id="uFabBtn" class="top-icon" onclick="toggleUMenu()" title="Mis cuentas" style="display:none;background:linear-gradient(135deg,var(--accent),var(--accent2));color:#fff;font-weight:900;font-size:0.95rem;letter-spacing:-0.5px;box-shadow:0 2px 10px var(--glow);">U</button>
      <button class="top-icon" id="btnVoz" onclick="toggleVoz()" title="Comando de voz" style="display:none;">🎙️</button>
      <button class="top-icon" onclick="abrirCalc()" title="Calculadora">🔢</button>
      <div id="syncDot" title="Sincronizado" style="display:none;width:8px;height:8px;border-radius:50%;background:#2bc070;margin-left:2px;transition:background 0.3s;flex-shrink:0;"></div>
    </div>
  </div>
  <!-- Pantalla de carga al sincronizar -->
  <div id="syncLoadingOverlay" style="display:none;position:fixed;inset:0;z-index:9999;background:var(--bg);flex-direction:column;align-items:center;justify-content:center;gap:16px;">
    <div style="font-size:2.5rem;animation:consejeroFloat 1.5s ease-in-out infinite;">&#x2601;&#xFE0F;</div>
    <div style="font-size:1rem;font-weight:800;color:var(--text);">Cargando tus datos...</div>
    <div id="syncLoadingMsg" style="font-size:0.8rem;color:var(--dim);">Conectando con la nube</div>
    <div style="width:200px;height:4px;background:var(--card2);border-radius:2px;overflow:hidden;margin-top:4px;">
      <div id="syncLoadingBar" style="height:100%;width:0%;background:linear-gradient(90deg,var(--accent),var(--accent2));border-radius:2px;transition:width 0.4s ease;"></div>
    </div>
  </div>
  <div class="content" id="mainContent"></div>
  <nav class="bot-nav">
    <button class="nb active" onclick="goTab('inicio',this)">
      <div class="nb-ico">🏠</div><div class="nb-lbl">Inicio</div>
    </button>
    <button class="nb" onclick="goTab('cuentas',this)">
      <div class="nb-ico">🏦</div><div class="nb-lbl">Cuentas</div>
    </button>
    <button class="nb" onclick="goTab('creditos',this)">
      <div class="nb-ico">🤝</div><div class="nb-lbl">Créditos</div>
    </button>
    <button class="nb" onclick="goTab('reportes',this)">
      <div class="nb-ico">📊</div><div class="nb-lbl">Reportes</div>
    </button>
    <button class="nb" onclick="goTab('mas',this)">
      <div class="nb-ico">⋯</div><div class="nb-lbl">Más</div>
    </button>
  </nav>
</div>

<!-- ══ TX MODAL ══ -->
<!-- ══ BIENVENIDA MODAL ══ -->
<div id="welcomeModal" style="display:none;position:fixed;inset:0;z-index:200;align-items:flex-end;justify-content:center;background:rgba(0,0,0,0);">
  <!-- Backdrop animado -->
  <div id="welcomeBackdrop" style="position:absolute;inset:0;background:rgba(0,0,0,0);transition:background 0.4s ease;"></div>

  <!-- Sheet principal -->
  <div id="welcomeSheet" style="
    position:relative;z-index:1;
    width:100%;max-width:480px;
    background:var(--card);
    border-radius:28px 28px 0 0;
    padding:0 0 40px;
    transform:translateY(100%);
    transition:transform 0.5s cubic-bezier(0.34,1.56,0.64,1);
    overflow:hidden;
  ">
    <!-- Hero gradient animado -->
    <div style="
      background:linear-gradient(135deg,#667eea,#764ba2,#f093fb);
      background-size:300% 300%;
      animation:gradShift 4s ease infinite;
      padding:36px 24px 28px;
      text-align:center;
      position:relative;
      overflow:hidden;
    ">
      <!-- Círculos decorativos flotantes -->
      <div style="position:absolute;top:-20px;left:-20px;width:100px;height:100px;background:rgba(255,255,255,0.08);border-radius:50%;animation:float1 3s ease-in-out infinite;"></div>
      <div style="position:absolute;bottom:-30px;right:-10px;width:140px;height:140px;background:rgba(255,255,255,0.06);border-radius:50%;animation:float2 4s ease-in-out infinite;"></div>
      <div style="position:absolute;top:20px;right:20px;width:50px;height:50px;background:rgba(255,255,255,0.1);border-radius:50%;animation:float1 2.5s ease-in-out infinite reverse;"></div>

      <!-- Emoji con pulso -->
      <div style="font-size:3.5rem;animation:popIn 0.7s cubic-bezier(0.34,1.56,0.64,1) 0.3s both;display:inline-block;">👋</div>

      <!-- Título personalizado -->
      <div id="welcomeName" style="
        font-size:1.5rem;font-weight:900;color:#fff;
        margin-top:10px;margin-bottom:4px;
        animation:slideUp 0.5s ease 0.5s both;
        text-shadow:0 2px 12px rgba(0,0,0,0.2);
      ">¡Bienvenid@ a USALA!</div>

      <!-- Subtítulo -->
      <div style="
        font-size:0.8rem;color:rgba(255,255,255,0.85);
        animation:slideUp 0.5s ease 0.65s both;
        font-weight:500;
      ">Tu dinero, finalmente bajo control ✨</div>
    </div>

    <!-- Cuerpo del mensaje -->
    <div style="padding:24px 24px 0;">

      <!-- Mensaje principal -->
      <div style="
        font-size:0.92rem;color:var(--text);line-height:1.75;
        text-align:center;margin-bottom:20px;
        animation:slideUp 0.5s ease 0.8s both;
      ">
        Ese dinero que <strong style="color:#764ba2;">"desaparece"</strong> cada quincena<br>— aquí lo vamos a encontrar juntos.
        <br><br>
        Desde hoy sabes exactamente <strong style="color:var(--accent);">cuánto tienes</strong>, cuánto debes y cuánto puedes gastar. Sin hojas de cálculo, sin estrés, sin juicios.
        <br><br>
        No necesitas ser experto en finanzas.<br><strong style="color:var(--text);">Solo necesitas empezar.</strong>
      </div>

      <!-- Frase motivacional destacada -->
      <div style="
        background:linear-gradient(135deg,rgba(102,126,234,0.12),rgba(118,75,162,0.12));
        border:1.5px solid rgba(118,75,162,0.2);
        border-radius:16px;padding:14px 18px;
        text-align:center;margin-bottom:20px;
        animation:slideUp 0.5s ease 1s both;
      ">
        <div style="font-size:1rem;font-weight:900;background:linear-gradient(135deg,#667eea,#764ba2);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;">
          El primer paso ya lo diste. 🚀
        </div>
      </div>

      <!-- Botón CTA -->
      <button onclick="cerrarWelcome()" style="
        width:100%;padding:16px;border:none;border-radius:18px;
        background:linear-gradient(135deg,#667eea,#764ba2);
        color:#fff;font-family:Outfit,sans-serif;
        font-size:1rem;font-weight:800;cursor:pointer;
        box-shadow:0 8px 24px rgba(102,126,234,0.4);
        animation:slideUp 0.5s ease 1.1s both;
        transition:transform 0.15s ease, box-shadow 0.15s ease;
      "
      onmousedown="this.style.transform='scale(0.97)';this.style.boxShadow='0 4px 12px rgba(102,126,234,0.3)'"
      onmouseup="this.style.transform='scale(1)';this.style.boxShadow='0 8px 24px rgba(102,126,234,0.4)'"
      ontouchstart="this.style.transform='scale(0.97)'"
      ontouchend="this.style.transform='scale(1)'">
        ¡Empezar ahora! →
      </button>
    </div>
  </div>
</div>

<!-- ══ MODAL TIPO INGRESO ══ -->

<!-- ══ MODAL TIPO GASTO ══ -->
<div class="modal" id="gastoTipoModal">
  <div class="modal-box" style="position:relative;z-index:2;">
    <div class="modal-header">
      <div class="modal-title">💳 Nuevo Gasto</div>
      <button class="modal-close" onclick="cerrarGastoTipo()">✕</button>
    </div>
    <p style="color:var(--dim);font-size:0.85rem;margin-bottom:18px;text-align:center;">¿Qué tipo de gasto es?</p>
    <div style="display:flex;flex-direction:column;gap:12px;">

      <button onclick="elegirTipoGasto('normal')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(255,95,87,0.12);display:flex;align-items:center;justify-content:center;">🧾</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Gasto normal</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Comida, transporte, servicios, etc.</div>
        </div>
      </button>

      <button onclick="elegirTipoGasto('preste')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(56,170,255,0.12);display:flex;align-items:center;justify-content:center;">🤝</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Presté dinero</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Me lo deben regresar — se registra en Créditos</div>
        </div>
      </button>

      <button onclick="elegirTipoGasto('abono')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(255,179,64,0.12);display:flex;align-items:center;justify-content:center;">💸</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Pagué una deuda / abono</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Abono a un crédito que debo — actualiza Créditos</div>
        </div>
      </button>

    </div>
  </div>
</div>

<div class="modal" id="ingresoTipoModal">
  <div class="modal-box" style="position:relative;z-index:2;">
    <div class="modal-header">
      <div class="modal-title">💰 Nuevo Ingreso</div>
      <button class="modal-close" onclick="cerrarIngresoTipo()">✕</button>
    </div>
    <p style="color:var(--dim);font-size:0.85rem;margin-bottom:18px;text-align:center;">¿Qué tipo de ingreso es?</p>
    <div style="display:flex;flex-direction:column;gap:12px;">

      <button onclick="elegirTipoIngreso('normal')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;
        color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(43,192,112,0.15);display:flex;align-items:center;justify-content:center;">💵</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Ingreso normal</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Sueldo, venta, comisión, etc.</div>
        </div>
      </button>

      <button onclick="elegirTipoIngreso('prestamo')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;
        color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(255,179,64,0.15);display:flex;align-items:center;justify-content:center;">🤝</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Me prestaron dinero</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Lo debo regresar — se registra en Créditos</div>
        </div>
      </button>

      <button onclick="elegirTipoIngreso('cobro')" style="
        display:flex;align-items:center;gap:14px;
        padding:16px 18px;border-radius:18px;border:1.5px solid var(--border);
        background:var(--card);backdrop-filter:blur(12px);
        cursor:pointer;text-align:left;transition:all 0.15s;
        color:var(--text);">
        <div style="font-size:1.8rem;width:44px;height:44px;border-radius:14px;background:rgba(56,170,255,0.15);display:flex;align-items:center;justify-content:center;">📥</div>
        <div>
          <div style="font-weight:700;font-size:0.95rem;">Me pagaron lo que me debían</div>
          <div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">Cobré un préstamo que le hice a alguien</div>
        </div>
      </button>

    </div>
  </div>
</div>

<div class="modal" id="txModal">
  <div class="modal-box" style="position:relative;z-index:2;">
    <div class="modal-header">
      <div class="modal-title" id="txModalTitle">Nueva Transacción</div>
      <button class="modal-close" onclick="cerrarTxModal()">✕</button>
    </div>
    <div class="tipo-selector" id="tipoSelector">
      <div class="tipo-opt selected" id="tipoGasto" onclick="selTipo('gasto')">💳 Gasto</div>
      <div class="tipo-opt" id="tipoIngreso" onclick="selTipo('ingreso')">💰 Ingreso</div>
    </div>
    <label class="inp-label">Descripción</label>
    <input class="inp" id="txDesc" placeholder="Ej: Supermercado" autocomplete="off">
    <div class="form-row">
      <div><label class="inp-label">Monto ($)</label><input class="inp" id="txMonto" type="number" inputmode="decimal" placeholder="0.00"></div>
      <div><label class="inp-label">Categoría</label>
        <select class="inp" id="txCat">
          <option>🍽️ Alimentación</option><option>🚗 Transporte</option><option>💡 Servicios</option>
          <option>💳 Pagos / Deudas</option><option>🛍️ Compras</option><option>🎬 Entretenimiento</option><option>💊 Salud</option><option>📚 Educación</option><option>📦 Otros gastos</option>
          <option>💼 Salario</option><option>🔧 Freelance</option><option>🏢 Negocio</option><option>🏠 Renta</option><option>📈 Inversión</option>
          <option>📥 Otros ingresos</option>
        </select>
        <button type="button" class="cat-add-btn" id="txCatAddBtn" onclick="abrirCatModalTx()">＋ Categoría</button>
      </div>
    </div>
    <label class="inp-label">💼 Cuenta / Bolsillo</label>
    <select class="inp" id="txCuenta">
      <option value="">— Sin asignar —</option>
      <option value="efectivo">💵 Efectivo</option>
    </select>
    <label class="inp-label">Fecha</label>
    <input class="inp" id="txFecha" type="date">
    <button class="btn-main" id="txSaveBtn" onclick="guardarTx()" style="margin-top:8px;">💾 Guardar</button>
    <button onclick="cerrarTxModal()" style="width:100%;padding:12px;background:none;border:1.5px solid var(--border);border-radius:12px;font-family:Outfit,sans-serif;font-size:0.88rem;color:var(--dim);cursor:pointer;margin-top:8px;">Cancelar</button>
  </div>
</div>

<!-- PANEL PAGOS PENDIENTES -->
<div id="ppOverlay" class="pp-overlay" style="display:none;" onclick="if(event.target===this)cerrarPP()">
  <div class="pp-panel">
    <div class="pp-handle"></div>
    <div class="pp-head">
      <div style="display:flex;justify-content:space-between;align-items:flex-start;">
        <div>
          <div class="pp-title">⏰ Pagos Pendientes</div>
          <div class="pp-subtitle" id="ppSubtitle">Panorama de lo que se viene</div>
        </div>
        <button onclick="cerrarPP()" style="background:none;border:none;font-size:1.4rem;cursor:pointer;color:var(--dim);padding:0;line-height:1;">×</button>
      </div>
    </div>
    <div class="pp-tabs">
      <button class="pp-tab active" onclick="ppSetTab('hoy',this)">📍 Hoy</button>
      <button class="pp-tab" onclick="ppSetTab('semana',this)">📅 Esta semana</button>
      <button class="pp-tab" onclick="ppSetTab('mes',this)">🗓️ Este mes</button>
      <button class="pp-tab" onclick="ppSetTab('año',this)">📆 Este año</button>
    </div>
    <div class="pp-body" id="ppBody"></div>
  </div>
</div>

<!-- PANTALLA DE BLOQUEO AUTOMÁTICO -->
<div id="lockScreen" class="lock-screen" style="display:none;">
  <div class="lock-card">
    <div class="lock-avatar">🔒</div>
    <div class="lock-nombre" id="lockNombre">Hola</div>
    <div class="lock-sub">La app se bloqueó por inactividad</div>
    <div class="lock-timeout-badge" id="lockTimeBadge">⏱ Bloqueado automáticamente</div>
    <div class="lock-dots" id="lockDots">
      <div class="lock-dot" id="ld0"></div>
      <div class="lock-dot" id="ld1"></div>
      <div class="lock-dot" id="ld2"></div>
      <div class="lock-dot" id="ld3"></div>
    </div>
    <div id="lockErr" style="font-size:0.75rem;color:#e53935;min-height:18px;margin-bottom:8px;font-weight:700;"></div>
    <div class="lock-pad">
      <button class="lock-key" onclick="lockKey('1')">1</button>
      <button class="lock-key" onclick="lockKey('2')">2</button>
      <button class="lock-key" onclick="lockKey('3')">3</button>
      <button class="lock-key" onclick="lockKey('4')">4</button>
      <button class="lock-key" onclick="lockKey('5')">5</button>
      <button class="lock-key" onclick="lockKey('6')">6</button>
      <button class="lock-key" onclick="lockKey('7')">7</button>
      <button class="lock-key" onclick="lockKey('8')">8</button>
      <button class="lock-key" onclick="lockKey('9')">9</button>
      <button class="lock-key del" onclick="lockCerrarSesion()" style="font-size:0.65rem;color:var(--dim);">Salir</button>
      <button class="lock-key" onclick="lockKey('0')">0</button>
      <button class="lock-key del" onclick="lockDel()">⌫</button>
    </div>
    <div id="lockNoNipMsg" style="display:none;margin-top:16px;">
      <button class="btn-main" onclick="lockDesbloquear()" style="width:100%;">🔓 Desbloquear</button>
    </div>
  </div>
</div>

<!-- MODAL AGREGAR CATEGORÍA -->
<div id="catModal" class="cat-modal-overlay" style="display:none;" onclick="if(event.target===this)cerrarCatModal()">
  <div class="cat-modal-box">
    <div class="cat-modal-title" id="catModalTitle">🏷️ Categorías</div>
    <div class="cat-modal-sub" id="catModalSub">Tus categorías personalizadas</div>
    <div class="cat-chips-wrap" id="catModalChips"></div>
    <div class="cat-new-row">
      <input class="cat-new-inp" id="catModalInp" placeholder="Nueva categoría..." maxlength="40"
        onkeydown="if(event.key==='Enter')guardarNuevaCat()">
      <button class="cat-save-btn" onclick="guardarNuevaCat()">+ Agregar</button>
    </div>
  </div>
</div>

<!-- CALCULADORA FLOTANTE -->

<!-- Menú desplegable del botón U (cae desde topbar) -->
<div id="uFabMenu" style="display:none;position:fixed;z-index:989;top:58px;right:14px;background:var(--card);border-radius:18px;box-shadow:0 8px 32px rgba(0,0,0,0.2);padding:6px;min-width:210px;transform:scale(0.85) translateY(-10px);opacity:0;transform-origin:top right;transition:all 0.25s cubic-bezier(0.34,1.4,0.64,1);">
  <div onclick="irACuenta('efectivo')" style="display:flex;align-items:center;gap:12px;padding:14px 16px;border-radius:12px;cursor:pointer;active-background:var(--inp);">
    <span style="font-size:1.4rem;">💵</span>
    <div>
      <div style="font-size:0.92rem;font-weight:800;color:var(--text);">Efectivo</div>
      <div id="uMenuEfectivo" style="font-size:0.74rem;color:var(--dim);">—</div>
    </div>
    <span style="margin-left:auto;color:var(--dim);">›</span>
  </div>
  <div style="height:1px;background:var(--border);margin:2px 8px;"></div>
  <div onclick="irACuenta('cheques')" style="display:flex;align-items:center;gap:12px;padding:14px 16px;border-radius:12px;cursor:pointer;">
    <span style="font-size:1.4rem;">🏦</span>
    <div>
      <div style="font-size:0.92rem;font-weight:800;color:var(--text);">Cheques / Banco</div>
      <div id="uMenuBanco" style="font-size:0.74rem;color:var(--dim);">—</div>
    </div>
    <span style="margin-left:auto;color:var(--dim);">›</span>
  </div>
  <div style="height:1px;background:var(--border);margin:2px 8px;"></div>
  <div onclick="irACuenta('tarjetas_credito')" style="display:flex;align-items:center;gap:12px;padding:14px 16px;border-radius:12px;cursor:pointer;">
    <span style="font-size:1.4rem;">💳</span>
    <div>
      <div style="font-size:0.92rem;font-weight:800;color:var(--text);">Tarjetas de Crédito</div>
      <div id="uMenuTC" style="font-size:0.74rem;color:#e53935;">—</div>
    </div>
    <span style="margin-left:auto;color:var(--dim);">›</span>
  </div>
</div>
<div id="calcFloat" style="display:none;position:fixed;z-index:999;bottom:100px;right:14px;width:280px;border-radius:28px;overflow:hidden;box-shadow:0 20px 60px rgba(0,0,0,0.5);font-family:Outfit,sans-serif;touch-action:none;transition:all 0.3s cubic-bezier(0.34,1.2,0.64,1);">
  <!-- Handle drag -->
  <div id="calcHandle" style="background:linear-gradient(135deg,#1a1a2e,#16213e);padding:12px 14px 8px;display:flex;align-items:center;justify-content:space-between;cursor:grab;user-select:none;">
    <div style="display:flex;align-items:center;gap:6px;">
      <span style="font-size:1rem;">🔢</span>
      <span style="color:rgba(255,255,255,0.5);font-size:0.65rem;font-weight:700;letter-spacing:0.1em;">CALCULADORA</span>
    </div>
    <div style="display:flex;gap:6px;align-items:center;">
      <!-- Botón minimizar -->
      <button id="calcMinBtn" onclick="minimizarCalc()" style="background:rgba(255,200,0,0.2);border:none;color:#ffd60a;width:28px;height:28px;border-radius:50%;cursor:pointer;font-size:1rem;font-weight:900;line-height:28px;text-align:center;flex-shrink:0;" title="Minimizar">−</button>
      <!-- Botón cerrar -->
      <button id="calcCloseBtn" onclick="cerrarCalc()" style="background:rgba(255,60,60,0.25);border:none;color:#ff6b6b;width:28px;height:28px;border-radius:50%;cursor:pointer;font-size:0.9rem;font-weight:900;line-height:28px;text-align:center;flex-shrink:0;" title="Cerrar">✕</button>
    </div>
  </div>
  <!-- Display -->
  <div id="calcBody">
    <div style="background:#0f0f1a;padding:10px 16px 12px;">
      <div id="calcExpr" style="text-align:right;font-size:0.68rem;color:rgba(255,255,255,0.35);min-height:16px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;"></div>
      <div id="calcDisplay" style="text-align:right;font-size:2.5rem;font-weight:700;color:#fff;min-height:54px;word-break:break-all;line-height:1.1;margin-top:2px;">0</div>
    </div>
    <!-- Teclado -->
    <div id="calcKeys" style="background:#1a1a2e;display:grid;grid-template-columns:repeat(4,1fr);gap:2px;padding:2px;">
      <button class="ck ck-fn" onclick="calcAc()">AC</button>
      <button class="ck ck-fn" onclick="calcPlusMinus()">+/−</button>
      <button class="ck ck-fn" onclick="calcOp('%')">%</button>
      <button class="ck ck-op" onclick="calcOp('/')">÷</button>
      <button class="ck" onclick="calcNum('7')">7</button>
      <button class="ck" onclick="calcNum('8')">8</button>
      <button class="ck" onclick="calcNum('9')">9</button>
      <button class="ck ck-op" onclick="calcOp('*')">×</button>
      <button class="ck" onclick="calcNum('4')">4</button>
      <button class="ck" onclick="calcNum('5')">5</button>
      <button class="ck" onclick="calcNum('6')">6</button>
      <button class="ck ck-op" onclick="calcOp('-')">−</button>
      <button class="ck" onclick="calcNum('1')">1</button>
      <button class="ck" onclick="calcNum('2')">2</button>
      <button class="ck" onclick="calcNum('3')">3</button>
      <button class="ck ck-op" onclick="calcOp('+')">+</button>
      <button class="ck ck-del" onclick="calcDel()">⌫</button>
      <button class="ck" onclick="calcNum('0')">0</button>
      <button class="ck" onclick="calcPunto()">.</button>
      <button class="ck ck-eq" onclick="calcEqual()">=</button>
    </div>
  </div>
</div>

<!-- Burbuja minimizada -->
<div id="calcBubble" style="display:none;position:fixed;z-index:999;bottom:100px;right:14px;width:68px;height:68px;border-radius:50%;background:linear-gradient(135deg,#1a1a2e,#16213e);box-shadow:0 8px 24px rgba(0,0,0,0.5);cursor:pointer;touch-action:none;flex-direction:column;align-items:center;justify-content:center;border:2px solid rgba(255,255,255,0.1);" onclick="restaurarCalc()">
  <div style="font-size:1.2rem;line-height:1;">🔢</div>
  <div id="calcBubbleVal" style="font-size:0.55rem;font-weight:800;color:#ffd60a;margin-top:2px;max-width:60px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;text-align:center;">0</div>
</div>

<!-- ══ SCRIPTS — orden de carga ══ -->

<!-- PWA Service Worker -->

<script>
// ─────────────────────────────────────────────
//  USALA Suite — Base de Datos & Configuración
//  config/supabase.js  ·  carga PRIMERO
// ─────────────────────────────────────────────

var SUPA_URL = 'https://mdllmtuitgsqlpjmnllf.supabase.co';
var SUPA_KEY = 'sb_publishable_I8RyoelqHZrsiM-4K6ypGg_5Ze5BSNG';

var DB = {
  _h: function(){ return { 'Content-Type':'application/json', 'apikey': SUPA_KEY, 'Authorization': 'Bearer ' + SUPA_KEY, 'Prefer': 'return=representation' }; },
  get: async function(table, params){
    var url = SUPA_URL + '/rest/v1/' + table;
    if(params) url += '?' + params;
    var r = await fetch(url, { headers: DB._h() });
    if(!r.ok) throw new Error(await r.text());
    return r.json();
  },
  insert: async function(table, data){
    var r = await fetch(SUPA_URL + '/rest/v1/' + table, {
      method: 'POST', headers: DB._h(), body: JSON.stringify(data)
    });
    if(!r.ok) throw new Error(await r.text());
    return r.json();
  },
  update: async function(table, match, data){
    var url = SUPA_URL + '/rest/v1/' + table + '?' + match;
    var r = await fetch(url, {
      method: 'PATCH',
      headers: Object.assign({}, DB._h(), {'Prefer':'return=representation'}),
      body: JSON.stringify(data)
    });
    if(!r.ok) throw new Error(await r.text());
    return r.json();
  },
  upsert: async function(table, data, onConflict){
    var h = Object.assign({}, DB._h(), {'Prefer':'resolution=merge-duplicates,return=representation'});
    if(onConflict) h['Prefer'] += ',on_conflict=' + onConflict;
    var r = await fetch(SUPA_URL + '/rest/v1/' + table, {
      method: 'POST', headers: h, body: JSON.stringify(data)
    });
    if(!r.ok) throw new Error(await r.text());
    return r.json();
  },
  del: async function(table, match){
    var url = SUPA_URL + '/rest/v1/' + table + '?' + match;
    var r = await fetch(url, { method: 'DELETE', headers: DB._h() });
    if(!r.ok) throw new Error(await r.text());
    return true;
  }
};


// USALA Suite - Variables globales & Arranque
// js/globals.js

var _cache = {};
var _cacheTs = {};
var CACHE_TTL = 30000;
var _syncQueue = [];
var _syncTimer = null;
var _syncIndicatorTimer = null;
var _realtimeInterval = null;
var _lastSyncTs = null;
var _realtimeActivo = false;
var _syncToastTimer = null;
var _dbOnline = true;
var _SYNC_KEYS = [
  'txs','cuentas','creditos','cxc','metas','pagos_mensuales',
  'activos_personales','presupuesto','alertas',
  'cats_gasto_custom','cats_ingreso_custom',
  'cats_activos_custom','cats_pagos_custom'
];
var S = {
  user: null,       // {nombre, codigo, isAdmin}
  tab: 'inicio',
  subtab: null,
  editTxId: null,
  editCrediIdx: null,
  editCrediTipo: null,
  theme: 'default'
};
var APP_VERSION = localStorage.getItem('usala_version') || '3.0.0';
var APP_NOTAS   = localStorage.getItem('usala_notas') || 'Versión 2 — Rediseño completo';
var _sesionPendiente = null;
var _nipBuffer = '';
var _accLookupTimer = null;
var _saltarPass = false;
var _accPassVerificada = false;
var _adminPanelTab = 'resumen';
var _aprobarIdx = -1;
var _undoFn = null, _undoTimer = null;
var _calcExpr = '', _calcResult = '0', _calcNewNum = true, _calcScale = 1.0;
var _carritoUndoTimer = null;
var GASTO_CATS_BASE = [
  {id:'🍽️ Alimentación',  color:'#ef6c00'},
  {id:'🚗 Transporte',    color:'#1e88e5'},
  {id:'🏠 Hogar',         color:'#8d6e63'},
  {id:'💡 Servicios',     color:'#26a69a'},
  {id:'💳 Pagos / Deudas',color:'#5c6bc0'},
  {id:'🛍️ Compras',       color:'#ab47bc'},
  {id:'🎬 Entretenimiento',color:'#f9a825'},
  {id:'💊 Salud',         color:'#e53935'},
  {id:'📚 Educación',     color:'#43a047'},
  {id:'👗 Ropa / Moda',   color:'#ec407a'},
  {id:'✈️ Viajes',        color:'#00acc1'},
  {id:'🍺 Restaurantes',  color:'#ff7043'},
  {id:'📦 Otros gastos',  color:'#78909c'}
];
var INGRESO_CATS_BASE = [
  {id:'💼 Salario'},
  {id:'🔧 Freelance'},
  {id:'🏢 Negocio'},
  {id:'🏠 Renta'},
  {id:'📈 Inversión'},
  {id:'🎁 Regalo'},
  {id:'💰 Venta'},
  {id:'📥 Otros ingresos'}
];
var _CAT_MIGRA = {
  'Alimentación':'🍽️ Alimentación',
  'Transporte':'🚗 Transporte',
  'Servicios':'💡 Servicios',
  'Compras':'🛍️ Compras',
  'Pagos':'💳 Pagos / Deudas',
  'Entretenimiento':'🎬 Entretenimiento',
  'Salud':'💊 Salud',
  'Educación':'📚 Educación',
  'Ropa':'👗 Ropa / Moda',
  'Otros':'📦 Otros gastos',
  'Otros gastos':'📦 Otros gastos',
  'Pago de servicio':'💡 Servicios',
  'Transferencia enviada':'💳 Pagos / Deudas',
  'Transferencia a banco':'💳 Pagos / Deudas',
  'Compra':'🛍️ Compras',
  'Retiro':'📦 Otros gastos',
  'Salario':'💼 Salario',
  'Activos':'📈 Inversión',
  'Freelance':'🔧 Freelance',
  'Renta':'🏠 Renta',
  'Inversión':'📈 Inversión',
  'Otros ingresos':'📥 Otros ingresos',
  'Negocio':'🏢 Negocio',
  'Venta':'💰 Venta',
  'Regalo':'🎁 Regalo',
  'Depósito':'📥 Otros ingresos',
  'Transferencia recibida':'📥 Otros ingresos',
  'Nómina':'💼 Salario'
};
var _CAT_KEYS = {
  gasto:   'cats_gasto_custom',
  ingreso: 'cats_ingreso_custom',
  activos: 'cats_activos_custom',
  pagos:   'cats_pagos_custom'
};
var PAGOS_CATS = ['💳 Tarjetas','💡 Servicios','🏠 Renta / Hipoteca','🏛 Impuestos','🚗 Auto','📱 Telefonía','🌐 Internet / Cable','🏥 Salud / Seguros','🎓 Educación','📦 Suscripciones','🔧 Otros'];
var ACTIVOS_CATS = ['🏠 Inmueble','🚗 Vehículo','💼 Negocio','📈 Inversión','💰 Ahorro / Efectivo','🌐 Criptomonedas','🏭 Maquinaria / Equipo','💍 Joyas / Arte','📦 Otros'];

var _CAT_BASE = {
  gasto:   GASTO_CATS_BASE.map(function(c){ return c.id; }),
  ingreso: INGRESO_CATS_BASE.map(function(c){ return c.id; }),
  activos: ACTIVOS_CATS.slice(),
  pagos:   PAGOS_CATS.slice()
};
var _CAT_TITLES = {
  gasto:   { title:'💸 Categorías de Gasto',   sub:'Añade tus propias categorías de gasto' },
  ingreso: { title:'💰 Categorías de Ingreso',  sub:'Añade tus propias fuentes de ingreso' },
  activos: { title:'🏦 Tipos de Activo',        sub:'Añade tipos de activo personalizados' },
  pagos:   { title:'📅 Tipos de Pago Fijo',     sub:'Añade categorías de pagos recurrentes' }
};
var _tipoInteresActual = 'total';
var _catModalTipo = null, _catSelectId = null, _catSelectVal = null;
var _ppTab = 'hoy';
var LOCK_OPCIONES = [
  {val:0,   label:'Desactivado'},
  {val:1,   label:'1 minuto'},
  {val:2,   label:'2 minutos'},
  {val:5,   label:'5 minutos'},
  {val:10,  label:'10 minutos'},
  {val:15,  label:'15 minutos'},
  {val:30,  label:'30 minutos'},
  {val:60,  label:'1 hora'}
];
var _lockTimer = null, _lockPin = '', _lockActivo = false;
var _editCuentaIdx = null, _editTCIdx = null;
var _vozRec = null, _vozActivo = false;
var FAQS = [
  {cat:'🏠 Inicio', q:'¿Qué muestra la pantalla de Inicio?',
   a:'Tu resumen financiero completo: Total disponible, Patrimonio Neto, Deudas, Pagos Pendientes, últimas transacciones y alertas de seguridad activas.'},
  {cat:'🏠 Inicio', q:'¿Qué es el botón ⏰ Pago Pendiente?',
   a:'Muestra cuántos pagos vencen pronto. El badge es rojo si hay vencidos, naranja si vencen esta semana. Tócalo para ver el detalle.'},
  {cat:'🏠 Inicio', q:'¿Qué es el aviso de seguridad en el inicio?',
   a:'Si tu cuenta no tiene NIP o bloqueo automático, aparece un banner de alerta. Puedes configurarlo desde ahí mismo o cerrarlo temporalmente.'},
  {cat:'🏠 Inicio', q:'¿Cómo registro un ingreso o gasto rápido?',
   a:'Usa el botón U azul flotante para acceder en un toque a Efectivo, Banco o Tarjetas. O di un comando de voz: "gasté 200" o "ingresé 500".'},
  {cat:'🔵 Botón U', q:'¿Para qué sirve el botón U azul?',
   a:'Acceso rápido a tus 3 cuentas desde cualquier pantalla. Tócalo y aparece un menú con Efectivo, Banco y Tarjetas con el saldo actual.'},
  {cat:'🎙️ Voz', q:'¿Cómo funciona el control por voz?',
   a:'Toca 🎙️ en la barra superior. Se activa y escucha. Di tu comando claramente. Ejecuta la acción al instante. Sin IA, solo acción.'},
  {cat:'🎙️ Voz', q:'¿Necesita internet para funcionar?',
   a:'Sí. En Chrome (Android) el reconocimiento de voz envía el audio a Google para procesarlo. Sin conexión el botón 🎙️ no funciona.'},
  {cat:'🎙️ Voz', q:'¿Qué comandos de navegación puedo usar?',
   a:'"inicio", "cuentas", "créditos", "reportes", "más", "efectivo", "banco", "tarjetas", "calculadora", "historial", "metas", "presupuesto", "conversor", "ayuda".'},
  {cat:'🎙️ Voz', q:'¿Puedo registrar gastos con voz?',
   a:'Sí. "Gasté 200" registra $200 de gasto en Efectivo. "Ingresé 500" registra un ingreso. El saldo se actualiza al instante.'},
  {cat:'🎙️ Voz', q:'El micrófono está bloqueado, ¿qué hago?',
   a:'Más → Configuración → 🎤 Restablecer micrófono. O en Chrome: ⋮ → Configuración → Privacidad → Micrófono → busca la app → Permitir.'},
  {cat:'🏦 Cuentas', q:'¿Qué módulos tiene Cuentas?',
   a:'3 secciones: 💵 Efectivo, 🏧 Banco y 💳 Tarjetas de Crédito. Cada una con historial y formulario de movimientos.'},
  {cat:'🏦 Cuentas', q:'¿Cómo transfiero efectivo a mi banco?',
   a:'Efectivo → Salida → en "¿A qué banco?" elige tu cuenta. Resta de Efectivo y suma al banco destino automáticamente.'},
  {cat:'🏦 Cuentas', q:'¿Qué pasa si borro una transacción?',
   a:'El saldo se revierte automáticamente. Tienes 6 segundos para tocar "Deshacer" y restaurar todo.'},
  {cat:'🏦 Cuentas', q:'¿Las compras con TC afectan mi efectivo?',
   a:'No. Las compras con tarjeta solo aumentan la deuda de esa TC. Tu efectivo y banco NO se ven afectados.'},
  {cat:'💳 Tarjetas', q:'¿Qué es el Saldo al Corte AUTO?',
   a:'Se calcula sumando todas las compras del período actual. Aparece con badge naranja "AUTO". No tienes que calcularlo manualmente.'},
  {cat:'💳 Tarjetas', q:'¿Cómo registro un pago de TC?',
   a:'Toca "💳 Pago" en la tarjeta. El saldo se reduce. Al llegar a $0 se marca "Al corriente".'},
  {cat:'📅 Pagos del Mes', q:'¿Para qué sirven los Pagos del Mes?',
   a:'Para registrar todos tus pagos fijos: servicios, renta, seguros, TC, etc. Llevas control de cuánto has pagado y cuánto falta cada mes.'},
  {cat:'📅 Pagos del Mes', q:'¿Cómo agrego un pago fijo?',
   a:'Créditos → Pagos del Mes → + Agregar. Escribe nombre, categoría, monto estimado, frecuencia y día de vencimiento.'},
  {cat:'📅 Pagos del Mes', q:'¿Cómo funciona el panel ⏰ de la pantalla principal?',
   a:'Muestra los pagos que vencen próximamente en 4 vistas: Hoy, Esta semana, Este mes y Este año. Badge rojo = pagos ya vencidos.'},
  {cat:'📅 Pagos del Mes', q:'¿Los pagos se resetean solos cada mes?',
   a:'Sí. El estado (pagado/pendiente) se resetea automáticamente cada mes. Tus pagos fijos permanecen.'},
  {cat:'🤝 Créditos', q:'¿Qué son los Créditos?',
   a:'"Mis Deudas" = dinero que tú pediste prestado. "Por Cobrar" = dinero que tú prestaste. Con seguimiento de abonos, intereses y fechas límite.'},
  {cat:'🤝 Créditos', q:'¿Cómo abono a una deuda?',
   a:'Toca "+ Abonar". La barra de progreso se actualiza. Al 100% se marca como pagado automáticamente.'},
  {cat:'🔐 Seguridad', q:'¿Por qué me aparece un aviso de seguridad?',
   a:'Tu cuenta no tiene NIP o bloqueo automático activos. Son medidas opcionales pero muy recomendadas para que nadie más vea tus finanzas.'},
  {cat:'🔐 Seguridad', q:'¿Qué es el NIP y para qué sirve?',
   a:'Un código secreto de 4 dígitos. Aunque alguien tenga tu dispositivo o código de invitado, sin el NIP no puede entrar a tus finanzas.'},
  {cat:'🔐 Seguridad', q:'¿Cómo activo mi NIP?',
   a:'Más → Configuración → 🔒 NIP de seguridad → escribe 4 dígitos y confirma. Desde ese momento se pedirá cada vez que entres.'},
  {cat:'🔐 Seguridad', q:'¿Qué es el bloqueo automático?',
   a:'La app se bloquea sola si no la usas por el tiempo elegido (1 min a 1 hora). Al bloquearse pedirá tu NIP para volver a entrar.'},
  {cat:'🔐 Seguridad', q:'¿Cómo activo el bloqueo automático?',
   a:'Más → Configuración → ⏱ Bloqueo automático → elige el tiempo. Cualquier toque reinicia el contador. Recomendamos 5 minutos.'},
  {cat:'🔐 Seguridad', q:'¿Qué pasa si me bloquea y no tengo NIP?',
   a:'Aparece un botón "Desbloquear" directo. Por eso recomendamos ambos: NIP + bloqueo automático. Sin NIP el bloqueo no protege realmente.'},
  {cat:'🔐 Seguridad', q:'¿Puedo cerrar sesión desde la pantalla bloqueada?',
   a:'Sí. En la pantalla de bloqueo hay un botón "Salir" que cierra sesión completamente.'},
  {cat:'🔐 Seguridad', q:'Olvidé mi NIP, ¿qué hago?',
   a:'El admin puede resetearlo: Más → Códigos de Acceso → busca tu código → toca 🔓. El NIP se elimina y puedes configurar uno nuevo.'},
  {cat:'🔐 Seguridad', q:'¿Mis datos son privados respecto a otros usuarios?',
   a:'Sí. Cada usuario tiene su espacio completamente aislado. Nadie puede ver los datos de otro, ni el administrador.'},
  {cat:'🏦 Activos', q:'¿Qué son los Activos Personales?',
   a:'Todo lo que posees con valor: casa, carro, negocio, inversiones, joyas, etc. Su valor suma a tu Patrimonio Neto.'},
  {cat:'🏦 Activos', q:'¿Cada cuánto actualizo el valor?',
   a:'Cuando cambie significativamente. Edita con ✏️ y actualiza el monto. Afectará tu Patrimonio Neto en el siguiente snapshot.'},
  {cat:'📈 Progreso', q:'¿Qué es el Patrimonio Neto?',
   a:'Efectivo + Banco + Activos − Total Deudas. Si sube mes a mes, estás progresando financieramente.'},
  {cat:'📈 Progreso', q:'¿Qué significa el semáforo de salud financiera?',
   a:'🟢 Progresando = patrimonio sube, deudas bajan. 🟡 Estable = sin cambios. 🔴 Atención = deudas suben o patrimonio baja.'},
  {cat:'📈 Progreso', q:'¿Cuándo se guarda el snapshot mensual?',
   a:'Automáticamente al abrir la app, una vez por mes. También puedes forzarlo con 📸 Guardar snapshot ahora dentro del módulo.'},
  {cat:'🔑 Acceso', q:'¿Cómo entran otras personas?',
   a:'El admin genera un código en Más → Códigos de Acceso. O el visitante solicita acceso y el admin aprueba desde el badge 🔴.'},
  {cat:'🔑 Acceso', q:'¿Los códigos de invitado tienen vencimiento?',
   a:'Sí. El admin define la fecha de vencimiento al crear el código. Pasada esa fecha el código deja de funcionar.'},
  {cat:'🔑 Acceso', q:'¿Olvidé mi contraseña de admin?',
   a:'Login → 🔐 Admin → "¿Olvidaste tu contraseña?". Usa la clave maestra admin1234 para recuperar el acceso.'},
  {cat:'⚙️ Config', q:'¿Cómo cambio el tema visual?',
   a:'Más → Configuración → 🎨 Cambiar tema. 5 temas: Verde Natural, Oscuro Pro, Dorado Élite, Océano y Rosa Elegante.'},
  {cat:'⚙️ Config', q:'¿Cómo cambio la moneda?',
   a:'Más → Configuración → 💱 Moneda. 9 monedas disponibles: MXN, USD, EUR, CAD, GBP, COP, ARS, GTQ, PEN.'},
  {cat:'⚙️ Config', q:'¿Cómo agrego categorías personalizadas?',
   a:'Más → Configuración → 🏷️ Mis categorías. Categorías ilimitadas para Gastos, Ingresos, Activos y Pagos fijos.'},
  {cat:'⚙️ Config', q:'¿Cómo borro mis datos?',
   a:'Más → Configuración → Zona de peligro. Borra transacciones o restablece toda la cuenta. ⚠️ No se puede deshacer.'},
  {cat:'↩️ General', q:'¿Puedo deshacer un borrado?',
   a:'Sí. Tienes 6 segundos para tocar "Deshacer". El saldo también se restaura automáticamente.'},
  {cat:'↩️ General', q:'¿Funciona sin internet?',
   a:'Sí, casi todo. Solo el reconocimiento de voz y el conversor de monedas requieren conexión.'},
  {cat:'↩️ General', q:'¿Cómo uso la calculadora?',
   a:'Toca 🔢 en la barra superior. Arrástrala, minimízala con − sin perder el cálculo, o ciérrala con ×.'},
];
(function(){
  var t = localStorage.getItem('usala_theme');
  if(t){ S.theme = t; if(typeof applyTheme === 'function') applyTheme(t); }
  if(document.readyState === 'loading'){
    document.addEventListener('DOMContentLoaded', function(){
      if(typeof arrancarApp === 'function') arrancarApp();
    });
  } else {
    if(typeof arrancarApp === 'function') arrancarApp();
  }
})();

// ─────────────────────────────────────────────
//  USALA Suite — App Core
//  js/app.js
// ─────────────────────────────────────────────

// ── Variables globales ──


// ── Sync Keys ──


function fmt(n){ return getSimboloMoneda() + Number(n||0).toLocaleString('es-MX',{minimumFractionDigits:2}); }

function today(){ return new Date().toISOString().split('T')[0]; }

function getSimboloMoneda(){
  var key = 'usala_moneda_app_' + (S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : 'anon');
  try{ var m = JSON.parse(localStorage.getItem(key)||'null'); return m ? m.simbolo : '$'; }catch(e){ return '$'; }
}


function ukey(k){
  var uid = S.user ? (S.user.isAdmin ? 'admin' : 'u_' + S.user.codigo) : 'anon';
  return 'usala_' + uid + '_' + k;
}

function load(k, def){
  try{ var v=localStorage.getItem(ukey(k)); return v!==null?JSON.parse(v):def; }catch(e){ return def; }
}

function save(k, v){
  try{ localStorage.setItem(ukey(k), JSON.stringify(v)); }catch(e){}
  if(S && S.user){ _syncQueue.push({key:k, value:v}); _schedulSync(); }
}

function _cacheGet(k){ if(_cacheTs[k] && Date.now()-_cacheTs[k]<CACHE_TTL) return _cache[k]; return null; }

function _cacheSet(k,v){ _cache[k]=v; _cacheTs[k]=Date.now(); }

function _cacheInvalid(k){ delete _cache[k]; delete _cacheTs[k]; }

function _cacheInvalidUser(){ var uc=getUCod(); Object.keys(_cache).forEach(function(k){ if(k.indexOf(uc)===0) { delete _cache[k]; delete _cacheTs[k]; } }); }

function _syncShowOverlay(show){
  var el = document.getElementById('syncLoadingOverlay');
  if(!el) return;
  el.style.display = show ? 'flex' : 'none';
}

function _syncSetProgress(msg, pct){
  var m = document.getElementById('syncLoadingMsg');
  var b = document.getElementById('syncLoadingBar');
  if(m) m.textContent = msg;
  if(b) b.style.width = pct + '%';
}

async function _flushSync(){
  if(!S.user || _syncQueue.length === 0) return;
  var uc = getUCod();
  var batch = _syncQueue.splice(0, _syncQueue.length);
  var latest = {};
  batch.forEach(function(op){ latest[op.key] = op; });
  _setSyncIndicator('syncing');
  var ok = 0, fail = 0;
  for(var key in latest){
    var op = latest[key];
    try {
      await DB.upsert('usala_kv', {
        user_codigo: uc,
        key: key,
        value: JSON.stringify(op.value),
        updated_at: new Date().toISOString()
      }, 'user_codigo,key');
      ok++;
    } catch(e) {
      _syncQueue.push(op);
      fail++;
    }
  }
  _setSyncIndicator(fail > 0 ? 'error' : 'ok');
}

async function dbRestaurarDatos(){
  var uc = getUCod();
  if(!uc){ console.warn('dbRestaurarDatos: sin usuario'); return; }
  _syncShowOverlay(true);
  _syncSetProgress('Conectando con la nube...', 10);
  try {
    // 1. Descargar TODO el KV del usuario desde Supabase
    var remote = await DB.get('usala_kv',
      'user_codigo=eq.' + encodeURIComponent(uc) + '&order=updated_at.desc');
    _syncSetProgress('Datos recibidos, aplicando...', 50);
    if(remote && remote.length > 0){
      var hayDatosRemoto = false;
      remote.forEach(function(row){
        try {
          var localKey = 'usala_' + uc + '_' + row.key;
          var localRaw = localStorage.getItem(localKey);
          var remoteVal = JSON.parse(row.value);
          var localVacio = !localRaw ||
            (function(v){ try{ var p=JSON.parse(v);
              return (Array.isArray(p)&&p.length===0)||(typeof p==='object'&&!Array.isArray(p)&&Object.keys(p||{}).length===0);
            }catch(e){ return true; } })(localRaw);
          if(localVacio){
            localStorage.setItem(localKey, row.value);
            _cacheInvalid(uc + '_kv_' + row.key);
            hayDatosRemoto = true;
          } else {
            try {
              var localVal = JSON.parse(localRaw);
              var remoteArr = Array.isArray(remoteVal) ? remoteVal : null;
              var localArr  = Array.isArray(localVal)  ? localVal  : null;
              if(remoteArr && localArr && remoteArr.length > localArr.length){
                localStorage.setItem(localKey, row.value);
                _cacheInvalid(uc + '_kv_' + row.key);
                hayDatosRemoto = true;
              }
            } catch(e){}
          }
        } catch(e){ console.warn('Error aplicando key:', row.key, e); }
      });
      _syncSetProgress(hayDatosRemoto ? 'Datos restaurados ✓' : 'Datos locales al día ✓', 80);
    } else {
      _syncSetProgress('Subiendo datos locales...', 60);
      _SYNC_KEYS.forEach(function(key){
        var raw = localStorage.getItem('usala_' + uc + '_' + key);
        if(raw){ try{
          var v = JSON.parse(raw);
          var noVacio = (Array.isArray(v)&&v.length>0)||(typeof v==='object'&&!Array.isArray(v)&&Object.keys(v||{}).length>0);
          if(noVacio) _syncQueue.push({key:key, value:v});
        }catch(e){} }
      });
      if(_syncQueue.length > 0) _flushSync();
      _syncSetProgress('Datos guardados en nube ✓', 80);
    }
    var cuentasKey = 'usala_cuentas_' + (S.user.isAdmin ? 'admin' : 'u_' + uc);
    if(!localStorage.getItem(cuentasKey)){
      var remCuentas = remote ? remote.find(function(r){ return r.key === 'cuentas'; }) : null;
      if(remCuentas){
        localStorage.setItem(cuentasKey, remCuentas.value);
      }
    }
    _syncSetProgress('Listo', 100);
    await new Promise(function(r){ setTimeout(r, 400); }); // pequeña pausa visual
  } catch(e){
    _syncSetProgress('Sin conexión — usando datos locales', 100);
    console.warn('dbRestaurarDatos offline:', e.message);
    await new Promise(function(r){ setTimeout(r, 600); });
  }
  _syncShowOverlay(false);
}

async function dbSyncFromLocal(){
  var uc = getUCod(); if(!uc) return;
  var keys = ['txs','cuentas','creditos','metas','pagos_mensuales','activos_personales',
              'presupuesto','alertas','cats_gasto_custom','cats_ingreso_custom',
              'cats_activos_custom','cats_pagos_custom','cxc'];
  console.log('🔄 Sincronizando con Supabase...');
  try {
    // 1. Bajar TODO lo que hay en remoto para este usuario
    var remote = await DB.get('usala_kv',
      'user_codigo=eq.'+encodeURIComponent(uc)+'&order=updated_at.desc');
    var remoteMap = {};
    if(remote && remote.length > 0){
      remote.forEach(function(row){ remoteMap[row.key] = row; });
    }
    keys.forEach(function(key){
      var localKey = 'usala_' + uc + '_' + key;
      var localRaw = localStorage.getItem(localKey);
      var remoteRow = remoteMap[key];
      if(remoteRow && localRaw){
        try{
          var localVal = JSON.parse(localRaw);
          var remoteVal = JSON.parse(remoteRow.value);
          var localVacio = (Array.isArray(localVal) && localVal.length===0) ||
                           (typeof localVal==='object' && !Array.isArray(localVal) && Object.keys(localVal||{}).length===0);
          if(localVacio && remoteVal){
            localStorage.setItem(localKey, remoteRow.value);
            _cacheInvalid(uc+'_kv_'+key);
            console.log('  ⬇️ Descargado desde nube:', key);
          } else {
            _syncQueue.push({key:key, value:localVal});
          }
        } catch(e){}
      } else if(remoteRow && !localRaw){
        localStorage.setItem(localKey, remoteRow.value);
        _cacheInvalid(uc+'_kv_'+key);
        console.log('  ⬇️ Descargado desde nube:', key);
      } else if(!remoteRow && localRaw){
        try{
          var v = JSON.parse(localRaw);
          var noVacio = (Array.isArray(v)&&v.length>0)||(typeof v==='object'&&!Array.isArray(v)&&Object.keys(v||{}).length>0);
          if(noVacio){ _syncQueue.push({key:key, value:v}); console.log('  ⬆️ Subiendo a nube:', key); }
        } catch(e){}
      }
    });
    if(_syncQueue.length > 0){ await _flushSync(); }
    if(remote && remote.length > 0 && S.tab){
      setTimeout(function(){ renderTab(S.tab); }, 100);
    }
    console.log('✅ Sync completo');
  } catch(e) {
    console.warn('⚠️ Sync falló (modo offline):', e.message);
  }
}

function iniciarRealtime(){
  if(_realtimeInterval) clearInterval(_realtimeInterval);
  _realtimeActivo = true;
  _lastSyncTs = new Date().toISOString();
  _realtimeTick();
  _realtimeInterval = setInterval(_realtimeTick, 30000);
  console.log('⚡ Realtime activo — sync cada 30s');
}

function _lockIniciarEscuchas(){
  ['touchstart','mousedown','keydown','scroll'].forEach(function(ev){
    document.addEventListener(ev, _lockActividad, {passive:true});
  });
}

function _lockReiniciar(){
  if(_lockTimer) clearTimeout(_lockTimer);
  var mins = getLockTimeout();
  if(!mins || _lockActivo) return;
  _lockTimer = setTimeout(function(){ _lockBloqueAhora(); }, mins * 60 * 1000);
}

function _lockVerificar(){
  var nipK = S.user.isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+S.user.codigo;
  var nip  = localStorage.getItem(nipK);
  if(nip && _lockPin === nip){
    lockDesbloquear();
  } else {
    for(var i=0;i<4;i++) document.getElementById('ld'+i).classList.add('error');
    document.getElementById('lockErr').textContent = '⚠ NIP incorrecto';
    setTimeout(function(){
      _lockPin=''; _lockActualizarDots();
      document.getElementById('lockErr').textContent='';
    }, 900);
  }
}

function getCuentas(){ return JSON.parse(localStorage.getItem('usala_cuentas_'+(S.user.isAdmin?'admin':'u_'+S.user.codigo))||'{"efectivo":0,"cheques":[],"tarjetas":[]}'); }

function saveCuentas(c){ localStorage.setItem('usala_cuentas_'+(S.user.isAdmin?'admin':'u_'+S.user.codigo), JSON.stringify(c)); }

function renderCuentas(){
  var c = getCuentas();
  var saldoEfec = (c.efectivo||0);
  var totalCheques = (c.cheques||[]).reduce(function(s,x){ return s+Number(x.saldo||0); },0);
  var totalTC = (c.tarjetas||[]).reduce(function(s,t){ return s+Number(t.balance||0); },0);
  var totalDisp = saldoEfec + totalCheques;
  var bancosHTML = (c.cheques||[]).map(function(ch){
    return '<div style="display:flex;justify-content:space-between;align-items:center;padding:10px 0;border-bottom:1px solid rgba(255,255,255,0.06);">'
      +'<div style="display:flex;align-items:center;gap:10px;">'
      +'<div style="width:32px;height:32px;border-radius:10px;background:var(--inp);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:0.9rem;">🏧</div>'
      +'<div><div style="font-weight:700;font-size:0.85rem;color:var(--text);">'+ch.banco+'</div>'
      +'<div style="font-size:0.65rem;color:var(--dim);">'+ch.tipo+'</div></div>'
      +'</div>'
      +'<div style="font-weight:800;font-size:0.92rem;color:var(--text);font-family:JetBrains Mono,monospace;">'+fmt(ch.saldo||0)+'</div>'
      +'</div>';
  }).join('') || '<div style="color:var(--dim);font-size:0.8rem;padding:10px 0;">Sin cuentas bancarias</div>';
  var tcHTML = (c.tarjetas||[]).map(function(t){
    return '<div style="display:flex;justify-content:space-between;align-items:center;padding:10px 0;border-bottom:1px solid rgba(255,255,255,0.06);">'
      +'<div style="display:flex;align-items:center;gap:10px;">'
      +'<div style="width:32px;height:32px;border-radius:10px;background:linear-gradient(135deg,rgba(255,95,87,0.2),rgba(255,95,87,0.08));border:1px solid rgba(255,95,87,0.2);display:flex;align-items:center;justify-content:center;font-size:0.9rem;">💳</div>'
      +'<div><div style="font-weight:700;font-size:0.85rem;color:var(--text);">'+t.nombre+'</div>'
      +'<div style="font-size:0.65rem;color:var(--dim);">Límite: '+fmt(t.limite||0)+'</div></div>'
      +'</div>'
      +'<div style="text-align:right;">'
      +'<div style="font-weight:800;font-size:0.92rem;color:var(--danger);font-family:JetBrains Mono,monospace;">'+fmt(t.balance||0)+'</div>'
      +'<div style="font-size:0.6rem;color:var(--dim);">deuda</div>'
      +'</div></div>';
  }).join('') || '<div style="color:var(--dim);font-size:0.8rem;padding:10px 0;">Sin tarjetas</div>';
  return ''
    +'<div class="hero-card" style="margin-bottom:16px;">'
    +'<div style="position:relative;z-index:1;">'
    +'<div class="hero-label">Total disponible</div>'
    +'<div class="hero-amount">'+fmt(totalDisp)+'</div>'
    +'<div class="hero-sub">Efectivo + Cuentas bancarias</div>'
    +'<div class="hero-pills">'
    +'<div class="hero-pill" onclick="goSub(\'efectivo\')"><span class="hero-pill-ico">💵</span>Efectivo '+fmt(saldoEfec)+'</div>'
    +'<div class="hero-pill" onclick="goSub(\'cheques\')"><span class="hero-pill-ico">🏧</span>Banco '+fmt(totalCheques)+'</div>'
    +(totalTC>0?'<div class="hero-pill" style="background:rgba(255,95,87,0.25);border-color:rgba(255,95,87,0.3);" onclick="goSub(\'tarjetas\')"><span class="hero-pill-ico">💳</span>TC '+fmt(totalTC)+'</div>':'')
    +'</div>'
    +'</div></div>'
    +'<div class="sec-title">💵 Efectivo</div>'
    +'<div class="cuenta-card">'
    +'<div class="cuenta-card-header">'
    +'<div class="cuenta-card-ico" style="background:linear-gradient(135deg,rgba(43,192,112,0.2),rgba(43,192,112,0.08));">💵</div>'
    +'<span class="cuenta-card-badge" style="background:rgba(43,192,112,0.12);color:var(--accent2);border:1px solid rgba(43,192,112,0.2);">En mano</span>'
    +'</div>'
    +'<div class="cuenta-saldo">'+fmt(saldoEfec)+'</div>'
    +'<div class="cuenta-label">Dinero físico disponible</div>'
    +'<div class="cuenta-actions">'
    +'<button class="cuenta-btn primary" onclick="goSub(\'efectivo\')">📊 Ver movimientos</button>'
    +'<button class="cuenta-btn" onclick="abrirTxModal(\'ingreso\')">➕</button>'
    +'<button class="cuenta-btn" onclick="abrirTxModal(\'gasto\')">➖</button>'
    +'</div></div>'
    +'<div class="sec-title">🏧 Banco</div>'
    +'<div class="cuenta-card">'
    +'<div class="cuenta-card-header">'
    +'<div class="cuenta-card-ico" style="background:linear-gradient(135deg,rgba(56,170,255,0.2),rgba(56,170,255,0.08));">🏧</div>'
    +'<span class="cuenta-card-badge" style="background:rgba(56,170,255,0.12);color:#60c8ff;border:1px solid rgba(56,170,255,0.2);">'+fmt(totalCheques)+'</span>'
    +'</div>'
    +'<div class="cuenta-saldo">'+fmt(totalCheques)+'</div>'
    +'<div class="cuenta-label">Total en cuentas bancarias</div>'
    +'<div style="margin-top:14px;">'+bancosHTML+'</div>'
    +'<div class="cuenta-actions">'
    +'<button class="cuenta-btn primary" onclick="goSub(\'cheques\')">📊 Ver movimientos</button>'
    +'<button class="cuenta-btn" onclick="abrirTxModal(\'ingreso\')">➕</button>'
    +'</div></div>'
    +'<div class="sec-title">💳 Tarjetas de crédito</div>'
    +'<div class="cuenta-card">'
    +'<div class="cuenta-card-header">'
    +'<div class="cuenta-card-ico" style="background:linear-gradient(135deg,rgba(255,95,87,0.2),rgba(255,95,87,0.08));">💳</div>'
    +(totalTC>0?'<span class="cuenta-card-badge" style="background:rgba(255,95,87,0.12);color:var(--danger);border:1px solid rgba(255,95,87,0.2);">Deuda '+fmt(totalTC)+'</span>':'<span class="cuenta-card-badge" style="background:rgba(43,192,112,0.12);color:var(--accent2);">✅ Al corriente</span>')
    +'</div>'
    +(totalTC>0?'<div class="cuenta-saldo" style="color:var(--danger);">'+fmt(totalTC)+'</div>':'<div class="cuenta-saldo" style="color:var(--accent2);">$0.00</div>')
    +'<div class="cuenta-label">Deuda total en tarjetas</div>'
    +'<div style="margin-top:14px;">'+tcHTML+'</div>'
    +'<div class="cuenta-actions">'
    +'<button class="cuenta-btn primary" onclick="goSub(\'tarjetas\')">💳 Ver tarjetas</button>'
    +'</div></div>';
}

function renderEfectivo(){
  var c = getCuentas();
  var txs = getTxs().filter(function(t){ return t.cuenta==='efectivo'; });
  var items = txs.slice().reverse().map(function(t){
    return '<div class="tx-item">'
      +'<div class="tx-ico">'+(t.tipo==='ingreso'?'💵':'💸')+'</div>'
      +'<div class="tx-info"><div class="tx-name">'+t.desc+'</div>'
      +'<div class="tx-date">'+t.fecha+' · '+t.cat+'</div></div>'
      +'<div class="tx-right"><div class="tx-amt '+(t.tipo==='ingreso'?'ing':'gas')+'">'
      +(t.tipo==='ingreso'?'+':'-')+fmt(t.monto)+'</div>'
      +'<div style="display:flex;gap:4px;">'
      +'<button class="ic-btn" onclick="editarTx(\"'+t.id+'\")"  >✏️</button>'
      +'<button class="ic-btn" onclick="borrarTx(\"'+t.id+'\")"  >🗑️</button>'
      +'</div></div></div>';
  }).join('')||'<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin movimientos</div>';
  var catEnt = getIngresoCats();
  var catSal = getGastoCats();
  return '<div class="page-header">'+backBtn('cuentas',1)+'<div class="page-title">💵 Efectivo</div></div>'
    +'<div class="card" style="margin-bottom:14px;text-align:center;padding:22px;">'
    +'<div style="font-size:0.65rem;font-weight:700;color:var(--dim);letter-spacing:0.1em;text-transform:uppercase;margin-bottom:6px;">Saldo en efectivo</div>'
    +'<div style="font-size:2.4rem;font-weight:900;color:var(--accent);">'+fmt(c.efectivo||0)+'</div>'
    +'</div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<div class="card-title">Registrar movimiento</div>'
    +'<div class="tipo-selector" style="margin-bottom:12px;">'
    +'<div class="tipo-opt selected" id="efTipoEnt" onclick="selEfTipo(\'ingreso\')">💵 Entrada (ingreso)</div>'
    +'<div class="tipo-opt" id="efTipoSal" onclick="selEfTipo(\'gasto\')">💸 Salida (gasto)</div>'
    +'</div>'
    +'<label class="inp-label">Descripción</label>'
    +'<input class="inp" id="efDesc" placeholder="Ej: Cobré trabajo / Compré despensa" autocomplete="off">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Monto ($)</label><input class="inp" id="efMonto" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'<div><label class="inp-label">Categoría</label>'
    +'<select class="inp" id="efCat">'
    + catEnt.map(function(cat){ return '<option>'+cat+'</option>'; }).join('')
    +'</select>'
    +'<button type="button" class="cat-add-btn" id="efCatAddBtn" onclick="abrirCatModalEf()">＋ Categoría</button></div>'
    +'</div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="efFecha" type="date" value="'+today()+'">'
    +'<div id="efDestRow" style="display:none;">'
    +'<label class="inp-label">¿A qué banco? (opcional)</label>'
    +'<select class="inp" id="efDestBanco"><option value="">— Solo registrar salida —</option>'
    + (c.cheques||[]).map(function(ch,i){ return '<option value="cheque_'+i+'">🏦 '+ch.banco+'</option>'; }).join('')
    +'</select></div>'
    +'<button class="btn-main" onclick="guardarMovEfectivo()">💾 Guardar</button>'
    +'</div>'
    +'<div class="card"><div class="card-title">Movimientos ('+txs.length+')</div>'+items+'</div>';
}

function renderCheques(){
  var c=getCuentas(); var cuentas=c.cheques||[];
  var total=cuentas.reduce(function(s,x){ return s+Number(x.saldo||0); },0);
  var items=cuentas.length ? cuentas.map(function(ct,i){
    var cval='cheque_'+i;
    var txsCuenta=getTxs().filter(function(t){ return t.cuenta===cval; });
    var ultMov=txsCuenta.length ? txsCuenta[txsCuenta.length-1] : null;
    return '<div class="cred-item" onclick="goSub(\'banco_\'+'+i+')" style="cursor:pointer;">'
      +'<div class="cred-top"><div><div class="cred-persona">🏧 '+ct.banco+'</div>'
      +'<div class="cred-desc">'+ct.tipo+(ct.numCuenta?' · ***'+ct.numCuenta.slice(-4):'')+(ultMov?' · Último mov: '+ultMov.fecha:'')+'</div></div>'
      +'<div><div style="font-size:1.1rem;font-weight:900;color:var(--accent);">'+fmt(ct.saldo||0)+'</div>'
      +'<div style="font-size:0.62rem;color:var(--dim);text-align:right;">'+txsCuenta.length+' mov.</div></div></div>'
      +(ct.nota?'<div style="font-size:0.72rem;color:var(--dim);margin-top:2px;">📝 '+ct.nota+'</div>':'')
      +'</div>';
  }).join('') : '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin cuentas bancarias. Agrega una abajo.</div>';
  return '<div class="page-header">'+backBtn('cuentas',1)+'<div class="page-title">🏧 Mis Bancos</div></div>'
    +'<div class="card" style="text-align:center;padding:18px;margin-bottom:14px;">'
    +'<div style="font-size:0.65rem;font-weight:700;color:var(--dim);letter-spacing:0.1em;text-transform:uppercase;margin-bottom:6px;">Total en bancos</div>'
    +'<div style="font-size:2rem;font-weight:900;color:var(--accent);">'+fmt(total)+'</div>'
    +'</div>'
    + items
    +'<div class="card" style="margin-top:14px;" id="chequesForm">'
    +'<div class="card-title" id="chFormTitle">+ Agregar cuenta bancaria</div>'
    +'<label class="inp-label">Banco / Institución</label>'
    +'<input class="inp" id="chBanco" placeholder="Ej: BBVA, Santander, HSBC...">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Tipo</label>'
    +'<select class="inp" id="chTipo"><option>Débito</option><option>Ahorro</option><option>Nómina</option><option>Inversión</option><option>Otro</option></select></div>'
    +'<div><label class="inp-label">Saldo inicial ($)</label><input class="inp" id="chSaldo" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'</div>'
    +'<label class="inp-label">No. cuenta (últimos 4 dígitos)</label>'
    +'<input class="inp" id="chNum" placeholder="Ej: 4521" maxlength="4" inputmode="numeric">'
    +'<label class="inp-label">Nota (opcional)</label>'
    +'<input class="inp" id="chNota" placeholder="Ej: Cuenta de nómina principal">'
    +'<button class="btn-main" id="chSaveBtn" onclick="guardarCuenta()">💾 Guardar cuenta</button>'
    +'</div>';
}

function renderBancoDetalle(idx){
  var c=getCuentas(); var ct=c.cheques[idx];
  if(!ct) return renderCheques();
  var cval='cheque_'+idx;
  var txs=getTxs().filter(function(t){ return t.cuenta===cval; });
  var catEnt=['Salario','Depósito','Transferencia recibida','Nómina','Inversión','Otros ingresos'];
  var catSal=getGastoCats();
  var items=txs.slice().reverse().map(function(t){
    return '<div class="tx-item">'
      +'<div class="tx-ico">'+(t.tipo==='ingreso'?'📥':'📤')+'</div>'
      +'<div class="tx-info"><div class="tx-name">'+t.desc+'</div>'
      +'<div class="tx-date">'+t.fecha+' · '+t.cat+'</div></div>'
      +'<div class="tx-right"><div class="tx-amt '+(t.tipo==='ingreso'?'ing':'gas')+'">'
      +(t.tipo==='ingreso'?'+':'-')+fmt(t.monto)+'</div>'
      +'<button class="ic-btn" onclick="borrarTxBanco(\"'+t.id+'\",'+idx+')">🗑️</button></div></div>';
  }).join('')||'<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin movimientos</div>';
  return '<div class="page-header">'+backBtn('cheques',1)+'<div class="page-title">🏧 '+ct.banco+'</div></div>'
    +'<div class="card" style="text-align:center;padding:18px;margin-bottom:14px;">'
    +'<div style="font-size:0.65rem;font-weight:700;color:var(--dim);letter-spacing:0.1em;text-transform:uppercase;margin-bottom:4px;">Saldo</div>'
    +'<div style="font-size:2.2rem;font-weight:900;color:var(--accent);">'+fmt(ct.saldo||0)+'</div>'
    +'<div style="font-size:0.7rem;color:var(--dim);margin-top:4px;">'+ct.tipo+(ct.numCuenta?' · ***'+ct.numCuenta:'')+'</div>'
    +'<div style="display:flex;gap:8px;justify-content:center;margin-top:10px;">'
    +'<button class="cred-btn" onclick="editarCuenta('+idx+');goSub(\'cheques\')">✏️ Editar</button>'
    +'<button class="cred-btn danger" onclick="borrarCuenta('+idx+')">🗑️ Eliminar</button>'
    +'</div></div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<div class="card-title">Registrar movimiento</div>'
    +'<div class="tipo-selector" style="margin-bottom:12px;">'
    +'<div class="tipo-opt selected" id="bkTipoEnt" onclick="selBkTipo(\'ingreso\','+idx+')">📥 Entrada</div>'
    +'<div class="tipo-opt" id="bkTipoSal" onclick="selBkTipo(\'gasto\','+idx+')">📤 Salida</div>'
    +'</div>'
    +'<label class="inp-label">Descripción</label>'
    +'<input class="inp" id="bkDesc" placeholder="Ej: Nómina quincenal / Pago luz" autocomplete="off">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Monto ($)</label><input class="inp" id="bkMonto" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'<div><label class="inp-label">Categoría</label>'
    +'<select class="inp" id="bkCat">'
    +catEnt.map(function(cat){ return '<option>'+cat+'</option>'; }).join('')
    +'</select><button type="button" class="cat-add-btn" id="bkCatAddBtn" onclick="abrirCatModalBk()">＋ Categoría</button></div></div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="bkFecha" type="date" value="'+today()+'">'
    +'<button class="btn-main" onclick="guardarMovBanco('+idx+')">💾 Guardar</button>'
    +'</div>'
    +'<div class="card"><div class="card-title">Movimientos ('+txs.length+')</div>'+items+'</div>';
}

function borrarTxBanco(id,idx){
  var txs=getTxs(); var t=txs.find(function(x){ return x.id===id; });
  if(!t) return;
  var _eliT=JSON.parse(JSON.stringify(t));
  var c=getCuentas();
  c.cheques[idx].saldo=(c.cheques[idx].saldo||0)-(t.tipo==='ingreso'?t.monto:-t.monto);
  saveCuentas(c);
  saveTxs(txs.filter(function(x){ return x.id!==id; }));
  goSub('banco_'+idx);
  mostrarUndo('🏧 Movimiento eliminado', function(){
    var c2=getCuentas();
    c2.cheques[idx].saldo=(c2.cheques[idx].saldo||0)+(_eliT.tipo==='ingreso'?_eliT.monto:-_eliT.monto);
    saveCuentas(c2);
    var t2=getTxs(); t2.push(_eliT); saveTxs(t2);
    goSub('banco_'+idx);
  });
}

function guardarCuenta(){
  var banco=document.getElementById('chBanco').value.trim();
  var tipo=document.getElementById('chTipo').value;
  var saldo=parseFloat(document.getElementById('chSaldo').value)||0;
  var num=document.getElementById('chNum').value.trim();
  var nota=document.getElementById('chNota').value.trim();
  if(!banco){ showToast('⚠ Escribe el nombre del banco'); return; }
  var c=getCuentas(); c.cheques=c.cheques||[];
  if(_editCuentaIdx!==null){
    c.cheques[_editCuentaIdx]=Object.assign(c.cheques[_editCuentaIdx],{banco:banco,tipo:tipo,saldo:saldo,numCuenta:num,nota:nota});
    _editCuentaIdx=null; showToast('✓ Cuenta actualizada');
  } else {
    c.cheques.push({banco:banco,tipo:tipo,saldo:saldo,numCuenta:num,nota:nota});
    showToast('✓ Cuenta bancaria agregada');
  }
  saveCuentas(c); goSub('cheques');
}

function editarCuenta(i){
  var c=getCuentas(); var ct=c.cheques[i]; _editCuentaIdx=i;
  goSub('cheques');
  setTimeout(function(){
    document.getElementById('chBanco').value=ct.banco;
    document.getElementById('chTipo').value=ct.tipo;
    document.getElementById('chSaldo').value=ct.saldo||0;
    document.getElementById('chNum').value=ct.numCuenta||'';
    document.getElementById('chNota').value=ct.nota||'';
    document.getElementById('chFormTitle').textContent='✏️ Editar cuenta';
    document.getElementById('chSaveBtn').textContent='💾 Guardar cambios';
    document.getElementById('chequesForm').scrollIntoView({behavior:'smooth'});
  },100);
}

function borrarCuenta(i){
  var c=getCuentas(); var _eliBanco=JSON.parse(JSON.stringify(c.cheques[i]));
  c.cheques.splice(i,1); saveCuentas(c); goSub('cheques');
  mostrarUndo('🏧 Cuenta eliminada', function(){
    var c2=getCuentas(); c2.cheques.splice(i,0,_eliBanco); saveCuentas(c2); goSub('cheques');
  });
}

function abonarCuenta(i){
  var c=getCuentas(); var ct=c.cheques[i];
  usalaPrompt('Ajustar saldo de '+ct.banco+' ($)', String(ct.saldo||0), function(val){
    var nuevo=parseFloat(val);
    if(isNaN(nuevo)){ showToast('Ingresa un monto valido'); return; }
    c.cheques[i].saldo=nuevo; saveCuentas(c);
    showToast('Saldo actualizado'); goSub('banco_'+i);
  },{type:'number', placeholder:'0.00'});
}

function renderPagosMes(){
  var mc = document.getElementById('mainContent');
  mc.innerHTML = '';
  var pagos  = loadPagosBase();
  var estado = loadPagosEstado();
  var hoy    = new Date(); hoy.setHours(0,0,0,0);
  var mesActKey = new Date().toISOString().slice(0,7);
  var mesNombre = hoy.toLocaleString('es-MX',{month:'long',year:'numeric'});
  // Helpers definidos primero para que todo el scope los vea
  function _calcFechaVenc(p, ref){
    if(p.proximoPago){
      var pts=p.proximoPago.split('-');
      return new Date(+pts[0],+pts[1]-1,+pts[2]);
    }
    var dia = Math.min(p.dia||1, 28);
    var f = new Date(ref.getFullYear(), ref.getMonth(), dia);
    f.setHours(0,0,0,0);
    if(f < ref) f.setMonth(f.getMonth()+1);
    return f;
  }
  function _diasLabel(diff){
    if(diff<0)  return {txt:'Vencido hace '+Math.abs(diff)+' día'+(Math.abs(diff)!==1?'s':''), col:'#e53935', bg:'rgba(229,57,53,0.08)'};
    if(diff===0)return {txt:'Vence HOY',     col:'#e53935', bg:'rgba(229,57,53,0.1)'};
    if(diff===1)return {txt:'Vence mañana',  col:'#f57c00', bg:'rgba(245,124,0,0.08)'};
    if(diff<=3) return {txt:'En '+diff+' días', col:'#f57c00', bg:'rgba(245,124,0,0.06)'};
    if(diff<=7) return {txt:'En '+diff+' días', col:'#f9a825', bg:'rgba(249,168,37,0.07)'};
    return      {txt:'Día '+diff, col:'var(--dim)', bg:'transparent'};
  }
  var hdr = document.createElement('div');
  hdr.innerHTML = '<div class="page-header">'+backSubBtn()+'<div class="page-title">📅 Pagos del Mes</div></div>';
  mc.appendChild(hdr);
  var totalMonto  = pagos.reduce(function(s,p){ return s+(p.monto||0); },0);
  var pagados     = pagos.filter(function(p){ return estado[p.id]&&estado[p.id].pagado; });
  var totalPagado = pagados.reduce(function(s,p){ return s+(estado[p.id].montoPagado||p.monto||0); },0);
  var pct         = totalMonto>0 ? Math.min(100,Math.round((totalPagado/totalMonto)*100)) : 0;
  var pendientes  = pagos.filter(function(p){ return !estado[p.id]||!estado[p.id].pagado; });
  var masUrgente = null;
  pendientes.forEach(function(p){
    var f = _calcFechaVenc(p, hoy);
    var d = Math.round((f-hoy)/86400000);
    if(masUrgente===null || d < masUrgente) masUrgente = d;
  });
  var alertaTxt = '';
  if(masUrgente!==null){
    var _nVencidos=pendientes.filter(function(p){ return Math.round((_calcFechaVenc(p,hoy)-hoy)/86400000)<0; }).length;
    if(masUrgente<0)       alertaTxt='⚠️ Tienes '+_nVencidos+' pago'+(_nVencidos!==1?'s':'')+' vencido'+(_nVencidos!==1?'s':'');
    else if(masUrgente===0) alertaTxt='📍 Tienes pagos que vencen HOY';
    else if(masUrgente===1) alertaTxt='⏰ Tu próximo pago vence MAÑANA';
    else if(masUrgente<=3)  alertaTxt='⏰ Próximo vencimiento en '+masUrgente+' días';
  }
  var res = document.createElement('div');
  res.className='card'; res.style.marginBottom='10px';
  res.innerHTML =
    '<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;">'
      +'<div style="font-size:0.8rem;font-weight:800;text-transform:capitalize;">'+mesNombre+'</div>'
      +'<div style="font-size:0.75rem;color:var(--dim);">'+pagados.length+' / '+pagos.length+' pagados</div>'
    +'</div>'
    +'<div class="prog-wrap" style="margin-bottom:8px;"><div class="prog-bar" style="width:'+pct+'%;'+(pct>=100?'background:#2d9e5f;':'')+'"></div></div>'
    +'<div style="display:flex;justify-content:space-between;font-size:0.78rem;">'
      +'<span style="color:var(--dim);">Total: <b>'+fmt(totalMonto)+'</b></span>'
      +'<span style="color:var(--accent2);">Pagado: <b>'+fmt(totalPagado)+'</b></span>'
    +'</div>'
    +(totalMonto-totalPagado>0?'<div style="font-size:0.75rem;margin-top:4px;color:var(--danger);">Pendiente: <b>'+fmt(totalMonto-totalPagado)+'</b></div>':'')
    +(alertaTxt?'<div style="margin-top:10px;padding:8px 12px;border-radius:10px;background:rgba(229,57,53,0.08);border:1px solid rgba(229,57,53,0.2);font-size:0.75rem;font-weight:700;color:#e53935;">'+alertaTxt+'</div>':'');
  mc.appendChild(res);
  var tabState = {active: 'pendientes'};
  var tabWrap = document.createElement('div');
  tabWrap.style.cssText='display:flex;gap:6px;margin-bottom:14px;overflow-x:auto;-webkit-overflow-scrolling:touch;padding-bottom:2px;';
  tabWrap.innerHTML =
    '<button class="pp-tab active" id="pmTab_pend" onclick="pmSetTab(\'pendientes\')">⏳ Pendientes ('+pendientes.length+')</button>'
    +'<button class="pp-tab" id="pmTab_pag"  onclick="pmSetTab(\'pagados\')">✅ Pagados ('+pagados.length+')</button>'
    +'<button class="pp-tab" id="pmTab_hist" onclick="pmSetTab(\'historial\')">📚 Historial</button>';
  mc.appendChild(tabWrap);
  var bAdd = document.createElement('button');
  bAdd.style.cssText='width:100%;padding:13px;background:var(--accent);color:var(--navtext);border:none;border-radius:12px;font-family:\'Outfit\',sans-serif;font-weight:700;cursor:pointer;margin-bottom:14px;font-size:0.95rem;';
  bAdd.textContent='+ Agregar pago fijo';
  bAdd.onclick=function(){ renderFormPago(null); };
  mc.appendChild(bAdd);
  var listaCont = document.createElement('div');
  listaCont.id = 'pmListaCont';
  mc.appendChild(listaCont);
  function renderPendientes(){
    var cont = document.getElementById('pmListaCont');
    if(!cont) return;
    cont.innerHTML='';
    if(!pagos.length){
      cont.innerHTML='<div style="text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;">Sin pagos registrados. Agrega tus pagos fijos del mes.</div>';
      return;
    }
    var pends = pagos.filter(function(p){ return !estado[p.id]||!estado[p.id].pagado; });
    pends.sort(function(a,b){
      return _calcFechaVenc(a,hoy) - _calcFechaVenc(b,hoy);
    });
    if(!pends.length){
      cont.innerHTML='<div style="text-align:center;padding:30px;color:var(--accent2);font-size:0.83rem;">🎉 ¡Todos los pagos de este mes están al corriente!</div>';
      return;
    }
    pends.forEach(function(p){
      var f    = _calcFechaVenc(p, hoy);
      var diff = Math.round((f-hoy)/86400000);
      var lbl  = _diasLabel(diff); lbl.p = p;
      var idx  = pagos.indexOf(p);
      cont.appendChild(_mkPagoCard(p, idx, f, diff, lbl, false));
    });
  }
  function renderPagadosMes(){
    var cont = document.getElementById('pmListaCont');
    if(!cont) return;
    cont.innerHTML='';
    var pags = pagos.filter(function(p){ return estado[p.id]&&estado[p.id].pagado; });
    pags.sort(function(a,b){
      var fa=estado[a.id].fecha||''; var fb=estado[b.id].fecha||'';
      return fb.localeCompare(fa); // más reciente primero
    });
    if(!pags.length){
      cont.innerHTML='<div style="text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;">Aún no hay pagos marcados como pagados este mes.</div>';
      return;
    }
    pags.forEach(function(p){
      var st  = estado[p.id];
      var idx = pagos.indexOf(p);
      var f   = st.fecha ? (function(){ var pts=st.fecha.split('-'); return new Date(+pts[0],+pts[1]-1,+pts[2]); })() : hoy;
      var lbl = {txt:'Pagado el '+f.toLocaleDateString('es-MX',{day:'numeric',month:'short'}), col:'var(--accent2)', bg:'rgba(45,158,95,0.06)'};
      cont.appendChild(_mkPagoCard(p, idx, f, null, lbl, true));
    });
  }
  function renderHistorialPagos(){
    var cont = document.getElementById('pmListaCont');
    if(!cont) return;
    cont.innerHTML='';
    // Recolectar todos los meses con estado guardado
    var u    = S.user;
    var base = u ? (u.isAdmin?'usala_admin':'usala_u_'+u.codigo) : 'usala_admin';
    var prefix = base+'_pagos_estado_';
    var mesesGuardados = [];
    for(var k in localStorage){
      if(k.indexOf(prefix)===0){
        var mesK = k.replace(prefix,'');
        mesesGuardados.push(mesK);
      }
    }
    mesesGuardados.sort().reverse(); // más reciente primero
    if(!mesesGuardados.length){
      cont.innerHTML='<div style="text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;">El historial se irá construyendo mes a mes conforme marques pagos.</div>';
      return;
    }
    var _mesesNombres=['Enero','Febrero','Marzo','Abril','Mayo','Junio','Julio','Agosto','Septiembre','Octubre','Noviembre','Diciembre'];
    mesesGuardados.forEach(function(mesK){
      var estadoMes;
      try{ estadoMes=JSON.parse(localStorage.getItem(prefix+mesK)||'{}'); }catch(e){ estadoMes={}; }
      var pagosEseMes = Object.keys(estadoMes);
      if(!pagosEseMes.length) return;
      var parts  = mesK.split('-');
      var yr     = parts[0]; var mn = parseInt(parts[1],10)-1;
      var mesLabel = _mesesNombres[mn]+' '+yr;
      var esMesAct = mesK===mesActKey;
      var totalPagMes  = 0;
      var totalEstMes  = 0;
      var countPag     = 0;
      pagosEseMes.forEach(function(pid){
        var st  = estadoMes[pid];
        var pag = pagos.find(function(p){ return p.id==pid; });
        if(!pag) return;
        totalEstMes += pag.monto||0;
        if(st&&st.pagado){ totalPagMes+=(st.montoPagado||pag.monto||0); countPag++; }
      });
      var secDiv = document.createElement('div');
      secDiv.style.cssText='margin-bottom:16px;';
      var secHdr = document.createElement('div');
      secHdr.style.cssText='display:flex;justify-content:space-between;align-items:center;padding:10px 14px;background:var(--inp);border-radius:12px;margin-bottom:8px;cursor:pointer;';
      secHdr.innerHTML =
        '<div>'
          +'<div style="font-weight:800;font-size:0.88rem;text-transform:capitalize;">'
            +(esMesAct?'📍 ':'')+ mesLabel
          +'</div>'
          +'<div style="font-size:0.7rem;color:var(--dim);margin-top:1px;">'+countPag+' pagado'+(countPag!==1?'s':'')+' · '+fmt(totalPagMes)+'</div>'
        +'</div>'
        +'<div style="text-align:right;">'
          +'<div style="font-weight:900;font-size:0.92rem;color:var(--accent2);">'+fmt(totalPagMes)+'</div>'
          +'<div style="font-size:0.68rem;color:var(--dim);">de '+fmt(totalEstMes)+'</div>'
        +'</div>';
      var detalleDiv = document.createElement('div');
      detalleDiv.style.display = esMesAct ? 'block' : 'none';
      secHdr.onclick = function(){
        detalleDiv.style.display = detalleDiv.style.display==='none'?'block':'none';
      };
      pagosEseMes.forEach(function(pid){
        var st  = estadoMes[pid];
        var pag = pagos.find(function(p){ return p.id==pid; });
        if(!pag) return;
        var row = document.createElement('div');
        row.style.cssText='display:flex;justify-content:space-between;align-items:center;padding:8px 10px;border-bottom:1px solid var(--border);';
        var pagadoOk = st&&st.pagado;
        row.innerHTML =
          '<div style="flex:1;">'
            +'<div style="font-size:0.82rem;font-weight:600;'+(pagadoOk?'':'color:var(--dim);')+'">'+(pagadoOk?'✅ ':'⏳ ')+pag.nombre+'</div>'
            +(pagadoOk&&st.fecha?'<div style="font-size:0.68rem;color:var(--dim);">Pagado el '+st.fecha+'</div>':'')
          +'</div>'
          +'<div style="font-weight:800;font-size:0.85rem;color:'+(pagadoOk?'var(--accent2)':'var(--danger)')+';">'
            +fmt(pagadoOk?(st.montoPagado||pag.monto||0):(pag.monto||0))
          +'</div>';
        detalleDiv.appendChild(row);
      });
      secDiv.appendChild(secHdr);
      secDiv.appendChild(detalleDiv);
      cont.appendChild(secDiv);
    });
  }
  function _mkPagoCard(p, idx, f, diff, lbl, esPagado){
    var st  = estado[p.id]||{};
    var card = document.createElement('div');
    card.style.cssText='background:var(--card);border-radius:14px;padding:0;margin-bottom:8px;'
      +'border:1.5px solid '+(esPagado?'rgba(45,158,95,0.3)':diff!==null&&diff<=1?'rgba(229,57,53,0.4)':diff!==null&&diff<=3?'rgba(245,124,0,0.35)':'var(--border)')
      +';overflow:hidden;';
    var inner = document.createElement('div');
    inner.style.cssText='display:flex;';
    var barra = document.createElement('div');
    barra.style.cssText='width:4px;background:'+(esPagado?'#2d9e5f':lbl.col)+';flex-shrink:0;';
    var cuerpo = document.createElement('div');
    cuerpo.style.cssText='flex:1;padding:12px 12px 12px 10px;opacity:'+(esPagado?'0.8':'1')+';';
    var topRow = document.createElement('div');
    topRow.style.cssText='display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:4px;';
    var left = document.createElement('div'); left.style.flex='1';
    var nombre = document.createElement('div');
    nombre.style.cssText='font-weight:800;font-size:0.9rem;'+(esPagado?'color:var(--dim);text-decoration:line-through;':'');
    nombre.textContent=p.nombre;
    left.appendChild(nombre);
    var badge = document.createElement('div');
    badge.style.cssText='display:inline-block;font-size:0.65rem;font-weight:800;padding:2px 8px;border-radius:20px;margin-top:4px;background:'+lbl.bg+';color:'+lbl.col+';';
    badge.textContent = lbl.txt;
    left.appendChild(badge);
    var fMeta = document.createElement('div');
    fMeta.style.cssText='font-size:0.68rem;color:var(--dim);margin-top:3px;';
    var fStr = f.toLocaleDateString('es-MX',{day:'numeric',month:'short',year:'numeric'});
    fMeta.textContent = (p.categoria||'')+' · '+fStr+(p.frecuencia&&p.frecuencia!=='mensual'?' · '+p.frecuencia:'');
    left.appendChild(fMeta);
    topRow.appendChild(left);
    var montoCol = esPagado?'var(--accent2)':diff!==null&&diff<=1?'#e53935':'var(--danger)';
    var montoDiv = document.createElement('div');
    montoDiv.style.cssText='font-weight:900;font-size:1rem;font-family:\'JetBrains Mono\',monospace;color:'+montoCol+';margin-left:8px;';
    montoDiv.textContent=fmt(esPagado?(st.montoPagado||p.monto||0):p.monto);
    topRow.appendChild(montoDiv);
    cuerpo.appendChild(topRow);
    var btns=document.createElement('div');
    btns.style.cssText='display:flex;gap:6px;margin-top:8px;';
    var bPag=document.createElement('button');
    bPag.style.cssText='flex:1;border:none;border-radius:8px;padding:6px 0;font-size:0.75rem;cursor:pointer;font-weight:700;font-family:\'Outfit\',sans-serif;background:'+(esPagado?'var(--inp)':'#2d9e5f')+';color:'+(esPagado?'var(--dim)':'#fff')+';';
    bPag.textContent=esPagado?'↩ Desmarcar':'✅ Marcar pagado';
    (function(pid,pmonto,pagado_){
      bPag.onclick=function(){
        if(pagado_){ var e2=loadPagosEstado(); delete e2[pid]; savePagosEstado(e2); renderPagosMes(); }
        else{ renderPagarPago(pid,pmonto); }
      };
    })(p.id,p.monto,esPagado);
    btns.appendChild(bPag);
    var bEd=document.createElement('button');
    bEd.style.cssText='border:1px solid var(--border);border-radius:8px;padding:6px 10px;font-size:0.75rem;cursor:pointer;background:none;color:var(--accent);';
    bEd.textContent='✏️';
    (function(i){ bEd.onclick=function(){ renderFormPago(i); }; })(idx);
    btns.appendChild(bEd);
    var bDel=document.createElement('button');
    bDel.style.cssText='border:1px solid rgba(229,57,53,0.3);border-radius:8px;padding:6px 10px;font-size:0.75rem;cursor:pointer;background:none;color:var(--danger);';
    bDel.textContent='🗑';
    (function(i){ bDel.onclick=function(){ borrarPago(i); }; })(idx);
    btns.appendChild(bDel);
    cuerpo.appendChild(btns);
    inner.appendChild(barra);
    inner.appendChild(cuerpo);
    card.appendChild(inner);
    return card;
  }
  // pmSetTab es función global
  renderPendientes();
}

function pmSetTab(tab){
  ['pend','pag','hist'].forEach(function(t){
    var el=document.getElementById('pmTab_'+t);
    if(el){ el.classList.remove('active'); el.classList.remove('pp-tab-active'); }
  });
  var mapId={pendientes:'pend', pagados:'pag', historial:'hist'};
  var activeEl = document.getElementById('pmTab_'+(mapId[tab]||tab));
  if(activeEl){ activeEl.classList.add('active'); activeEl.classList.add('pp-tab-active'); }
  var cont = document.getElementById('pmListaCont');
  if(!cont) return;
  if(tab==='pendientes'){
    var pendientes = loadPagosBase().filter(function(p){ return !_estaPagado(p.nombre); });
    cont.innerHTML = renderPendientes(pendientes);
  } else if(tab==='pagados'){
    var pagados = loadPagosBase().filter(function(p){ return _estaPagado(p.nombre); });
    cont.innerHTML = renderPagadosMes(pagados);
  } else {
    cont.innerHTML = renderHistorialPagos();
  }
}

function renderFormPago(idx){
  var pagos=loadPagosBase();
  var p=idx!==null?pagos[idx]:{};
  var mc=document.getElementById('mainContent');
  mc.innerHTML='';
  var d=document.createElement('div'); d.style.padding='20px 16px';
  var catOpts=getPagosCats().map(function(c){
    return '<option value="'+c+'"'+(p.categoria===c?' selected':'')+'>'+c+'</option>';
  }).join('');
  d.innerHTML='<div style="font-size:1rem;font-weight:800;margin-bottom:14px;">'+(idx!==null?'✏️ Editar':'➕ Nuevo')+' Pago Fijo</div>'
    +'<label class="inp-label">Nombre del pago</label>'
    +'<input class="inp" id="fpNombre" placeholder="Ej: CFE, TELMEX, Renta..." value="'+(p.nombre||'')+'">'
    +'<label class="inp-label">Categoría</label>'
    +'<select class="inp" id="fpCat">'+catOpts+'</select>'
    +'<button type="button" class="cat-add-btn" onclick="abrirCatModal(\'pagos\',\'fpCat\')">＋ Categoría</button>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Monto estimado</label><input class="inp" id="fpMonto" type="number" min="0" placeholder="$0.00" value="'+(p.monto||'')+'"></div>'
    +'<div><label class="inp-label">Día de vencimiento</label><input class="inp" id="fpDia" type="number" min="1" max="31" placeholder="15" value="'+(p.dia||'')+'"></div>'
    +'</div>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Frecuencia</label>'
    +'<select class="inp" id="fpFrec">'
    +'<option value="mensual"'+((!p.frecuencia||p.frecuencia==="mensual")?" selected":"")+'>Mensual</option>'
    +'<option value="bimestral"'+(p.frecuencia==="bimestral"?" selected":"")+'>Bimestral (c/2 meses)</option>'
    +'<option value="trimestral"'+(p.frecuencia==="trimestral"?" selected":"")+'>Trimestral (c/3 meses)</option>'
    +'<option value="cuatrimestral"'+(p.frecuencia==="cuatrimestral"?" selected":"")+'>Cuatrimestral (c/4 meses)</option>'
    +'<option value="semestral"'+(p.frecuencia==="semestral"?" selected":"")+'>Semestral (c/6 meses)</option>'
    +'<option value="anual"'+(p.frecuencia==="anual"?" selected":"")+'>Anual</option>'
    +'</select></div>'
    +'<div><label class="inp-label">Próximo pago</label>'
    +'<input class="inp" id="fpProximo" type="date" value="'+(p.proximoPago||today())+'">'
    +'</div>'
    +'</div>'
    +'<label class="inp-label">Notas (opcional)</label>'
    +'<input class="inp" id="fpNotas" placeholder="Cuenta, referencia, etc." value="'+(p.notas||'')+'" style="margin-bottom:16px;">';
  var bOk=document.createElement('button');
  bOk.className='btn-main'; bOk.textContent=idx!==null?'💾 Guardar cambios':'➕ Agregar';
  bOk.onclick=function(){
    var nombre=document.getElementById('fpNombre').value.trim();
    var cat=document.getElementById('fpCat').value;
    var monto=parseFloat(document.getElementById('fpMonto').value)||0;
    var dia=parseInt(document.getElementById('fpDia').value)||1;
    var notas=document.getElementById('fpNotas').value.trim();
    var frec=document.getElementById('fpFrec')?document.getElementById('fpFrec').value:'mensual';
    var proximo=document.getElementById('fpProximo')?document.getElementById('fpProximo').value:'';
    if(!nombre||!monto){ showToast('⚠ Nombre y monto son obligatorios'); return; }
    var pp=loadPagosBase();
    if(idx!==null){
      pp[idx].nombre=nombre; pp[idx].categoria=cat; pp[idx].monto=monto; pp[idx].dia=dia;
      pp[idx].notas=notas; pp[idx].frecuencia=frec; pp[idx].proximoPago=proximo;
      showToast('✓ Actualizado');
    } else {
      pp.push({id:'pm_'+Date.now(),nombre:nombre,categoria:cat,monto:monto,dia:dia,
               notas:notas,frecuencia:frec,proximoPago:proximo});
      showToast('✓ Pago agregado');
    }
    savePagosBase(pp); renderPagosMes();
  };
  var bCan=document.createElement('button');
  bCan.className='btn-sec'; bCan.style.marginTop='8px'; bCan.textContent='Cancelar';
  bCan.onclick=function(){ renderPagosMes(); };
  d.appendChild(bOk); d.appendChild(bCan);
  mc.appendChild(d);
  setTimeout(function(){ var el=document.getElementById('fpNombre'); if(el) el.focus(); },80);
}

function renderPagarPago(pid, montoEst){
  var mc = document.getElementById('mainContent');
  mc.innerHTML='';
  var d=document.createElement('div'); d.style.padding='20px 16px';
  d.innerHTML='<div style="font-size:1rem;font-weight:800;margin-bottom:14px;">✅ Registrar Pago</div>'
    +'<label class="inp-label">Monto pagado</label>'
    +'<input class="inp" id="pmPagado" type="number" min="0" placeholder="'+montoEst+'" style="margin-bottom:16px;">';
  var bOk=document.createElement('button');
  bOk.className='btn-main'; bOk.textContent='Confirmar pago';
  bOk.onclick=function(){
    var m=parseFloat(document.getElementById('pmPagado').value)||montoEst;
    var e=loadPagosEstado(); e[pid]={pagado:true,montoPagado:m,fecha:today()};
    savePagosEstado(e); showToast('✅ Pago registrado'); renderPagosMes();
  };
  var bCan=document.createElement('button');
  bCan.className='btn-sec'; bCan.style.marginTop='8px'; bCan.textContent='Cancelar';
  bCan.onclick=function(){ renderPagosMes(); };
  d.appendChild(bOk); d.appendChild(bCan);
  mc.appendChild(d);
  setTimeout(function(){ var el=document.getElementById('pmPagado'); if(el){el.value=montoEst;el.focus();el.select();} },80);
}

function loadPagosBase(){ return load('pagos_mensuales',[]); }

function savePagosBase(p){ save('pagos_mensuales',p); }

function loadPagosEstado(){ try{ return JSON.parse(localStorage.getItem(keyPagosMes())||'{}'); }catch(e){ return {}; } }

function savePagosEstado(e){ localStorage.setItem(keyPagosMes(), JSON.stringify(e)); }

function getPagosCats(){ return PAGOS_CATS.concat(load('cats_pagos_custom',[])); }

function borrarPago(i){
  var pp=loadPagosBase();
  if(!pp[i]) return;
  var eli=JSON.parse(JSON.stringify(pp[i]));
  pp.splice(i,1); savePagosBase(pp);
  renderPagosMes();
  mostrarUndo('📅 '+eli.nombre+' eliminado', function(){
    var pp2=loadPagosBase(); pp2.splice(i,0,eli); savePagosBase(pp2); renderPagosMes();
  });
}

function renderCarrito(){
  var cats   = getCarritoCats();
  var actual = getCarritoActual();
  var hist   = getCarritoHistorial();
  var tabActual = (S._carritoTab || 'lista') === 'lista';
  var tabHist   = (S._carritoTab) === 'historial';
  var tabCat    = (S._carritoTab) === 'catalogo';
  var tabs = '<div style="display:flex;gap:6px;margin-bottom:14px;">'
    + ['lista','historial','catalogo'].map(function(t,i){
        var labels = ['🛒 Lista actual','📋 Historial','🔍 Catálogo'];
        var active = (S._carritoTab||'lista') === t;
        return '<button onclick="_carritoTab(\''+t+'\')" style="flex:1;padding:9px 4px;border-radius:12px;border:none;font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;cursor:pointer;transition:all 0.18s;background:'+(active?'var(--accent)':'var(--inp)')+';color:'+(active?'#fff':'var(--dim)')+';">'+labels[i]+'</button>';
      }).join('')
    + '</div>';
  var content = '';
  if(tabHist)   content = _renderCarritoHistorial();
  else if(tabCat) content = _renderCarritoCatalogo();
  else          content = _renderCarritoLista(actual, cats);
  return '<div class="page-header">'
    + backSubBtn()
    + '<div class="page-title">🛒 Carrito</div>'
    + '<button onclick="_carritoNuevo()" style="background:var(--accent);border:none;border-radius:10px;padding:6px 12px;font-size:0.75rem;font-weight:700;color:#fff;cursor:pointer;">+ Nueva lista</button>'
    + '</div>'
    + tabs
    + content;
}

function _renderCarritoLista(actual, cats){
  var items = actual.items || [];
  var comprados = items.filter(function(i){ return i.comprado; });
  var total = comprados.reduce(function(s,i){ return s + (i.precio||0)*(i.qty||1); },0);
  var totalEst = items.reduce(function(s,i){ return s + (i.precio||0)*(i.qty||1); },0);
  var headerLista = '<div class="card" style="margin-bottom:12px;padding:14px 16px;">'
    + '<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;">'
    + '<input id="carritoNombreLista" class="inp" placeholder="Nombre de la lista (ej: Super semanal)" '
    + 'style="flex:1;margin-right:8px;font-weight:700;" value="'+( actual.nombre||'')+'" '
    + 'onchange="carritoActualizarNombre(this.value)">'
    + '</div>'
    + '<input id="carritoTienda" class="inp" placeholder="🏪 Tienda / lugar" '
    + 'value="'+(actual.tienda||'')+'" onchange="carritoActualizarTienda(this.value)" style="margin-bottom:10px;">'
    + '<div style="font-size:0.7rem;font-weight:700;color:var(--dim);margin-bottom:8px;">CATEGORÍA</div>'
    + '<div class="carrito-cat-grid">'
    + cats.map(function(c){
        var activa = (actual.catId === c.id) ? ' activa' : '';
        return '<button class="carrito-cat-btn'+activa+'" onclick="carritoSelCat(\''+c.id+'\')">'+
          '<div class="carrito-cat-ico">'+c.ico+'</div>'+
          '<div class="carrito-cat-lbl">'+c.nombre+'</div></button>';
      }).join('')
    + '<button class="carrito-cat-btn" onclick="carritoNuevaCat()" style="border-style:dashed;opacity:0.7;">'
    + '<div class="carrito-cat-ico">➕</div><div class="carrito-cat-lbl">Nueva</div></button>'
    + '</div>'
    + '</div>';
  var formAdd = '<div class="card" style="margin-bottom:12px;padding:14px 16px;">'
    + '<div style="font-size:0.72rem;font-weight:700;color:var(--dim);margin-bottom:8px;">AGREGAR PRODUCTO</div>'
    + '<input id="carritoNombreItem" class="inp" placeholder="Nombre del producto" '
    + 'style="margin-bottom:8px;" oninput="carritoSugerirPrecio(this.value)" autocomplete="off">'
    + '<div id="carritoSugerencia" style="display:none;font-size:0.72rem;color:var(--accent);'
    + 'background:var(--inp);border-radius:10px;padding:7px 12px;margin-bottom:8px;cursor:pointer;" '
    + 'onclick="carritoAplicarSugerencia()"></div>'
    + '<div style="display:flex;gap:8px;margin-bottom:8px;">'
    + '<input id="carritoPrecioItem" class="inp" type="number" placeholder="Precio est." style="flex:1;">'
    + '<input id="carritoQtyItem" class="inp" type="number" placeholder="Cant." style="width:70px;" value="1">'
    + '<select id="carritoUnidadItem" class="inp" style="width:80px;padding:10px 6px;">'
    + '<option value="pza">pza</option><option value="kg">kg</option><option value="lt">lt</option>'
    + '<option value="caja">caja</option><option value="paq">paq</option><option value="doc">doc</option>'
    + '</select>'
    + '</div>'
    + '<input id="carritoNotaItem" class="inp" placeholder="Nota (opcional)" style="margin-bottom:10px;">'
    + '<button class="btn-main" onclick="carritoAgregarItem()">+ Agregar a la lista</button>'
    + '</div>';
  var listaItems = '';
  if(items.length === 0){
    listaItems = '<div class="card" style="text-align:center;padding:32px 20px;color:var(--dim);">'
      + '<div style="font-size:2.5rem;margin-bottom:10px;">🛒</div>'
      + '<div style="font-size:0.85rem;">Tu lista está vacía</div>'
      + '<div style="font-size:0.72rem;margin-top:4px;">Agrega productos arriba</div></div>';
  } else {
    var pendientes = items.filter(function(i){ return !i.comprado; });
    var compradosItems = items.filter(function(i){ return i.comprado; });
    if(pendientes.length > 0){
      listaItems += '<div style="font-size:0.7rem;font-weight:700;color:var(--dim);margin-bottom:8px;">PENDIENTES ('+pendientes.length+')</div>';
      listaItems += pendientes.map(function(it,i){
        var ri = items.indexOf(it);
        return _carritoItemHTML(it, ri);
      }).join('');
    }
    if(compradosItems.length > 0){
      listaItems += '<div style="font-size:0.7rem;font-weight:700;color:var(--dim);margin:12px 0 8px;">COMPRADOS ('+compradosItems.length+')</div>';
      listaItems += compradosItems.map(function(it){
        var ri = items.indexOf(it);
        return _carritoItemHTML(it, ri);
      }).join('');
    }
  }
  var totalBar = items.length > 0 ? '<div class="carrito-total-bar" id="carritoTotalBar" style="touch-action:none;">'
    + '<button onclick="_carritoColapsarBarra()" style="background:none;border:none;font-size:0.75rem;color:var(--dim);cursor:pointer;padding:0 6px 0 0;flex-shrink:0;" title="Minimizar">✕</button>'
    + '<div class="ctb-detalle" style="display:flex;flex:1;justify-content:space-between;align-items:center;gap:8px;">'
    + '<div>'
    + '<div style="font-size:0.65rem;color:var(--dim);">Estimado</div>'
    + '<div style="font-size:1rem;font-weight:900;color:var(--text);">'+fmt(totalEst)+'</div>'
    + '</div>'
    + '<div style="text-align:right;">'
    + '<div style="font-size:0.65rem;color:var(--accent);">Comprado</div>'
    + '<div style="font-size:1rem;font-weight:900;color:var(--accent);">'+fmt(total)+'</div>'
    + '</div>'
    + '<div style="display:flex;gap:6px;">'
    + '<button onclick="carritoCompartir()" style="background:var(--inp);border:1px solid var(--border);border-radius:14px;padding:9px 11px;font-family:Outfit,sans-serif;font-size:0.95rem;cursor:pointer;">&#x1F4E4;</button>'
    + '<button onclick="carritoFinalizar()" style="background:var(--accent);border:none;border-radius:14px;padding:9px 14px;font-family:Outfit,sans-serif;font-size:0.78rem;font-weight:800;color:#fff;cursor:pointer;box-shadow:0 4px 14px rgba(43,192,112,0.3);">✅ Finalizar</button>'
    + '</div>'
    + '</div>'
    + '<div class="ctb-mini" style="display:none;font-size:0.78rem;font-weight:800;color:var(--accent);cursor:pointer;" onclick="_carritoExpandirBarra()">'+fmt(totalEst)+' — ver ›</div>'
    + '</div>' : '';
  return headerLista + formAdd + listaItems + totalBar;
}

function _renderCarritoHistorial(){
  var hist = getCarritoHistorial();
  if(hist.length === 0){
    return '<div class="card" style="text-align:center;padding:40px 20px;color:var(--dim);">'
      + '<div style="font-size:2.5rem;margin-bottom:10px;">📋</div>'
      + '<div style="font-size:0.85rem;">Sin listas guardadas aún</div>'
      + '<div style="font-size:0.72rem;margin-top:4px;">Finaliza una compra para guardarla aquí</div></div>';
  }
  return hist.map(function(lista, hi){
    var total = (lista.items||[]).reduce(function(s,i){ return s+(i.precio||0)*(i.qty||1); },0);
    var comprados = (lista.items||[]).filter(function(i){ return i.comprado; }).length;
    var cats = getCarritoCats();
    var cat = cats.find(function(c){ return c.id === lista.catId; });
    return '<div class="card" style="margin-bottom:10px;padding:14px 16px;">'
      + '<div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:10px;">'
      + '<div>'
      + '<div style="font-weight:800;font-size:0.9rem;color:var(--text);">'+(cat?cat.ico+' ':'')+( lista.nombre||'Sin nombre')+'</div>'
      + '<div style="font-size:0.68rem;color:var(--dim);margin-top:2px;">'
      + lista.fecha + (lista.tienda?' · '+lista.tienda:'')
      + ' · '+comprados+'/'+(lista.items||[]).length+' productos'
      + '</div>'
      + '</div>'
      + '<div style="font-size:1rem;font-weight:900;color:var(--accent);">'+fmt(total)+'</div>'
      + '</div>'
      + '<div style="font-size:0.72rem;color:var(--dim);margin-bottom:10px;line-height:1.6;">'
      + (lista.items||[]).slice(0,5).map(function(i){ return i.nombre+(i.precio?' ('+fmt(i.precio)+')':''); }).join(' · ')
      + ((lista.items||[]).length > 5 ? ' · +'+((lista.items||[]).length-5)+' más' : '')
      + '</div>'
      + '<div style="display:flex;gap:8px;">'
      + '<button onclick="carritoCargarLista('+hi+')" style="flex:1;background:var(--accent);border:none;border-radius:12px;padding:9px;font-family:Outfit,sans-serif;font-size:0.78rem;font-weight:700;color:#fff;cursor:pointer;">📂 Usar lista</button>'
      + '<button onclick="carritoCompartirLista('+hi+')" style="background:var(--inp);border:1px solid var(--border);border-radius:12px;padding:9px 12px;font-family:Outfit,sans-serif;font-size:0.78rem;color:var(--text);cursor:pointer;">&#x1F4E4;</button>'
      + '<button onclick="carritoEliminarLista('+hi+')" style="background:var(--inp);border:1px solid var(--border);border-radius:12px;padding:9px 12px;font-family:Outfit,sans-serif;font-size:0.78rem;color:var(--dim);cursor:pointer;">🗑</button>'
      + '</div>'
      + '</div>';
  }).join('');
}

function _renderCarritoCatalogo(){
  var cat = getProductosCatalogo();
  var keys = Object.keys(cat).sort();
  if(keys.length === 0){
    return '<div class="card" style="text-align:center;padding:40px 20px;color:var(--dim);">'
      + '<div style="font-size:2.5rem;margin-bottom:10px;">🔍</div>'
      + '<div style="font-size:0.85rem;">Sin precios registrados aún</div>'
      + '<div style="font-size:0.72rem;margin-top:4px;">Los precios se guardan al marcar productos como comprados</div></div>';
  }
  return '<div style="margin-bottom:10px;">'
    + '<input class="inp" placeholder="🔍 Buscar producto..." oninput="_filtrarCatalogo(this.value)" id="catBuscar">'
    + '</div>'
    + '<div id="catLista">'
    + keys.map(function(k){
        var hist = cat[k];
        var ultimo = hist[0];
        var mejor  = hist.reduce(function(m,h){ return h.precio < m.precio ? h : m; }, hist[0]);
        var mayor  = hist.reduce(function(m,h){ return h.precio > m.precio ? h : m; }, hist[0]);
        return '<div class="card" style="margin-bottom:8px;padding:12px 16px;" data-prod="'+k+'">'
          + '<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;">'
          + '<div style="font-weight:800;font-size:0.88rem;color:var(--text);">'+hist[0].tienda&&false?'':''
          + k.charAt(0).toUpperCase()+k.slice(1)+'</div>'
          + '<div style="font-size:1rem;font-weight:900;color:var(--text);">'+fmt(ultimo.precio)+'</div>'
          + '</div>'
          + '<div style="display:flex;gap:8px;margin-bottom:8px;">'
          + '<span style="font-size:0.67rem;background:rgba(43,192,112,0.12);color:#1a8c4e;border-radius:8px;padding:3px 8px;font-weight:700;">Mínimo: '+fmt(mejor.precio)+(mejor.tienda?' en '+mejor.tienda:'')+'</span>'
          + (hist.length > 1 ? '<span style="font-size:0.67rem;background:rgba(255,95,87,0.1);color:#cc2a2a;border-radius:8px;padding:3px 8px;font-weight:700;">Máximo: '+fmt(mayor.precio)+'</span>' : '')
          + '</div>'
          + hist.slice(0,4).map(function(h){
              return '<div class="hist-precio-row">'
                + '<span class="hist-precio-tienda">'+(h.tienda||'Sin tienda')+'</span>'
                + '<span class="hist-precio-fecha">'+h.fecha+'</span>'
                + '<span class="hist-precio-val">'+fmt(h.precio)+'</span>'
                + '</div>';
            }).join('')
          + '</div>';
      }).join('')
    + '</div>';
}

function carritoAgregarItem(){
  var nombre = (document.getElementById('carritoNombreItem').value||'').trim();
  var precio = parseFloat(document.getElementById('carritoPrecioItem').value)||0;
  var qty    = parseInt(document.getElementById('carritoQtyItem').value)||1;
  var unidad = document.getElementById('carritoUnidadItem').value||'pza';
  var nota   = (document.getElementById('carritoNotaItem').value||'').trim();
  if(!nombre){ showToast('⚠ Escribe el nombre del producto'); return; }
  var actual = getCarritoActual();
  actual.items = actual.items || [];
  actual.items.push({ nombre:nombre, precio:precio, qty:qty, unidad:unidad, nota:nota, comprado:false, id: Date.now() });
  if(!actual.fecha) actual.fecha = today();
  saveCarritoActual(actual);
  ['carritoNombreItem','carritoPrecioItem','carritoNotaItem'].forEach(function(id){
    var el = document.getElementById(id); if(el) el.value='';
  });
  var qEl = document.getElementById('carritoQtyItem'); if(qEl) qEl.value='1';
  var sug = document.getElementById('carritoSugerencia'); if(sug) sug.style.display='none';
  goSub('carrito');
  showToast('✓ '+nombre+' agregado');
}

function carritoToggleItem(ri){
  var actual = getCarritoActual();
  var item = actual.items[ri];
  if(!item) return;
  item.comprado = !item.comprado;
  if(item.comprado && item.precio){
    carritoRegistrarPrecio(item.nombre, item.precio, actual.tienda);
  }
  saveCarritoActual(actual);
  goSub('carrito');
}

function carritoQty(ri, delta){
  var actual = getCarritoActual();
  var item = actual.items[ri];
  if(!item) return;
  item.qty = Math.max(1, (item.qty||1) + delta);
  saveCarritoActual(actual);
  goSub('carrito');
}

function carritoEliminarItem(ri){
  var actual = getCarritoActual();
  var item = actual.items[ri];
  if(!item) return;
  var backup = JSON.parse(JSON.stringify(actual));
  actual.items.splice(ri, 1);
  saveCarritoActual(actual);
  goSub('carrito');
  mostrarUndo('🗑 "'+item.nombre+'" eliminado', function(){
    saveCarritoActual(backup); goSub('carrito');
  });
}

function carritoFinalizar(){
  var actual = getCarritoActual();
  if(!actual.items || actual.items.length === 0){ showToast('⚠ Lista vacía'); return; }
  var comprados = actual.items.filter(function(i){ return i.comprado; });
  var totalComp = comprados.reduce(function(s,i){ return s+(i.precio||0)*(i.qty||1); },0);
  var totalEst  = actual.items.reduce(function(s,i){ return s+(i.precio||0)*(i.qty||1); },0);
  if(comprados.length === 0){
    showToast('⚠ Marca al menos un producto como comprado');
    return;
  }
  var modal = document.createElement('div');
  modal.style.cssText = 'position:fixed;inset:0;z-index:9000;background:rgba(0,0,0,0.55);display:flex;align-items:flex-end;';
  var cats = getCarritoCats();
  var cat  = cats.find(function(c){ return c.id===actual.catId; });
  var catNombre = cat ? cat.nombre : 'Compras';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 40px;width:100%;max-width:480px;margin:0 auto;">'
    + '<div style="font-size:1.1rem;font-weight:900;margin-bottom:6px;">✅ Finalizar compra</div>'
    + '<div style="font-size:0.78rem;color:var(--dim);margin-bottom:18px;">'+comprados.length+' productos · Total gastado: <b style="color:var(--accent);">'+fmt(totalComp)+'</b></div>'
    + '<div style="background:var(--inp);border-radius:14px;padding:12px 14px;margin-bottom:16px;">'
    + '<div style="font-size:0.68rem;color:var(--dim);margin-bottom:8px;">RESUMEN</div>'
    + '<div style="display:flex;justify-content:space-between;font-size:0.82rem;margin-bottom:4px;">'
    + '<span>Estimado</span><span style="font-weight:700;">'+fmt(totalEst)+'</span></div>'
    + '<div style="display:flex;justify-content:space-between;font-size:0.82rem;">'
    + '<span>Real comprado</span><span style="font-weight:800;color:var(--accent);">'+fmt(totalComp)+'</span></div>'
    + '</div>'
    + '<div style="font-size:0.72rem;font-weight:700;color:var(--dim);margin-bottom:6px;">¿REGISTRAR COMO GASTO?</div>'
    + '<div style="background:var(--inp);border-radius:14px;padding:12px 14px;margin-bottom:14px;">'
    + '<div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">'
    + '<input type="checkbox" id="finRegGasto" checked style="width:18px;height:18px;cursor:pointer;">'
    + '<label for="finRegGasto" style="font-size:0.82rem;font-weight:600;cursor:pointer;">Sí, registrar '+fmt(totalComp)+' como gasto</label>'
    + '</div>'
    + '<select id="finCuentaGasto" class="inp" style="font-size:0.8rem;">'
    + _carritoOpsCuentas()
    + '</select>'
    + '</div>'
    + '<button class="btn-main" onclick="carritoConfirmarFin()">✅ Confirmar y guardar</button>'
    + '<button onclick="document.getElementById(\'modalFinCarrito\').remove()" style="width:100%;margin-top:8px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    + '</div>';
  modal.id = 'modalFinCarrito';
  document.body.appendChild(modal);
}

function _carritoNuevo(){
  usalaConfirm('Empezar lista nueva? La lista actual se perdera si no la guardas.', function(){
    saveCarritoActual({nombre:'',catId:'super',items:[],fecha:'',tienda:''});
      S._carritoTab = 'lista';
      goSub('carrito');
  });
}

function carritoCargarLista(hi){
  var hist = getCarritoHistorial();
  var lista = hist[hi];
  if(!lista) return;
  var nueva = JSON.parse(JSON.stringify(lista));
  nueva.items = nueva.items.map(function(i){
    return { nombre:i.nombre, precio:i.precio, qty:i.qty, unidad:i.unidad, nota:i.nota, comprado:false, id:Date.now()+Math.random() };
  });
  nueva.fecha = today();
  nueva.fechaFin = null;
  nueva.totalReal = null;
  saveCarritoActual(nueva);
  S._carritoTab = 'lista';
  goSub('carrito');
  showToast('📂 Lista cargada — ya puedes modificarla');
}

function carritoEliminarLista(hi){
  var hist = getCarritoHistorial();
  var lista = hist[hi];
  if(!lista) return;
  var backup = JSON.parse(JSON.stringify(hist));
  hist.splice(hi, 1);
  saveCarritoHistorial(hist);
  goSub('carrito');
  mostrarUndo('🗑 Lista eliminada', function(){ saveCarritoHistorial(backup); goSub('carrito'); });
}

function carritoCompartir(){
  var actual = getCarritoActual();
  if(!actual.items || actual.items.length === 0){ showToast('⚠ Lista vacía'); return; }
  var texto = _carritoTextoLista(actual);
  _carritoMostrarModalCompartir(texto);
}

function _initCarritoDrag(){
  var bar = document.getElementById('carritoTotalBar');
  if(!bar) return;
  var isDragging = false, startY = 0, startBottom = 72;
  function getBottom(){ return parseInt(bar.style.bottom)||72; }
  function onStart(e){
    var target = e.target || e.srcElement;
    if(target.tagName==='BUTTON'||target.tagName==='A') return;
    isDragging = true;
    startY = e.touches ? e.touches[0].clientY : e.clientY;
    startBottom = getBottom();
    bar.style.transition = 'none';
    e.preventDefault();
  }
  function onMove(e){
    if(!isDragging) return;
    var y = e.touches ? e.touches[0].clientY : e.clientY;
    var delta = startY - y; // mover hacia arriba = delta positivo
    var newBottom = Math.max(8, Math.min(window.innerHeight - 80, startBottom + delta));
    bar.style.bottom = newBottom + 'px';
    e.preventDefault();
  }
  function onEnd(){
    if(!isDragging) return;
    isDragging = false;
    bar.style.transition = 'all 0.25s';
  }
  bar.addEventListener('touchstart', onStart, {passive:false});
  bar.addEventListener('touchmove',  onMove,  {passive:false});
  bar.addEventListener('touchend',   onEnd);
  bar.addEventListener('mousedown',  onStart);
  document.addEventListener('mousemove', onMove);
  document.addEventListener('mouseup',   onEnd);
}

function getCarritoActual(){ return load('carrito_actual', {nombre:'',catId:'super',items:[],fecha:'',tienda:''}); }

function saveCarritoActual(c){ save('carrito_actual', c); }

function getCarritoHistorial(){ return load('carrito_historial', []); }

function saveCarritoHistorial(h){ save('carrito_historial', h); }

function getCarritoCats(){
  var defaults = [
    {id:'agro',   ico:'🌾', nombre:'Agropecuario'},
    {id:'shop',   ico:'🛍️', nombre:'Shopping'},
    {id:'super',  ico:'🛒', nombre:'Súper'},
    {id:'mat',    ico:'🧱', nombre:'Materiales'},
    {id:'ins',    ico:'📦', nombre:'Insumos'},
  ];
  var custom = load('carrito_cats', []);
  return defaults.concat(custom);
}

function carritoRegistrarPrecio(nombre, precio, tienda){
  if(!nombre || !precio) return;
  var cat = getProductosCatalogo();
  var key = nombre.trim().toLowerCase();
  if(!cat[key]) cat[key] = [];
  cat[key].unshift({ precio: precio, tienda: tienda||'', fecha: today() });
  if(cat[key].length > 10) cat[key] = cat[key].slice(0,10); // max 10 registros por producto
  saveProductosCatalogo(cat);
}

function abrirCalc(){
  var cf = document.getElementById('calcFloat');
  var bb = document.getElementById('calcBubble');
  if(bb && bb.style.display !== 'none'){
    restaurarCalc(); return;
  }
  if(cf.style.display === 'block') return;
  _calcExpr=''; _calcResult='0'; _calcNewNum=true;
  document.getElementById('calcDisplay').textContent='0';
  document.getElementById('calcExpr').textContent='';
  cf.style.display='block';
  cf.style.bottom='100px'; cf.style.right='14px';
  cf.style.left='auto'; cf.style.top='auto';
  if(bb) bb.style.display='none';
  iniciarDragCalc();
  iniciarDragBurbuja();
}

function cerrarCalc(){
  var cf = document.getElementById('calcFloat');
  var bb = document.getElementById('calcBubble');
  cf.style.transition = 'transform 0.2s ease, opacity 0.2s ease';
  cf.style.transform  = 'scale(0.8)';
  cf.style.opacity    = '0';
  setTimeout(function(){
    cf.style.display='none';
    cf.style.transform=''; cf.style.opacity=''; cf.style.transition='';
  }, 200);
  if(bb) bb.style.display='none';
  _calcExpr=''; _calcResult='0'; _calcNewNum=true;
}

function calcDel(){
  if(_calcNewNum||_calcResult==='0') return;
  _calcResult=_calcResult.length>1?_calcResult.slice(0,-1):'0';
  document.getElementById('calcDisplay').textContent=_calcResult;
}

function calcOp(op){
  _calcExpr+=_calcResult+' '+op+' ';
  document.getElementById('calcExpr').textContent=_calcExpr;
  _calcNewNum=true; _calcResult='0';
}

function restaurarCalc(){
  var cf = document.getElementById('calcFloat');
  var bb = document.getElementById('calcBubble');
  var r  = bb.getBoundingClientRect();
  cf.style.left  = Math.max(0, r.left - 100) + 'px';
  cf.style.top   = Math.max(0, r.top  - 200) + 'px';
  cf.style.right = 'auto'; cf.style.bottom = 'auto';
  cf.style.transform = 'scale(0.3)';
  cf.style.opacity = '0';
  cf.style.display = 'block';
  bb.style.display = 'none';
  requestAnimationFrame(function(){
    cf.style.transition = 'transform 0.3s cubic-bezier(0.34,1.4,0.64,1), opacity 0.25s ease';
    cf.style.transform  = 'scale(1)';
    cf.style.opacity    = '1';
    setTimeout(function(){ cf.style.transition=''; }, 350);
  });
}

function minimizarCalc(){
  var cf = document.getElementById('calcFloat');
  var bb = document.getElementById('calcBubble');
  var r = cf.getBoundingClientRect();
  bb.style.left = (r.left + r.width/2 - 34) + 'px';
  bb.style.top  = (r.top  + r.height/2 - 34) + 'px';
  bb.style.right = 'auto'; bb.style.bottom = 'auto';
  bb.style.display = 'flex';
  document.getElementById('calcBubbleVal').textContent = _calcResult !== '0' ? _calcResult : (_calcExpr ? '...' : '0');
  cf.style.transform = 'scale(0.3)';
  cf.style.opacity = '0';
  setTimeout(function(){ cf.style.display='none'; cf.style.transform=''; cf.style.opacity=''; }, 280);
}

function toggleVoz(){
  if(_vozActivo){ detenerVoz(); return; }
  iniciarVoz();
}


// ── Funciones adicionales ──

function nkPress(n){
  if(_nipBuffer.length >= 4) return;
  _nipBuffer += String(n);
  _actualizarNipDots();
  if(_nipBuffer.length === 4) setTimeout(verificarNip, 120);
}

function nkDel(){
  _nipBuffer = _nipBuffer.slice(0,-1);
  _actualizarNipDots();
  var err = document.getElementById('nipErr');
  if(err) err.style.display='none';
}

function _actualizarNipDots(){
  for(var i=1;i<=4;i++){
    var d = document.getElementById('nd'+i);
    if(d) d.className = 'nip-dot' + (i<=_nipBuffer.length ? ' on' : '');
  }
}

function nipKey(){
  if(!_sesionPendiente) return null;
  return _sesionPendiente.isAdmin ? 'usala_nip_admin' : 'usala_nip_u_' + _sesionPendiente.codigo;
}


function copiarCodigo(c){ navigator.clipboard.writeText(c).catch(function(){}); showToast('✓ Copiado: '+c); }


// ── Funciones restantes ──

function getUCod(){ return S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : null; }

async function dbGetCodigos(){
  var ck = 'codigos';
  var cached = _cacheGet(ck); if(cached) return cached;
  try {
    var rows = await DB.get('usala_usuarios', 'is_admin=eq.false&order=creado_en.desc');
    _cacheSet(ck, rows||[]);
    return rows||[];
  } catch(e) { console.warn('dbGetCodigos:', e); return []; }
}

async function dbGetTxs(){
  var uc = getUCod(); if(!uc) return [];
  var ck = uc + '_txs';
  var cached = _cacheGet(ck); if(cached) return cached;
  try {
    var rows = await DB.get('usala_txs', 'user_codigo=eq.' + encodeURIComponent(uc) + '&order=fecha.asc,id.asc');
    _cacheSet(ck, rows||[]);
    return rows||[];
  } catch(e) { console.warn('dbGetTxs:', e); return []; }
}

async function dbSaveTx(tx){
  var uc = getUCod(); if(!uc) return;
  try {
    var data = { user_codigo: uc, tipo: tx.tipo, monto: tx.monto, desc: tx.desc, cat: tx.cat, fecha: tx.fecha, cuenta: tx.cuenta||'efectivo' };
    if(tx.id && typeof tx.id === 'number' && tx.id > 0){
      await DB.update('usala_txs', 'id=eq.'+tx.id+'&user_codigo=eq.'+encodeURIComponent(uc), data);
    } else {
      await DB.insert('usala_txs', data);
    }
    _cacheInvalid(uc + '_txs');
  } catch(e) { console.warn('dbSaveTx:', e); }
}

async function dbDeleteTx(id){
  var uc = getUCod(); if(!uc) return;
  try {
    await DB.del('usala_txs', 'id=eq.'+id+'&user_codigo=eq.'+encodeURIComponent(uc));
    _cacheInvalid(uc + '_txs');
  } catch(e) { console.warn('dbDeleteTx:', e); }
}

function _schedulSync(){
  if(_syncTimer) clearTimeout(_syncTimer);
  _syncTimer = setTimeout(_flushSync, 2000); // esperar 2s de inactividad
}

function _setSyncIndicator(estado){
  var el = document.getElementById('syncDot');
  if(!el) return;
  el.style.display = 'block';
  if(estado === 'syncing'){
    el.style.background = '#ffb340';
    el.title = 'Guardando...';
  } else if(estado === 'ok'){
    el.style.background = '#2bc070';
    el.title = 'Guardado en la nube ✓';
    if(_syncIndicatorTimer) clearTimeout(_syncIndicatorTimer);
    _syncIndicatorTimer = setTimeout(function(){ el.style.display='none'; }, 3000);
  } else {
    el.style.background = '#ff5f57';
    el.title = 'Sin conexión — datos guardados localmente';
  }
}

async function dbKVGet(key){
  var uc = getUCod(); if(!uc) return null;
  var ck = uc + '_kv_' + key;
  var cached = _cacheGet(ck); if(cached !== null) return cached;
  try {
    var rows = await DB.get('usala_kv', 'user_codigo=eq.'+encodeURIComponent(uc)+'&key=eq.'+encodeURIComponent(key));
    var val = (rows && rows.length > 0) ? JSON.parse(rows[0].value) : null;
    _cacheSet(ck, val);
    return val;
  } catch(e) { return null; }
}

async function dbKVSet(key, value){
  var uc = getUCod(); if(!uc) return;
  var ck = uc + '_kv_' + key;
  _cacheSet(ck, value);
  try { localStorage.setItem('usala_'+uc+'_'+key, JSON.stringify(value)); } catch(e){}
  _syncQueue.push({ key: key, value: value });
  _schedulSync();
}

function detenerRealtime(){
  if(_realtimeInterval) clearInterval(_realtimeInterval);
  _realtimeActivo = false;
  console.log('⏹ Realtime detenido');
}

async function _realtimeTick(){
  if(!S.user || !_realtimeActivo) return;
  var uc = getUCod();
  if(!uc) return;
  try {
    var remote = await DB.get('usala_kv',
      'user_codigo=eq.' + encodeURIComponent(uc) +
      '&updated_at=gt.' + encodeURIComponent(_lastSyncTs) +
      '&order=updated_at.desc');
    if(remote && remote.length > 0){
      var cambio = false;
      remote.forEach(function(row){
        try {
          var localKey = 'usala_' + uc + '_' + row.key;
          var localRaw = localStorage.getItem(localKey);
          if(localRaw !== row.value){
            localStorage.setItem(localKey, row.value);
            _cacheInvalid(uc + '_kv_' + row.key);
            cambio = true;
            console.log('⚡ Actualizado desde nube:', row.key);
          }
        } catch(e){}
      });
      if(cambio){
        _realtimeRefrescarUI();
        _setSyncIndicator('ok');
      }
    }
    // También revisar noticias del admin para TODOS los usuarios
    if(!S.user.isAdmin){
      var noticias = await DB.get('usala_noticias', 'order=fecha.desc&limit=5');
      if(noticias && noticias.length > 0){
        var stored = JSON.parse(localStorage.getItem('usala_noticias')||'[]');
        if(JSON.stringify(noticias) !== JSON.stringify(stored)){
          localStorage.setItem('usala_noticias', JSON.stringify(noticias));
          if(S.tab === 'inicio') renderTab('inicio');
        }
      }
    }
    _lastSyncTs = new Date().toISOString();
  } catch(e){
    _setSyncIndicator('error');
    console.warn('⚡ Realtime tick falló:', e.message);
  }
}

function _realtimeRefrescarUI(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  var tab = S.tab || 'inicio';
  var sub = S.subtab;
  var subsRefresca = ['historial','creditos_debo','creditos_cobrar','progreso','reportes'];
  if(sub && subsRefresca.indexOf(sub) > -1){
    goSub(sub);
  } else if(!sub || sub === tab){
    renderTab(tab);
  }
  _mostrarToastSync();
}

function _mostrarToastSync(){
  if(_syncToastTimer) return; // no spamear
  var t = document.createElement('div');
  t.style.cssText = 'position:fixed;bottom:80px;left:50%;transform:translateX(-50%);'
    +'background:rgba(43,192,112,0.9);color:#fff;font-size:0.72rem;font-weight:700;'
    +'padding:6px 14px;border-radius:20px;z-index:9998;pointer-events:none;'
    +'backdrop-filter:blur(8px);box-shadow:0 2px 12px rgba(43,192,112,0.3);';
  t.textContent = '⚡ Datos actualizados';
  document.body.appendChild(t);
  _syncToastTimer = setTimeout(function(){
    t.remove(); _syncToastTimer = null;
  }, 2000);
}

async function dbPing(){
  try {
    await DB.get('usala_usuarios', 'codigo=eq.admin&select=codigo');
    _dbOnline = true;
  } catch(e) { _dbOnline = false; }
  return _dbOnline;
}

function selectTheme(el){
  document.querySelectorAll('.theme-card').forEach(function(c){ c.classList.remove('selected'); });
  el.classList.add('selected');
  S.theme = el.dataset.theme;
  applyTheme(S.theme);
}

function applyTheme(t){
  document.documentElement.dataset.theme = (t === 'default') ? '' : t;
}

function confirmarTema(){
  localStorage.setItem('usala_theme', S.theme);
}

function mostrarPanelSolicitud(){
  ['panelSesion','panelCodigo','panelEnviada'].forEach(function(id){
    var el=document.getElementById(id); if(el) el.style.display='none';
  });
  var ps = document.getElementById('panelSolicitud');
  if(ps) ps.style.display='block';
}

function formatearContacto(inp){
  var v = inp.value.replace(/\D/g,'');
  if(v.startsWith('521')) v=v.slice(2);
  else if(v.startsWith('52')) v=v.slice(2);
  else if(v.startsWith('1') && v.length===11) v=v.slice(1);
  if(v.length>10) v=v.slice(0,10);
  var fmt='';
  if(v.length>0) fmt=v.slice(0,2);
  if(v.length>2) fmt+=' '+v.slice(2,6);
  if(v.length>6) fmt+=' '+v.slice(6,10);
  if(inp.value.includes('@')) return;
  inp.value = fmt;
  var hint = document.getElementById('solContactoHint');
  if(hint){
    if(v.length===10){ hint.textContent='✅ Número válido'; hint.style.display='block'; hint.style.color='var(--accent2)'; }
    else if(v.length>4){ hint.textContent='⚠ Verifica el número'; hint.style.display='block'; hint.style.color='#f57c00'; }
    else{ hint.style.display='none'; }
  }
}

function enviarSolicitud(){
  var nombre   = (document.getElementById('solNombre').value||'').trim();
  var motivo   = (document.getElementById('solMotivo').value||'').trim();
  var contacto = (document.getElementById('solContacto').value||'').trim();
  var msg      = document.getElementById('solicitudMsg');
  var btn      = document.querySelector('#panelSolicitud .lg-btn');
  if(!nombre){ showErr('⚠ Escribe tu nombre'); return; }
  if(!contacto || (contacto.replace(/\D/g,'').length < 7 && !contacto.includes('@'))){
    showErr('⚠ Escribe tu WhatsApp o email'); return;
  }
  if(msg) msg.style.display='none';
  if(btn){ btn.textContent='Enviando...'; btn.disabled=true; }
  var sol = {
    nombre: nombre, motivo: motivo, contacto: contacto,
    fecha: today(), estado: 'pendiente'
  };
  DB.insert('usala_solicitudes', sol).then(function(res){
    if(btn){ btn.textContent='📩 Enviar solicitud'; btn.disabled=false; }
    ['panelSolicitud'].forEach(function(id){ var el=document.getElementById(id); if(el) el.style.display='none'; });
    var pe = document.getElementById('panelEnviada'); if(pe) pe.style.display='block';
    var txt = '🔑 Solicitud USALA\n👤 '+nombre+'\n📞 '+contacto+(motivo?'\n💬 '+motivo:'');
    var waBtn = document.getElementById('_solWaBtn');
    if(waBtn) waBtn.href='https://wa.me/?text='+encodeURIComponent(txt);
    var cpBtn = document.getElementById('_solCopyBtn');
    if(cpBtn) cpBtn.onclick=function(){ navigator.clipboard.writeText(txt).catch(function(){}); showToast('✓ Copiado'); };
  }).catch(function(e){
    console.warn('Supabase error:', e);
    var sols = JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
    sols.push(Object.assign({id:Date.now()}, sol));
    localStorage.setItem('usala_solicitudes', JSON.stringify(sols));
    if(btn){ btn.textContent='📩 Enviar solicitud'; btn.disabled=false; }
    ['panelSolicitud'].forEach(function(id){ var el=document.getElementById(id); if(el) el.style.display='none'; });
    var pe = document.getElementById('panelEnviada'); if(pe) pe.style.display='block';
    var txt = '🔑 Solicitud USALA\n👤 '+nombre+'\n📞 '+contacto+(motivo?'\n💬 '+motivo:'');
    var waBtn = document.getElementById('_solWaBtn');
    if(waBtn) waBtn.href='https://wa.me/?text='+encodeURIComponent(txt);
  });
}

function importarSolicitud(){
  var raw = (document.getElementById('importSolInp').value||'').trim();
  if(!raw){ showToast('⚠ Pega el mensaje primero'); return; }
  var sol=null;
  try{
    var match = raw.match(/([A-Za-z0-9+/]{20,}={0,2})/);
    if(match) sol=JSON.parse(decodeURIComponent(escape(atob(match[1]))));
    else sol=JSON.parse(raw);
  } catch(e){ showToast('⚠ No se pudo leer el mensaje'); return; }
  if(!sol||!sol.nombre){ showToast('⚠ Mensaje inválido'); return; }
  var sols=JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
  var ya=sols.find(function(s){ return s.contacto===sol.contacto && s.estado==='pendiente'; });
  if(ya){ showToast('Ya existe solicitud pendiente de '+sol.nombre); return; }
  sol.estado='pendiente'; sol.importada=true;
  sols.push(sol); localStorage.setItem('usala_solicitudes',JSON.stringify(sols));
  document.getElementById('importSolInp').value='';
  showToast('✅ Solicitud de '+sol.nombre+' registrada');
  goSub('codigos');
}

async function _hashPass(pass){
  var enc = new TextEncoder();
  var buf = await crypto.subtle.digest('SHA-256', enc.encode(pass));
  return Array.from(new Uint8Array(buf)).map(function(b){ return b.toString(16).padStart(2,'0'); }).join('');
}

function olvidarContraseña(){
  var codigo = (document.getElementById('accCodigo').value||'').trim().toUpperCase();
  showToast('📩 Pídele al administrador que te genere un nuevo código para '+codigo);
}

function cerrarWelcome(){
  var m = document.getElementById('welcomeModal');
  var bd = document.getElementById('welcomeBackdrop');
  var sh = document.getElementById('welcomeSheet');
  if(bd) bd.style.background = 'rgba(0,0,0,0)';
  if(sh) sh.style.transform = 'translateY(100%)';
  setTimeout(function(){ if(m) m.style.display = 'none'; }, 500);
  if(S.user && !S.user.isAdmin){
    localStorage.setItem('usala_bienvenida_' + S.user.codigo, '1');
  }
}

function iniciarDragBurbuja(){
  var bb = document.getElementById('calcBubble');
  var startX,startY,startL,startT,dragging=false,moved=false;
  bb.ontouchstart=function(e){
    if(e.touches.length!==1) return;
    dragging=true; moved=false;
    var r=bb.getBoundingClientRect();
    startX=e.touches[0].clientX; startY=e.touches[0].clientY;
    startL=r.left; startT=r.top;
    bb.style.right='auto'; bb.style.bottom='auto';
    e.preventDefault();
  };
  bb.ontouchmove=function(e){
    if(!dragging||e.touches.length!==1) return;
    moved=true;
    var dx=e.touches[0].clientX-startX, dy=e.touches[0].clientY-startY;
    bb.style.left=Math.max(0,Math.min(window.innerWidth-68,startL+dx))+'px';
    bb.style.top =Math.max(0,Math.min(window.innerHeight-68,startT+dy))+'px';
    e.preventDefault();
  };
  bb.ontouchend=function(e){
    dragging=false;
    if(!moved) restaurarCalc(); // tap sin drag = restaurar
  };
}

function iniciarDragCalc(){
  var handle = document.getElementById('calcHandle');
  var cf = document.getElementById('calcFloat');
  var startX,startY,startL,startT,dragging=false;
  function esBtnCalc(el){ return el.id==='calcMinBtn'||el.id==='calcCloseBtn'||el.closest&&(el.closest('#calcMinBtn')||el.closest('#calcCloseBtn')); }
  handle.ontouchstart = function(e){
    if(esBtnCalc(e.target)) return;
    if(e.touches.length!==1) return;
    dragging=true;
    var r=cf.getBoundingClientRect();
    startX=e.touches[0].clientX; startY=e.touches[0].clientY;
    startL=r.left; startT=r.top;
    cf.style.right='auto'; cf.style.bottom='auto';
    cf.style.left=startL+'px'; cf.style.top=startT+'px';
    e.preventDefault();
  };
  handle.ontouchmove = function(e){
    if(!dragging||e.touches.length!==1) return;
    var dx=e.touches[0].clientX-startX, dy=e.touches[0].clientY-startY;
    var newL=Math.max(0,Math.min(window.innerWidth-cf.offsetWidth, startL+dx));
    var newT=Math.max(0,Math.min(window.innerHeight-cf.offsetHeight, startT+dy));
    cf.style.left=newL+'px'; cf.style.top=newT+'px';
    e.preventDefault();
  };
  handle.ontouchend=function(){ dragging=false; };
  handle.onmousedown=function(e){
    if(esBtnCalc(e.target)) return;
    dragging=true;
    var r=cf.getBoundingClientRect();
    startX=e.clientX; startY=e.clientY;
    startL=r.left; startT=r.top;
    cf.style.right='auto'; cf.style.bottom='auto';
    cf.style.left=startL+'px'; cf.style.top=startT+'px';
    e.preventDefault();
  };
  document.onmousemove=function(e){
    if(!dragging) return;
    var newL=Math.max(0,Math.min(window.innerWidth-cf.offsetWidth, startL+(e.clientX-startX)));
    var newT=Math.max(0,Math.min(window.innerHeight-cf.offsetHeight, startT+(e.clientY-startY)));
    cf.style.left=newL+'px'; cf.style.top=newT+'px';
  };
  document.onmouseup=function(){ dragging=false; };
}


function calcNum(n){
  if(_calcNewNum){ _calcResult=n; _calcNewNum=false; }
  else { _calcResult=_calcResult==='0'?n:_calcResult+n; }
  document.getElementById('calcDisplay').textContent=_calcResult;
}

function calcPlusMinus(){
  if(_calcResult==='0') return;
  _calcResult=_calcResult.startsWith('-')?_calcResult.slice(1):'-'+_calcResult;
  document.getElementById('calcDisplay').textContent=_calcResult;
}

function calcPunto(){
  if(_calcNewNum){ _calcResult='0.'; _calcNewNum=false; }
  else if(!_calcResult.includes('.')) _calcResult+='.';
  document.getElementById('calcDisplay').textContent=_calcResult;
}

function calcEqual(){
  try{
    var expr=(_calcExpr+_calcResult).replace(/÷/g,'/').replace(/×/g,'*');
    expr=expr.replace(/(\d+\.?\d*)\s*%/g,function(m,n){ return (parseFloat(n)/100); });
    var res=Function('"use strict";return ('+expr+')')();
    _calcResult=parseFloat(res.toFixed(10)).toString();
    document.getElementById('calcDisplay').textContent=_calcResult;
    document.getElementById('calcExpr').textContent=_calcExpr+'=';
    _calcExpr=''; _calcNewNum=true;
  }catch(e){ document.getElementById('calcDisplay').textContent='Error'; _calcExpr=''; _calcNewNum=true; }
}

function calcAc(){ _calcExpr=''; _calcResult='0'; _calcNewNum=true; document.getElementById('calcDisplay').textContent='0'; document.getElementById('calcExpr').textContent=''; }

function poblarCuentas(cuentaActual){
  var c = getCuentas();
  var sel = document.getElementById('txCuenta');
  if(!sel) return;
  var ops = '<option value="">— Sin asignar —</option>'
    +'<option value="efectivo"'+(cuentaActual==='efectivo'?' selected':'')+'>💵 Efectivo</option>';
  (c.cheques||[]).forEach(function(ch, i){
    var val = 'cheque_'+i;
    ops += '<option value="'+val+'"'+(cuentaActual===val?' selected':'')+'>🏧 '+ch.banco+' ('+ch.tipo+')</option>';
  });
  sel.innerHTML = ops;
}

function _abrirTxModalDirecto(tipo){
  S.editTxId = null;
  document.getElementById('txModalTitle').textContent = 'Nueva Transacción';
  document.getElementById('txDesc').value = '';
  document.getElementById('txMonto').value = '';
  document.getElementById('txFecha').value = today();
  document.getElementById('tipoSelector').style.display = 'grid';
  document.getElementById('txSaveBtn').textContent = '💾 Guardar';
  selTipo(tipo || 'gasto');
  poblarCuentas('');
  document.getElementById('txModal').classList.add('open');
  setTimeout(function(){ document.getElementById('txDesc').focus(); }, 400);
}

function cerrarIngresoTipo(){ document.getElementById('ingresoTipoModal').classList.remove('open'); }

function elegirTipoIngreso(tipo){
  cerrarIngresoTipo();
  if(tipo === 'normal'){
    _abrirTxModalDirecto('ingreso');
  } else if(tipo === 'prestamo'){
    _abrirModalPrestamoRecibido();
  } else if(tipo === 'cobro'){
    _abrirModalCobrarCxC();
  }
}

function _cobrarCxC(i){
  var cxcs = load('cxc',[]);
  var c = cxcs[i];
  if(!c) return;
  var txs = load('txs',[]);
  txs.push({ id:Date.now(), tipo:'ingreso', monto:c.monto,
    desc:'Cobré a: '+c.nombre, cat:'Cobro de deuda',
    fecha:today(), cuenta:'efectivo' });
  save('txs', txs);
  cxcs.splice(i,1);
  save('cxc', cxcs);
  document.getElementById('cobrarCxCModal').remove();
  showToast('✅ Cobro registrado');
  if(S.tab==='inicio') renderTab('inicio');
}

function cerrarGastoTipo(){ document.getElementById('gastoTipoModal').classList.remove('open'); }

function elegirTipoGasto(tipo){
  cerrarGastoTipo();
  if(tipo === 'normal'){
    _abrirTxModalDirecto('gasto');
  } else if(tipo === 'preste'){
    _abrirModalPreste();
  } else if(tipo === 'abono'){
    _abrirModalAbonoDeuda();
  }
}

function _abrirModalAbonoDeuda(){
  var creds = load('creditos',[]);
  var deudas = creds.filter(function(c){ return c.tipo==='deuda' && c.estado!=='pagado'; });
  if(deudas.length === 0){
    _abrirTxModalDirecto('gasto');
    showToast('No tienes deudas activas — registra como gasto normal');
    return;
  }
  var m = document.createElement('div');
  m.className = 'modal open';
  m.id = 'abonoModal';
  var lista = deudas.map(function(c){
    var ri = creds.indexOf(c);
    var pendiente = c.monto - (c.abonado||0);
    return '<button onclick="_seleccionarDeudaAbono('+ri+')" style="'
      +'display:flex;align-items:center;justify-content:space-between;'
      +'padding:14px 16px;border-radius:16px;border:1.5px solid var(--border);'
      +'background:var(--card);cursor:pointer;width:100%;color:var(--text);margin-bottom:10px;">'
      +'<div style="text-align:left;">'
      +'<div style="font-weight:700;">'+c.persona+'</div>'
      +'<div style="font-size:0.78rem;color:var(--dim);">'+(c.descripcion||'')+'</div>'
      +'</div>'
      +'<div style="text-align:right;">'
      +'<div style="font-weight:800;color:#ff5f57;">-'+fmt(pendiente)+'</div>'
      +'<div style="font-size:0.72rem;color:var(--dim);">pendiente</div>'
      +'</div>'
      +'</button>';
  }).join('');
  m.innerHTML = '<div class="modal-box" style="position:relative;z-index:2;">'
    +'<div class="modal-header"><div class="modal-title">💸 ¿A qué deuda abonaste?</div>'
    +'<button class="modal-close" onclick="document.getElementById(&quot;abonoModal&quot;).remove()">✕</button></div>'
    +'<p style="color:var(--dim);font-size:0.82rem;margin-bottom:14px;">Selecciona la deuda que pagaste</p>'
    +lista+'</div>';
  document.body.appendChild(m);
}

function _seleccionarDeudaAbono(ri){
  document.getElementById('abonoModal').remove();
  var creds = load('creditos',[]);
  var c = creds[ri];
  if(!c) return;
  var pendiente = c.monto - (c.abonado||0);
  var m = document.createElement('div');
  m.className = 'modal open';
  m.id = 'montoAbonoModal';
  m.setAttribute('data-ri', ri);
  m.innerHTML = '<div class="modal-box" style="position:relative;z-index:2;">'
    +'<div class="modal-header"><div class="modal-title">💸 Abono a '+c.persona+'</div>'
    +'<button class="modal-close" onclick="document.getElementById(&quot;montoAbonoModal&quot;).remove()">✕</button></div>'
    +'<p style="color:var(--dim);font-size:0.82rem;margin-bottom:4px;">'+( c.descripcion||'')+'</p>'
    +'<p style="font-size:0.82rem;margin-bottom:14px;">Pendiente: <b style="color:#ff5f57;">'+fmt(pendiente)+'</b></p>'
    +'<label class="inp-label">Monto del abono ($)</label>'
    +'<input class="inp" id="abonoMonto" type="number" inputmode="decimal" placeholder="0.00">'
    +'<label class="inp-label">¿De qué cuenta salió?</label>'
    +'<select class="inp" id="abonoCuenta"><option value="efectivo">💵 Efectivo</option><option value="banco">🏦 Banco</option></select>'
    +'<button class="lg-btn" style="margin-top:18px;" onclick="_guardarAbonoDeuda('+ri+')">💾 Guardar abono</button>'
    +'</div>';
  document.body.appendChild(m);
}

function _guardarAbonoDeuda(ri){
  var monto  = parseFloat(document.getElementById('abonoMonto').value||0);
  var cuenta = document.getElementById('abonoCuenta').value;
  if(!monto){ showToast('⚠ Ingresa el monto del abono'); return; }
  var creds = load('creditos',[]);
  var c = creds[ri];
  if(!c){ showToast('Error: deuda no encontrada'); return; }
  var pendiente = c.monto - (c.abonado||0);
  if(monto > pendiente) monto = pendiente;
  if(!c.historialAbonos) c.historialAbonos = [];
  c.historialAbonos.push({ fecha:today(), monto:monto, nota:'Pago directo' });
  c.abonado = (parseFloat(c.abonado)||0) + monto;
  if(c.abonado >= c.monto) c.estado = 'pagado';
  save('creditos', creds);
  var txs = load('txs',[]);
  txs.push({ id:Date.now(), tipo:'gasto', monto:monto,
    desc:'Abono: '+c.persona, cat:'Pagos / Deudas', fecha:today(), cuenta:cuenta });
  save('txs', txs);
  document.getElementById('montoAbonoModal').remove();
  showToast(c.estado==='pagado' ? '🎉 ¡Deuda saldada!' : '✅ Abono registrado');
  if(S.tab==='inicio') renderTab('inicio');
  if(S.tab==='creditos') renderTab('creditos');
}

function selTipo(t){
  document.getElementById('tipoGasto').classList.toggle('selected', t==='gasto');
  document.getElementById('tipoIngreso').classList.toggle('selected', t==='ingreso');
  var sel = document.getElementById('txCat');
  sel.innerHTML = t==='ingreso' ? buildIngresoCatSelect('txCat','') : buildGastoCatSelect('txCat','');
}

function _consejeroSVG(expresion){
  var ojos = {
    feliz:     '<circle cx="22" cy="26" r="3" fill="#2a1a00"/><circle cx="42" cy="26" r="3" fill="#2a1a00"/><circle cx="23" cy="25" r="1" fill="white"/><circle cx="43" cy="25" r="1" fill="white"/>',
    contento:  '<circle cx="22" cy="27" r="2.5" fill="#2a1a00"/><circle cx="42" cy="27" r="2.5" fill="#2a1a00"/><circle cx="23" cy="26" r="1" fill="white"/><circle cx="43" cy="26" r="1" fill="white"/>',
    preocupado:'<ellipse cx="22" cy="27" rx="3" ry="2.5" fill="#2a1a00"/><ellipse cx="42" cy="27" rx="3" ry="2.5" fill="#2a1a00"/><path d="M19 22 Q22 20 25 22" stroke="#2a1a00" stroke-width="1.5" fill="none"/>',
    triste:    '<ellipse cx="22" cy="28" rx="3" ry="2" fill="#2a1a00"/><ellipse cx="42" cy="28" rx="3" ry="2" fill="#2a1a00"/><path d="M18 22 Q22 19 26 22" stroke="#2a1a00" stroke-width="1.5" fill="none"/><path d="M38 22 Q42 19 46 22" stroke="#2a1a00" stroke-width="1.5" fill="none"/>',
  };
  var boca = {
    feliz:     '<path d="M24 35 Q32 42 40 35" stroke="#2a1a00" stroke-width="2" fill="none" stroke-linecap="round"/>',
    contento:  '<path d="M25 35 Q32 40 39 35" stroke="#2a1a00" stroke-width="2" fill="none" stroke-linecap="round"/>',
    preocupado:'<path d="M24 38 Q32 34 40 38" stroke="#2a1a00" stroke-width="2" fill="none" stroke-linecap="round"/>',
    triste:    '<path d="M24 40 Q32 34 40 40" stroke="#2a1a00" stroke-width="2" fill="none" stroke-linecap="round"/>',
  };
  var mejilla = (expresion==='feliz'||expresion==='contento')
    ? '<ellipse cx="16" cy="34" rx="5" ry="4" fill="rgba(255,150,120,0.3)"/><ellipse cx="48" cy="34" rx="5" ry="4" fill="rgba(255,150,120,0.3)"/>'
    : '';
  var colorCara = expresion==='triste'||expresion==='preocupado' ? '#FFD580' : '#FFE066';
  var colorSombrero = expresion==='feliz' ? '#1a8c4e' : expresion==='contento' ? '#0070cc' : expresion==='preocupado' ? '#c07a10' : '#cc2a2a';
  var signo = expresion==='feliz' ? '$' : expresion==='contento' ? '$' : expresion==='preocupado' ? '!' : '?';
  return '<svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">'
    +'<ellipse cx="32" cy="60" rx="18" ry="4" fill="rgba(0,0,0,0.08)"/>'
    +'<rect x="20" y="46" width="24" height="16" rx="8" fill="'+colorSombrero+'"/>'
    +'<rect x="27" y="42" width="10" height="8" rx="4" fill="'+colorCara+'"/>'
    +'<circle cx="32" cy="28" r="20" fill="'+colorCara+'"/>'
    +'<circle cx="32" cy="28" r="20" fill="none" stroke="rgba(0,0,0,0.06)" stroke-width="1"/>'
    +mejilla
    +ojos[expresion]
    +boca[expresion]
    +'<rect x="14" y="10" width="36" height="4" rx="2" fill="'+colorSombrero+'"/>'
    +'<rect x="20" y="2" width="24" height="10" rx="4" fill="'+colorSombrero+'"/>'
    +'<text x="32" y="10" text-anchor="middle" font-size="7" font-weight="900" fill="white">'+signo+'</text>'
    +'<ellipse cx="23" cy="20" rx="4" ry="3" fill="rgba(255,255,255,0.25)"/>'
    +'</svg>';
}

function renderConsejeroDetalle(){
  irProgreso();
}

function saveCarritoCats(cats){
  var defaultIds = ['agro','shop','super','mat','ins'];
  save('carrito_cats', cats.filter(function(c){ return defaultIds.indexOf(c.id)===-1; }));
}

function getProductosCatalogo(){ return load('carrito_catalogo', {}); }

function saveProductosCatalogo(c){ save('carrito_catalogo', c); }

function carritoUltimoPrecio(nombre){
  var cat = getProductosCatalogo();
  var key = nombre.trim().toLowerCase();
  var hist = cat[key];
  if(!hist || hist.length === 0) return null;
  return hist[0];
}

function carritoHistorialPreciosTienda(nombre){
  var cat = getProductosCatalogo();
  var key = nombre.trim().toLowerCase();
  return cat[key] || [];
}

function _carritoTab(t){ S._carritoTab = t; goSub('carrito'); }

function _carritoItemHTML(it, ri){
  var chkClass = it.comprado ? ' on' : '';
  var itemClass = it.comprado ? ' comprado' : '';
  var hist = carritoHistorialPreciosTienda(it.nombre);
  var mejorPrecio = hist.length > 1 ? hist.reduce(function(m,h){ return h.precio < m.precio ? h : m; }, hist[0]) : null;
  var precioStr = it.precio ? fmt(it.precio) : '—';
  var qtyStr = (it.qty||1) + ' ' + (it.unidad||'pza');
  return '<div class="carrito-item'+itemClass+'" id="ci_'+ri+'">'
    + '<div class="ci-check'+chkClass+'" onclick="carritoToggleItem('+ri+')">'+(it.comprado?'✓':'')+'</div>'
    + '<div class="ci-body" onclick="carritoEditarItem('+ri+')">'
    + '<div class="ci-nombre">'+it.nombre+'</div>'
    + '<div class="ci-meta">'+qtyStr+(it.nota?' · '+it.nota:'')+'</div>'
    + (mejorPrecio && !it.comprado ? '<div class="ci-precio-hist">💡 Mejor precio visto: '+fmt(mejorPrecio.precio)+' en '+mejorPrecio.tienda+'</div>' : '')
    + '</div>'
    + '<div class="ci-right">'
    + '<div class="ci-precio">'+precioStr+'</div>'
    + '<div class="ci-qty">'
    + '<button onclick="carritoQty('+ri+',-1)">−</button>'
    + '<span>'+(it.qty||1)+'</span>'
    + '<button onclick="carritoQty('+ri+',1)">+</button>'
    + '</div>'
    + '</div>'
    + '<button onclick="carritoEliminarItem('+ri+')" style="position:absolute;top:6px;right:6px;background:none;border:none;font-size:0.7rem;color:var(--dim);cursor:pointer;padding:2px 4px;">✕</button>'
    + '</div>';
}

function _filtrarCatalogo(q){
  var items = document.querySelectorAll('#catLista [data-prod]');
  items.forEach(function(el){
    var prod = el.getAttribute('data-prod') || '';
    el.style.display = prod.indexOf(q.toLowerCase()) > -1 ? '' : 'none';
  });
}

function carritoSelCat(id){
  var actual = getCarritoActual();
  actual.catId = id;
  saveCarritoActual(actual);
  goSub('carrito');
}

function carritoActualizarNombre(v){
  var actual = getCarritoActual(); actual.nombre = v; saveCarritoActual(actual);
}

function carritoActualizarTienda(v){
  var actual = getCarritoActual(); actual.tienda = v; saveCarritoActual(actual);
}

function carritoSugerirPrecio(nombre){
  var sug = document.getElementById('carritoSugerencia');
  if(!sug) return;
  if(!nombre || nombre.length < 2){ sug.style.display='none'; return; }
  var ultimo = carritoUltimoPrecio(nombre);
  if(ultimo){
    sug.style.display = 'block';
    sug.innerHTML = '💡 Última vez: <b>'+fmt(ultimo.precio)+'</b>'
      +(ultimo.tienda?' en '+ultimo.tienda:'')
      +' — '+ultimo.fecha
      +' <span style="font-size:0.65rem;opacity:0.7;">(toca para usar)</span>';
    sug._precio = ultimo.precio;
  } else {
    sug.style.display = 'none';
  }
}

function carritoAplicarSugerencia(){
  var sug = document.getElementById('carritoSugerencia');
  var inp = document.getElementById('carritoPrecioItem');
  if(sug && inp && sug._precio) inp.value = sug._precio;
}

function carritoEditarItem(ri){
  var actual = getCarritoActual();
  var item = actual.items[ri];
  if(!item) return;
  var modal = document.createElement('div');
  modal.style.cssText = 'position:fixed;inset:0;z-index:9000;background:rgba(0,0,0,0.5);display:flex;align-items:flex-end;';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 40px;width:100%;max-width:480px;margin:0 auto;">'
    + '<div style="font-size:1rem;font-weight:800;margin-bottom:16px;">✏️ Editar producto</div>'
    + '<input class="inp" id="editNombre" value="'+item.nombre+'" placeholder="Nombre" style="margin-bottom:8px;">'
    + '<div style="display:flex;gap:8px;margin-bottom:8px;">'
    + '<input class="inp" id="editPrecio" type="number" value="'+(item.precio||'')+'" placeholder="Precio" style="flex:1;">'
    + '<input class="inp" id="editQty" type="number" value="'+(item.qty||1)+'" placeholder="Cant." style="width:70px;">'
    + '</div>'
    + '<input class="inp" id="editNota" value="'+(item.nota||'')+'" placeholder="Nota" style="margin-bottom:12px;">'
    + '<button class="btn-main" onclick="carritoGuardarEdicion('+ri+',this.closest(\'div\').parentElement.parentElement)">💾 Guardar</button>'
    + '<button onclick="this.closest(\'div\').parentElement.parentElement.remove()" style="width:100%;margin-top:8px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    + '</div>';
  document.body.appendChild(modal);
}

function carritoGuardarEdicion(ri, modal){
  var actual = getCarritoActual();
  var item = actual.items[ri];
  if(!item) return;
  item.nombre = document.getElementById('editNombre').value.trim()||item.nombre;
  item.precio = parseFloat(document.getElementById('editPrecio').value)||0;
  item.qty    = parseInt(document.getElementById('editQty').value)||1;
  item.nota   = document.getElementById('editNota').value.trim();
  saveCarritoActual(actual);
  if(modal) modal.remove();
  goSub('carrito');
  showToast('✓ Producto actualizado');
}

function _carritoTextoLista(lista){
  var cats = getCarritoCats();
  var cat  = cats.find(function(c){ return c.id === lista.catId; });
  var lineas = [];
  lineas.push('🛒 *' + (lista.nombre || 'Lista de compras') + '*');
  if(lista.tienda) lineas.push('📍 ' + lista.tienda);
  lineas.push('📅 ' + (lista.fecha || today()));
  lineas.push('');
  var pendientes = (lista.items||[]).filter(function(i){ return !i.comprado; });
  var comprados  = (lista.items||[]).filter(function(i){ return i.comprado; });
  if(pendientes.length > 0){
    lineas.push('📋 *Pendientes:*');
    pendientes.forEach(function(i){
      var precio = i.precio ? ' — ' + fmt(i.precio) : '';
      lineas.push('☐ ' + i.nombre + ' x' + (i.qty||1) + ' ' + (i.unidad||'pza') + precio + (i.nota?' ('+i.nota+')':''));
    });
  }
  if(comprados.length > 0){
    lineas.push('');
    lineas.push('✅ *Comprados:*');
    comprados.forEach(function(i){
      var precio = i.precio ? ' — ' + fmt(i.precio) : '';
      lineas.push('☑ ' + i.nombre + ' x' + (i.qty||1) + ' ' + (i.unidad||'pza') + precio);
    });
  }
  var total = (lista.items||[]).reduce(function(s,i){ return s+(i.precio||0)*(i.qty||1); },0);
  if(total > 0){
    lineas.push('');
    lineas.push('💰 *Total estimado: ' + fmt(total) + '*');
  }
  lineas.push('');
  lineas.push('_Compartido desde USALA Finanzas_');
  return lineas.join('\n');
}

function _carritoMostrarModalCompartir(texto){
  var modal = document.createElement('div');
  modal.style.cssText = 'position:fixed;inset:0;z-index:9100;background:rgba(0,0,0,0.55);display:flex;align-items:flex-end;';
  var waUrl = 'https://wa.me/?text=' + encodeURIComponent(texto);
  var tgUrl = 'https://t.me/share/url?url=&text=' + encodeURIComponent(texto);
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 44px;width:100%;max-width:480px;margin:0 auto;">'
    + '<div style="width:36px;height:4px;background:var(--border);border-radius:2px;margin:0 auto 20px;"></div>'
    + '<div style="font-size:1rem;font-weight:800;color:var(--text);margin-bottom:16px;">📤 Compartir lista</div>'
    + '<div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px;">'
    + '<a href="'+waUrl+'" target="_blank" style="display:flex;align-items:center;justify-content:center;gap:8px;padding:14px;background:linear-gradient(135deg,#25D366,#1da855);border-radius:16px;text-decoration:none;color:#fff;font-family:Outfit,sans-serif;font-size:0.85rem;font-weight:700;box-shadow:0 4px 14px rgba(37,211,102,0.3);">'+
      '<span style="font-size:1.3rem;">💬</span> WhatsApp</a>'
    + '<a href="'+tgUrl+'" target="_blank" style="display:flex;align-items:center;justify-content:center;gap:8px;padding:14px;background:linear-gradient(135deg,#2AABEE,#1a8bc4);border-radius:16px;text-decoration:none;color:#fff;font-family:Outfit,sans-serif;font-size:0.85rem;font-weight:700;box-shadow:0 4px 14px rgba(42,171,238,0.25);">'+
      '<span style="font-size:1.3rem;">✈️</span> Telegram</a>'
    + '<button onclick="_carritoCopiarTexto(this)" data-texto="'+encodeURIComponent(texto)+'" style="display:flex;align-items:center;justify-content:center;gap:8px;padding:14px;background:var(--inp);border:1px solid var(--border);border-radius:16px;font-family:Outfit,sans-serif;font-size:0.85rem;font-weight:700;color:var(--text);cursor:pointer;">'+
      '<span style="font-size:1.3rem;">📋</span> Copiar texto</button>'
    + '<button onclick="_carritoShareNativo()" data-texto="'+encodeURIComponent(texto)+'" style="display:flex;align-items:center;justify-content:center;gap:8px;padding:14px;background:var(--inp);border:1px solid var(--border);border-radius:16px;font-family:Outfit,sans-serif;font-size:0.85rem;font-weight:700;color:var(--text);cursor:pointer;">'+
      '<span style="font-size:1.3rem;">&#x1F4F2;</span> Más opciones</button>'
    + '</div>'
    + '<div style="font-size:0.72rem;color:var(--dim);margin-bottom:6px;">Vista previa:</div>'
    + '<div style="background:var(--inp);border-radius:14px;padding:12px 14px;font-size:0.75rem;color:var(--text);line-height:1.6;max-height:150px;overflow-y:auto;white-space:pre-wrap;word-break:break-word;">'
    + texto.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;')
    + '</div>'
    + '<button onclick="this.parentElement.parentElement.remove()" style="width:100%;margin-top:14px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;padding:8px;">Cerrar</button>'
    + '</div>';
  document.body.appendChild(modal);
  modal.addEventListener('click', function(e){ if(e.target===modal) modal.remove(); });
}

function _carritoCopiarTexto(btn){
  var texto = decodeURIComponent(btn.getAttribute('data-texto'));
  navigator.clipboard.writeText(texto).then(function(){
    btn.innerHTML = '<span style="font-size:1.3rem;">✅</span> ¡Copiado!';
    setTimeout(function(){ btn.innerHTML = '<span style="font-size:1.3rem;">📋</span> Copiar texto'; }, 2000);
  }).catch(function(){
    var ta = document.createElement('textarea');
    ta.value = texto; ta.style.position='fixed'; ta.style.opacity='0';
    document.body.appendChild(ta); ta.select();
    document.execCommand('copy');
    ta.remove();
    showToast('✓ Lista copiada al portapapeles');
  });
}

function _carritoShareNativo(){
  var btn = document.querySelector('[data-texto]');
  var texto = btn ? decodeURIComponent(btn.getAttribute('data-texto')) : '';
  if(navigator.share){
    navigator.share({ title: 'Lista de compras', text: texto })
      .catch(function(){});
  } else {
    showToast('Usa WhatsApp o Telegram arriba');
  }
}

function _carritoColapsarBarra(){
  var bar = document.getElementById('carritoTotalBar');
  if(!bar) return;
  bar.querySelector('.ctb-detalle').style.display = 'none';
  bar.querySelector('.ctb-mini').style.display = 'block';
  bar.style.padding = '6px 14px';
  bar.style.opacity = '0.8';
}

function _carritoExpandirBarra(){
  var bar = document.getElementById('carritoTotalBar');
  if(!bar) return;
  bar.querySelector('.ctb-detalle').style.display = 'flex';
  bar.querySelector('.ctb-mini').style.display = 'none';
  bar.style.padding = '12px 16px';
  bar.style.opacity = '1';
}

function carritoCompartirLista(hi){
  var hist = getCarritoHistorial();
  var lista = hist[hi];
  if(!lista){ showToast('Lista no encontrada'); return; }
  var texto = _carritoTextoLista(lista);
  _carritoMostrarModalCompartir(texto);
}

function _carritoOpsCuentas(){
  var c = getCuentas();
  var ops = '<option value="">— Sin asignar —</option>'
    + '<option value="efectivo">💵 Efectivo</option>';
  (c.cheques||[]).forEach(function(ch,i){
    ops += '<option value="cheque_'+i+'">🏧 '+ch.banco+'</option>';
  });
  (c.tarjetas||[]).forEach(function(t,i){
    ops += '<option value="tc_'+i+'">💳 '+t.banco+'</option>';
  });
  return ops;
}

function carritoNuevaCat(){
  var modal = document.createElement('div');
  modal.style.cssText = 'position:fixed;inset:0;z-index:9000;background:rgba(0,0,0,0.5);display:flex;align-items:center;justify-content:center;padding:20px;';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px;padding:24px 20px;width:100%;max-width:380px;">'
    + '<div style="font-size:1rem;font-weight:800;margin-bottom:16px;">➕ Nueva categoría</div>'
    + '<input class="inp" id="nuevaCatIco" placeholder="Emoji (ej: 🌿)" style="margin-bottom:8px;width:80px;">'
    + '<input class="inp" id="nuevaCatNombre" placeholder="Nombre de la categoría" style="margin-bottom:14px;">'
    + '<button class="btn-main" onclick="carritoGuardarNuevaCat(this.closest(\'div\').parentElement)">✅ Crear categoría</button>'
    + '<button onclick="this.closest(\'div\').parentElement.remove()" style="width:100%;margin-top:8px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    + '</div>';
  document.body.appendChild(modal);
}

function carritoGuardarNuevaCat(modal){
  var ico    = (document.getElementById('nuevaCatIco').value||'🏷️').trim();
  var nombre = (document.getElementById('nuevaCatNombre').value||'').trim();
  if(!nombre){ showToast('⚠ Escribe el nombre'); return; }
  var defaultIds = ['agro','shop','super','mat','ins'];
  var custom = load('carrito_cats', []);
  var id = 'cat_'+Date.now();
  custom.push({ id:id, ico:ico, nombre:nombre });
  save('carrito_cats', custom);
  if(modal) modal.remove();
  showToast('✓ Categoría "'+nombre+'" creada');
  goSub('carrito');
}

function getGastoCats(){
  var custom = load('cats_gasto_custom', []);
  return GASTO_CATS_BASE.map(function(c){ return c.id; }).concat(custom);
}

function getIngresoCats(){
  var custom = load('cats_ingreso_custom', []);
  return INGRESO_CATS_BASE.map(function(c){ return c.id; }).concat(custom);
}

function getColorCat(id){
  var found = GASTO_CATS_BASE.find(function(c){ return c.id===id; });
  return found ? found.color : '#78909c';
}

function buildGastoCatSelect(id, valSeleccionado){
  var cats = getGastoCats();
  var sel = valSeleccionado ? migrarCat(valSeleccionado) : cats[0];
  return cats.map(function(c){ return '<option'+(c===sel?' selected':'')+'>'+c+'</option>'; }).join('');
}

function buildIngresoCatSelect(id, valSeleccionado){
  var cats = getIngresoCats();
  var sel = valSeleccionado ? migrarCat(valSeleccionado) : cats[0];
  return cats.map(function(c){ return '<option'+(c===sel?' selected':'')+'>'+c+'</option>'; }).join('');
}

function keyPagosMes(){
  var mes = new Date().toISOString().slice(0,7); // YYYY-MM
  var u = S.user;
  var base = u.isAdmin ? 'usala_admin' : 'usala_u_'+u.codigo;
  return base+'_pagos_estado_'+mes;
}

function getActivosCats(){ return ACTIVOS_CATS.concat(load('cats_activos_custom',[])); }

function renderFormActivo(idx){
  var activos=load('activos_personales',[]);
  var a=idx!==null?activos[idx]:{};
  var mc=document.getElementById('mainContent'); mc.innerHTML='';
  var d=document.createElement('div'); d.style.padding='20px 16px';
  var catOpts=getActivosCats().map(function(c){ return '<option value="'+c+'"'+(a.categoria===c?' selected':'')+'>'+c+'</option>'; }).join('');
  d.innerHTML='<div style="font-size:1rem;font-weight:800;margin-bottom:14px;">'+(idx!==null?'✏️ Editar':'➕ Nuevo')+' Activo</div>'
    +'<label class="inp-label">Nombre del activo</label><input class="inp" id="faName" placeholder="Ej: Casa Colonia Roma, Toyota Corolla..." value="'+(a.nombre||'')+'">'
    +'<label class="inp-label">Categoría</label><select class="inp" id="faCat">'+catOpts+'</select>'
    +'<button type="button" class="cat-add-btn" onclick="abrirCatModal(\'activos\',\'faCat\')">＋ Categoría</button>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Valor estimado ($)</label><input class="inp" id="faValor" type="number" min="0" placeholder="0.00" value="'+(a.valor||'')+'"></div>'
    +'<div><label class="inp-label">Fecha de adquisición</label><input class="inp" id="faFecha" type="date" value="'+(a.fecha||'')+'"></div>'
    +'</div>'
    +'<label class="inp-label">Descripción / notas</label><input class="inp" id="faDesc" placeholder="Notas opcionales..." value="'+(a.descripcion||'')+'" style="margin-bottom:16px;">';
  var bOk=document.createElement('button'); bOk.className='btn-main'; bOk.textContent=idx!==null?'💾 Guardar':'➕ Agregar';
  bOk.onclick=function(){
    var nombre=document.getElementById('faName').value.trim();
    var valor=parseFloat(document.getElementById('faValor').value)||0;
    if(!nombre||!valor){ showToast('⚠ Nombre y valor son obligatorios'); return; }
    var cat=document.getElementById('faCat').value;
    var fecha=document.getElementById('faFecha').value;
    var desc=document.getElementById('faDesc').value.trim();
    var aa=load('activos_personales',[]);
    if(idx!==null){ aa[idx]={nombre:nombre,categoria:cat,valor:valor,fecha:fecha,descripcion:desc}; showToast('✓ Actualizado'); }
    else { aa.push({nombre:nombre,categoria:cat,valor:valor,fecha:fecha,descripcion:desc}); showToast('✓ Activo registrado'); }
    save('activos_personales',aa); renderActivos();
  };
  var bCan=document.createElement('button'); bCan.className='btn-sec'; bCan.style.marginTop='8px'; bCan.textContent='Cancelar';
  bCan.onclick=function(){ renderActivos(); };
  d.appendChild(bOk); d.appendChild(bCan); mc.appendChild(d);
  setTimeout(function(){ var el=document.getElementById('faName'); if(el) el.focus(); },80);
}

function _snapKey(){
  var u=S.user;
  return (u.isAdmin?'usala_admin':'usala_u_'+u.codigo)+'_snap_';
}

function guardarSnapshotMes(){
  var mes=new Date().toISOString().slice(0,7);
  var key=_snapKey()+mes;
  if(localStorage.getItem(key)) return; // ya existe
  _forzarSnapshot(mes, key);
}

function _forzarSnapshot(mes, key){
  var cu=getCuentas();
  var creds=load('creditos',[]);
  var activos=load('activos_personales',[]);
  var txs=getTxs();
  var txsMes=txs.filter(function(t){ return t.fecha&&t.fecha.slice(0,7)===mes; });
  var ingresos=txsMes.filter(function(t){ return t.tipo==='ingreso'; }).reduce(function(s,t){ return s+Number(t.monto||0); },0);
  var gastos  =txsMes.filter(function(t){ return t.tipo==='gasto';   }).reduce(function(s,t){ return s+Number(t.monto||0); },0);
  var efectivo=Number(cu.efectivo||0);
  var banco   =(cu.cheques||[]).reduce(function(s,x){ return s+Number(x.saldo||0); },0);
  var deudaTC =(cu.tarjetas||[]).reduce(function(s,t){ return s+Number(t.balance||0); },0);
  var deudaCred=creds.filter(function(c){ return c.tipo==='deuda'&&c.estado!=='pagado'; })
                     .reduce(function(s,c){ return s+Number(c.monto-(c.abonado||0)); },0);
  var totalActivos=activos.reduce(function(s,a){ return s+Number(a.valor||0); },0);
  var totalDeudas=deudaTC+deudaCred;
  var patrimonioNeto=(efectivo+banco+totalActivos)-totalDeudas;
  var snap={mes:mes,efectivo:efectivo,banco:banco,deudaTC:deudaTC,deudaCred:deudaCred,
    totalActivos:totalActivos,totalDeudas:totalDeudas,patrimonioNeto:patrimonioNeto,
    ingresos:ingresos,gastos:gastos,fecha:new Date().toISOString()};
  localStorage.setItem(key, JSON.stringify(snap));
}

function getSnapshots(){
  var prefix=_snapKey();
  var snaps=[];
  for(var k in localStorage){
    if(k.indexOf(prefix)===0){
      var raw=localStorage.getItem(k);
      if(raw){ try{ snaps.push(JSON.parse(raw)); }catch(e){} }
    }
  }
  snaps.sort(function(a,b){ return a.mes.localeCompare(b.mes); });
  return snaps;
}

function _selTipoInteres(tipo){
  _tipoInteresActual = tipo;
  ['total','mensual','anual'].forEach(function(t){
    var el = document.getElementById('tiInt' + t.charAt(0).toUpperCase() + t.slice(1));
    if(el) el.classList.toggle('selected', t === tipo);
  });
  _actualizarResumenInteres();
}

function _getTipoInteresSeleccionado(){
  return _tipoInteresActual || 'total';
}

function _actualizarResumenInteres(){
  var montoEl   = document.getElementById('crMonto');
  var interesEl = document.getElementById('crInteres');
  var resEl     = document.getElementById('resumenInteres');
  if(!montoEl || !interesEl || !resEl) return;
  var monto   = parseFloat(montoEl.value) || 0;
  var interes = parseFloat(interesEl.value) || 0;
  if(!monto || !interes){ resEl.style.display='none'; return; }
  var tipo  = _tipoInteresActual || 'total';
  var texto = '';
  if(tipo === 'total'){
    var montoInteres = monto * interes / 100;
    var total = monto + montoInteres;
    texto = '📦 Interés sobre el total: <b>+' + fmt(montoInteres) + '</b> → Total a pagar: <b>' + fmt(total) + '</b>';
  } else if(tipo === 'mensual'){
    var porMes = monto * interes / 100;
    texto = '📅 Interés mensual: <b>+' + fmt(porMes) + '/mes</b> — se acumula cada mes hasta liquidar';
  } else if(tipo === 'anual'){
    var porAnio = monto * interes / 100;
    var porMesAnual = porAnio / 12;
    texto = '📆 Interés anual: <b>+' + fmt(porAnio) + '/año</b> (~' + fmt(porMesAnual) + '/mes)';
  }
  resEl.innerHTML = texto;
  resEl.style.display = 'block';
}

function _initTipoInteres(tipoGuardado){
  _tipoInteresActual = tipoGuardado || 'total';
  var grid = document.getElementById('tipoInteresGrid');
  if(!grid) return;
  var opts = [['total','📦 Total'],['mensual','📅 Mensual'],['anual','📆 Anual']];
  grid.innerHTML = opts.map(function(o){
    var sel = _tipoInteresActual === o[0] ? 'selected' : '';
    return '<button type="button" id="tiInt'+o[0]+'" onclick="_selTipoInteres(&quot;'+o[0]+'&quot;)" class="tipo-opt '+sel+'" style="border-radius:12px;padding:10px 4px;font-size:0.78rem;">'+o[1]+'</button>';
  }).join('');
}

function guardarEdicionAbono(ri, ai, tipo){
  var capital = parseFloat(document.getElementById('eaCapital').value)||0;
  var interes = parseFloat(document.getElementById('eaInteres').value)||0;
  var fecha   = document.getElementById('eaFecha').value;
  var nota    = document.getElementById('eaNota').value.trim();
  if(!fecha){ showToast('⚠ Selecciona la fecha'); return; }
  if(capital<=0 && interes<=0){ showToast('⚠ Ingresa al menos un monto'); return; }
  var creds = load('creditos',[]);
  var a = creds[ri].historialAbonos[ai];
  var diffCap = capital - (a.monto||0);
  var diffInt = interes  - (a.interes||0);
  creds[ri].abonado          = Math.max(0,(creds[ri].abonado||0)+diffCap);
  creds[ri].interesesPagados = Math.max(0,(creds[ri].interesesPagados||0)+diffInt);
  creds[ri].historialAbonos[ai] = { monto:capital, interes:interes, fecha:fecha, nota:nota };
  if(creds[ri].abonado >= creds[ri].monto) creds[ri].estado='pagado';
  else if(creds[ri].estado==='pagado')     creds[ri].estado='pendiente';
  save('creditos', creds);
  showToast('✓ Abono actualizado');
  goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
}

function confirmarAbono(ri, tipo){
  if(ri === undefined || ri === null) ri = window._abonoRi;
  if(ri === undefined || ri === null){ showToast('⚠ Error: recarga e intenta de nuevo'); return; }
  var monto   = parseFloat(document.getElementById('abonoMonto').value)||0;
  var interes = parseFloat(document.getElementById('abonoInteres').value)||0;
  var fecha   = document.getElementById('abonoFecha').value;
  if(monto<=0 && interes<=0){ showToast('⚠ Ingresa al menos un monto'); return; }
  if(!fecha){ showToast('⚠ Selecciona la fecha'); return; }
  var nota = (document.getElementById('abonoNota') ? document.getElementById('abonoNota').value.trim() : '') || '';
  var creds = load('creditos',[]);
  if(!creds[ri]){ showToast('⚠ Crédito no encontrado'); return; }
  var esCobrar = (tipo||creds[ri].tipo) === 'prestamo';
  creds[ri].abonado = (creds[ri].abonado||0) + monto;
  creds[ri].interesesPagados = (creds[ri].interesesPagados||0) + interes;
  if(!creds[ri].historialAbonos) creds[ri].historialAbonos = [];
  creds[ri].historialAbonos.push({ monto:monto, interes:interes, fecha:fecha, nota:nota });
  var resumen = fmt(monto) + (interes>0 ? ' + '+fmt(interes)+' int.' : '');
  if(creds[ri].abonado >= creds[ri].monto){
    creds[ri].estado = 'pagado';
    showToast(esCobrar ? '🎉 ¡Cobro completo! '+resumen : '🎉 ¡Liquidado! '+resumen);
  } else {
    var pendiente = creds[ri].monto - creds[ri].abonado;
    showToast((esCobrar?'💰 Pago recibido: ':'✓ Abono: ') + resumen + ' · Resta: '+fmt(pendiente));
  }
  save('creditos', creds);
  window._abonoRi = null; window._abonoTipo = null;
  goSub(esCobrar ? 'creditos_cobrar' : 'creditos_debo');
}

function _adminTab(t){ _adminPanelTab = t; renderAdminPanel(); }

function _adminCfgNombreApp(){
  var actual = (JSON.parse(localStorage.getItem('usala_cfg_global')||'{}')).nombreApp || 'USALA Finanzas';
  usalaPrompt('Nombre de la app:', actual, function(nuevo){
    if(!nuevo||!nuevo.trim()) return;
    _adminToggleCfg('nombreApp', nuevo.trim());
    _adminRenderConfig();
  });
}

function _adminCfgBienvenida(){
  var actual = (JSON.parse(localStorage.getItem('usala_cfg_global')||'{}')).msgBienvenida || '';
  usalaPrompt('Mensaje de bienvenida para nuevos usuarios:', actual, function(nuevo){
    if(nuevo===null||nuevo===undefined) return;
    _adminToggleCfg('msgBienvenida', nuevo.trim());
    _adminRenderConfig();
  });
}

function _adminMetricCard(label, valor, color){
  return '<div class="card" style="padding:14px;text-align:center;">'
    + '<div style="font-size:0.7rem;color:var(--dim);margin-bottom:4px;">' + label + '</div>'
    + '<div style="font-size:1rem;font-weight:900;color:' + color + ';">' + valor + '</div>'
    + '</div>';
}

function abonarMeta(i){
  var m=load('metas',[]);
  usalaPrompt('💰 Abonar a meta: '+m[i].nombre, '', function(val){
    var a=parseFloat(val);
    if(!a||a<=0){ showToast('Ingresa un monto válido'); return; }
    m[i].actual=(m[i].actual||0)+a;
    if(m[i].actual>=m[i].meta){ showToast('🎉 Meta alcanzada!'); }
    else { showToast('Abono registrado: '+fmt(a)); }
    save('metas',m); goSub('metas');
  },{type:'number', placeholder:'0.00'});
}

function editarMeta(i){
  var m=load('metas',[]);
  usalaPrompt2('✏️ Editar meta', [
    {label:'Nombre', value:m[i].nombre, placeholder:'Nombre de la meta'},
    {label:'Objetivo ($)', value:m[i].meta, type:'number', placeholder:'0.00'}
  ], function(vals){
    var nombre=vals[0].trim(); var meta=parseFloat(vals[1]);
    if(!nombre||!meta){ showToast('Completa nombre y objetivo'); return; }
    m[i]=Object.assign(m[i],{nombre:nombre,meta:meta});
    save('metas',m); showToast('Meta actualizada'); goSub('metas');
  });
}

function getPresCats(){
  var custom = load('cats_gasto_custom',[]);
  var extra = custom.map(function(id){ return {id:id, color:'#78909c'}; });
  return GASTO_CATS_BASE.concat(extra);
}

function guardarPres(cat,val){ var p=load('presupuesto',{}); p[cat]=parseFloat(val)||0; save('presupuesto',p); showToast('✓ Límite guardado'); }

function editarAlerta(i){
  var a=load('alertas',[])[i];
  document.getElementById('alNombre').value=a.nombre;
  document.getElementById('alLimite').value=a.limite;
  document.getElementById('alFecha').value=a.fecha;
  document.getElementById('alSaveBtn').textContent='💾 Guardar cambios';
  window._editAlerta=i;
  document.getElementById('alertaForm').scrollIntoView({behavior:'smooth'});
}

function _toggleImportPanel(){
  var p=document.getElementById('importSolPanel');
  var b=document.getElementById('btnToggleImport');
  if(!p) return;
  var open = p.style.display==='none';
  p.style.display = open ? 'block' : 'none';
  if(b) b.textContent = open ? '✕ Cerrar' : '+ Pegar';
}

function _generarCodigoUnico(prefijo){
  var chars = 'ABCDEFGHJKMNPQRSTUVWXYZ23456789'; // sin 0,O,1,I,L
  function rnd4(){ var s=''; for(var i=0;i<4;i++) s+=chars[Math.floor(Math.random()*chars.length)]; return s; }
  var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var codigo = prefijo+'-'+rnd4();
  var intentos = 0;
  while(cods.find(function(x){ return x.codigo===codigo; }) && intentos++<20){
    codigo = prefijo+'-'+rnd4();
  }
  return codigo;
}


function aprobarSolicitud(idx){
  var solicitudes=JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
  var s=solicitudes[idx]; if(!s) return;
  _aprobarIdx = idx;
  var mc = document.getElementById('aprobarModal');
  if(!mc){
    mc = document.createElement('div');
    mc.id = 'aprobarModal';
    mc.style.cssText = 'position:fixed;inset:0;background:rgba(0,0,0,0.55);z-index:9999;display:flex;align-items:flex-end;justify-content:center;';
    mc.innerHTML =
      '<div style="background:var(--card);border-radius:24px 24px 0 0;padding:24px 20px 32px;width:100%;max-width:480px;">'
      +'<div style="font-weight:900;font-size:1rem;margin-bottom:4px;">✅ Aprobar solicitud</div>'
      +'<div id="aprobarNombreLabel" style="font-size:0.8rem;color:var(--dim);margin-bottom:18px;"></div>'
      +'<label class="inp-label">Prefijo del código</label>'
      +'<input class="inp" id="aprobarPrefijo" maxlength="5" style="text-transform:uppercase;">'
      +'<label class="inp-label">Vigencia del acceso</label>'
      +'<select class="inp" id="aprobarVence">'
        +'<option value="7">7 días</option>'
        +'<option value="15">15 días</option>'
        +'<option value="30" selected>1 mes</option>'
        +'<option value="90">3 meses</option>'
        +'<option value="180">6 meses</option>'
        +'<option value="365">1 año</option>'
      +'</select>'
      +'<button onclick="_confirmarAprobacion()" style="width:100%;margin-top:14px;padding:14px;background:var(--accent2);color:#fff;border:none;border-radius:14px;font-family:Outfit,sans-serif;font-weight:800;font-size:0.92rem;cursor:pointer;">🔑 Generar código</button>'
      +'<button onclick="cerrarAprobarModal()" style="width:100%;margin-top:8px;padding:12px;background:none;border:none;color:var(--dim);font-family:Outfit,sans-serif;font-size:0.85rem;cursor:pointer;">Cancelar</button>'
      +'</div>';
    document.body.appendChild(mc);
  }
  var prefijoAuto = (s.nombre.split(' ')[0]).substring(0,4).toUpperCase()||'USR';
  document.getElementById('aprobarPrefijo').value = prefijoAuto;
  document.getElementById('aprobarNombreLabel').textContent = '👤 '+s.nombre+(s.contacto?' · 📞 '+s.contacto:'');
  mc.style.display = 'flex';
}

function cerrarAprobarModal(){ var m=document.getElementById('aprobarModal'); if(m) m.remove(); }

function _confirmarAprobacion(){
  var solicitudes=JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
  var s=solicitudes[_aprobarIdx]; if(!s) return;
  var prefijo=(document.getElementById('aprobarPrefijo').value.trim().toUpperCase()||'USR').substring(0,5);
  var dias=parseInt(document.getElementById('aprobarVence').value)||30;
  var codigo=_generarCodigoUnico(prefijo);
  var venc=new Date(); venc.setDate(venc.getDate()+dias);
  var vencStr=venc.toISOString().split('T')[0];
  var codigos=JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  codigos.push({codigo:codigo,vencimiento:vencStr,nota:s.nombre,contacto:s.contacto||'',activo:true,usado:false,creado:today()});
  localStorage.setItem('usala_codigos',JSON.stringify(codigos));
  solicitudes[_aprobarIdx].estado='aprobada';
  solicitudes[_aprobarIdx].codigoGenerado=codigo;
  localStorage.setItem('usala_solicitudes',JSON.stringify(solicitudes));
  navigator.clipboard.writeText(codigo).catch(function(){});
  var modal=document.getElementById('aprobarModal'); if(modal) modal.remove();
  showToast('✅ Código '+codigo+' generado y copiado — compártelo con '+s.nombre);
  goSub('codigos');
}

function rechazarSolicitud(idx){
  usalaConfirm('Rechazar esta solicitud?', function(){
    var solicitudes=JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
      solicitudes[idx].estado='rechazada';
      localStorage.setItem('usala_solicitudes',JSON.stringify(solicitudes));
      showToast('✓ Solicitud rechazada');
      goSub('codigos');
  });
}

function _actualizarCodPreview(){
  var pref = (document.getElementById('codPrefijo').value||'FIN').toUpperCase().slice(0,4);
  var prev = document.getElementById('codPreview');
  if(prev) prev.textContent = pref + '-????';
}

function generarCodigo(){
  var prefijo=document.getElementById('codPrefijo').value.trim().toUpperCase()||'FIN';
  var dias=parseInt(document.getElementById('codVence').value);
  var nota=document.getElementById('codNota').value.trim();
  var contacto=document.getElementById('codContacto').value.trim();
  if(!nota){ showToast('⚠ Escribe el nombre del usuario'); return; }
  var codigo=_generarCodigoUnico(prefijo);
  var venc=new Date(); venc.setDate(venc.getDate()+dias);
  var vencStr=venc.toISOString().split('T')[0];
  var codigos=JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  codigos.push({codigo:codigo,vencimiento:vencStr,nota:nota,contacto:contacto,activo:true,usado:false,creado:today(),nombreUsuario:nota});
  localStorage.setItem('usala_codigos',JSON.stringify(codigos));
  dbCrearCodigo(codigo, nota, vencStr+'T23:59:59Z', contacto, nota).then(function(res){
    if(res) console.log('✅ Código en Supabase:', codigo);
    else console.warn('⚠️ Solo guardado local');
  });
  navigator.clipboard.writeText(codigo).catch(function(){});
  showToast('✓ Código '+codigo+' copiado — compártelo con '+nota);
  goSub('codigos');
}

function resetearNipUsuario(arg){
  usalaConfirm('Resetear el NIP de este usuario?\nEl usuario podra entrar sin NIP.', function(){
    localStorage.removeItem('usala_nip_u_'+codigo);
      showToast('🔓 NIP de '+nombre+' reseteado. Ya puede entrar sin NIP.');
      goSub('codigos');
  });
}

function pickTema(){
  var html = '<div class="page-header">'
    + '<button onclick="goSub(&quot;config&quot;)" style="background:none;border:none;color:var(--accent);font-size:1rem;cursor:pointer;padding:4px 8px;">← Atrás</button>'
    + '<div class="page-title">🎨 Tema visual</div></div>'
    + '<div class="card">'
    + '<div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;">'
    + '<div class="theme-card" data-theme="default" style="background:#f0f4f0;color:#1e6b3c;border:2px solid transparent;" onclick="elegirTema(this,&quot;default&quot;)">'
    +   '<div style="width:28px;height:28px;border-radius:50%;background:#1e6b3c;margin-bottom:8px;"></div>'
    +   '<div style="font-weight:700;font-size:0.9rem;">Verde Natural</div></div>'
    + '<div class="theme-card" data-theme="dark" style="background:#162016;color:#2d9e5f;border:2px solid transparent;" onclick="elegirTema(this,&quot;dark&quot;)">'
    +   '<div style="width:28px;height:28px;border-radius:50%;background:#2d9e5f;margin-bottom:8px;"></div>'
    +   '<div style="font-weight:700;font-size:0.9rem;color:#e8f5e8;">Oscuro Pro</div></div>'
    + '<div class="theme-card" data-theme="gold" style="background:#140f00;color:#c9841a;border:2px solid transparent;" onclick="elegirTema(this,&quot;gold&quot;)">'
    +   '<div style="width:28px;height:28px;border-radius:50%;background:#c9841a;margin-bottom:8px;"></div>'
    +   '<div style="font-weight:700;font-size:0.9rem;color:#f5e6c0;">Dorado Élite</div></div>'
    + '<div class="theme-card" data-theme="ocean" style="background:#e8f4fd;color:#0066cc;border:2px solid transparent;" onclick="elegirTema(this,&quot;ocean&quot;)">'
    +   '<div style="width:28px;height:28px;border-radius:50%;background:#0066cc;margin-bottom:8px;"></div>'
    +   '<div style="font-weight:700;font-size:0.9rem;">Océano</div></div>'
    + '<div class="theme-card" data-theme="rose" style="background:#fff5f7;color:#c02040;border:2px solid transparent;grid-column:1/-1;" onclick="elegirTema(this,&quot;rose&quot;)">'
    +   '<div style="width:28px;height:28px;border-radius:50%;background:#c02040;margin-bottom:8px;"></div>'
    +   '<div style="font-weight:700;font-size:0.9rem;">Rosa Elegante</div></div>'
    + '</div></div>';
  document.getElementById('mainContent').innerHTML = html;
  var activo = document.querySelector('.theme-card[data-theme="'+(S.theme||'default')+'"]');
  if(activo) activo.style.border = '2px solid currentColor';
}

function elegirTema(el, t){
  document.querySelectorAll('.theme-card').forEach(function(c){ c.style.border='2px solid transparent'; });
  el.style.border = '2px solid currentColor';
  S.theme = t;
  applyTheme(t);
  localStorage.setItem('usala_theme', t);
  showToast('🎨 Tema aplicado');
}

function _getMicEstado(){
  var p = localStorage.getItem('usala_mic_permiso');
  if(!p)    return 'No solicitado aún';
  if(p === 'granted') return '✅ Permitido';
  if(p === 'denied')  return '❌ Denegado';
  return p;
}

function _getMonedaApp(){
  var key = 'usala_moneda_app_' + (S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : 'anon');
  try{ var m = JSON.parse(localStorage.getItem(key)||'null');
    return m ? (m.bandera+' '+m.nombre+' ('+m.simbolo+')') : '🇲🇽 Pesos mexicanos ($)'; }
  catch(e){ return '🇲🇽 Pesos mexicanos ($)'; }
}

function abrirSelectorMoneda(){
  var monedas = [
    {codigo:'MXN', nombre:'Pesos mexicanos', simbolo:'$', bandera:'🇲🇽'},
    {codigo:'USD', nombre:'Dólares',          simbolo:'$', bandera:'🇺🇸'},
    {codigo:'EUR', nombre:'Euros',            simbolo:'€', bandera:'🇪🇺'},
    {codigo:'CAD', nombre:'Dólar canadiense', simbolo:'$', bandera:'🇨🇦'},
    {codigo:'GBP', nombre:'Libras',           simbolo:'£', bandera:'🇬🇧'},
    {codigo:'COP', nombre:'Pesos colombianos',simbolo:'$', bandera:'🇨🇴'},
    {codigo:'ARS', nombre:'Pesos argentinos', simbolo:'$', bandera:'🇦🇷'},
    {codigo:'GTQ', nombre:'Quetzales',        simbolo:'Q', bandera:'🇬🇹'},
    {codigo:'PEN', nombre:'Soles',            simbolo:'S/',bandera:'🇵🇪'},
  ];
  var key = 'usala_moneda_app_' + (S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : 'anon');
  var actual;
  try{ actual = JSON.parse(localStorage.getItem(key)||'null'); }catch(e){ actual = null; }
  var html = '<div class="page-header">'
    +'<button onclick="goSub(&quot;config&quot;)" style="background:none;border:none;color:var(--accent);font-size:1rem;cursor:pointer;padding:4px 8px;">← Atrás</button>'
    +'<div class="page-title">💱 Moneda de la app</div></div>'
    +'<div class="card">'
    +'<div style="font-size:0.8rem;color:var(--dim);margin-bottom:14px;line-height:1.5;">El símbolo se mostrará en toda la app: saldos, historial y reportes.</div>'
    + monedas.map(function(m){
        var activa = actual && actual.codigo === m.codigo;
        return '<div onclick="guardarMonedaApp(&quot;'+m.codigo+'&quot;)" style="display:flex;align-items:center;gap:12px;padding:14px 12px;border-radius:14px;margin-bottom:6px;cursor:pointer;background:'+(activa?'rgba(30,107,60,0.10)':'var(--inp)')+';border:2px solid '+(activa?'var(--accent)':'transparent')+';">'
          +'<span style="font-size:1.4rem;">'+m.bandera+'</span>'
          +'<div style="flex:1;"><div style="font-weight:700;font-size:0.9rem;color:var(--text);">'+m.nombre+'</div>'
          +'<div style="font-size:0.72rem;color:var(--dim);">'+m.codigo+' · símbolo: '+m.simbolo+'</div></div>'
          +(activa?'<span style="color:var(--accent);font-size:1.1rem;">✓</span>':'')
          +'</div>';
      }).join('')
    +'</div>';
  document.getElementById('mainContent').innerHTML = html;
}

function guardarMonedaApp(codigo){
  var monedas = {
    MXN:{codigo:'MXN',nombre:'Pesos mexicanos', simbolo:'$', bandera:'🇲🇽'},
    USD:{codigo:'USD',nombre:'Dólares',          simbolo:'$', bandera:'🇺🇸'},
    EUR:{codigo:'EUR',nombre:'Euros',            simbolo:'€', bandera:'🇪🇺'},
    CAD:{codigo:'CAD',nombre:'Dólar canadiense', simbolo:'$', bandera:'🇨🇦'},
    GBP:{codigo:'GBP',nombre:'Libras',           simbolo:'£', bandera:'🇬🇧'},
    COP:{codigo:'COP',nombre:'Pesos colombianos',simbolo:'$', bandera:'🇨🇴'},
    ARS:{codigo:'ARS',nombre:'Pesos argentinos', simbolo:'$', bandera:'🇦🇷'},
    GTQ:{codigo:'GTQ',nombre:'Quetzales',        simbolo:'Q', bandera:'🇬🇹'},
    PEN:{codigo:'PEN',nombre:'Soles',            simbolo:'S/',bandera:'🇵🇪'},
  };
  var m = monedas[codigo];
  if(!m) return;
  var key = 'usala_moneda_app_' + (S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : 'anon');
  localStorage.setItem(key, JSON.stringify(m));
  showToast(m.bandera+' Moneda cambiada a '+m.nombre);
  renderTab(S.tab); // refrescar pantalla actual
  abrirSelectorMoneda(); // refrescar selector con nuevo check
}

function restablecerMic(){
  localStorage.removeItem('usala_mic_permiso');
  showToast('🎤 Micrófono restablecido');
  var el = document.getElementById('micEstadoLabel');
  if(el) el.textContent = 'No solicitado aún';
}

function restablecerMonedaIA(){
  var key = 'usala_ia_moneda_' + (S.user ? (S.user.isAdmin ? 'admin' : S.user.codigo) : 'anon');
  localStorage.removeItem(key);
  _iaMoneda = null;
  _iaHistorial = [];
  _iaInicializado = false;
  _iaAbierto = false;
  if(p){ p.style.display = 'none'; }
  if(bub) bub.innerHTML = '';
  showToast('💱 Moneda restablecida. Abre el asistente 🎙️ para elegir de nuevo.');
  var el = document.getElementById('monedaEstadoLabel');
  if(el) el.textContent = 'No configurada';
}

function irACuenta(sub){
  cerrarUMenu();
  goTab('cuentas', document.querySelectorAll('.nb')[1]);
  setTimeout(function(){ goSub(sub); }, 120);
}

function cambiarPass(){
  var p1=document.getElementById('np1').value;
  var p2=document.getElementById('np2').value;
  if(!p1||p1.length<4){ showToast('⚠ Mínimo 4 caracteres'); return; }
  if(p1!==p2){ showToast('⚠ Las contraseñas no coinciden'); return; }
  localStorage.setItem('usala_admin_pass',p1);
  showToast('✓ Contraseña actualizada');
}

function resetTxs(){
  usalaConfirm('Borrar TODAS las transacciones?\n\nTambien se restablecen los saldos de efectivo y cuentas bancarias. Esta accion no se puede deshacer.', function(){
    save('txs',[]);
      var uid = S.user.isAdmin ? 'admin' : 'u_'+S.user.codigo;
      var cu = JSON.parse(localStorage.getItem('usala_cuentas_'+uid)||'{}');
      cu.efectivo = 0;
      cu.movEfectivo = [];
      (cu.cheques||[]).forEach(function(ch){ ch.saldo = 0; });
      localStorage.setItem('usala_cuentas_'+uid, JSON.stringify(cu));
      showToast('✓ Transacciones y saldos borrados');
      goSub('config');
  });
}

function resetCuenta(){
  usalaConfirm('BORRAR TODA tu informacion?\n\nSe eliminaran transacciones, cuentas, creditos, metas y presupuestos.\n\nEsta accion NO se puede deshacer.', function(){
    var uid = S.user.isAdmin ? 'admin' : 'u_'+S.user.codigo;
      var prefix = 'usala_'+uid+'_';
      Object.keys(localStorage).filter(function(k){
        return k.indexOf(prefix)===0;
      }).forEach(function(k){ localStorage.removeItem(k); });
      localStorage.removeItem('usala_cuentas_'+uid);
      showToast('✅ Cuenta restablecida completamente');
      setTimeout(function(){ goTab('inicio',document.querySelector('.nb')); },600);
  });
}

function abrirCatModalTx(){
  var tipo = document.getElementById('tipoGasto') &&
    document.getElementById('tipoGasto').classList.contains('selected') ? 'gasto' : 'ingreso';
  abrirCatModal(tipo, 'txCat');
}

function abrirCatModalEf(){
  var esEnt = document.getElementById('efTipoEnt') &&
    document.getElementById('efTipoEnt').classList.contains('selected');
  abrirCatModal(esEnt ? 'ingreso' : 'gasto', 'efCat');
}

function abrirCatModalBk(){
  var esEnt = document.getElementById('bkTipoEnt') &&
    document.getElementById('bkTipoEnt').classList.contains('selected');
  abrirCatModal(esEnt ? 'ingreso' : 'gasto', 'bkCat');
}

function abrirPP(){
  var _todos = _ppGetPagos();
  var _hayVenc = _todos.some(function(p){ return p.diffDias < 0; });
  _ppTab = _hayVenc ? 'hoy' : 'semana';
  document.querySelectorAll('.pp-tab').forEach(function(b,i){
    var tabs=['hoy','semana','mes','año'];
    b.classList.toggle('active', tabs[i]===_ppTab);
  });
  _ppRender();
  document.getElementById('ppOverlay').style.display='flex';
}

function cerrarPP(){ document.getElementById('ppOverlay').style.display='none'; }

function ppSetTab(tab, btn){
  _ppTab = tab;
  document.querySelectorAll('.pp-tab').forEach(function(b){ b.classList.remove('active'); });
  if(btn) btn.classList.add('active');
  _ppRender();
}

function _ppGetPagos(){
  var hoy     = new Date(); hoy.setHours(0,0,0,0);
  var anioAct = hoy.getFullYear();
  var mesAct  = hoy.getMonth();    // 0-11
  var diaAct  = hoy.getDate();
  var lista = [];
  var pagosBase  = loadPagosBase();
  var pagosEst   = loadPagosEstado();
  var _meses = ['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'];
  pagosBase.forEach(function(p){
    var pid = p.id;
    if(pagosEst[pid] && pagosEst[pid].pagado) return;
    var freq = p.frecuencia || 'mensual';
    var diasFrec = {mensual:1,bimestral:2,trimestral:3,cuatrimestral:4,semestral:6,anual:12};
    var mesesFrec = diasFrec[freq] || 1;
    var fechasOcurr = [];
    var fechaRel = null;
    if(p.proximoPago){
      var _pts = p.proximoPago.split('-');
      fechaRel = new Date(+_pts[0], +_pts[1]-1, +_pts[2]);
      fechaRel.setHours(0,0,0,0);
    } else if(p.dia){
      var dia = Math.min(p.dia, 28);
      fechaRel = new Date(anioAct, mesAct, dia);
      fechaRel.setHours(0,0,0,0);
    }
    if(fechaRel){
      var diffDias = Math.round((fechaRel - hoy) / 86400000);
      lista.push({
        nombre:   p.nombre||'Sin nombre',
        monto:    p.monto||0,
        fecha:    fechaRel,
        diffDias: diffDias,
        cat:      p.categoria||'📦 Otros',
        freq:     freq,
        fuente:   'pago',
        pagado:   false,
        urgencia: diffDias<0?'vencido': diffDias===0?'hoy': diffDias<=2?'urgente': diffDias<=7?'pronto':'ok'
      });
    }
  });
  var creds = load('creditos',[]);
  creds.forEach(function(c){
    if(c.estado==='pagado') return;
    if(!c.fechaLimite) return;
    var parts = c.fechaLimite.split('-');
    var fecha = new Date(+parts[0], +parts[1]-1, +parts[2]); fecha.setHours(0,0,0,0);
    if(fecha.getFullYear() < anioAct) return;
    var diffDias = Math.round((fecha - hoy) / 86400000);
    var pendiente = (c.monto||0) - (c.abonado||0);
    lista.push({
      nombre:   (c.tipo==='deuda'?'💳 Debo a ':'📥 Me debe ')+c.persona,
      monto:    pendiente,
      fecha:    fecha,
      diffDias: diffDias,
      cat:      c.tipo==='deuda'?'🤝 Crédito':'📥 Por cobrar',
      freq:     'único',
      fuente:   c.tipo==='deuda'?'deuda':'cobrar',
      pagado:   false,
      urgencia: diffDias<=0?'vencido': diffDias<=2?'urgente': diffDias<=7?'pronto':'ok'
    });
  });
  return lista.sort(function(a,b){ return a.fecha-b.fecha; });
}

function _ppFiltrar(lista, tab){
  var hoy   = new Date(); hoy.setHours(0,0,0,0);
  var fin;
  if(tab==='hoy'){
    return lista.filter(function(p){ return p.diffDias <= 0; });
  }
  if(tab==='semana'){
    fin = new Date(hoy); fin.setDate(fin.getDate()+7);
    return lista.filter(function(p){ return p.fecha<=fin; });
  }
  if(tab==='mes'){
    fin = new Date(hoy.getFullYear(), hoy.getMonth()+1, 0);
    return lista.filter(function(p){ return p.fecha<=fin; });
  }
  return lista;
}

function _ppFechaLabel(p){
  var hoy = new Date(); hoy.setHours(0,0,0,0);
  var d = p.diffDias;
  if(d<0)  return '⚠️ Vencido hace '+Math.abs(d)+' día'+(Math.abs(d)!==1?'s':'');
  if(d===0) return '📍 Hoy';
  if(d===1) return '⏰ Mañana';
  if(d<=7)  return 'En '+d+' días · '+p.fecha.toLocaleDateString('es-MX',{weekday:'long'});
  return p.fecha.toLocaleDateString('es-MX',{day:'numeric',month:'long'})
    +(p.freq!=='único'&&p.freq!=='mensual'?' · '+p.freq:'');
}

function _ppUrgColor(u){
  return u==='vencido'?'#e53935': u==='urgente'?'#f57c00': u==='pronto'?'#f9a825':'var(--accent2)';
}

function _ppRender(){
  var body  = document.getElementById('ppBody');
  var sub   = document.getElementById('ppSubtitle');
  if(!body) return;
  var todos  = _ppGetPagos();
  var lista  = _ppFiltrar(todos, _ppTab);
  var total  = lista.reduce(function(s,p){ return s+p.monto; },0);
  var labels = {hoy:'Hoy, '+new Date().toLocaleDateString('es-MX',{weekday:'long',day:'numeric',month:'long'}),
    semana:'Semana del '+new Date().toLocaleDateString('es-MX',{day:'numeric',month:'short'}),
    mes:new Date().toLocaleDateString('es-MX',{month:'long',year:'numeric'}),
    año:new Date().getFullYear()+' completo'};
  sub.textContent = labels[_ppTab];
  body.innerHTML = '';
  if(!lista.length){
    body.innerHTML = '<div class="pp-empty">'
      +'<div style="font-size:2.5rem;margin-bottom:10px;">🎉</div>'
      +'<div style="font-weight:800;margin-bottom:6px;">¡Todo al corriente!</div>'
      +'<div>No hay pagos pendientes para '+labels[_ppTab].toLowerCase()+'</div>'
      +'</div>';
    return;
  }
  var vencidos = lista.filter(function(p){ return p.urgencia==='vencido'; }).length;
  var urgentes = lista.filter(function(p){ return p.urgencia==='urgente'; }).length;
  var resumen  = document.createElement('div');
  resumen.style.cssText='background:var(--inp);border-radius:14px;padding:14px;margin-bottom:14px;display:flex;justify-content:space-between;align-items:center;';
  resumen.innerHTML =
    '<div>'
      +'<div style="font-size:1.45rem;font-weight:900;color:var(--danger);">'+fmt(total)+'</div>'
      +'<div style="font-size:0.72rem;color:var(--dim);">'+lista.length+' pago'+(lista.length!==1?'s':'')+'</div>'
    +'</div>'
    +'<div style="display:flex;gap:8px;flex-wrap:wrap;justify-content:flex-end;">'
    +(vencidos?'<div style="font-size:0.7rem;font-weight:800;padding:4px 10px;border-radius:20px;background:rgba(229,57,53,0.12);color:#e53935;">⚠️ '+vencidos+' vencido'+(vencidos!==1?'s':'')+'</div>':'')
    +(urgentes?'<div style="font-size:0.7rem;font-weight:800;padding:4px 10px;border-radius:20px;background:rgba(245,124,0,0.12);color:#f57c00;">⏰ '+urgentes+' urgente'+(urgentes!==1?'s':'')+'</div>':'')
    +'</div>';
  body.appendChild(resumen);
  if(_ppTab==='año'){
    var grupos = {};
    lista.forEach(function(p){
      var k = p.fecha.toLocaleDateString('es-MX',{month:'long',year:'numeric'});
      if(!grupos[k]) grupos[k]=[];
      grupos[k].push(p);
    });
    Object.keys(grupos).forEach(function(mes){
      var secTit = document.createElement('div');
      secTit.className='pp-section-title';
      var totMes = grupos[mes].reduce(function(s,p){ return s+p.monto; },0);
      secTit.innerHTML = mes.charAt(0).toUpperCase()+mes.slice(1)
        +' <span style="font-weight:900;color:var(--text);">'+fmt(totMes)+'</span>';
      body.appendChild(secTit);
      grupos[mes].forEach(function(p){ body.appendChild(_ppMkItem(p)); });
    });
  } else {
    lista.forEach(function(p){ body.appendChild(_ppMkItem(p)); });
  }
  var link = document.createElement('div');
  link.style.cssText='text-align:center;padding:16px 0 4px;';
  link.innerHTML='<button onclick="cerrarPP();goSub(\'pagos_mes\')" style="background:none;border:1.5px solid var(--border);border-radius:20px;padding:8px 20px;font-family:\'Outfit\',sans-serif;font-size:0.78rem;font-weight:700;cursor:pointer;color:var(--dim);">📅 Gestionar pagos del mes ›</button>';
  body.appendChild(link);
}

function _ppMkItem(p){
  var col = _ppUrgColor(p.urgencia);
  var row = document.createElement('div');
  row.className='pp-item';
  var ico = document.createElement('div');
  ico.className='pp-ico';
  ico.style.background = col+'18';
  ico.textContent = p.fuente==='deuda'?'💳': p.fuente==='cobrar'?'📥': '📅';
  var info = document.createElement('div');
  info.className='pp-info';
  var name = document.createElement('div'); name.className='pp-name'; name.textContent=p.nombre;
  var when = document.createElement('div'); when.className='pp-when'; when.textContent=_ppFechaLabel(p);
  info.appendChild(name); info.appendChild(when);
  var right = document.createElement('div');
  right.style.cssText='display:flex;flex-direction:column;align-items:flex-end;gap:4px;flex-shrink:0;';
  var amt = document.createElement('div');
  amt.className='pp-amt'; amt.style.color=col; amt.textContent=fmt(p.monto);
  var cat = document.createElement('div');
  cat.style.cssText='font-size:0.62rem;color:var(--dim);';
  cat.textContent=p.cat;
  right.appendChild(amt); right.appendChild(cat);
  var dot = document.createElement('div');
  dot.style.cssText='width:3px;align-self:stretch;border-radius:99px;background:'+col+';flex-shrink:0;margin-right:-4px;';
  row.appendChild(dot); row.appendChild(ico); row.appendChild(info); row.appendChild(right);
  return row;
}

function _lockKey(){
  var u = S.user;
  if(!u) return null;
  return 'usala_autolock_' + (u.isAdmin ? 'admin' : 'u_'+u.codigo);
}

function getLockTimeout(){
  var k = _lockKey();
  if(!k) return 0;
  return parseInt(localStorage.getItem(k)||'0', 10);
}

function setLockTimeout(minutos){
  var k = _lockKey();
  if(!k) return;
  if(minutos===0){ localStorage.removeItem(k); }
  else { localStorage.setItem(k, String(minutos)); }
  _lockReiniciar();
  showToast(minutos===0 ? '🔓 Bloqueo automático desactivado' : '⏱ Se bloqueará tras '+minutos+' min de inactividad');
}

function _lockActividad(){
  if(_lockActivo) return;
  _lockReiniciar();
}

function _lockBloqueAhora(){
  if(!S.user) return;
  _lockActivo = true;
  if(_lockTimer) clearTimeout(_lockTimer);
  var nombre = S.user.nombre || 'Usuario';
  document.getElementById('lockNombre').textContent = nombre.split(' ')[0];
  var mins = getLockTimeout();
  document.getElementById('lockTimeBadge').textContent = '⏱ Bloqueado tras '+mins+' min sin uso';
  var nipK = S.user.isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+S.user.codigo;
  var tieneNip = !!localStorage.getItem(nipK);
  document.getElementById('lockNoNipMsg').style.display = tieneNip ? 'none' : 'block';
  _lockPin = '';
  _lockActualizarDots();
  document.getElementById('lockErr').textContent = '';
  document.getElementById('lockScreen').style.display = 'flex';
}

function lockKey(d){
  if(_lockPin.length >= 4) return;
  _lockPin += d;
  _lockActualizarDots();
  if(_lockPin.length === 4) setTimeout(_lockVerificar, 120);
}

function lockDel(){
  _lockPin = _lockPin.slice(0,-1);
  _lockActualizarDots();
  document.getElementById('lockErr').textContent='';
}

function _lockActualizarDots(){
  for(var i=0;i<4;i++){
    var dot = document.getElementById('ld'+i);
    dot.classList.toggle('filled', i < _lockPin.length);
    dot.classList.remove('error');
  }
}

function lockDesbloquear(){
  _lockActivo = false;
  _lockPin    = '';
  document.getElementById('lockScreen').style.display = 'none';
  _lockReiniciar(); // reiniciar timer
}

function lockCerrarSesion(){
  document.getElementById('lockScreen').style.display = 'none';
  _lockActivo = false;
  cerrarSesion();
}

function _getSecurityStatus(){
  if(!S.user) return {nip:false, autolock:false};
  var uid    = S.user.isAdmin ? 'admin' : 'u_' + S.user.codigo;
  var nipKey = 'usala_nip_' + uid;
  var lockKey2 = 'usala_autolock_' + uid;
  return {
    nip:      !!localStorage.getItem(nipKey),
    autolock: parseInt(localStorage.getItem(lockKey2)||'0',10) > 0
  };
}

function cerrarBannerSeg(){ var b=document.getElementById('secBanner'); if(b) b.style.display='none'; }

function _bannerSeguridad(){
  var st = _getSecurityStatus();
  if(st.nip && st.autolock) return ''; // Todo protegido — sin banner
  var nivel  = (!st.nip && !st.autolock) ? 'critico' : 'medio';
  var titulo, msg, acciones;
  if(nivel === 'critico'){
    titulo  = '⚠️ Tu cuenta no está protegida';
    msg     = 'Cualquier persona que acceda a este dispositivo podría ver tus finanzas. Activa al menos el NIP y el bloqueo automático.';
    acciones = [
      {label:'🔒 Activar NIP',     fn:"goSub('config_nip')"},
      {label:'⏱ Bloqueo auto',     fn:"abrirConfigAutolock()"}
    ];
  } else if(!st.nip){
    titulo  = '🔑 Falta tu NIP de seguridad';
    msg     = 'Tienes bloqueo automático, pero sin NIP cualquiera puede desbloquear con un toque. Añade tu NIP para protección real.';
    acciones = [{label:'🔒 Configurar NIP', fn:"goSub('config_nip')"}];
  } else {
    titulo  = '⏱ Sin bloqueo automático';
    msg     = 'Tienes NIP, pero si dejas la app abierta queda expuesta. Programa un tiempo de bloqueo automático.';
    acciones = [{label:'⏱ Activar bloqueo', fn:"abrirConfigAutolock()"}];
  }
  var colorBg  = nivel==='critico' ? 'rgba(229,57,53,0.07)'  : 'rgba(245,124,0,0.07)';
  var colorBrd = nivel==='critico' ? 'rgba(229,57,53,0.25)'  : 'rgba(245,124,0,0.25)';
  var colorTxt = nivel==='critico' ? '#c62828'                : '#e65100';
  var icoBig   = nivel==='critico' ? '🛡️'                     : '🔐';
  var btns = acciones.map(function(a){
    return '<button onclick="'+a.fn+'" style="'
      +'background:'+colorTxt+';color:#fff;border:none;border-radius:20px;'
      +'padding:7px 16px;font-family:Outfit,sans-serif;font-size:0.72rem;'
      +'font-weight:800;cursor:pointer;white-space:nowrap;">'+a.label+'</button>';
  }).join('');
  return '<div id="secBanner" style="'
    +'background:'+colorBg+';border:1.5px solid '+colorBrd+';'
    +'border-radius:16px;padding:14px 16px;margin-bottom:14px;'
    +'animation:fadeIn 0.4s;">'
    +'<div style="display:flex;gap:12px;align-items:flex-start;margin-bottom:10px;">'
      +'<div style="font-size:1.8rem;line-height:1;flex-shrink:0;">'+icoBig+'</div>'
      +'<div>'
        +'<div style="font-weight:900;font-size:0.85rem;color:'+colorTxt+';margin-bottom:3px;">'+titulo+'</div>'
        +'<div style="font-size:0.75rem;color:var(--dim);line-height:1.5;">'+msg+'</div>'
      +'</div>'
    +'</div>'
    +'<div style="display:flex;gap:8px;align-items:center;flex-wrap:wrap;">'
      +btns
      +'<button onclick="cerrarBannerSeg()" '
        +'style="margin-left:auto;background:none;border:none;color:var(--dim);'
        +'font-size:0.7rem;cursor:pointer;white-space:nowrap;padding:4px 6px;">Ahora no ✕</button>'
    +'</div>'
    +'</div>';
}

function abrirCatModal(tipo, selectId){
  _catModalTipo = tipo;
  _catSelectId  = selectId;
  _catSelectVal = (document.getElementById(selectId)||{}).value || '';
  var t = _CAT_TITLES[tipo] || {title:'🏷️ Categorías', sub:''};
  document.getElementById('catModalTitle').textContent = t.title;
  document.getElementById('catModalSub').textContent   = t.sub;
  document.getElementById('catModalInp').value = '';
  _renderCatChips();
  var m = document.getElementById('catModal');
  m.style.display = 'flex';
  setTimeout(function(){ document.getElementById('catModalInp').focus(); }, 200);
}

function cerrarCatModal(){
  document.getElementById('catModal').style.display = 'none';
  _catModalTipo = null; _catSelectId = null;
}

function _renderCatChips(){
  var wrap = document.getElementById('catModalChips');
  if(!wrap) return;
  wrap.innerHTML = '';
  var custom = load(_CAT_KEYS[_catModalTipo], []);
  var base = _CAT_BASE[_catModalTipo] || [];
  base.forEach(function(c){
    var chip = document.createElement('div');
    chip.className = 'cat-chip';
    chip.style.opacity = '0.55';
    chip.innerHTML = '<span>'+c+'</span>';
    wrap.appendChild(chip);
  });
  custom.forEach(function(c, i){
    var chip = document.createElement('div');
    chip.className = 'cat-chip';
    chip.style.borderColor = 'var(--accent)';
    chip.style.background = 'var(--accent)18';
    var txt = document.createElement('span'); txt.textContent = c;
    var del = document.createElement('button'); del.className='del-chip'; del.textContent='×';
    del.title = 'Eliminar';
    (function(idx){ del.onclick = function(){
      var c2=load(_CAT_KEYS[_catModalTipo],[]); var eli=c2[idx];
      c2.splice(idx,1); save(_CAT_KEYS[_catModalTipo],c2);
      _renderCatChips();
      _refrescarSelect(_catSelectVal);
      mostrarUndo('🏷️ "'+eli+'" eliminada', function(){
        var c3=load(_CAT_KEYS[_catModalTipo],[]); c3.splice(idx,0,eli);
        save(_CAT_KEYS[_catModalTipo],c3); _renderCatChips(); _refrescarSelect(eli);
      });
    }; })(i);
    chip.appendChild(txt); chip.appendChild(del);
    wrap.appendChild(chip);
  });
  if(!custom.length){
    var hint = document.createElement('div');
    hint.style.cssText='font-size:0.75rem;color:var(--dim);padding:8px 0;width:100%;';
    hint.textContent = 'Aún no tienes categorías personalizadas. ¡Agrega la primera!';
    wrap.appendChild(hint);
  }
}

function guardarNuevaCat(){
  var inp = document.getElementById('catModalInp');
  var val = inp ? inp.value.trim() : '';
  if(!val){ showToast('⚠ Escribe un nombre'); inp && inp.focus(); return; }
  if(val.length > 40){ showToast('⚠ Máximo 40 caracteres'); return; }
  var custom = load(_CAT_KEYS[_catModalTipo], []);
  var base   = _CAT_BASE[_catModalTipo] || [];
  var todas  = base.concat(custom).map(function(c){ return c.toLowerCase(); });
  if(todas.indexOf(val.toLowerCase())>=0){ showToast('⚠ Ya existe "'+val+'"'); return; }
  custom.push(val);
  save(_CAT_KEYS[_catModalTipo], custom);
  inp.value = '';
  _renderCatChips();
  _refrescarSelect(val);   // seleccionar la nueva en el select
  showToast('✅ "'+val+'" agregada');
  inp.focus();
}

function _refrescarSelect(val){
  var sel = _catSelectId ? document.getElementById(_catSelectId) : null;
  if(!sel) return;
  var tipo = _catModalTipo;
  if(tipo==='gasto'){
    sel.innerHTML = buildGastoCatSelect(_catSelectId, val);
  } else if(tipo==='ingreso'){
    sel.innerHTML = buildIngresoCatSelect(_catSelectId, val);
  } else if(tipo==='activos'){
    var all = ACTIVOS_CATS.concat(load('cats_activos_custom',[]));
    sel.innerHTML = all.map(function(c){ return '<option'+(c===val?' selected':'')+'>'+c+'</option>'; }).join('');
  } else if(tipo==='pagos'){
    var all2 = PAGOS_CATS.concat(load('cats_pagos_custom',[]));
    sel.innerHTML = all2.map(function(c){ return '<option'+(c===val?' selected':'')+'>'+c+'</option>'; }).join('');
  }
}

function mkCatBtn(tipo, selectId){
  var btn = document.createElement('button');
  btn.type = 'button';
  btn.className = 'cat-add-btn';
  btn.innerHTML = '＋ Categoría';
  btn.onclick = function(e){ e.preventDefault(); abrirCatModal(tipo, selectId); };
  return btn;
}

function agregarCatCustom(){
  abrirCatModal('gasto', null);
}

function borrarCatCustom(i){
  var custom = load('cats_gasto_custom',[]);
  var _eliCat = custom[i];
  custom.splice(i,1); save('cats_gasto_custom',custom);
  goSub('config');
  mostrarUndo('🏷️ Categoría eliminada', function(){
    var c2=load('cats_gasto_custom',[]); c2.splice(i,0,_eliCat); save('cats_gasto_custom',c2); goSub('config');
  });
}

function guardarVersion(){
  var v=document.getElementById('vNum').value.trim();
  var n=document.getElementById('vNotas').value.trim();
  if(!v) return;
  localStorage.setItem('usala_version',v);
  localStorage.setItem('usala_notas',n);
  APP_VERSION=v; APP_NOTAS=n;
  showToast('✓ Versión actualizada');
  document.getElementById('verBadge').textContent='v'+v;
  goSub('version');
}

function abrirAyuda(){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('ayuda'); },10); }

function saveNoticias(n){ localStorage.setItem('usala_noticias', JSON.stringify(n)); }

function saldoRealCuenta(cuentaVal){
  var txs = getTxs().filter(function(t){ return t.cuenta===cuentaVal; });
  return txs.reduce(function(s,t){
    return s + (t.tipo==='ingreso' ? Number(t.monto) : -Number(t.monto));
  }, 0);
}

function selEfTipo(t){
  var esEnt = t==='ingreso';
  document.getElementById('efTipoEnt').classList.toggle('selected', esEnt);
  document.getElementById('efTipoSal').classList.toggle('selected', !esEnt);
  var sel = document.getElementById('efCat');
  if(sel) sel.innerHTML = esEnt ? buildIngresoCatSelect('efCat','') : buildGastoCatSelect('efCat','');
  var destRow = document.getElementById('efDestRow');
  if(destRow) destRow.style.display = esEnt ? 'none' : 'block';
}

function guardarMovEfectivo(){
  var desc  = document.getElementById('efDesc').value.trim();
  var monto = parseFloat(document.getElementById('efMonto').value);
  var fecha = document.getElementById('efFecha').value||today();
  var cat   = document.getElementById('efCat').value;
  var tipo  = document.getElementById('efTipoEnt').classList.contains('selected')?'ingreso':'gasto';
  var destEl = document.getElementById('efDestBanco');
  var dest  = destEl ? destEl.value : '';
  if(!desc||!monto||monto<=0){ showToast('⚠ Completa descripción y monto'); return; }
  var id = Date.now();
  var txs = getTxs();
  txs.push({id:id, tipo:tipo, desc:desc, monto:monto, cat:cat, fecha:fecha, cuenta:'efectivo'});
  saveTxs(txs);
  var c = getCuentas();
  c.efectivo = (c.efectivo||0) + (tipo==='ingreso'?monto:-monto);
  if(tipo==='gasto' && dest && dest.indexOf('cheque_')===0){
    var idx = parseInt(dest.replace('cheque_',''));
    if(c.cheques && c.cheques[idx]){
      c.cheques[idx].saldo = (Number(c.cheques[idx].saldo)||0) + monto;
      var txs2 = getTxs();
      txs2.push({id:Date.now()+1, tipo:'ingreso', desc:'Transferencia desde Efectivo: '+desc, monto:monto, cat:'Transferencia recibida', fecha:fecha, cuenta:dest});
      saveTxs(txs2);
    }
  }
  saveCuentas(c);
  showToast('✓ '+(tipo==='ingreso'?'Entrada':'Salida')+' registrada en Efectivo');
  goSub('efectivo');
}

function selBkTipo(t, idx){
  var esEnt=t==='ingreso';
  document.getElementById('bkTipoEnt').classList.toggle('selected',esEnt);
  document.getElementById('bkTipoSal').classList.toggle('selected',!esEnt);
  var cats=esEnt?getIngresoCats():getGastoCats();
  var sel=document.getElementById('bkCat'); if(sel) sel.innerHTML=cats.map(function(cat){ return '<option>'+cat+'</option>'; }).join('');
}

function guardarMovBanco(idx){
  var desc=document.getElementById('bkDesc').value.trim();
  var monto=parseFloat(document.getElementById('bkMonto').value);
  var fecha=document.getElementById('bkFecha').value||today();
  var cat=document.getElementById('bkCat').value;
  var tipo=document.getElementById('bkTipoEnt').classList.contains('selected')?'ingreso':'gasto';
  if(!desc||!monto||monto<=0){ showToast('⚠ Completa descripción y monto'); return; }
  var cval='cheque_'+idx;
  var id=Date.now(); var txs=getTxs();
  txs.push({id:id,tipo:tipo,desc:desc,monto:monto,cat:cat,fecha:fecha,cuenta:cval});
  saveTxs(txs);
  var c=getCuentas();
  c.cheques[idx].saldo=(c.cheques[idx].saldo||0)+(tipo==='ingreso'?monto:-monto);
  saveCuentas(c);
  showToast('✓ '+(tipo==='ingreso'?'Ingreso':'Gasto')+' en '+c.cheques[idx].banco);
  goSub('banco_'+idx);
}

function renderFaqs(q, catFiltro){
  var term = (q||'').toLowerCase().trim();
  var filtrados = FAQS.filter(function(f){
    var matchQ   = !term || f.q.toLowerCase().includes(term) || f.a.toLowerCase().includes(term) || f.cat.toLowerCase().includes(term);
    var matchCat = !catFiltro || f.cat.toLowerCase().includes(catFiltro.toLowerCase());
    return matchQ && matchCat;
  });
  if(!filtrados.length) return '<div style="text-align:center;padding:24px;color:var(--dim);font-size:0.83rem;">No se encontraron resultados para "'+q+'"</div>';
  var porCat = {};
  filtrados.forEach(function(f){ if(!porCat[f.cat]) porCat[f.cat]=[]; porCat[f.cat].push(f); });
  return Object.keys(porCat).map(function(cat){
    return '<div style="font-size:0.65rem;font-weight:800;letter-spacing:0.1em;text-transform:uppercase;color:var(--accent);margin:14px 0 6px;">'+cat+'</div>'
      + porCat[cat].map(function(f,i){
          var id='faq_'+cat.replace(/\W/g,'')+'_'+i;
          return '<div class="card" style="margin-bottom:6px;cursor:pointer;" onclick="toggleFaq(\''+id+'\')">'
            +'<div style="display:flex;justify-content:space-between;align-items:center;">'
            +'<div style="font-weight:700;font-size:0.85rem;flex:1;padding-right:8px;">'+f.q+'</div>'
            +'<div id="arr_'+id+'" style="color:var(--dim);font-size:1rem;flex-shrink:0;">›</div>'
            +'</div>'
            +'<div id="'+id+'" style="display:none;font-size:0.78rem;color:var(--dim);line-height:1.6;margin-top:8px;padding-top:8px;border-top:1px solid var(--border);">'+f.a+'</div>'
            +'</div>';
        }).join('');
  }).join('');
}

function ayudaChipEv(btn){
  ayudaChip(btn, btn.getAttribute('data-cat')||'');
}

function ayudaChip(btn, cat){
  document.querySelectorAll('.ayuda-chip').forEach(function(b){ b.classList.remove('active'); });
  btn.classList.add('active');
  var q = document.getElementById('ayudaBusca').value;
  document.getElementById('ayudaLista').innerHTML = renderFaqs(q, cat);
}

function filtrarAyuda(){
  var q=document.getElementById('ayudaBusca').value;
  var chipActivo = document.querySelector('.ayuda-chip.active');
  var cat = chipActivo ? (chipActivo.id==='chip_todos'?'':chipActivo.textContent.replace(/[^a-zA-ZáéíóúÁÉÍÓÚ ]/g,'').trim()) : '';
  document.getElementById('ayudaLista').innerHTML=renderFaqs(q, cat);
}

function toggleFaq(id){
  var el=document.getElementById(id);
  var arr=document.getElementById('arr_'+id);
  if(!el) return;
  var open=el.style.display==='block';
  el.style.display=open?'none':'block';
  arr.textContent=open?'›':'↓';
}

function iniciarVoz(){
  var SR = window.SpeechRecognition || window.webkitSpeechRecognition;
  if(!SR){ showToast('⚠ Tu navegador no soporta voz'); return; }
  _vozRec = new SR();
  _vozRec.lang = 'es-MX';
  _vozRec.continuous = false;
  _vozRec.interimResults = false;
  _vozRec.onstart = function(){
    _vozActivo = true;
    var btn = document.getElementById('btnVoz');
    if(btn){ btn.style.background='#ff3b30'; btn.style.color='#fff'; btn.textContent='🔴'; }
    showToast('🎤 Escuchando...');
  };
  _vozRec.onend = function(){ detenerVoz(); };
  _vozRec.onerror = function(e){
    detenerVoz();
    if(e.error === 'not-allowed') showToast('🔒 Micrófono bloqueado. Actívalo en Configuración del sitio.');
    else if(e.error !== 'no-speech') showToast('⚠ Error de voz: ' + e.error);
  };
  _vozRec.onresult = function(e){
    var t = e.results[0][0].transcript.toLowerCase().trim();
    showToast('🎤 "' + t + '"');
    procesarComandoVoz(t);
  };
  try{ _vozRec.start(); } catch(e){ showToast('⚠ No se pudo iniciar el mic'); }
}

function detenerVoz(){
  _vozActivo = false;
  var btn = document.getElementById('btnVoz');
  if(btn){ btn.style.background=''; btn.style.color=''; btn.textContent='🎙️'; }
  if(_vozRec){ try{ _vozRec.stop(); }catch(e){} _vozRec = null; }
}

function procesarComandoVoz(t){
  var nb = document.querySelectorAll('.nb');
  if(/\binicio\b|\bhome\b/.test(t)){ goTab('inicio',nb[0]); showToast('🏠 Inicio'); return; }
  if(/\bcuentas?\b/.test(t) && !/tarjeta|tc\b/.test(t)){ goTab('cuentas',nb[1]); showToast('🏦 Cuentas'); return; }
  if(/\bcr[eé]ditos?\b|\bpr[eé]stamo\b/.test(t)){ goTab('creditos',nb[2]); showToast('🤝 Créditos'); return; }
  if(/\breportes?\b/.test(t)){ goTab('reportes',nb[3]); showToast('📊 Reportes'); return; }
  if(/\bm[aá]s\b|\bajuste\b|\bconfig\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); showToast('⋯ Más'); return; }
  if(/\befectivo\b/.test(t)){ goTab('cuentas',nb[1]); setTimeout(function(){ goSub('efectivo'); },60); showToast('💵 Efectivo'); return; }
  if(/\bbanco\b|\bcheque\b/.test(t)){ goTab('cuentas',nb[1]); setTimeout(function(){ goSub('cheques'); },60); showToast('🏦 Banco'); return; }
  if(/\btarjeta\b|\btc\b/.test(t)){ goTab('cuentas',nb[1]); setTimeout(function(){ goSub('tarjetas_credito'); },60); showToast('💳 Tarjetas'); return; }
  if(/\bcalculadora\b|\bcalc\b/.test(t)){ abrirCalc(); showToast('🔢 Calculadora'); return; }
  if(/\bhistorial\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('historial'); },60); showToast('📋 Historial'); return; }
  if(/\bayuda\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('ayuda'); },60); showToast('❓ Ayuda'); return; }
  if(/\bmetas?\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('metas'); },60); showToast('🎯 Metas'); return; }
  if(/\bpresupuesto\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('presupuesto'); },60); showToast('💰 Presupuesto'); return; }
  if(/\bconversor\b|\btipo de cambio\b/.test(t)){ goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('conversor'); },60); showToast('💱 Conversor'); return; }
  var mG = t.match(/gast[eé]\s+(\d+[\.,]?\d*)/);
  var mI = t.match(/ingres[eé]\s+(\d+[\.,]?\d*)/);
  if(mG){
    var m = parseFloat(mG[1].replace(',','.'));
    if(m > 0){
      var c = getCuentas(); c.efectivo = (c.efectivo||0) - m; saveCuentas(c);
      var txs = getTxs(); txs.push({id:Date.now(),tipo:'gasto',desc:'Voz',monto:m,cat:'Otros gastos',fecha:today(),cuenta:'efectivo'}); saveTxs(txs);
      showToast('💸 Gasto ' + getSimboloMoneda() + m.toFixed(2) + ' en Efectivo'); renderTab(S.tab); return;
    }
  }
  if(mI){
    var m2 = parseFloat(mI[1].replace(',','.'));
    if(m2 > 0){
      var c2 = getCuentas(); c2.efectivo = (c2.efectivo||0) + m2; saveCuentas(c2);
      var txs2 = getTxs(); txs2.push({id:Date.now(),tipo:'ingreso',desc:'Voz',monto:m2,cat:'Otros ingresos',fecha:today(),cuenta:'efectivo'}); saveTxs(txs2);
      showToast('💰 Ingreso ' + getSimboloMoneda() + m2.toFixed(2) + ' en Efectivo'); renderTab(S.tab); return;
    }
  }
  showToast('❓ No entendí: "' + t + '"');
}

function verFichaCodigo(codigo){
  var cods=JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var c=cods.find(function(x){ return x.codigo===codigo; });
  if(!c) return;
  var hoy=new Date(); hoy.setHours(0,0,0,0);
  var vencDate=new Date(c.vencimiento.split('-').join('/'));
  var estaVenc=vencDate<hoy;
  var diffDias=Math.round((vencDate-hoy)/86400000);
  var tieneNip=!!localStorage.getItem('usala_nip_u_'+c.codigo);
  var nombre=c.nombreUsuario||c.nota||'Sin nombre';
  var contacto=c.contacto||'';
  var initials=nombre.split(' ').map(function(p){ return p[0]||''; }).slice(0,2).join('').toUpperCase();
  var stCol=estaVenc?'#9e9e9e':diffDias<=7?'#f57c00':'var(--accent2)';
  var mc=document.getElementById('mainContent');
  mc.innerHTML=
    '<div class="page-header"><button onclick="goSub(\'codigos\')" style="background:none;border:none;color:var(--accent);font-size:1rem;cursor:pointer;padding:4px 8px;">← Atrás</button>'
    +'<div class="page-title">👤 Ficha</div></div>'
    +'<div style="text-align:center;padding:24px 0 18px;">'
      +'<div style="width:72px;height:72px;border-radius:50%;background:'+stCol+';display:flex;align-items:center;justify-content:center;color:#fff;font-weight:900;font-size:1.6rem;margin:0 auto 12px;">'+initials+'</div>'
      +'<div style="font-size:1.2rem;font-weight:900;">'+nombre+'</div>'
      +(contacto?'<div style="font-size:0.82rem;color:var(--accent);margin-top:4px;">📞 '+contacto+'</div>':'<div style="font-size:0.78rem;color:var(--dim);margin-top:4px;">Sin contacto registrado</div>')
    +'</div>'
    +'<div class="card" style="margin-bottom:14px;">'
      +'<div class="card-title">📋 Datos de acceso</div>'
      +'<div style="display:flex;flex-direction:column;gap:10px;">'
        +'<div style="display:flex;justify-content:space-between;align-items:center;padding:12px;background:var(--inp);border-radius:12px;">'
          +'<div><div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;margin-bottom:3px;">Código</div>'
          +'<div style="font-family:monospace;font-size:1.15rem;font-weight:700;letter-spacing:0.1em;">'+c.codigo+'</div></div>'
          +'<button id="btnCopiarFicha" style="background:var(--accent);color:var(--navtext);border:none;border-radius:10px;padding:8px 14px;font-family:Outfit,sans-serif;font-weight:700;font-size:0.78rem;cursor:pointer;">📋 Copiar</button>'
        +'</div>'
        +'<div style="display:grid;grid-template-columns:1fr 1fr;gap:8px;">'
          +'<div style="padding:10px;background:var(--inp);border-radius:12px;">'
            +'<div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;margin-bottom:3px;">Estado</div>'
            +'<div style="font-size:0.85rem;font-weight:800;color:'+stCol+';">'+(estaVenc?'⛔ Vencido':diffDias<=7?'⚠️ Pronto':'✅ Activo')+'</div>'
          +'</div>'
          +'<div style="padding:10px;background:var(--inp);border-radius:12px;">'
            +'<div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;margin-bottom:3px;">Vencimiento</div>'
            +'<div style="font-size:0.82rem;font-weight:700;">'+c.vencimiento+'</div>'
          +'</div>'
          +'<div style="padding:10px;background:var(--inp);border-radius:12px;">'
            +'<div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;margin-bottom:3px;">Primer acceso</div>'
            +'<div style="font-size:0.82rem;font-weight:700;">'+(c.fechaUso||'Sin usar')+'</div>'
          +'</div>'
          +'<div style="padding:10px;background:var(--inp);border-radius:12px;">'
            +'<div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;margin-bottom:3px;">NIP</div>'
            +'<div style="font-size:0.82rem;font-weight:700;">'+(tieneNip?'🔒 Configurado':'🔓 Sin NIP')+'</div>'
          +'</div>'
        +'</div>'
        +(c.creado?'<div style="font-size:0.7rem;color:var(--dim);">📅 Código creado el '+c.creado+'</div>':'')
      +'</div>'
    +'</div>'
    +'<div class="card" id="fichaAcciones">'
      +'<div class="card-title">⚡ Acciones</div>'
      +'<div style="display:flex;flex-direction:column;gap:8px;">'
        +(estaVenc?'<button id="btnRenovarFicha" style="width:100%;padding:13px;background:rgba(45,158,95,0.1);color:var(--accent2);border:1.5px solid rgba(45,158,95,0.3);border-radius:14px;font-family:Outfit,sans-serif;font-weight:700;font-size:0.88rem;cursor:pointer;">🔄 Renovar acceso 30 días</button>':'')
        +(tieneNip?'<button id="btnNipFicha" style="width:100%;padding:13px;background:rgba(229,57,53,0.07);color:var(--danger);border:1.5px solid rgba(229,57,53,0.2);border-radius:14px;font-family:Outfit,sans-serif;font-weight:700;font-size:0.88rem;cursor:pointer;">🔓 Resetear NIP</button>':'')
        +'<button id="btnBorrarFicha" style="width:100%;padding:13px;background:rgba(229,57,53,0.06);color:var(--danger);border:1.5px solid rgba(229,57,53,0.15);border-radius:14px;font-family:Outfit,sans-serif;font-weight:700;font-size:0.88rem;cursor:pointer;">🗑 Eliminar usuario</button>'
      +'</div>'
    +'</div>';
  var btnC=document.getElementById('btnCopiarFicha');
  if(btnC) btnC.onclick=function(){ copiarCodigo(codigo); };
  var btnR=document.getElementById('btnRenovarFicha');
  if(btnR) btnR.onclick=function(){ renovarCodigo(codigo); };
  var btnN=document.getElementById('btnNipFicha');
  if(btnN) btnN.onclick=function(){ resetearNipUsuario(codigo); };
  var btnD=document.getElementById('btnBorrarFicha');
  if(btnD) btnD.onclick=function(){ borrarCodigo(codigo); };
}

function borrarCodigo(codigo){
  var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var idx  = cods.findIndex(function(x){ return x.codigo===codigo; });
  if(idx < 0) return;
  var _backup = JSON.parse(JSON.stringify(cods[idx]));
  var nombre  = _backup.nombreUsuario || _backup.nota || codigo;
  cods.splice(idx, 1);
  localStorage.setItem('usala_codigos', JSON.stringify(cods));
  goSub('codigos');
  mostrarUndo('🗑 Usuario "'+nombre+'" eliminado', function(){
    var c2 = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
    c2.splice(idx, 0, _backup);
    localStorage.setItem('usala_codigos', JSON.stringify(c2));
    showToast('↩ Usuario restaurado');
    goSub('codigos');
  });
}

function renovarCodigo(codigo){
  var cods=JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var c=cods.find(function(x){ return x.codigo===codigo; });
  if(!c) return;
  var nombre=c.nombreUsuario||c.nota||codigo;
  var venc=new Date(); venc.setDate(venc.getDate()+30);
  c.vencimiento=venc.toISOString().split('T')[0];
  c.activo=true;
  localStorage.setItem('usala_codigos',JSON.stringify(cods));
  showToast('✅ Acceso de '+nombre+' renovado 30 días');
  goSub('codigos');
}

function desactivarCodigo(codigo){
  usalaConfirm('Desactivar el acceso de '+codigo+'?', function(){
    var cods=JSON.parse(localStorage.getItem('usala_codigos')||'[]');
      var ci=cods.find(function(x){ return x.codigo===codigo; });
      if(ci) ci.activo=false;
      localStorage.setItem('usala_codigos',JSON.stringify(cods));
      goSub('codigos');
  });
}


// ═══════════════════════════════════════════════════════
//  SISTEMA DE MODALES — reemplaza confirm() y prompt()
// ═══════════════════════════════════════════════════════

// Modal de confirmación (reemplaza confirm)
function usalaConfirm(msg, onOk, onCancel){
  var viejo = document.getElementById('_usalaConfirmModal');
  if(viejo) viejo.remove();
  var m = document.createElement('div');
  m.id = '_usalaConfirmModal';
  m.style.cssText = 'position:fixed;inset:0;background:rgba(0,0,0,0.65);z-index:9999;'
    +'display:flex;align-items:center;justify-content:center;padding:16px;';
  m.innerHTML = '<div style="background:var(--card);border:1px solid var(--border);border-radius:20px;'
    +'padding:24px 20px;max-width:340px;width:100%;box-shadow:0 20px 60px rgba(0,0,0,0.5);">'
    +'<div style="font-size:0.95rem;font-weight:700;color:var(--txt);margin-bottom:20px;line-height:1.45;">'
    + msg.replace(/\n/g,'<br>') +'</div>'
    +'<div style="display:flex;gap:10px;">'
    +'<button id="_usalaConfirmOk" class="btn-main" style="flex:1;">Confirmar</button>'
    +'<button id="_usalaConfirmCancel" class="btn-sec" style="flex:1;">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
  document.getElementById('_usalaConfirmOk').onclick = function(){
    m.remove(); if(onOk) onOk();
  };
  document.getElementById('_usalaConfirmCancel').onclick = function(){
    m.remove(); if(onCancel) onCancel();
  };
  m.onclick = function(e){ if(e.target===m){ m.remove(); if(onCancel) onCancel(); } };
}

// Modal de prompt con un campo (reemplaza prompt)
function usalaPrompt(msg, defaultVal, onOk, opts){
  var viejo = document.getElementById('_usalaPromptModal');
  if(viejo) viejo.remove();
  opts = opts || {};
  var tipo = opts.type || 'text';
  var placeholder = opts.placeholder || '';
  var m = document.createElement('div');
  m.id = '_usalaPromptModal';
  m.style.cssText = 'position:fixed;inset:0;background:rgba(0,0,0,0.65);z-index:9999;'
    +'display:flex;align-items:center;justify-content:center;padding:16px;';
  m.innerHTML = '<div style="background:var(--card);border:1px solid var(--border);border-radius:20px;'
    +'padding:24px 20px;max-width:340px;width:100%;">'
    +'<div style="font-size:0.88rem;font-weight:700;color:var(--txt);margin-bottom:12px;">'+ msg +'</div>'
    +'<input id="_usalaPromptInp" class="inp" type="'+ tipo +'" '
    +'placeholder="'+ placeholder +'" value="'+(defaultVal||'')+'" '
    +'style="margin-bottom:14px;">'
    +'<div style="display:flex;gap:10px;">'
    +'<button id="_usalaPromptOk" class="btn-main" style="flex:1;">Aceptar</button>'
    +'<button id="_usalaPromptCancel" class="btn-sec" style="flex:1;">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
  var inp = document.getElementById('_usalaPromptInp');
  setTimeout(function(){ inp.focus(); inp.select(); }, 80);
  var doOk = function(){
    var val = inp.value;
    m.remove();
    if(onOk) onOk(val);
  };
  document.getElementById('_usalaPromptOk').onclick = doOk;
  inp.onkeydown = function(e){ if(e.key==='Enter') doOk(); if(e.key==='Escape') m.remove(); };
  document.getElementById('_usalaPromptCancel').onclick = function(){ m.remove(); };
  m.onclick = function(e){ if(e.target===m) m.remove(); };
}

// Modal de prompt con DOS campos (para editarMeta)
function usalaPrompt2(msg, fields, onOk){
  var viejo = document.getElementById('_usalaPrompt2Modal');
  if(viejo) viejo.remove();
  var m = document.createElement('div');
  m.id = '_usalaPrompt2Modal';
  m.style.cssText = 'position:fixed;inset:0;background:rgba(0,0,0,0.65);z-index:9999;'
    +'display:flex;align-items:center;justify-content:center;padding:16px;';
  var inputs = fields.map(function(f,i){
    return '<div style="margin-bottom:12px;">'
      +'<label class="inp-label">'+ f.label +'</label>'
      +'<input id="_usalaP2_'+i+'" class="inp" type="'+(f.type||'text')+'" '
      +'value="'+(f.value||'')+'" placeholder="'+(f.placeholder||'')+'">'
      +'</div>';
  }).join('');
  m.innerHTML = '<div style="background:var(--card);border:1px solid var(--border);border-radius:20px;'
    +'padding:24px 20px;max-width:340px;width:100%;">'
    +'<div style="font-size:0.9rem;font-weight:800;color:var(--txt);margin-bottom:14px;">'+ msg +'</div>'
    + inputs
    +'<div style="display:flex;gap:10px;">'
    +'<button id="_usalaP2Ok" class="btn-main" style="flex:1;">Guardar</button>'
    +'<button class="btn-sec" style="flex:1;" onclick="document.getElementById(\'_usalaPrompt2Modal\').remove()">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
  setTimeout(function(){ var el=document.getElementById('_usalaP2_0'); if(el){el.focus();el.select();}},80);
  document.getElementById('_usalaP2Ok').onclick = function(){
    var vals = fields.map(function(_,i){ return document.getElementById('_usalaP2_'+i).value; });
    m.remove();
    if(onOk) onOk(vals);
  };
  m.onclick = function(e){ if(e.target===m) m.remove(); };
}


// ═════════════════════════════════════════════════════════════
//  USALA Suite — Créditos & Tarjetas de Crédito
//  js/creditos-tarjetas.js
//  Módulo completo: TC, Deudas, Préstamos, CxC
// ═════════════════════════════════════════════════════════════

// ──────────────────────────────────────────────────────────────
//  TARJETAS DE CRÉDITO
// ──────────────────────────────────────────────────────────────

function renderTarjetasCredito(){
  var c=getCuentas(); var tcs=c.tarjetas||[];
  var txs=getTxs();
  var items=tcs.map(function(t,i){
    var pct=t.limite>0?Math.min(100,Math.round((t.balance/t.limite)*100)):0;
    var disp=Math.max(0,(t.limite||0)-(t.balance||0));
    var color=pct>=90?'var(--danger)':pct>=70?'#f57c00':'var(--accent)';
    var hoy=new Date(); var diasCorte='';
    var saldoAutoCorte = 0;
    if(t.fechaCorte){
      var fc=new Date(t.fechaCorte.split('-').join('/'));
      var diff=Math.ceil((fc-hoy)/(1000*60*60*24));
      diasCorte=diff>0?diff+' días para corte':'Cortó hace '+Math.abs(diff)+' días';
      var fcPrev = new Date(fc);
      fcPrev.setMonth(fcPrev.getMonth()-1);
      txs.forEach(function(tx){
        if(tx.cuenta==='tc_'+i && tx.tipo==='gasto'){
          var txDate = new Date(tx.fecha.split('-').join('/'));
          if(txDate >= fcPrev && txDate <= fc){
            saldoAutoCorte += Number(tx.monto);
          }
        }
      });
    } else {
      txs.forEach(function(tx){
        if(tx.cuenta==='tc_'+i && tx.tipo==='gasto'){
          saldoAutoCorte += Number(tx.monto);
        }
      });
    }
    return '<div class="cred-item">'
      +'<div style="display:flex;align-items:center;gap:10px;margin-bottom:8px;">'
      +'<div style="width:42px;height:28px;background:linear-gradient(135deg,var(--accent),var(--accent2));border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:0.6rem;color:#fff;font-weight:800;">'+t.banco.substring(0,4).toUpperCase()+'</div>'
      +'<div style="flex:1;"><div style="font-weight:800;font-size:0.9rem;">'+t.banco+'</div>'
      +'<div style="font-size:0.68rem;color:var(--dim);">'+t.tipo+(t.ultimos?' · ***'+t.ultimos:'')+'</div></div>'
      +'<span class="cred-badge '+(t.pagoPendiente?'badge-vencido':'badge-pagado')+'">'+(t.pagoPendiente?'⚠ Pago pend.':'✅ Al corriente')+'</span>'
      +'</div>'
      +'<div style="display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:8px;">'
      +'<div style="background:var(--inp);border-radius:10px;padding:10px;">'
      +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.05em;">Saldo usado</div>'
      +'<div style="font-size:1rem;font-weight:900;color:var(--danger);">'+fmt(t.balance||0)+'</div></div>'
      +'<div style="background:var(--inp);border-radius:10px;padding:10px;">'
      +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.05em;">Disponible</div>'
      +'<div style="font-size:1rem;font-weight:900;color:var(--accent);">'+fmt(disp)+'</div></div>'
      +'<div style="background:var(--inp);border-radius:10px;padding:10px;">'
      +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.05em;">Límite</div>'
      +'<div style="font-size:1rem;font-weight:900;">'+fmt(t.limite||0)+'</div></div>'
      +'<div style="background:var(--inp);border-radius:10px;padding:10px;">'
      +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.05em;">Corte</div>'
      +'<div style="font-size:0.78rem;font-weight:700;color:var(--dim);">'+(diasCorte||'—')+'</div></div>'
      +'</div>'
      +'<div style="margin-bottom:8px;">'
      +'<div style="display:flex;justify-content:space-between;font-size:0.68rem;color:var(--dim);margin-bottom:4px;">'
      +'<span>Uso de crédito</span><span style="color:'+color+';">'+pct+'%</span></div>'
      +'<div style="height:6px;background:var(--inp);border-radius:3px;overflow:hidden;">'
      +'<div style="height:100%;width:'+pct+'%;background:'+color+';border-radius:3px;transition:width 0.5s ease;"></div></div>'
      +'</div>'
      +(saldoAutoCorte>0?'<div style="font-size:0.72rem;color:var(--dim);margin-bottom:8px;">📊 Gasto en período actual: <b style="color:var(--danger);">'+fmt(saldoAutoCorte)+'</b></div>':'')
      +'<div style="display:flex;gap:6px;flex-wrap:wrap;">'
      +'<button class="cred-btn success" onclick="registrarPagoTC('+i+')">💳 Pagar</button>'
      +'<button class="cred-btn" onclick="abrirDetalleTC('+i+')" style="background:rgba(56,170,255,0.1);color:var(--blue);border-color:rgba(56,170,255,0.3);">📋 Detalle</button>'
      +'<button class="cred-btn" onclick="editarTC('+i+')">✏️</button>'
      +'<button class="cred-btn danger" onclick="borrarTC('+i+')">🗑️</button>'
      +'</div>'
      +'</div>';
  }).join('');

  var totalDeuda = tcs.reduce(function(s,t){ return s+(t.balance||0); },0);
  var totalLimite= tcs.reduce(function(s,t){ return s+(t.limite||0); },0);
  var totalDisp  = Math.max(0, totalLimite - totalDeuda);

  var html = '<div class="page-header">'+backSubBtn()+'<div class="page-title">💳 Tarjetas de Crédito</div></div>';

  if(tcs.length>0){
    html += '<div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;margin-bottom:16px;">'
      +'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;text-align:center;">'
      +'<div style="font-size:0.58rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.06em;margin-bottom:4px;">Deuda total</div>'
      +'<div style="font-size:0.95rem;font-weight:900;color:var(--danger);">'+fmt(totalDeuda)+'</div></div>'
      +'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;text-align:center;">'
      +'<div style="font-size:0.58rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.06em;margin-bottom:4px;">Disponible</div>'
      +'<div style="font-size:0.95rem;font-weight:900;color:var(--accent);">'+fmt(totalDisp)+'</div></div>'
      +'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;text-align:center;">'
      +'<div style="font-size:0.58rem;font-weight:700;color:var(--dim);text-transform:uppercase;letter-spacing:0.06em;margin-bottom:4px;">Límite total</div>'
      +'<div style="font-size:0.95rem;font-weight:900;">'+fmt(totalLimite)+'</div></div>'
      +'</div>';
  }

  html += '<button class="btn-main" style="margin-bottom:16px;" onclick="goSub(\'nueva_tarjeta\')">+ Nueva tarjeta</button>';
  html += items || '<div style="text-align:center;padding:40px 20px;color:var(--dim);">'+
    '<div style="font-size:3rem;margin-bottom:12px;">💳</div>'+
    '<div style="font-size:0.85rem;">Sin tarjetas registradas</div>'+
    '<div style="font-size:0.75rem;margin-top:4px;opacity:0.6;">Agrega tu primera tarjeta de crédito</div></div>';

  document.getElementById('mainContent').innerHTML = html;
}

function renderFormTC(data){
  var d=data||{}; var titulo=d.banco?'Editar tarjeta':'Nueva Tarjeta';
  return '<div class="page-header">'+backBtn('cuentas',1)+'<div class="page-title">💳 '+titulo+'</div></div>'
    +'<div class="card">'
    +'<label class="inp-label">Banco / Emisor</label>'
    +'<input class="inp" id="tcBanco" placeholder="Ej: BBVA, Santander, Citibanamex..." value="'+(d.banco||'')+'">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Tipo</label>'
    +'<select class="inp" id="tcTipo">'
    +'<option'+(d.tipo==='Visa'?' selected':'')+'>Visa</option>'
    +'<option'+(d.tipo==='Mastercard'?' selected':'')+'>Mastercard</option>'
    +'<option'+(d.tipo==='Amex'?' selected':'')+'>Amex</option>'
    +'<option'+(d.tipo==='Otro'?' selected':'')+'>Otro</option>'
    +'</select></div>'
    +'<div><label class="inp-label">Últimos 4 dígitos</label>'
    +'<input class="inp" id="tcUltimos" placeholder="1234" maxlength="4" inputmode="numeric" value="'+(d.ultimos||'')+'">'
    +'</div></div>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Límite de crédito ($)</label>'
    +'<input class="inp" id="tcLimite" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.limite||'')+'"></div>'
    +'<div><label class="inp-label">Saldo usado ($)</label>'
    +'<input class="inp" id="tcBalance" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.balance||'')+'"></div>'
    +'</div>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Interés anual (%)</label>'
    +'<input class="inp" id="tcInteres" type="number" inputmode="decimal" placeholder="Ej: 36" value="'+(d.interes||'')+'"></div>'
    +'<div><label class="inp-label">Día de pago</label>'
    +'<input class="inp" id="tcDiaPago" type="number" inputmode="numeric" placeholder="Ej: 15" min="1" max="31" value="'+(d.diaPago||'')+'"></div>'
    +'</div>'
    +'<label class="inp-label">Fecha de corte</label>'
    +'<input class="inp" id="tcFechaCorte" type="date" value="'+(d.fechaCorte||'')+'">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Pago mínimo ($)</label>'
    +'<input class="inp" id="tcPagoMin" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.pagoMinimo||'')+'"></div>'
    +'<div><label class="inp-label">Pago total ($)</label>'
    +'<input class="inp" id="tcPagoTotal" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.pagoTotal||'')+'"></div>'
    +'</div>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Saldo al corte ($)</label>'
    +'<input class="inp" id="tcSaldoCorte" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.saldoCorte||'')+'"></div>'
    +'<div style="display:flex;align-items:flex-end;padding-bottom:4px;">'
    +'<label style="display:flex;align-items:center;gap:8px;font-size:0.82rem;color:var(--txt);cursor:pointer;">'
    +'<input type="checkbox" id="tcPagoPend" '+(d.pagoPendiente?'checked':'')+' style="width:16px;height:16px;accent-color:var(--accent);"> Pago pendiente'
    +'</label></div>'
    +'</div>'
    +'<button class="btn-main" onclick="guardarTC()">💾 Guardar</button>'
    +'<button class="btn-sec" onclick="goSub(\'tarjetas_credito\')">Cancelar</button>'
    +'</div>';
}

function guardarTC(){
  var banco=document.getElementById('tcBanco').value.trim();
  if(!banco){ showToast('⚠ Escribe el banco'); return; }
  var tc={
    banco:banco,
    tipo:document.getElementById('tcTipo').value,
    ultimos:document.getElementById('tcUltimos').value.trim(),
    limite:parseFloat(document.getElementById('tcLimite').value)||0,
    balance:parseFloat(document.getElementById('tcBalance').value)||0,
    interes:parseFloat(document.getElementById('tcInteres').value)||0,
    diaPago:document.getElementById('tcDiaPago').value,
    fechaCorte:document.getElementById('tcFechaCorte').value,
    pagoMinimo:parseFloat(document.getElementById('tcPagoMin').value)||0,
    pagoTotal:parseFloat(document.getElementById('tcPagoTotal').value)||0,
    saldoCorte:parseFloat(document.getElementById('tcSaldoCorte').value)||0,
    pagoPendiente:document.getElementById('tcPagoPend').checked
  };
  var c=getCuentas(); c.tarjetas=c.tarjetas||[];
  if(_editTCIdx!==null){ c.tarjetas[_editTCIdx]=tc; _editTCIdx=null; showToast('Tarjeta actualizada'); }
  else { c.tarjetas.push(tc); showToast('Tarjeta registrada'); }
  saveCuentas(c); goSub('tarjetas_credito');
}

function editarTC(i){
  var c=getCuentas(); _editTCIdx=i;
  document.getElementById('mainContent').innerHTML=renderFormTC(c.tarjetas[i]);
}

function borrarTC(i){
  var c=getCuentas(); c.tarjetas=c.tarjetas||[];
  var eli=c.tarjetas[i];
  usalaConfirm('Eliminar tarjeta '+eli.banco+'?', function(){
    c.tarjetas.splice(i,1); saveCuentas(c);
    showToast('Tarjeta eliminada');
    goSub('tarjetas_credito');
  });
}

// ── Registrar pago de TC ──────────────────────────
function registrarPagoTC(i){
  var c=getCuentas(); var tcs=c.tarjetas||[]; var t=tcs[i];
  if(!t){ showToast('Tarjeta no encontrada'); return; }

  // Crear modal de pago
  var m = document.createElement('div');
  m.className='modal open'; m.id='pagoTCModal';
  m.innerHTML='<div class="modal-body">'
    +'<div class="modal-title">💳 Pagar '+t.banco+'</div>'
    +'<div style="background:var(--inp);border-radius:12px;padding:12px;margin-bottom:14px;">'
    +'<div style="display:flex;justify-content:space-between;margin-bottom:4px;">'
    +'<span style="font-size:0.75rem;color:var(--dim);">Saldo actual</span>'
    +'<span style="font-size:0.9rem;font-weight:900;color:var(--danger);">'+fmt(t.balance||0)+'</span></div>'
    +'<div style="display:flex;justify-content:space-between;">'
    +'<span style="font-size:0.75rem;color:var(--dim);">Pago mínimo</span>'
    +'<span style="font-size:0.8rem;font-weight:700;color:var(--accent);">'+fmt(t.pagoMinimo||0)+'</span></div>'
    +'</div>'
    +'<label class="inp-label">Monto del pago ($)</label>'
    +'<input class="inp" id="pagoTCMonto" type="number" inputmode="decimal" placeholder="0.00" '
    +'value="'+(t.pagoMinimo||'')+'"><br>'
    +'<label class="inp-label">¿De qué cuenta?</label>'
    +buildCuentaOpts('pagoTCCuenta')
    +'<div style="display:flex;gap:8px;margin-top:12px;">'
    +'<button class="btn-main" style="flex:1;" onclick="_confirmarPagoTC('+i+')">Registrar pago</button>'
    +'<button class="btn-sec" onclick="document.getElementById(\'pagoTCModal\').remove()">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
}

function _confirmarPagoTC(i){
  var monto = parseFloat(document.getElementById('pagoTCMonto').value)||0;
  var cuenta = document.getElementById('pagoTCCuenta').value;
  if(!monto||monto<=0){ showToast('Ingresa el monto'); return; }

  var c=getCuentas(); var t=c.tarjetas[i];
  if(!t){ showToast('Tarjeta no encontrada'); return; }

  // Reducir saldo de TC
  var saldoAnterior = t.balance||0;
  t.balance = Math.max(0, saldoAnterior - monto);
  t.pagoPendiente = t.balance > 0;
  c.tarjetas[i] = t;
  saveCuentas(c);

  // Registrar como gasto en la cuenta de origen
  if(cuenta && cuenta !== 'ninguna'){
    aplicarMovimientoCuenta(cuenta, monto, 'gasto', 'Pago tarjeta '+t.banco, today(), Date.now());
  }

  // Registrar transacción
  var txs = getTxs();
  txs.push({
    id: Date.now(), tipo:'gasto', desc:'Pago TC '+t.banco,
    monto:monto, fecha:today(), cat:'Tarjeta de crédito',
    cuenta:cuenta||'efectivo', nota:'Pago tarjeta'
  });
  save('txs', txs);

  document.getElementById('pagoTCModal').remove();
  showToast('Pago registrado: '+fmt(monto));
  goSub('tarjetas_credito');
}

// ── Detalle de TC (movimientos) ───────────────────
function abrirDetalleTC(i){
  var c=getCuentas(); var t=(c.tarjetas||[])[i];
  if(!t){ showToast('Tarjeta no encontrada'); return; }

  var txs = getTxs().filter(function(tx){ return tx.cuenta==='tc_'+i; });
  txs.sort(function(a,b){ return b.fecha.localeCompare(a.fecha); });

  var mc = document.getElementById('mainContent');
  var pct = t.limite>0 ? Math.min(100, Math.round((t.balance/t.limite)*100)) : 0;
  var color = pct>=90?'var(--danger)':pct>=70?'#f57c00':'var(--accent)';

  var html = '<div class="page-header">'+backSubBtn()+'<div class="page-title">💳 '+t.banco+'</div></div>'
    // Resumen
    +'<div style="display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:16px;">'
    +'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:14px;">'
    +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;margin-bottom:4px;">Saldo usado</div>'
    +'<div style="font-size:1.2rem;font-weight:900;color:var(--danger);">'+fmt(t.balance||0)+'</div>'
    +'<div style="font-size:0.68rem;color:var(--dim);margin-top:2px;">de '+fmt(t.limite||0)+' de límite</div>'
    +'</div>'
    +'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:14px;">'
    +'<div style="font-size:0.6rem;font-weight:700;color:var(--dim);text-transform:uppercase;margin-bottom:4px;">Disponible</div>'
    +'<div style="font-size:1.2rem;font-weight:900;color:var(--accent);">'+fmt(Math.max(0,(t.limite||0)-(t.balance||0)))+'</div>'
    +'<div style="font-size:0.68rem;color:var(--dim);margin-top:2px;">'+pct+'% usado</div>'
    +'</div></div>'
    // Barra de uso
    +'<div style="margin-bottom:16px;">'
    +'<div style="height:8px;background:var(--inp);border-radius:4px;overflow:hidden;">'
    +'<div style="height:100%;width:'+pct+'%;background:'+color+';border-radius:4px;transition:width 0.5s;"></div></div>'
    +'</div>'
    // Detalles
    +(t.fechaCorte?'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;margin-bottom:12px;font-size:0.78rem;display:flex;justify-content:space-between;align-items:center;">'
    +'<span style="color:var(--dim);">📅 Fecha de corte</span><b>'+t.fechaCorte+'</b></div>':'')
    +(t.diaPago?'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;margin-bottom:12px;font-size:0.78rem;display:flex;justify-content:space-between;align-items:center;">'
    +'<span style="color:var(--dim);">💳 Día de pago</span><b>Día '+t.diaPago+' de cada mes</b></div>':'')
    +(t.interes?'<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px;margin-bottom:16px;font-size:0.78rem;display:flex;justify-content:space-between;align-items:center;">'
    +'<span style="color:var(--dim);">% Interés anual</span><b>'+t.interes+'%</b></div>':'')
    // Botones
    +'<div style="display:flex;gap:8px;margin-bottom:16px;">'
    +'<button class="btn-main" style="flex:1;" onclick="registrarPagoTC('+i+')">💳 Registrar pago</button>'
    +'<button class="btn-sec" onclick="editarTC('+i+')">✏️ Editar</button>'
    +'</div>'
    // Movimientos
    +'<div style="font-size:0.75rem;font-weight:800;color:var(--dim);text-transform:uppercase;letter-spacing:0.06em;margin-bottom:10px;">Movimientos ('+txs.length+')</div>';

  if(txs.length===0){
    html += '<div style="text-align:center;padding:24px;color:var(--dim);font-size:0.8rem;">Sin movimientos registrados en esta tarjeta</div>';
  } else {
    txs.forEach(function(tx){
      html += '<div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:12px 14px;margin-bottom:6px;display:flex;align-items:center;justify-content:space-between;">'
        +'<div><div style="font-size:0.82rem;font-weight:700;">'+tx.desc+'</div>'
        +'<div style="font-size:0.68rem;color:var(--dim);">'+tx.fecha+(tx.cat?' · '+tx.cat:'')+'</div></div>'
        +'<div style="font-size:0.95rem;font-weight:900;color:'+(tx.tipo==='ingreso'?'var(--accent)':'var(--danger)')+';">'
        +(tx.tipo==='ingreso'?'+':'-')+fmt(tx.monto)+'</div>'
        +'</div>';
    });
  }

  mc.innerHTML = html;
}

// ── Compras con TC (toggle + guardar) ────────────
function toggleFormCompraTC(i){
  var id='compraTC_'+i;
  var el=document.getElementById(id);
  if(el){ el.style.display=el.style.display==='none'?'block':'none'; return; }
  var div=document.createElement('div'); div.id=id;
  div.style.cssText='margin-top:8px;padding:12px;background:var(--inp);border-radius:12px;';
  div.innerHTML='<label class="inp-label">Descripción</label>'
    +'<input class="inp" id="compraDesc_'+i+'" placeholder="¿Qué compraste?">'
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="compraMonto_'+i+'" type="number" inputmode="decimal" placeholder="0.00">'
    +'</div><div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="compraFecha_'+i+'" type="date" value="'+today()+'">'
    +'</div></div>'
    +'<label class="inp-label">Categoría</label>'
    +'<select class="inp" id="compraCat_'+i+'">'
    +'<option>Supermercado</option><option>Restaurante</option>'
    +'<option>Gasolina</option><option>Ropa</option>'
    +'<option>Salud</option><option>Entretenimiento</option>'
    +'<option>Servicios</option><option>Otro</option></select>'
    +'<button class="btn-main" onclick="guardarCompraTC('+i+')" style="margin-top:8px;">Guardar compra</button>';
  var parent=document.querySelector('[data-tc-idx="'+i+'"]');
  if(parent) parent.after(div);
  else document.getElementById('mainContent').appendChild(div);
}

function guardarCompraTC(i){
  var desc=(document.getElementById('compraDesc_'+i).value||'').trim();
  var monto=parseFloat(document.getElementById('compraMonto_'+i).value)||0;
  var fecha=document.getElementById('compraFecha_'+i).value||today();
  var cat=document.getElementById('compraCat_'+i).value||'Otro';
  if(!desc||!monto){ showToast('Completa descripción y monto'); return; }
  var c=getCuentas(); c.tarjetas=c.tarjetas||[];
  if(!c.tarjetas[i]){ showToast('Tarjeta no encontrada'); return; }
  c.tarjetas[i].balance=(c.tarjetas[i].balance||0)+monto;
  saveCuentas(c);
  var txs=getTxs();
  txs.push({id:Date.now(),tipo:'gasto',desc:desc,monto:monto,
    fecha:fecha,cat:cat,cuenta:'tc_'+i,nota:'Compra con tarjeta '+c.tarjetas[i].banco});
  save('txs',txs);
  showToast('Compra registrada: '+fmt(monto));
  goSub('tarjetas_credito');
}

// ──────────────────────────────────────────────────────────────
//  CRÉDITOS — Lo que debo / Lo que me deben
// ──────────────────────────────────────────────────────────────

function renderCreditos(){
  var mc=document.getElementById('mainContent');
  var creds=load('creditos',[]);
  var deudas   = creds.filter(function(c){ return c.tipo==='deuda'; });
  var prestamos= creds.filter(function(c){ return c.tipo==='prestamo'; });
  var totalDebo  = deudas.reduce(function(s,c){ return s+(c.monto-(c.abonado||0)); },0);
  var totalCobro = prestamos.reduce(function(s,c){ return s+(c.monto-(c.abonado||0)); },0);

  mc.innerHTML = '<div class="page-header">'+backBtn('creditos',2)+'<div class="page-title">🤝 Créditos</div></div>'
    +'<div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px;">'
    +'<div class="cred-item" style="cursor:pointer;border:1.5px solid rgba(229,57,53,0.3);" onclick="goSub(\'creditos_debo\')">'
    +'<div style="font-size:1.5rem;margin-bottom:6px;">📤</div>'
    +'<div style="font-size:0.78rem;font-weight:800;color:var(--txt);">Lo que debo</div>'
    +'<div style="font-size:1.1rem;font-weight:900;color:var(--danger);margin-top:4px;">'+fmt(totalDebo)+'</div>'
    +'<div style="font-size:0.65rem;color:var(--dim);margin-top:2px;">'+deudas.length+' crédito'+(deudas.length!==1?'s':'')+'</div>'
    +'</div>'
    +'<div class="cred-item" style="cursor:pointer;border:1.5px solid rgba(43,192,112,0.3);" onclick="goSub(\'creditos_cobrar\')">'
    +'<div style="font-size:1.5rem;margin-bottom:6px;">📥</div>'
    +'<div style="font-size:0.78rem;font-weight:800;color:var(--txt);">Me deben</div>'
    +'<div style="font-size:1.1rem;font-weight:900;color:var(--accent);margin-top:4px;">'+fmt(totalCobro)+'</div>'
    +'<div style="font-size:0.65rem;color:var(--dim);margin-top:2px;">'+prestamos.length+' préstamo'+(prestamos.length!==1?'s':'')+'</div>'
    +'</div></div>'
    +'<div style="display:flex;gap:8px;margin-bottom:16px;">'
    +'<button class="btn-main" style="flex:1;" onclick="goSub(\'creditos_debo\')">📤 Mis deudas</button>'
    +'<button class="btn-main" style="flex:1;background:rgba(43,192,112,0.15);border:1px solid rgba(43,192,112,0.3);color:var(--accent);" onclick="goSub(\'creditos_cobrar\')">📥 Me deben</button>'
    +'</div>'
    +'<button class="btn-sec" style="width:100%;margin-bottom:12px;" onclick="goSub(\'cxc\')">📋 Cuentas por cobrar (CxC)</button>';
}

function renderCreditosDebo(){
  var mc=document.getElementById('mainContent');
  mc.innerHTML='<div class="page-header">'+backSubBtn()+'<div class="page-title">📤 Mis Deudas</div></div>';
  var bNew=document.createElement('button');
  bNew.className='btn-main';
  bNew.style.cssText='width:100%;margin-bottom:14px;';
  bNew.textContent='+ Nueva deuda';
  bNew.onclick=function(){ goSub('nueva_deuda'); };
  mc.appendChild(bNew);
  renderListaCreds('deuda');
}

function renderCreditosCobrar(){
  var mc=document.getElementById('mainContent');
  mc.innerHTML='<div class="page-header">'+backSubBtn()+'<div class="page-title">📥 Me deben</div></div>';
  var bNew=document.createElement('button');
  bNew.className='btn-main';
  bNew.style.cssText='width:100%;margin-bottom:14px;background:rgba(43,192,112,0.15);border:1px solid rgba(43,192,112,0.3);color:var(--accent);';
  bNew.textContent='+ Nuevo préstamo que hice';
  bNew.onclick=function(){ goSub('nuevo_prestamo'); };
  mc.appendChild(bNew);
  renderListaCreds('prestamo');
}

function renderListaCreds(tipo){
  var allCreds=load('creditos',[]);
  var creds=allCreds.filter(function(c){ return c.tipo===tipo; });
  var mc=document.getElementById('mainContent');
  if(!creds.length){
    var emptyDiv=document.createElement('div');
    emptyDiv.style.cssText='text-align:center;padding:40px 20px;color:var(--dim);';
    emptyDiv.innerHTML='<div style="font-size:3rem;margin-bottom:12px;">'+(tipo==='deuda'?'📤':'📥')+'</div>'
      +'<div style="font-size:0.85rem;">Sin registros</div>';
    mc.appendChild(emptyDiv);
    return;
  }
  var fragment=document.createDocumentFragment();
  creds.forEach(function(c,i){
    var ri=allCreds.indexOf(c);
    var pct=c.monto>0?Math.min(100,Math.round(((c.abonado||0)/c.monto)*100)):0;
    var hoy=new Date();
    var fv=c.fechaLimite?(function(){ var p=c.fechaLimite.split('-'); return new Date(+p[0],+p[1]-1,+p[2]); })():null;
    var venc=fv&&fv<hoy&&c.estado!=='pagado';
    var div=document.createElement('div');
    div.className='cred-item';
    var badgeTxt=c.estado==='pagado'?'✅ Pagado':venc?'🔴 Vencido':'⏳ Pendiente';
    var badgeCls=c.estado==='pagado'?'badge-pagado':venc?'badge-vencido':'badge-pend';
    var _tiLabel=c.tipoInteres==='mensual'?'📅 mensual':c.tipoInteres==='anual'?'📆 anual':'📦 total';
    var descExtra=(c.interes?' · '+c.interes+'% ('+_tiLabel+')':'')
      +(c.fechaOrigen?' · Otorgado: '+c.fechaOrigen:'')
      +(c.fechaLimite?' · Vence: '+c.fechaLimite:'');
    var totalIntPag=c.interesesPagados||0;
    var totalCap=c.abonado||0;
    var resumenExtra='';
    if(totalIntPag>0){
      resumenExtra='<span style="font-size:0.73rem;background:#fff3e0;border-radius:6px;padding:3px 8px;color:#e07b00;">Intereses: <b>'+fmt(totalIntPag)+'</b></span>';
    } else if(c.interes>0){
      resumenExtra='<span style="font-size:0.73rem;background:var(--inp);border-radius:6px;padding:3px 8px;color:var(--dim);">Sin int. pagados</span>';
    }
    var histId='hist_'+tipo+'_'+i;
    var histDiv=null;
    if(c.historialAbonos&&c.historialAbonos.length){
      var totCapH=c.historialAbonos.reduce(function(s,a){ return s+(a.monto||0); },0);
      var totIntH=c.historialAbonos.reduce(function(s,a){ return s+(a.interes||0); },0);
      histDiv=document.createElement('div');
      histDiv.id=histId;
      histDiv.style.cssText='display:none;margin-top:8px;background:var(--inp);border-radius:10px;padding:8px 12px;';
      var tit=document.createElement('div');
      tit.style.cssText='font-size:0.72rem;font-weight:800;color:var(--dim);margin-bottom:4px;text-transform:uppercase;letter-spacing:0.06em;';
      tit.textContent='Historial de abonos';
      histDiv.appendChild(tit);
      var idxsRev=c.historialAbonos.map(function(_,x){ return x; }).reverse();
      idxsRev.forEach(function(ai){
        var a=c.historialAbonos[ai];
        var fila=document.createElement('div');
        fila.style.cssText='padding:6px 0;border-bottom:1px solid var(--border);font-size:0.76rem;';
        var row=document.createElement('div');
        row.style.cssText='display:flex;justify-content:space-between;align-items:center;';
        var fechaSpan=document.createElement('span');
        fechaSpan.style.color='var(--dim)';
        fechaSpan.textContent=a.fecha;
        var rightSpan=document.createElement('span');
        rightSpan.style.cssText='display:flex;align-items:center;gap:6px;';
        if(a.monto>0){
          var ms=document.createElement('span');
          ms.style.cssText='font-weight:700;color:var(--accent);';
          ms.textContent=fmt(a.monto);
          rightSpan.appendChild(ms);
        }
        if(a.interes>0){
          var is=document.createElement('span');
          is.style.cssText='color:#e07b00;font-size:0.7rem;';
          is.textContent='+'+fmt(a.interes)+' int.';
          rightSpan.appendChild(is);
        }
        var bEditA=document.createElement('button');
        bEditA.style.cssText='background:none;border:1px solid var(--border);border-radius:6px;padding:2px 7px;font-size:0.7rem;cursor:pointer;color:var(--accent);';
        bEditA.textContent='✏️';
        (function(ri_,ai_,tipo_){ bEditA.onclick=function(e){ e.stopPropagation(); editarAbono(ri_,ai_,tipo_); }; })(ri,ai,tipo);
        rightSpan.appendChild(bEditA);
        var bDelA=document.createElement('button');
        bDelA.style.cssText='background:none;border:1px solid rgba(229,57,53,0.35);border-radius:6px;padding:2px 7px;font-size:0.7rem;cursor:pointer;color:var(--danger);';
        bDelA.textContent='🗑';
        (function(ri_,ai_,tipo_){ bDelA.onclick=function(e){ e.stopPropagation(); eliminarAbono(ri_,ai_,tipo_); }; })(ri,ai,tipo);
        rightSpan.appendChild(bDelA);
        row.appendChild(fechaSpan); row.appendChild(rightSpan);
        fila.appendChild(row);
        if(a.nota){
          var notaDiv=document.createElement('div');
          notaDiv.style.cssText='font-size:0.72rem;color:var(--dim);margin-top:2px;font-style:italic;';
          notaDiv.textContent='📝 '+a.nota;
          fila.appendChild(notaDiv);
        }
        histDiv.appendChild(fila);
      });
      var pie=document.createElement('div');
      pie.style.cssText='display:flex;justify-content:space-between;padding:6px 0 2px;font-size:0.74rem;font-weight:800;border-top:1.5px solid var(--border);margin-top:4px;';
      pie.innerHTML='<span>Total</span><span>Capital: '+fmt(totCapH)+(totIntH>0?' + Int: '+fmt(totIntH):'')+'</span>';
      histDiv.appendChild(pie);
    }
    var pendiente=c.monto-(c.abonado||0);
    div.innerHTML=
      '<div class="cred-top"><div>'
        +'<div class="cred-persona">'+c.persona+'</div>'
        +'<div class="cred-desc">'+c.descripcion+descExtra+'</div>'
      +'</div><span class="cred-badge '+badgeCls+'">'+badgeTxt+'</span></div>'
      +'<div style="display:flex;gap:6px;flex-wrap:wrap;margin-bottom:6px;">'
        +'<span style="font-size:0.73rem;background:var(--inp);border-radius:6px;padding:3px 8px;">Capital: <b>'+fmt(totalCap)+'</b> / '+fmt(c.monto)+'</span>'
        +'<span style="font-size:0.73rem;background:var(--inp);border-radius:6px;padding:3px 8px;">Pendiente: <b style="color:'+(tipo==='deuda'?'var(--danger)':'var(--accent)')+'">'+fmt(pendiente)+'</b></span>'
        +resumenExtra
      +'</div>'
      +'<div class="prog-wrap"><div class="prog-bar" style="width:'+pct+'%;'+(pct>=100?'background:#2d9e5f;':'')+'" ></div></div>'
      +'<div class="cred-btns" id="btns_'+tipo+'_'+i+'"></div>';
    if(histDiv) div.appendChild(histDiv);
    var btnsDiv=div.querySelector('#btns_'+tipo+'_'+i);
    if(c.estado!=='pagado'){
      var bAbonar=document.createElement('button');
      bAbonar.className='cred-btn success'; bAbonar.textContent='+ Abonar';
      (function(ri_,tipo_){ bAbonar.onclick=function(){ abonarCred(ri_,tipo_); }; })(ri,tipo);
      btnsDiv.appendChild(bAbonar);
      var bPagar=document.createElement('button');
      bPagar.className='cred-btn success'; bPagar.style.cssText='background:rgba(45,158,95,0.15);color:#2d9e5f;';
      bPagar.textContent='✅ Liquidar';
      (function(i_,tipo_){ bPagar.onclick=function(){ pagarCred(i_,tipo_); }; })(i,tipo);
      btnsDiv.appendChild(bPagar);
    }
    if(c.historialAbonos&&c.historialAbonos.length){
      var bHist=document.createElement('button');
      bHist.className='cred-btn';
      bHist.style.cssText='color:#fff;background:var(--accent);border-color:var(--accent);';
      bHist.innerHTML='📋 <b>'+c.historialAbonos.length+'</b>';
      (function(hid){ bHist.onclick=function(){
        var h=document.getElementById(hid);
        if(h) h.style.display=h.style.display==='none'?'block':'none';
      }; })(histId);
      btnsDiv.appendChild(bHist);
    }
    var bEdit=document.createElement('button');
    bEdit.className='cred-btn'; bEdit.textContent='✏️';
    (function(i_,tipo_){ bEdit.onclick=function(){ editarCred(i_,tipo_); }; })(i,tipo);
    btnsDiv.appendChild(bEdit);
    var bDel=document.createElement('button');
    bDel.className='cred-btn danger'; bDel.textContent='🗑️';
    (function(i_,tipo_){ bDel.onclick=function(){ borrarCred(i_,tipo_); }; })(i,tipo);
    btnsDiv.appendChild(bDel);
    fragment.appendChild(div);
  });
  mc.appendChild(fragment);
}

function renderFormCredito(tipo,data){
  var esD=tipo==='deuda';
  var d=data||{};
  var titulo=(d.persona?'Editar':'Nuevo')+(esD?' · Deuda':' · Préstamo');
  return '<div class="page-header">'+backSubBtn()+'<div class="page-title">'+(esD?'📤':'📥')+' '+titulo+'</div></div>'
    +'<div class="card">'
    +'<label class="inp-label">'+(esD?'¿A quién le debo?':'¿Quién me debe?')+'</label>'
    +'<input class="inp" id="crPersona" placeholder="Nombre" value="'+(d.persona||'')+'">'
    +'<label class="inp-label">Descripción / Concepto</label>'
    +'<input class="inp" id="crDesc" placeholder="Ej: Préstamo para auto" value="'+(d.descripcion||'')+'">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="crMonto" type="number" inputmode="decimal" placeholder="0.00" value="'+(d.monto||'')+'"></div>'
    +'<div><label class="inp-label">Interés (%)</label>'
    +'<input class="inp" id="crInteres" type="number" inputmode="decimal" placeholder="0" value="'+(d.interes||'')+'"></div>'
    +'</div>'
    +'<label class="inp-label">Tipo de interés</label>'
    +'<select class="inp" id="crTipoInteres">'
    +'<option value="total"'+(d.tipoInteres==='total'?' selected':'')+'>📦 Total (aplica una vez)</option>'
    +'<option value="mensual"'+(d.tipoInteres==='mensual'?' selected':'')+'>📅 Mensual</option>'
    +'<option value="anual"'+(d.tipoInteres==='anual'?' selected':'')+'>📆 Anual</option>'
    +'</select>'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Fecha otorgado</label>'
    +'<input class="inp" id="crFecha" type="date" value="'+(d.fechaOrigen||today())+'"></div>'
    +'<div><label class="inp-label">Fecha límite</label>'
    +'<input class="inp" id="crVencimiento" type="date" value="'+(d.fechaLimite||'')+'"></div>'
    +'</div>'
    +'<button class="btn-main" onclick="guardarCred(\''+tipo+'\')">💾 Guardar</button>'
    +'<button class="btn-sec" onclick="goSub(\''+(esD?'creditos_debo':'creditos_cobrar')+'\')">Cancelar</button>'
    +'</div>';
}

function guardarCred(tipo){
  var persona=document.getElementById('crPersona').value.trim();
  var desc=document.getElementById('crDesc').value.trim();
  var monto=parseFloat(document.getElementById('crMonto').value);
  var interes=parseFloat(document.getElementById('crInteres').value)||0;
  var tipoInteres=document.getElementById('crTipoInteres').value;
  var fecha=document.getElementById('crFecha').value;
  var vencimiento=document.getElementById('crVencimiento').value;
  if(!persona||!desc||!monto){ showToast('Completa persona, descripción y monto'); return; }
  var creds=load('creditos',[]);
  var item={
    tipo:tipo, persona:persona, descripcion:desc, monto:monto,
    interes:interes, tipoInteres:tipoInteres,
    fechaOrigen:fecha, fechaLimite:vencimiento,
    estado:'pendiente', abonado:0, interesesPagados:0, historialAbonos:[]
  };
  if(S.editCrediIdx!==null){
    var all=creds.filter(function(c){ return c.tipo===tipo; });
    var existing=all[S.editCrediIdx];
    var ri=creds.indexOf(existing);
    item.abonado=existing.abonado||0;
    item.interesesPagados=existing.interesesPagados||0;
    item.historialAbonos=existing.historialAbonos||[];
    item.estado=existing.estado||'pendiente';
    creds[ri]=item;
    S.editCrediIdx=null; S.editCrediTipo=null;
    showToast('Crédito actualizado');
  } else {
    creds.push(item);
    showToast('Crédito registrado');
  }
  save('creditos',creds);
  goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
}

function pagarCred(i,tipo){
  var creds=load('creditos',[]);
  var all=creds.filter(function(c){ return c.tipo===tipo; });
  var item=all[i]; var ri=creds.indexOf(item);
  creds[ri].estado='pagado'; creds[ri].abonado=creds[ri].monto;
  save('creditos',creds); showToast('Marcado como pagado');
  goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
}

function editarCred(i,tipo){
  var creds=load('creditos',[]).filter(function(c){ return c.tipo===tipo; });
  S.editCrediIdx=i; S.editCrediTipo=tipo;
  document.getElementById('mainContent').innerHTML=renderFormCredito(tipo,creds[i]);
}

function borrarCred(i,tipo){
  var creds=load('creditos',[]);
  var all=creds.filter(function(c){ return c.tipo===tipo; });
  var item=all[i]; var ri=creds.indexOf(item); var eli=creds[ri];
  usalaConfirm('Eliminar credito con '+eli.persona+'?', function(){
    creds.splice(ri,1); save('creditos',creds);
    goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
    mostrarUndo('Credito eliminado',function(){
      var c2=load('creditos',[]); c2.splice(ri,0,eli); save('creditos',c2);
      goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
    });
  });
}

function abonarCred(ri,tipo){
  var creds=load('creditos',[]);
  var item=creds[ri];
  if(!item){ showToast('Crédito no encontrado'); return; }
  window._abonoRi=ri; window._abonoTipo=tipo;
  var esCobrar=tipo==='prestamo';
  var pendiente=item.monto-(item.abonado||0);
  var mc=document.getElementById('mainContent');
  mc.innerHTML='';
  var d=document.createElement('div'); d.style.padding='20px 16px';
  var accentColor=esCobrar?'var(--accent2)':'var(--accent)';

  d.innerHTML='<div class="page-header">'+backSubBtn()+'<div class="page-title">'+(esCobrar?'📥 Cobrar abono':'📤 Registrar abono')+'</div></div>'
    +'<div class="card">'
    +'<div style="background:var(--inp);border-radius:12px;padding:12px;margin-bottom:14px;">'
    +'<div style="font-weight:800;font-size:0.9rem;margin-bottom:2px;">'+item.persona+'</div>'
    +'<div style="font-size:0.78rem;color:var(--dim);margin-bottom:8px;">'+item.descripcion+'</div>'
    +'<div style="display:flex;gap:12px;">'
    +'<div><div style="font-size:0.6rem;color:var(--dim);font-weight:700;text-transform:uppercase;">Total</div>'
    +'<div style="font-weight:900;font-size:0.9rem;">'+fmt(item.monto)+'</div></div>'
    +'<div><div style="font-size:0.6rem;color:var(--dim);font-weight:700;text-transform:uppercase;">Pagado</div>'
    +'<div style="font-weight:900;font-size:0.9rem;color:'+accentColor+';">'+fmt(item.abonado||0)+'</div></div>'
    +'<div><div style="font-size:0.6rem;color:var(--dim);font-weight:700;text-transform:uppercase;">Pendiente</div>'
    +'<div style="font-weight:900;font-size:0.9rem;color:var(--danger);">'+fmt(pendiente)+'</div></div>'
    +'</div></div>'
    +'<label class="inp-label">Monto del abono ($)</label>'
    +'<input class="inp" id="abonoMonto" type="number" inputmode="decimal" placeholder="0.00" value="'+pendiente+'">'
    +(item.interes>0
      ?'<label class="inp-label">Interés incluido ($)</label><input class="inp" id="abonoInteres" type="number" inputmode="decimal" placeholder="0.00" value="0">'
      :'')
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="abonoFecha" type="date" value="'+today()+'"></div>'
    +(esCobrar
      ?'<div><label class="inp-label">¿A qué cuenta?</label>'+buildCuentaOpts('abonoCuenta')+'</div>'
      :'<div><label class="inp-label">¿De qué cuenta?</label>'+buildCuentaOpts('abonoCuenta')+'</div>')
    +'</div>'
    +'<label class="inp-label">Nota (opcional)</label>'
    +'<input class="inp" id="abonoNota" placeholder="Ej: Transferencia SPEI">'
    +'<button class="btn-main" onclick="_confirmarAbono()">✅ Registrar abono</button>'
    +'<button class="btn-sec" onclick="goSub(\''+(tipo==='deuda'?'creditos_debo':'creditos_cobrar')+'\')">Cancelar</button>'
    +'</div>';
  mc.appendChild(d);
}

function _confirmarAbono(){
  var ri=window._abonoRi;
  var tipo=window._abonoTipo;
  var monto=parseFloat(document.getElementById('abonoMonto').value)||0;
  var interesEl=document.getElementById('abonoInteres');
  var interes=interesEl?parseFloat(interesEl.value)||0:0;
  var fecha=document.getElementById('abonoFecha').value||today();
  var cuenta=document.getElementById('abonoCuenta')?document.getElementById('abonoCuenta').value:'efectivo';
  var nota=(document.getElementById('abonoNota').value||'').trim();
  if(!monto||monto<=0){ showToast('Ingresa el monto'); return; }

  var creds=load('creditos',[]);
  var item=creds[ri];
  if(!item){ showToast('Crédito no encontrado'); return; }

  item.abonado=(item.abonado||0)+monto;
  item.interesesPagados=(item.interesesPagados||0)+interes;
  if(item.abonado>=item.monto){ item.estado='pagado'; item.abonado=item.monto; }
  item.historialAbonos=item.historialAbonos||[];
  item.historialAbonos.push({fecha:fecha, monto:monto, interes:interes, nota:nota, cuenta:cuenta});
  creds[ri]=item;
  save('creditos',creds);

  // Mover dinero en la cuenta
  if(cuenta && cuenta!=='ninguna'){
    if(tipo==='deuda'){
      // Pagué una deuda → salida de mi cuenta
      aplicarMovimientoCuenta(cuenta, monto+interes, 'gasto', 'Abono deuda: '+item.persona, fecha, Date.now());
    } else {
      // Me pagaron un préstamo → entrada a mi cuenta
      aplicarMovimientoCuenta(cuenta, monto, 'ingreso', 'Cobro préstamo: '+item.persona, fecha, Date.now());
    }
  }

  showToast('Abono registrado: '+fmt(monto));
  goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
}

function editarAbono(ri,ai,tipo){
  var creds=load('creditos',[]);
  var item=creds[ri];
  if(!item||!item.historialAbonos||!item.historialAbonos[ai]){ showToast('Abono no encontrado'); return; }
  var a=item.historialAbonos[ai];
  var mc=document.getElementById('mainContent');
  mc.innerHTML='<div class="page-header">'+backSubBtn()+'<div class="page-title">✏️ Editar abono</div></div>'
    +'<div class="card">'
    +'<label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="editAbonoMonto" type="number" value="'+(a.monto||0)+'">'
    +'<label class="inp-label">Interés incluido ($)</label>'
    +'<input class="inp" id="editAbonoInt" type="number" value="'+(a.interes||0)+'">'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="editAbonoFecha" type="date" value="'+(a.fecha||today())+'">'
    +'<label class="inp-label">Nota</label>'
    +'<input class="inp" id="editAbonoNota" value="'+(a.nota||'')+'">'
    +'<button class="btn-main" onclick="_guardarEditAbono('+ri+','+ai+',\''+tipo+'\')">💾 Guardar cambios</button>'
    +'<button class="btn-sec" onclick="goSub(\''+(tipo==='deuda'?'creditos_debo':'creditos_cobrar')+'\')">Cancelar</button>'
    +'</div>';
}

function _guardarEditAbono(ri,ai,tipo){
  var creds=load('creditos',[]);
  var item=creds[ri];
  if(!item||!item.historialAbonos){ return; }
  var viejoMonto=item.historialAbonos[ai].monto||0;
  var viejoInt=item.historialAbonos[ai].interes||0;
  var nuevoMonto=parseFloat(document.getElementById('editAbonoMonto').value)||0;
  var nuevoInt=parseFloat(document.getElementById('editAbonoInt').value)||0;
  item.historialAbonos[ai]={
    fecha:document.getElementById('editAbonoFecha').value||today(),
    monto:nuevoMonto, interes:nuevoInt,
    nota:document.getElementById('editAbonoNota').value||''
  };
  // Recalcular totales
  item.abonado=(item.abonado||0)-viejoMonto+nuevoMonto;
  item.interesesPagados=(item.interesesPagados||0)-viejoInt+nuevoInt;
  item.estado=item.abonado>=item.monto?'pagado':'pendiente';
  creds[ri]=item;
  save('creditos',creds);
  showToast('Abono actualizado');
  goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
}

function eliminarAbono(ri,ai,tipo){
  var creds=load('creditos',[]);
  var item=creds[ri];
  if(!item||!item.historialAbonos||!item.historialAbonos[ai]){ showToast('No encontrado'); return; }
  usalaConfirm('Eliminar este abono?', function(){
    var a=item.historialAbonos[ai];
    item.abonado=Math.max(0,(item.abonado||0)-(a.monto||0));
    item.interesesPagados=Math.max(0,(item.interesesPagados||0)-(a.interes||0));
    item.historialAbonos.splice(ai,1);
    item.estado=item.abonado>=item.monto&&item.monto>0?'pagado':'pendiente';
    creds[ri]=item;
    save('creditos',creds);
    showToast('Abono eliminado');
    goSub(tipo==='deuda'?'creditos_debo':'creditos_cobrar');
  });
}

// ──────────────────────────────────────────────────────────────
//  CUENTAS POR COBRAR (CxC)
// ──────────────────────────────────────────────────────────────

function renderCxC(){
  var cxcs=load('cxc',[]);
  var mc=document.getElementById('mainContent');
  var total=cxcs.reduce(function(s,c){ return s+c.monto; },0);
  var html='<div class="page-header">'+backSubBtn()+'<div class="page-title">📋 CxC — Por Cobrar</div></div>'
    +'<div style="background:var(--card);border:1px solid var(--border);border-radius:14px;padding:14px 16px;margin-bottom:14px;display:flex;justify-content:space-between;align-items:center;">'
    +'<div><div style="font-size:0.62rem;color:var(--dim);font-weight:700;text-transform:uppercase;letter-spacing:0.06em;">Total por cobrar</div>'
    +'<div style="font-size:1.3rem;font-weight:900;color:var(--accent);">'+fmt(total)+'</div></div>'
    +'<button class="btn-main" style="padding:10px 16px;" onclick="goSub(\'nueva_cxc\')">+ Nueva CxC</button>'
    +'</div>';

  if(!cxcs.length){
    html+='<div style="text-align:center;padding:40px 20px;color:var(--dim);">'
      +'<div style="font-size:3rem;margin-bottom:12px;">📋</div>'
      +'<div style="font-size:0.85rem;">Sin cuentas por cobrar</div></div>';
  } else {
    cxcs.forEach(function(c,i){
      var venc=c.fechaVence&&new Date(c.fechaVence)<new Date();
      html+='<div class="cred-item">'
        +'<div class="cred-top"><div>'
        +'<div class="cred-persona">'+c.nombre+'</div>'
        +'<div class="cred-desc">'+c.concepto+(c.fechaVence?' · Vence: '+c.fechaVence:'')+'</div></div>'
        +'<span class="cred-badge '+(venc?'badge-vencido':'badge-pend')+'">'+(venc?'🔴 Vencido':'⏳ Pendiente')+'</span>'
        +'</div>'
        +'<div style="font-size:1.1rem;font-weight:900;color:var(--accent);margin:8px 0;">'+fmt(c.monto)+'</div>'
        +'<div style="display:flex;gap:6px;">'
        +'<button class="cred-btn success" onclick="cobrarCxC('+i+')">✅ Cobrar</button>'
        +'<button class="cred-btn danger" onclick="borrarCxC('+i+')">🗑️</button>'
        +'</div></div>';
    });
  }

  mc.innerHTML=html;
}

function guardarCxC(){
  var nombre=(document.getElementById('cxcNombre').value||'').trim();
  var monto=parseFloat(document.getElementById('cxcMonto').value)||0;
  var concepto=(document.getElementById('cxcConcepto').value||'').trim();
  var fechaVence=document.getElementById('cxcFechaVence').value;
  if(!nombre||!monto){ showToast('Ingresa nombre y monto'); return; }
  var cxcs=load('cxc',[]);
  cxcs.push({nombre:nombre, monto:monto, concepto:concepto||'Deuda', fechaVence:fechaVence, fechaReg:today()});
  save('cxc',cxcs);
  showToast('CxC registrada');
  goSub('cxc');
}

function cobrarCxC(i){
  var cxcs=load('cxc',[]);
  var c=cxcs[i];
  if(!c){ showToast('No encontrado'); return; }

  var m=document.createElement('div');
  m.className='modal open'; m.id='cobrarCxCModal';
  m.innerHTML='<div class="modal-body">'
    +'<div class="modal-title">✅ Cobrar a '+c.nombre+'</div>'
    +'<div style="font-size:0.85rem;color:var(--dim);margin-bottom:14px;">'+c.concepto+' · '+fmt(c.monto)+'</div>'
    +'<label class="inp-label">¿A qué cuenta ingresa?</label>'
    +buildCuentaOpts('cobrarCxCCuenta')
    +'<label class="inp-label" style="margin-top:10px;">Fecha</label>'
    +'<input class="inp" id="cobrarCxCFecha" type="date" value="'+today()+'">'
    +'<div style="display:flex;gap:8px;margin-top:12px;">'
    +'<button class="btn-main" style="flex:1;" onclick="_confirmarCobrarCxC('+i+')">Cobrar</button>'
    +'<button class="btn-sec" onclick="document.getElementById(\'cobrarCxCModal\').remove()">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
}

function _confirmarCobrarCxC(i){
  var cxcs=load('cxc',[]);
  var c=cxcs[i];
  if(!c) return;
  var cuenta=document.getElementById('cobrarCxCCuenta').value||'efectivo';
  var fecha=document.getElementById('cobrarCxCFecha').value||today();

  // Registrar ingreso
  var txs=load('txs',[]);
  txs.push({id:Date.now(),tipo:'ingreso',monto:c.monto,
    desc:'Cobré a: '+c.nombre,cat:'Cobro de deuda',
    fecha:fecha,cuenta:cuenta});
  save('txs',txs);

  // Mover saldo en la cuenta
  aplicarMovimientoCuenta(cuenta, c.monto, 'ingreso', 'Cobro: '+c.nombre, fecha, Date.now());

  cxcs.splice(i,1);
  save('cxc',cxcs);
  var modal=document.getElementById('cobrarCxCModal');
  if(modal) modal.remove();
  showToast('Cobro registrado: '+fmt(c.monto));
  goSub('cxc');
}

function borrarCxC(i){
  var cxcs=load('cxc',[]);
  usalaConfirm('Eliminar esta cuenta por cobrar?', function(){
    var eli=cxcs[i];
    cxcs.splice(i,1);
    save('cxc',cxcs);
    goSub('cxc');
    mostrarUndo('CxC eliminada',function(){
      var c2=load('cxc',[]); c2.splice(i,0,eli); save('cxc',c2); goSub('cxc');
    });
  });
}

// ── Formulario nueva CxC ──────────────────────────
function renderNuevaCxC(){
  document.getElementById('mainContent').innerHTML=
    '<div class="page-header">'+backSubBtn()+'<div class="page-title">📋 Nueva CxC</div></div>'
    +'<div class="card">'
    +'<label class="inp-label">¿Quién te debe?</label>'
    +'<input class="inp" id="cxcNombre" placeholder="Nombre">'
    +'<label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="cxcMonto" type="number" inputmode="decimal" placeholder="0.00">'
    +'<label class="inp-label">Concepto</label>'
    +'<input class="inp" id="cxcConcepto" placeholder="Ej: Préstamo para renta">'
    +'<label class="inp-label">Fecha límite (opcional)</label>'
    +'<input class="inp" id="cxcFechaVence" type="date">'
    +'<button class="btn-main" onclick="guardarCxC()">💾 Guardar</button>'
    +'<button class="btn-sec" onclick="goSub(\'cxc\')">Cancelar</button>'
    +'</div>';
}

// ── Modales rápidos desde inicio ─────────────────
function _abrirModalPreste(){
  var m=document.createElement('div');
  m.className='modal open'; m.id='presteModal';
  m.innerHTML='<div class="modal-body">'
    +'<div class="modal-title">🤝 Presté dinero</div>'
    +'<p style="color:var(--dim);font-size:0.82rem;margin-bottom:14px;">Se registrará en <b>Créditos → Me deben</b></p>'
    +'<label class="inp-label">¿A quién le presté?</label>'
    +'<input class="inp" id="ptPersona" placeholder="Nombre">'
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="ptMonto" type="number" inputmode="decimal" placeholder="0.00">'
    +'</div><div>'
    +'<label class="inp-label">Interés (%)</label>'
    +'<input class="inp" id="ptInteres" type="number" inputmode="decimal" placeholder="0">'
    +'</div></div>'
    +'<label class="inp-label">Concepto</label>'
    +'<input class="inp" id="ptDesc" placeholder="Ej: Para renta">'
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="ptFecha" type="date" value="'+today()+'">'
    +'</div><div>'
    +'<label class="inp-label">Vence</label>'
    +'<input class="inp" id="ptVence" type="date">'
    +'</div></div>'
    +'<label class="inp-label">¿De qué cuenta sale?</label>'
    +buildCuentaOpts('ptCuenta')
    +'<div style="display:flex;gap:8px;margin-top:12px;">'
    +'<button class="btn-main" style="flex:1;" onclick="_guardarPreste()">💾 Registrar</button>'
    +'<button class="btn-sec" onclick="document.getElementById(\'presteModal\').remove()">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
}

function _guardarPreste(){
  var persona=(document.getElementById('ptPersona').value||'').trim();
  var monto=parseFloat(document.getElementById('ptMonto').value||0);
  var interes=parseFloat(document.getElementById('ptInteres').value||0);
  var desc=(document.getElementById('ptDesc').value||'').trim();
  var fecha=document.getElementById('ptFecha').value;
  var vence=document.getElementById('ptVence').value;
  var cuenta=document.getElementById('ptCuenta').value;
  if(!persona||!monto){ showToast('Ingresa a quién y el monto'); return; }
  if(!desc) desc='Prestamo a '+persona;
  var creds=load('creditos',[]);
  creds.push({tipo:'prestamo',persona:persona,descripcion:desc,monto:monto,
    interes:interes,tipoInteres:'total',fechaOrigen:fecha,fechaLimite:vence,
    estado:'pendiente',abonado:0,interesesPagados:0,historialAbonos:[]});
  save('creditos',creds);
  if(cuenta&&cuenta!=='ninguna'){
    aplicarMovimientoCuenta(cuenta,monto,'gasto','Prestamo a: '+persona,fecha,Date.now());
  }
  document.getElementById('presteModal').remove();
  showToast('Préstamo registrado: '+fmt(monto));
}

function _abrirModalPrestamoRecibido(){
  var m=document.createElement('div');
  m.className='modal open'; m.id='prestamoRecibidoModal';
  m.innerHTML='<div class="modal-body">'
    +'<div class="modal-title">📥 Recibí un préstamo</div>'
    +'<p style="color:var(--dim);font-size:0.82rem;margin-bottom:14px;">Se registrará en <b>Créditos → Lo que debo</b></p>'
    +'<label class="inp-label">¿Quién me prestó?</label>'
    +'<input class="inp" id="prPersona" placeholder="Nombre">'
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Monto ($)</label>'
    +'<input class="inp" id="prMonto" type="number" inputmode="decimal" placeholder="0.00">'
    +'</div><div>'
    +'<label class="inp-label">Interés (%)</label>'
    +'<input class="inp" id="prInteres" type="number" inputmode="decimal" placeholder="0">'
    +'</div></div>'
    +'<label class="inp-label">Concepto</label>'
    +'<input class="inp" id="prDesc" placeholder="Ej: Para emergencia">'
    +'<div class="form-row"><div>'
    +'<label class="inp-label">Fecha</label>'
    +'<input class="inp" id="prFecha" type="date" value="'+today()+'">'
    +'</div><div>'
    +'<label class="inp-label">Vence</label>'
    +'<input class="inp" id="prVence" type="date">'
    +'</div></div>'
    +'<label class="inp-label">¿A qué cuenta entra?</label>'
    +buildCuentaOpts('prCuenta')
    +'<div style="display:flex;gap:8px;margin-top:12px;">'
    +'<button class="btn-main" style="flex:1;" onclick="_guardarPrestamoRecibido()">💾 Registrar</button>'
    +'<button class="btn-sec" onclick="document.getElementById(\'prestamoRecibidoModal\').remove()">Cancelar</button>'
    +'</div></div>';
  document.body.appendChild(m);
}

function _guardarPrestamoRecibido(){
  var persona=(document.getElementById('prPersona').value||'').trim();
  var monto=parseFloat(document.getElementById('prMonto').value||0);
  var interes=parseFloat(document.getElementById('prInteres').value||0);
  var desc=(document.getElementById('prDesc').value||'').trim();
  var fecha=document.getElementById('prFecha').value;
  var vence=document.getElementById('prVence').value;
  var cuenta=document.getElementById('prCuenta').value;
  if(!persona||!monto){ showToast('Ingresa quién y el monto'); return; }
  if(!desc) desc='Prestamo de '+persona;
  var creds=load('creditos',[]);
  creds.push({tipo:'deuda',persona:persona,descripcion:desc,monto:monto,
    interes:interes,tipoInteres:'total',fechaOrigen:fecha,fechaLimite:vence,
    estado:'pendiente',abonado:0,interesesPagados:0,historialAbonos:[]});
  save('creditos',creds);
  if(cuenta&&cuenta!=='ninguna'){
    aplicarMovimientoCuenta(cuenta,monto,'ingreso','Prestamo recibido: '+persona,fecha,Date.now());
  }
  document.getElementById('prestamoRecibidoModal').remove();
  showToast('Préstamo recibido: '+fmt(monto));
}

function _abrirModalCobrarCxC(){
  var cxcs=load('cxc',[]);
  if(!cxcs.length){ showToast('No tienes cuentas por cobrar'); return; }
  var m=document.createElement('div');
  m.className='modal open'; m.id='cobrarCxCModal';
  var lista=cxcs.map(function(c,i){
    return '<button onclick="_confirmarCobrarCxC('+i+')" style="'
      +'display:flex;align-items:center;justify-content:space-between;'
      +'padding:14px 16px;border-radius:16px;border:1.5px solid var(--border);'
      +'background:var(--card);cursor:pointer;width:100%;color:var(--txt);margin-bottom:10px;'
      +'font-family:Outfit,sans-serif;">'
      +'<div style="text-align:left;">'
      +'<div style="font-weight:800;font-size:0.9rem;">'+c.nombre+'</div>'
      +'<div style="font-size:0.72rem;color:var(--dim);">'+c.concepto+'</div></div>'
      +'<div style="font-size:0.95rem;font-weight:900;color:var(--accent);">'+fmt(c.monto)+'</div>'
      +'</button>';
  }).join('');
  m.innerHTML='<div class="modal-body">'
    +'<div class="modal-title">✅ ¿Qué cobras?</div>'
    +'<div style="max-height:280px;overflow-y:auto;margin-bottom:10px;">'+lista+'</div>'
    +'<button class="btn-sec" onclick="document.getElementById(\'cobrarCxCModal\').remove()">Cancelar</button>'
    +'</div>';
  document.body.appendChild(m);
}



// ── Validación de contraseña (6 reglas) ──────────
function validarPassword(pass){
  var errores = [];

  // 1. Longitud mínima 8 caracteres
  if(pass.length < 8){
    errores.push('Mínimo 8 caracteres');
  }

  // 2. Al menos una mayúscula
  if(!/[A-Z]/.test(pass)){
    errores.push('Al menos una mayúscula (A-Z)');
  }

  // 3. Al menos una minúscula
  if(!/[a-z]/.test(pass)){
    errores.push('Al menos una minúscula (a-z)');
  }

  // 4. Al menos un carácter especial (no letra, no número)
  if(!/[^A-Za-z0-9]/.test(pass)){
    errores.push('Al menos un carácter especial (!@#$%...)');
  }

  // 5. No números consecutivos (3+ seguidos en secuencia: 123, 234, 345...)
  var digits = pass.split('');
  for(var i = 0; i <= digits.length - 3; i++){
    var a = digits[i].charCodeAt(0);
    var b = digits[i+1].charCodeAt(0);
    var c = digits[i+2].charCodeAt(0);
    var isDigitSeq = (
      digits[i] >= '0' && digits[i] <= '9' &&
      digits[i+1] >= '0' && digits[i+1] <= '9' &&
      digits[i+2] >= '0' && digits[i+2] <= '9'
    );
    if(isDigitSeq && b === a+1 && c === b+1){
      errores.push('No se permiten números consecutivos (ej: 123, 456)');
      break;
    }
  }

  // 6. No letras consecutivas del abecedario (3+ seguidas: abc, bcd, xyz...)
  var letras = pass.toLowerCase().split('');
  for(var j = 0; j <= letras.length - 3; j++){
    var l1 = letras[j];
    var l2 = letras[j+1];
    var l3 = letras[j+2];
    var esLetra = function(ch){ return ch >= 'a' && ch <= 'z'; };
    if(esLetra(l1) && esLetra(l2) && esLetra(l3)){
      var c1 = l1.charCodeAt(0);
      var c2 = l2.charCodeAt(0);
      var c3 = l3.charCodeAt(0);
      if(c2 === c1+1 && c3 === c2+1){
        errores.push('No se permiten letras consecutivas del abecedario (ej: abc, xyz)');
        break;
      }
    }
  }

  return errores; // [] = válida, [msg1, msg2...] = inválida
}

// ── Indicador visual de fortaleza de contraseña ──
function renderPasswordStrength(pass, containerId){
  var el = document.getElementById(containerId);
  if(!el) return;

  var errores = validarPassword(pass);
  var reglas = [
    { label:'8+ caracteres',         ok: pass.length >= 8 },
    { label:'Mayúscula',             ok: /[A-Z]/.test(pass) },
    { label:'Minúscula',             ok: /[a-z]/.test(pass) },
    { label:'Carácter especial',     ok: /[^A-Za-z0-9]/.test(pass) },
    { label:'Sin números seguidos',  ok: !/(?:0(?=1)|1(?=2)|2(?=3)|3(?=4)|4(?=5)|5(?=6)|6(?=7)|7(?=8)|8(?=9)){2}/.test(pass) },
    { label:'Sin letras seguidas',   ok: !/(?:a(?=b)|b(?=c)|c(?=d)|d(?=e)|e(?=f)|f(?=g)|g(?=h)|h(?=i)|i(?=j)|j(?=k)|k(?=l)|l(?=m)|m(?=n)|n(?=o)|o(?=p)|p(?=q)|q(?=r)|r(?=s)|s(?=t)|t(?=u)|u(?=v)|v(?=w)|w(?=x)|x(?=y)|y(?=z)){2}/i.test(pass) },
  ];

  var cumplidas = reglas.filter(function(r){ return r.ok; }).length;
  var pct = Math.round((cumplidas / reglas.length) * 100);

  // Color de la barra
  var barColor = pct < 40 ? '#ff5f57' : pct < 70 ? '#ffd60a' : pct < 100 ? '#38aaff' : '#2bc070';

  var html = '<div style="margin-top:10px;">'
    + '<div style="display:flex;justify-content:space-between;margin-bottom:4px;">'
    + '<span style="font-size:0.65rem;color:rgba(255,255,255,0.4);font-weight:600;">Seguridad</span>'
    + '<span style="font-size:0.65rem;font-weight:700;color:'+barColor+';">'
    + (pct===100?'Contraseña segura ✅':pct>=70?'Casi lista':'Muy débil')
    + '</span></div>'
    + '<div style="height:4px;background:rgba(255,255,255,0.08);border-radius:4px;overflow:hidden;margin-bottom:10px;">'
    + '<div style="height:100%;width:'+pct+'%;background:'+barColor+';border-radius:4px;transition:width 0.3s ease,background 0.3s ease;"></div>'
    + '</div>'
    + '<div style="display:grid;grid-template-columns:1fr 1fr;gap:4px;">';

  reglas.forEach(function(r){
    html += '<div style="display:flex;align-items:center;gap:5px;font-size:0.65rem;color:'
      + (r.ok ? 'rgba(43,192,112,0.9)' : 'rgba(255,255,255,0.3)') + ';">'
      + '<span style="font-size:0.6rem;">' + (r.ok ? '✓' : '○') + '</span>'
      + r.label + '</div>';
  });

  html += '</div></div>';
  el.innerHTML = html;
}

// ── Mostrar errores de validación inline ──────────
function mostrarErroresPass(errores, containerId){
  var el = document.getElementById(containerId);
  if(!el) return;
  if(!errores || errores.length === 0){ el.innerHTML = ''; return; }
  var html = '<div style="background:rgba(255,95,87,0.08);border:1px solid rgba(255,95,87,0.2);border-radius:10px;padding:10px 12px;margin-top:8px;">'
    + '<div style="font-size:0.68rem;font-weight:700;color:#ff8a80;margin-bottom:6px;">La contraseña no cumple con:</div>';
  errores.forEach(function(e){
    html += '<div style="font-size:0.65rem;color:rgba(255,138,128,0.8);margin-bottom:2px;">• ' + e + '</div>';
  });
  html += '</div>';
  el.innerHTML = html;
}
// ─────────────────────────────────────────────
//  USALA Suite — Autenticación y Sesión
//  js/auth.js
// ─────────────────────────────────────────────

// ── Variables de estado ──


function arrancarApp(){
    var raw = localStorage.getItem('usala_session');
    if(raw){
      try{
        var ses = JSON.parse(raw);
        if(ses.isAdmin){
          var nipKeyA = 'usala_nip_admin';
          var nipA = localStorage.getItem(nipKeyA);
          if(nipA){
            showScreen('accessScreen');
            _sesionPendiente = ses;
            mostrarPanelConNip('Admin');
          } else {
            showScreen('accessScreen');
            document.getElementById('panelSesion').style.display = 'block';
            document.getElementById('panelCodigo').style.display  = 'none';
            document.getElementById('nipZona').style.display = 'none';
            document.getElementById('sinNipZona').style.display = 'block';
            var elNomA = document.getElementById('sesionNombre');
            if(elNomA) elNomA.textContent = 'Administrador';
            var elAvA = document.getElementById('sesionAvatar');
            if(elAvA) elAvA.textContent = '👑';
            _sesionPendiente = ses;
          }
          return;
        }
        // Sesión de usuario invitado — confiar en la sesión guardada
        // (la validación real de vencimiento ocurre en Supabase al entrar)
        showScreen('accessScreen');
        var nipKey2 = 'usala_nip_u_' + ses.codigo;
        var nip2 = localStorage.getItem(nipKey2);
        if(nip2){
          _sesionPendiente = ses;
          mostrarPanelConNip(ses.nombre ? ses.nombre.split(' ')[0] : 'Hola');
        } else {
          document.getElementById('panelSesion').style.display = 'block';
          document.getElementById('panelCodigo').style.display  = 'none';
          document.getElementById('nipZona').style.display = 'none';
          document.getElementById('sinNipZona').style.display = 'block';
          var elNom = document.getElementById('sesionNombre');
          if(elNom) elNom.textContent = ses.nombre || 'Bienvenido';
          var elAv = document.getElementById('sesionAvatar');
          if(elAv) elAv.textContent = ses.nombre ? ses.nombre.charAt(0).toUpperCase() : '👤';
          _sesionPendiente = ses;
        }
        return;
      }catch(e){ localStorage.removeItem('usala_session'); }
    }
    showScreen('accessScreen');
    document.getElementById('panelSesion').style.display = 'none';
    document.getElementById('panelCodigo').style.display  = 'block';
  }

async function verificarCodigo(){
  var codigo   = (document.getElementById('accCodigo').value||'').trim().toUpperCase();
  var errEl    = document.getElementById('accessErr');
  var btn      = document.querySelector('#panelCodigo .lg-btn');
  var nombreInp= document.getElementById('accNombre');
  var passEl   = document.getElementById('accPassword');
  var passRow  = document.getElementById('accPassRow');
  var nombreRow= document.getElementById('accNombreRow');

  function showErr(msg){
    if(errEl){ errEl.textContent=msg; errEl.style.display='block'; }
    if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
  }
  function clearErr(){
    if(errEl) errEl.style.display='none';
  }

  clearErr();
  if(!codigo){ showErr('Ingresa tu código de acceso'); return; }
  if(btn){ btn.textContent='Verificando...'; btn.disabled=true; }

  dbVerificarCodigo(codigo).then(async function(u){
    // ── CASO A: usuario encontrado en Supabase ──
    if(u){
      // Verificar si está bloqueado
      if(u.activo === false){ showErr('Tu acceso ha sido suspendido. Contacta al administrador.'); return; }

      // Verificar vencimiento
      if(u.vencimiento){
        var venc = new Date(u.vencimiento);
        if(!isNaN(venc.getTime()) && venc < new Date()){ showErr('Tu acceso ha vencido. Pide al admin que lo renueve.'); return; }
      }

      // Nombre: de Supabase o del input
      var nombre = (nombreInp ? nombreInp.value.trim() : '') || u.nombre || '';

      // Contraseña: si tiene, verificar
      if(u.password_hash && !_accPassVerificada){
        if(!passEl || !passEl.value.trim()){
          if(passRow) passRow.style.display = 'block';
          if(nombreRow) nombreRow.style.display = 'none';
          showErr('Ingresa tu contraseña');
          if(passEl) passEl.focus();
          return;
        }
        var ok = await dbVerificarPass(codigo, passEl.value);
        if(!ok){ showErr('Contraseña incorrecta'); _accPassVerificada=false; return; }
        _accPassVerificada = true;
      }

      // Contraseña nueva opcional
      if(!u.password_hash && !_saltarPass){
        var npEl = document.getElementById('accNuevaPass');
        if(npEl && npEl.value && npEl.value.length >= 1){
          // Validar contraseña con las 6 reglas
          var passErrList = validarPassword(npEl.value);
          if(passErrList.length > 0){
            var errEl2 = document.getElementById('accessErr');
            if(errEl2){
              errEl2.innerHTML = '<b style="display:block;margin-bottom:4px;">La contraseña no cumple:</b>'
                + passErrList.map(function(e){ return '• '+e; }).join('<br>');
              errEl2.style.display = 'block';
            }
            if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
            if(npEl) npEl.focus();
            return;
          }
          await dbGuardarPass(codigo, npEl.value);
          // ── Registro completado → redirigir al login ──
          _saltarPass = false; _accPassVerificada = false;
          if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
          mostrarExitoRegistro(nombre, codigo);
          return;
        }
      }

      // Nombre obligatorio si no se tiene
      if(!nombre){
        if(nombreRow) nombreRow.style.display='block';
        showErr('Escribe tu nombre para continuar');
        return;
      }

      // Actualizar registros
      _saltarPass=false; _accPassVerificada=false;
      DB.update('usala_usuarios','codigo=eq.'+encodeURIComponent(codigo),
        {nombre:nombre, ultimo_acceso:new Date().toISOString()}).catch(function(){});
      _guardarCodigoLocal(codigo, nombre, u.vencimiento||'2099-12-31');
      if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
      _entrarComoUsuario(nombre, codigo);
      return;
    }

    // ── CASO B: no está en Supabase — buscar en localStorage ──
    var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
    var cod  = cods.find(function(c){ return c.codigo===codigo && c.activo!==false; });

    if(!cod){
      showErr('Código incorrecto o no existe');
      return;
    }

    // Verificar vencimiento local
    if(cod.vencimiento && cod.vencimiento !== '3650'){
      var vencL = new Date((cod.vencimiento||'2099-12-31').replace(/-/g,'/'));
      if(vencL < new Date()){ showErr('Este código ha vencido. Pide al admin que lo renueve.'); return; }
    }

    // Nombre
    var nombreLocal = (nombreInp ? nombreInp.value.trim() : '') || cod.nombreUsuario || cod.nombre || '';
    if(!nombreLocal){
      if(nombreRow) nombreRow.style.display='block';
      showErr('Escribe tu nombre para continuar');
      return;
    }

    if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
    _entrarComoUsuario(nombreLocal, codigo);

  }).catch(function(e){
    // ── CASO C: sin conexión — usar localStorage ──
    console.warn('verificarCodigo sin conexion:', e);
    var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
    var cod  = cods.find(function(c){ return c.codigo===codigo && c.activo!==false; });
    if(cod){
      var nombre = (nombreInp ? nombreInp.value.trim() : '') || cod.nombreUsuario || cod.nombre || '';
      if(!nombre){
        if(nombreRow) nombreRow.style.display='block';
        showErr('Escribe tu nombre para continuar');
        return;
      }
      showToast('Sin conexion — entrando con datos locales');
      _entrarComoUsuario(nombre, codigo);
    } else {
      showErr('Sin conexion y codigo no encontrado localmente');
    }
  });
}

function _entrarComoUsuario(nombre, codigo){
  var btn = document.querySelector('#panelCodigo .lg-btn');
  if(btn){ btn.textContent='Entrar →'; btn.disabled=false; }
  localStorage.setItem('usala_session', JSON.stringify({nombre:nombre,codigo:codigo,isAdmin:false}));
  var nip = localStorage.getItem('usala_nip_u_'+codigo);
  if(nip){ _sesionPendiente={nombre:nombre,codigo:codigo,isAdmin:false}; mostrarPanelConNip(nombre.split(' ')[0]); }
  else   { S.user={nombre:nombre,codigo:codigo,isAdmin:false}; initDashboard(); }
}

function entrarSesionGuardada(){
  var ses = _sesionPendiente || JSON.parse(localStorage.getItem('usala_session')||'null');
  if(!ses){ mostrarPanelCodigo(); return; }
  S.user = { nombre: ses.nombre, codigo: ses.codigo, isAdmin: !!ses.isAdmin };
  localStorage.setItem('usala_session', JSON.stringify(S.user));
  _sesionPendiente = null;
  initDashboard();
}

function verificarAdmin(){
  var pass=(document.getElementById('adminPass').value||'').trim();
  var err=document.getElementById('adminErr');
  var guardada=localStorage.getItem('usala_admin_pass')||'admin1234';
  if(pass==='admin1234'||pass===guardada){
    cerrarAdminModal();
    var nip=localStorage.getItem('usala_nip_admin');
    if(nip){
      _sesionPendiente={nombre:'Administrador',codigo:'admin',isAdmin:true};
      mostrarPanelConNip('Admin');
    } else {
      S.user={nombre:'Administrador',codigo:'admin',isAdmin:true};
      localStorage.setItem('usala_session',JSON.stringify({nombre:'Administrador',codigo:'admin',isAdmin:true}));
      dbEnsureUser('admin','Administrador',true).then(function(){
        dbSyncFromLocal();
      });
      initDashboard();
    }
  } else {
    if(err){ err.textContent='Contraseña incorrecta'; err.style.display='block'; }
    var p=document.getElementById('adminPass'); if(p) p.value='';
  }
}

function verificarNip(){
  var key=nipKey();
  if(!key) return;
  var stored=localStorage.getItem(key);
  if(_nipBuffer===stored){
    var err=document.getElementById('nipErr'); if(err) err.style.display='none';
    if(_sesionPendiente.isAdmin){
      S.user={nombre:'Administrador',codigo:'ADMIN',isAdmin:true};
    } else {
      S.user={nombre:_sesionPendiente.nombre,codigo:_sesionPendiente.codigo,isAdmin:false};
    }
    localStorage.setItem('usala_session',JSON.stringify(S.user));
    _sesionPendiente=null; _nipBuffer='';
    initDashboard();
  } else {
    _nipBuffer='';
    _actualizarNipDots();
    var err=document.getElementById('nipErr');
    if(err){ err.textContent='NIP incorrecto'; err.style.display='block'; }
    var nd=document.querySelector('.nip-dots');
    if(nd){ nd.style.animation='none'; setTimeout(function(){ nd.style.animation=''; },10); }
  }
}

function mostrarPanelConNip(nombre){
  // Ocultar todos los paneles y mostrar el de sesión con NIP
  ['panelCodigo','panelSolicitud','panelEnviada'].forEach(function(id){
    var el=document.getElementById(id); if(el) el.style.display='none';
  });
  var ps=document.getElementById('panelSesion'); if(ps) ps.style.display='block';
  document.getElementById('nipZona').style.display='block';
  document.getElementById('sinNipZona').style.display='none';
  document.getElementById('nipErr').style.display='none';
  var sn=document.getElementById('sesionNombre'); if(sn) sn.textContent=nombre;
  _nipBuffer='';
  _actualizarNipDots();
}

function abrirAdminModal(){
  var m=document.getElementById('adminModal');
  if(m){ m.classList.add('open'); }
  var p=document.getElementById('adminPass'); if(p){ p.value=''; setTimeout(function(){p.focus();},100); }
  var e=document.getElementById('adminErr'); if(e) e.style.display='none';
}

function cerrarAdminModal(){
  var m=document.getElementById('adminModal');
  if(m) m.classList.remove('open');
}

function cerrarSesion(){
  usalaConfirm('Cerrar sesion?\n\nTus datos quedan guardados localmente.', function(){
    localStorage.removeItem('usala_session');
      S.user=null; S.tab='inicio';
      document.getElementById('accNombre').value='';
      document.getElementById('accCodigo').value='';
      _accMostrarNombreRow(true);  // resetear UI al estado inicial
      document.getElementById('panelSesion').style.display='none';
      document.getElementById('panelCodigo').style.display='block';
      var ub = document.getElementById('uFabBtn');
      var um = document.getElementById('uFabMenu');
      if(ub) ub.style.display='none';
      if(um) um.style.display='none';
      showScreen('accessScreen');
  });
}

function initDashboard(){
  showScreen('dashboard');
  _lockIniciarEscuchas();
  _lockReiniciar();
  dbRestaurarDatos().then(function(){
    renderTab(S.tab || 'inicio');
    setTimeout(iniciarRealtime, 1000);
    if(S.user && S.user.isAdmin){
      actualizarBadgeSolicitudes();
      setInterval(actualizarBadgeSolicitudes, 30000);
    }
  });
  var ub = document.getElementById('uFabBtn');
  if(ub) ub.style.display = 'flex';
  actualizarUMenu();
  if('webkitSpeechRecognition' in window || 'SpeechRecognition' in window){
    var bv = document.getElementById('btnVoz');
    if(bv) bv.style.display = 'flex';
  }
  var u = S.user;
  var un = document.getElementById('topUserName');
  if(un) un.textContent = u.isAdmin ? '⚙️ Admin' : '👤 ' + (u.nombre||'Usuario');
  var vb = document.getElementById('verBadge'); if(vb) vb.textContent = 'v' + APP_VERSION;
  if(u.isAdmin){
    actualizarBadgeSolicitudes();
  }
  goTab('inicio', document.querySelector('.nb'));
  setTimeout(guardarSnapshotMes, 1500); // snapshot silencioso al arrancar
  if(!u.isAdmin){
    var keyVisto = 'usala_bienvenida_' + u.codigo;
    if(!localStorage.getItem(keyVisto)){
      setTimeout(function(){
        var wn = document.getElementById('welcomeName');
        if(wn) wn.textContent = '¡Bienvenid@, ' + ((u.nombre||'').split(' ')[0]||'') + '! 👋';
        var m = document.getElementById('welcomeModal');
        var bd = document.getElementById('welcomeBackdrop');
        var sh = document.getElementById('welcomeSheet');
        if(m){
          m.style.display = 'flex';
          requestAnimationFrame(function(){
            if(bd) bd.style.background = 'rgba(0,0,0,0.55)';
            if(sh) sh.style.transform = 'translateY(0)';
          });
        }
      }, 700);
    }
  }
}

function mostrarPanelCodigo(forzar){
  ['panelSesion','panelSolicitud','panelEnviada'].forEach(function(id){
    var el=document.getElementById(id); if(el) el.style.display='none';
  });
  var pc = document.getElementById('panelCodigo');
  if(pc){ pc.style.display='block'; }
  var err = document.getElementById('accessErr');
  if(err){ err.style.display='none'; }
  if(forzar){
    localStorage.removeItem('usala_session');
    var ci = document.getElementById('accCodigo'); if(ci) ci.value='';
    var ni = document.getElementById('accNombre'); if(ni) ni.value='';
    var nr = document.getElementById('accNombreRow'); if(nr) nr.style.display='block';
    var sa = document.getElementById('accSaludo');   if(sa) sa.style.display='none';
  }
}

async function dbVerificarCodigo(codigo){
  try {
    var rows = await DB.get('usala_usuarios',
      'codigo=eq.' + encodeURIComponent(codigo) +
      '&activo=eq.true'
    );
    if(!rows || rows.length === 0) return null;
    var u = rows[0];
    if(u.is_admin) return null;
    if(u.vencimiento){
      var venc = new Date(u.vencimiento);
      if(!isNaN(venc.getTime()) && venc < new Date()) return null;
    }
    return u;
  } catch(e) { console.warn('dbVerificarCodigo:', e); return null; }
}

async function dbVerificarPass(codigo, pass){
  var hash = await _hashPass(pass);
  try {
    var rows = await DB.get('usala_usuarios',
      'codigo=eq.' + encodeURIComponent(codigo) +
      '&password_hash=eq.' + encodeURIComponent(hash));
    return rows && rows.length > 0;
  } catch(e){ return false; }
}

async function dbGuardarPass(codigo, pass){
  var hash = await _hashPass(pass);
  try {
    await DB.update('usala_usuarios', 'codigo=eq.' + encodeURIComponent(codigo), { password_hash: hash });
    return true;
  } catch(e){ return false; }
}

async function dbEnsureUser(codigo, nombre, isAdmin){
  try {
    var rows = await DB.get('usala_usuarios', 'codigo=eq.' + encodeURIComponent(codigo));
    if(rows && rows.length > 0){
      DB.update('usala_usuarios', 'codigo=eq.' + encodeURIComponent(codigo), { ultimo_acceso: new Date().toISOString() });
      return rows[0];
    }
    var res = await DB.insert('usala_usuarios', { codigo: codigo, nombre: nombre, is_admin: isAdmin, activo: true });
    return res[0];
  } catch(e) { console.warn('dbEnsureUser:', e); return null; }
}

async function dbCrearCodigo(codigo, nombre, vencimiento, contacto, nota){
  try {
    var res = await DB.insert('usala_usuarios', {
      codigo: codigo, nombre: nombre, is_admin: false,
      activo: true, vencimiento: vencimiento, contacto: contacto, nota: nota
    });
    _cacheInvalid('codigos');
    return res[0];
  } catch(e) { console.warn('dbCrearCodigo:', e); return null; }
}

async function dbActualizarSolicitud(id, estado, codigoGenerado){
  try {
    var data = { estado: estado };
    if(codigoGenerado) data.codigo_generado = codigoGenerado;
    await DB.update('usala_solicitudes', 'id=eq.'+id, data);
  } catch(e){ console.warn('dbActualizarSolicitud:', e); }
}

async function dbGetSolicitudes(){
  try {
    // Traer pendientes Y aprobadas (para poder revocar códigos al eliminar)
    var rows = await DB.get('usala_solicitudes',
      'estado=in.(pendiente,aprobada)&order=fecha.desc');
    return rows || [];
  } catch(e){
    return JSON.parse(localStorage.getItem('usala_solicitudes')||'[]')
      .filter(function(s){ return s.estado==='pendiente' || s.estado==='aprobada'; });
  }
}

function _guardarCodigoLocal(codigo, nombre, vencimiento){
  var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var ex = cods.find(function(c){ return c.codigo===codigo; });
  if(!ex){ cods.push({codigo:codigo, nombre:nombre, nombreUsuario:nombre, activo:true, vencimiento:vencimiento}); }
  else   { ex.nombreUsuario=nombre; ex.nombre=nombre; ex.activo=true; if(vencimiento) ex.vencimiento=vencimiento; }
  localStorage.setItem('usala_codigos', JSON.stringify(cods));
}

function accCodigoLookup(val){
  if(_accLookupTimer) clearTimeout(_accLookupTimer);
  val = (val||'').toUpperCase().trim();
  var passRow  = document.getElementById('accPassRow');
  var crearRow = document.getElementById('accCrearPassRow');
  var nombreRow= document.getElementById('accNombreRow');
  var errEl    = document.getElementById('accessErr');
  if(passRow)  passRow.style.display  = 'none';
  if(crearRow) crearRow.style.display = 'none';
  if(errEl)    errEl.style.display    = 'none';
  if(val.length >= 4){
    var cods = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
    var cod  = cods.find(function(c){ return c.codigo===val; });
    if(cod && cod.nombreUsuario){
      _accMostrarNombreRow(false, cod.nombreUsuario);
    }
  }
  if(!val || val.length < 4) { _accMostrarNombreRow(true); return; }
  _accLookupTimer = setTimeout(function(){
    dbVerificarCodigo(val).then(function(u){
      if(!u){
        return;
      }
      if(u.nombre) _accMostrarNombreRow(false, u.nombre);
      if(u.password_hash){
        if(passRow)  passRow.style.display  = 'block';
        if(nombreRow) nombreRow.style.display = 'none';
        var passEl = document.getElementById('accPassword');
        if(passEl) passEl.focus();
      } else {
        if(crearRow) crearRow.style.display = 'block';
        if(!u.nombre && nombreRow) nombreRow.style.display = 'block';
      }
    }).catch(function(){}); // silencioso — offline no es error
  }, 600);
}

function _accMostrarNombreRow(mostrar,nombre){
  var row    = document.getElementById('accNombreRow');
  var saludo = document.getElementById('accSaludo');
  var av     = document.getElementById('accSaludoAvatar');
  var sNom   = document.getElementById('accSaludoNombre');
  var titulo = document.getElementById('accTitulo');
  var sub    = document.getElementById('accSubtitulo');
  if(mostrar){
    if(row)    row.style.display='block';
    if(saludo) saludo.style.display='none';
    if(titulo) titulo.textContent='Ingresa tu código';
    if(sub)    sub.textContent='El administrador te lo compartió';
  } else {
    if(row)    row.style.display='none';
    if(saludo) saludo.style.display='block';
    if(av)     av.textContent=nombre.charAt(0).toUpperCase();
    if(sNom)   sNom.textContent=nombre;
    if(titulo) titulo.textContent='¡Hola, '+nombre.split(' ')[0]+'!';
    if(sub)    sub.textContent='Confirma tu código para continuar';
  }
}

function saltarCrearPass(){
  _saltarPass = true;
  var crearRow = document.getElementById('accCrearPassRow');
  if(crearRow) crearRow.style.display = 'none';
  verificarCodigo();
}

function toggleAccPass(){
  var inp = document.getElementById('accPassword');
  if(!inp) return;
  inp.type = inp.type === 'password' ? 'text' : 'password';
}

function toggleAccNuevaPass(){
  var inp = document.getElementById('accNuevaPass');
  if(!inp) return;
  inp.type = inp.type === 'password' ? 'text' : 'password';
}

function abrirConfigNip(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  var isAdmin = S.user && S.user.isAdmin;
  var nipKey  = isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+(S.user&&S.user.codigo);
  var tiene   = !!localStorage.getItem(nipKey);
  var modal   = document.createElement('div');
  modal.id    = 'nipConfigModal';
  modal.style.cssText = 'position:fixed;inset:0;z-index:9300;background:rgba(0,0,0,0.55);display:flex;align-items:flex-end;';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 40px;width:100%;max-width:480px;margin:0 auto;">'
    +'<div style="font-weight:900;font-size:1rem;margin-bottom:4px;">🔒 NIP de seguridad</div>'
    +'<div style="font-size:0.78rem;color:var(--dim);margin-bottom:18px;">'+(tiene?'Ya tienes un NIP configurado':'Protege tu acceso con un NIP de 4 dígitos')+'</div>'
    +(tiene
      ? '<button onclick="_nipCambiar()" class="btn-main" style="margin-bottom:8px;">🔄 Cambiar NIP</button>'
        +'<button onclick="_nipEliminar()" style="width:100%;padding:12px;background:rgba(255,95,87,0.08);border:1px solid rgba(255,95,87,0.2);border-radius:14px;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--danger);cursor:pointer;margin-bottom:8px;">🗑 Eliminar NIP</button>'
      : '<button onclick="_nipCrear()" class="btn-main" style="margin-bottom:8px;">✅ Crear NIP</button>')
    +'<button onclick="_cerrarNipModal()" style="width:100%;padding:12px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    +'</div>';
  document.body.appendChild(modal);
}

function _nipCrear(){
  var modal=document.getElementById('nipConfigModal'); if(modal) modal.remove();
  usalaPrompt('Elige tu NIP (4 digitos):', '', function(nip1){
    if(!nip1||nip1.length!==4||!(/^[0-9]{4}$/.test(nip1))){ showToast('El NIP debe ser 4 digitos'); return; }
    usalaPrompt('Confirma tu NIP:', '', function(nip2){
      if(nip1!==nip2){ showToast('Los NIPs no coinciden'); return; }
      var k=S.user&&S.user.isAdmin?'usala_nip_admin':'usala_nip_u_'+(S.user&&S.user.codigo);
      localStorage.setItem(k, nip1);
      showToast('NIP configurado');
      goSub('config');
    },{type:'tel',placeholder:'4 digitos'});
  },{type:'tel',placeholder:'4 digitos'});
}

function _nipCambiar(){
  var m=document.getElementById('nipConfigModal'); if(m) m.remove();
  var isAdmin=S.user&&S.user.isAdmin;
  var nipKey  = isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+(S.user&&S.user.codigo);
  usalaPrompt('Ingresa tu NIP actual:', '', function(actual){
    if(actual!==localStorage.getItem(nipKey)){ showToast('NIP incorrecto'); return; }
    usalaPrompt('Nuevo NIP (4 digitos):', '', function(nuevo){
      if(!nuevo||nuevo.length!==4||!(/^[0-9]{4}$/.test(nuevo))){ showToast('NIP debe ser 4 digitos'); return; }
      localStorage.setItem(nipKey, nuevo);
      showToast('NIP actualizado');
      goSub('config');
    },{type:'tel',placeholder:'4 digitos'});
  },{type:'tel',placeholder:'4 digitos'});
}

function _nipEliminar(){
  usalaConfirm('Eliminar tu NIP? Podras entrar sin NIP.', function(){
    var isAdmin = S.user && S.user.isAdmin;
      var nipKey  = isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+(S.user&&S.user.codigo);
      localStorage.removeItem(nipKey);
      showToast('NIP eliminado');
      goSub('config');
  });
}

function _cerrarNipModal(){ var m=document.getElementById("nipConfigModal"); if(m) m.remove(); }

async function renderCodigos(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  mc.innerHTML = '<div class="page-header">'+backSubBtn()+'<div class="page-title">👥 Códigos & Solicitudes</div></div>'
    + '<div style="text-align:center;padding:40px;color:var(--dim);font-size:0.85rem;">Cargando...</div>';
  var solicitudes = await dbGetSolicitudes();
  var pendientes  = solicitudes.filter(function(s){ return s.estado==='pendiente'; });
  var codigos = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  var hoy = new Date(); hoy.setHours(0,0,0,0);
  var solBlock = '';
  if(pendientes.length){
    var solItems = pendientes.map(function(s){
      return '<div style="border:1.5px solid rgba(255,179,64,0.4);border-radius:14px;padding:12px 14px;margin-bottom:8px;background:rgba(255,179,64,0.07);">'
        +'<div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:6px;">'
        +'<div>'
        +'<div style="font-weight:800;font-size:0.88rem;">'+s.nombre+'</div>'
        +'<div style="font-size:0.7rem;color:var(--dim);">'+s.contacto+' · '+s.fecha+'</div>'
        +(s.motivo?'<div style="font-size:0.75rem;color:var(--dim);margin-top:3px;">'+s.motivo+'</div>':'')
        +'</div>'
        +'<span style="font-size:0.65rem;background:#ffb340;color:#fff;border-radius:8px;padding:3px 8px;font-weight:700;">PENDIENTE</span>'
        +'</div>'
        +'<div style="display:flex;gap:6px;">'
        +'<button data-sol-id="'+s.id+'" data-sol-nombre="'+encodeURIComponent(s.nombre)+'" onclick="aprobarSolicitudDB(this.dataset.solId, decodeURIComponent(this.dataset.solNombre))" style="flex:1;background:var(--accent);border:none;border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.78rem;font-weight:700;color:#fff;cursor:pointer;">✅ Aprobar</button>'
        +'<button data-sol-id="'+s.id+'" onclick="rechazarSolicitudDB(this.dataset.solId)" style="background:rgba(255,179,64,0.12);border:1px solid rgba(255,179,64,0.3);border-radius:10px;padding:8px 10px;font-family:Outfit,sans-serif;font-size:0.75rem;color:#c07a10;cursor:pointer;">✕ Rechazar</button>'
        +'<button data-sol-id="'+s.id+'" data-sol-codigo="'+(s.codigo_generado||'')+'" onclick="eliminarSolicitudDB(this.dataset.solId, this.dataset.solCodigo)" style="background:rgba(255,95,87,0.1);border:1px solid rgba(255,95,87,0.25);border-radius:10px;padding:8px 10px;font-family:Outfit,sans-serif;font-size:0.75rem;color:var(--danger);cursor:pointer;">🗑</button>'
        +'</div>'
        +'</div>';
    }).join('');
    solBlock = '<div style="background:rgba(255,179,64,0.06);border:1px solid rgba(255,179,64,0.2);border-radius:18px;padding:14px 16px;margin-bottom:14px;">'
      +'<div style="font-size:0.72rem;font-weight:800;color:#c07a10;margin-bottom:10px;">📩 SOLICITUDES PENDIENTES ('+pendientes.length+')</div>'
      +solItems+'</div>';
  }
  var codsHtml = codigos.length ? codigos.slice().reverse().map(function(c){
    var venc = new Date((c.vencimiento||'2099-12-31').split('-').join('/'));
    var vencida = venc < hoy;
    var color = vencida ? '#ff6057' : (c.usado ? 'var(--accent2)' : 'var(--accent)');
    var badge  = vencida ? 'Vencido' : (c.usado ? 'En uso' : 'Disponible');
    return '<div style="display:flex;align-items:center;justify-content:space-between;padding:12px 14px;border-radius:14px;background:var(--inp);margin-bottom:8px;">'
      +'<div>'
      +'<div style="font-weight:800;font-size:0.88rem;color:var(--text);">'+c.codigo+'</div>'
      +'<div style="font-size:0.68rem;color:var(--dim);">'+(c.nota||c.nombreUsuario||'—')+' · Vence: '+c.vencimiento+'</div>'
      +'</div>'
      +'<div style="display:flex;align-items:center;gap:8px;">'
      +'<span style="font-size:0.65rem;background:'+color+';color:#fff;border-radius:8px;padding:3px 8px;font-weight:700;">'+badge+'</span>'
      +'<button data-codigo="'+c.codigo+'" onclick="copiarCodigo(this.dataset.codigo)" style="background:none;border:none;font-size:1rem;cursor:pointer;" title="Copiar">📋</button>'
      +'</div>'
      +'</div>';
  }).join('') : '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.82rem;">Sin códigos creados aún</div>';
  mc.innerHTML = '<div class="page-header">'+backSubBtn()+'<div class="page-title">👥 Códigos & Solicitudes</div></div>'
    + solBlock
    + '<div class="sec-title">🔑 Crear nuevo código</div>'
    + '<div class="card" style="margin-bottom:14px;padding:14px 16px;">'
    + '<input class="inp" id="codPrefijo" placeholder="Prefijo (ej: MARI)" style="margin-bottom:8px;" autocapitalize="characters">'
    + '<input class="inp" id="codNota" placeholder="Nombre del usuario *" style="margin-bottom:8px;">'
    + '<input class="inp" id="codContacto" placeholder="WhatsApp o email" style="margin-bottom:8px;">'
    + '<select class="inp" id="codVence" style="margin-bottom:12px;">'
    + '<option value="30">30 días</option><option value="90">90 días</option>'
    + '<option value="180">6 meses</option><option value="365">1 año</option>'
    + '<option value="3650">Sin vencimiento</option>'
    + '</select>'
    + '<button class="btn-main" onclick="generarCodigo()">🔑 Generar código</button>'
    + '</div>'
    + '<div class="sec-title">📋 Códigos existentes</div>'
    + codsHtml;
}

function aprobarSolicitudDB(solId, nombre){
  var prefijo = nombre.split(' ')[0].toUpperCase().slice(0,4).replace(/[^A-Z]/g,'') || 'FIN';
  var modal = document.createElement('div');
  modal.id = 'modalAprobSol';
  modal.style.cssText = 'position:fixed;inset:0;z-index:9200;background:rgba(0,0,0,0.55);display:flex;align-items:flex-end;';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 40px;width:100%;max-width:480px;margin:0 auto;">'
    +'<div style="font-size:1rem;font-weight:900;margin-bottom:4px;">✅ Aprobar solicitud</div>'
    +'<div style="font-size:0.8rem;color:var(--dim);margin-bottom:18px;">👤 '+nombre+'</div>'
    +'<label class="inp-label">Prefijo del código</label>'
    +'<input class="inp" id="_asPrefijo" value="'+prefijo+'" maxlength="5" style="text-transform:uppercase;margin-bottom:10px;">'
    +'<label class="inp-label">Vigencia del acceso</label>'
    +'<select class="inp" id="_asVence" style="margin-bottom:16px;">'
    +'<option value="8">8 días</option>'
    +'<option value="15">15 días</option>'
    +'<option value="30" selected>1 mes</option>'
    +'<option value="90">3 meses</option>'
    +'<option value="180">6 meses</option>'
    +'<option value="365">1 año</option>'
    +'<option value="3650">Sin vencimiento</option>'
    +'</select>'
    +'<button class="btn-main" id="_btnConfAprobSol">🔑 Generar código</button>'
    +'<button onclick="document.getElementById(\'modalAprobSol\').remove()" style="width:100%;margin-top:8px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    +'</div>';
  document.body.appendChild(modal);
  // Asignar handler al botón DESPUÉS de insertar en DOM
  var _sid = solId, _snm = nombre;
  document.getElementById('_btnConfAprobSol').onclick = function(){
    _confirmarAprobSol(_sid, encodeURIComponent(_snm));
  };
}

async function _confirmarAprobSol(solId, nombreEnc){
  var nombre  = decodeURIComponent(nombreEnc);
  var prefijo = (document.getElementById('_asPrefijo').value.trim().toUpperCase()||'FIN').slice(0,5);
  var dias    = parseInt(document.getElementById('_asVence').value)||30;
  var codigo  = _generarCodigoUnico(prefijo);
  var venc    = new Date(); venc.setDate(venc.getDate()+dias);
  var vencStr = venc.toISOString().split('T')[0];
  var modal = document.getElementById('modalAprobSol'); if(modal) modal.remove();
  var codigos = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
  codigos.push({codigo:codigo, vencimiento:vencStr, nota:nombre, activo:true, usado:false, creado:today(), nombreUsuario:nombre});
  localStorage.setItem('usala_codigos', JSON.stringify(codigos));
  await dbCrearCodigo(codigo, nombre, vencStr+'T23:59:59Z', '', nombre);
  await dbActualizarSolicitud(solId, 'aprobada', codigo);
  navigator.clipboard.writeText(codigo).catch(function(){});
  showToast('✅ Código '+codigo+' ('+dias+' días) copiado — compártelo con '+nombre);
  renderCodigos();
}

async function rechazarSolicitudDB(solId){
  usalaConfirm('¿Rechazar esta solicitud?', async function(){
    await dbActualizarSolicitud(solId, 'rechazada', null);
      showToast('✕ Solicitud rechazada');
      renderCodigos();
  });
}

async function eliminarSolicitudDB(solId, codigoGenerado){
  var tieneCode = codigoGenerado && codigoGenerado.trim() !== '';
    var msg = tieneCode
      ? ('Eliminar esta solicitud y REVOCAR el codigo ' + codigoGenerado + '? El usuario perdera el acceso.')
      : 'Eliminar permanentemente esta solicitud?';
  usalaConfirm(msg, async function(){
    
  });
}


function recuperarAdmin(){
  usalaConfirm('Restablecer la contrasena de administrador?\nSolo hazlo si olvidaste la contrasena.', function(){
    localStorage.removeItem('usala_admin_pass');
      showToast('✓ Contraseña restablecida — usa admin1234');
      cerrarAdminModal();
  });
}

function limpiarTodasSolicitudes(){
  usalaConfirm('Borrar TODAS las solicitudes?', function(){
    localStorage.removeItem('usala_solicitudes');
      showToast('✓ Solicitudes borradas');
      goSub('codigos');
  });
}

function abrirConfigAutolock(){
  var mc = document.getElementById('mainContent');
  mc.innerHTML = '';
  var actual = getLockTimeout();
  var d = document.createElement('div');
  d.style.padding = '20px 16px';
  d.innerHTML =
    '<div class="page-header">'+backSubBtn()+'<div class="page-title">⏱ Bloqueo automático</div></div>'
    +'<div style="font-size:0.8rem;color:var(--dim);margin-bottom:20px;line-height:1.5;">'
      +'Bloquea la app automáticamente si no la usas durante el tiempo elegido. '
      +'Al bloquearse pedirá tu NIP para volver a entrar.'
    +'</div>';
  var lista = document.createElement('div');
  lista.className = 'card';
  lista.style.padding = '4px 0';
  LOCK_OPCIONES.forEach(function(op){
    var row = document.createElement('div');
    row.style.cssText = 'display:flex;justify-content:space-between;align-items:center;padding:14px 18px;cursor:pointer;border-bottom:1px solid var(--border);transition:background 0.1s;';
    row.innerHTML =
      '<div style="font-weight:600;font-size:0.9rem;">'+(op.val===0?'🔓 ':'⏱ ')+op.label+'</div>'
      +'<div id="lockOpt_'+op.val+'" style="font-size:1.1rem;">'+(op.val===actual?'✅':'')+'</div>';
    row.onmouseenter = function(){ this.style.background='var(--inp)'; };
    row.onmouseleave = function(){ this.style.background=''; };
    (function(v, lbl){
      row.onclick = function(){
        setLockTimeout(v);
        LOCK_OPCIONES.forEach(function(o){
          var el=document.getElementById('lockOpt_'+o.val);
          if(el) el.textContent = (o.val===v?'✅':'');
        });
        var sub = document.getElementById('autolockSubLabel');
        if(sub) sub.textContent = lbl;
      };
    })(op.val, op.label);
    lista.appendChild(row);
  });
  lista.lastChild.style.borderBottom = 'none';
  var nipK = S.user && S.user.isAdmin ? 'usala_nip_admin' : 'usala_nip_u_'+(S.user&&S.user.codigo);
  var tieneNip = !!localStorage.getItem(nipK);
  var nota = document.createElement('div');
  nota.style.cssText = 'font-size:0.74rem;margin-top:12px;padding:10px 14px;border-radius:12px;'
    +(tieneNip
      ? 'background:rgba(45,158,95,0.08);color:var(--accent2);border:1px solid rgba(45,158,95,0.2);'
      : 'background:rgba(245,124,0,0.08);color:#f57c00;border:1px solid rgba(245,124,0,0.2);');
  nota.innerHTML = tieneNip
    ? '🔒 Tienes NIP activo — se pedirá al desbloquear'
    : '⚠️ No tienes NIP configurado. Al bloquearse solo habrá un botón de desbloquear. <b>Configura tu NIP para mayor seguridad.</b>';
  d.appendChild(lista);
  d.appendChild(nota);
  mc.appendChild(d);
  S.subtab = 'config';
}

async function renderAdminPanel(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  var tab = _adminPanelTab;
  var tabs = ['resumen','usuarios','config_app'].map(function(t){
    var labels = {resumen:'📊 Resumen', usuarios:'👥 Usuarios', config_app:'⚙️ Config'};
    var act = tab === t;
    return '<button onclick="_adminTab(\''+t+'\')" style="flex:1;padding:9px 4px;border-radius:12px;border:none;'
      +'font-family:Outfit,sans-serif;font-size:0.7rem;font-weight:700;cursor:pointer;transition:all 0.18s;'
      +'background:'+(act?'var(--accent)':'var(--inp)')+';color:'+(act?'#fff':'var(--dim)')+';">'+labels[t]+'</button>';
  }).join('');
  var tabBar = '<div style="display:flex;gap:6px;margin-bottom:16px;">'+tabs+'</div>';
  mc.innerHTML = '<div class="page-header">'+backSubBtn()
    +'<div class="page-title">🛡️ Panel Admin</div>'
    +'<button onclick="renderAdminPanel()" style="background:var(--inp);border:1px solid var(--border);'
    +'border-radius:10px;padding:6px 10px;font-size:0.75rem;color:var(--text);cursor:pointer;">🔄</button>'
    +'</div>'
    + tabBar
    + '<div id="adminPanelBody"><div style="text-align:center;padding:40px;color:var(--dim);">Cargando...</div></div>';
  if(tab === 'resumen')    await _adminRenderResumen();
  else if(tab === 'usuarios') await _adminRenderUsuarios();
  else if(tab === 'config_app') _adminRenderConfig();
}

async function _adminRenderResumen(){
  var body = document.getElementById('adminPanelBody');
  if(!body) return;
  var usuarios = [];
  try { usuarios = await DB.get('usala_usuarios','is_admin=eq.false&activo=eq.true&order=creado_en.desc'); }
  catch(e){ usuarios = []; }
  var totalIng = 0, totalGas = 0, totalTxs = 0, activos = 0;
  var usuariosData = [];
  for(var i=0; i<(usuarios||[]).length; i++){
    var u = usuarios[i];
    try {
      var kvRows = await DB.get('usala_kv',
        'user_id=eq.'+encodeURIComponent(u.codigo)+'&key=in.(txs,cuentas)');
      var txsRow = (kvRows||[]).find(function(r){ return r.key==='txs'; });
      var txs = txsRow ? JSON.parse(txsRow.value||'[]') : [];
      var ing = txs.filter(function(t){ return t.tipo==='ingreso'; }).reduce(function(s,t){ return s+Number(t.monto||0); },0);
      var gas = txs.filter(function(t){ return t.tipo==='gasto'; }).reduce(function(s,t){ return s+Number(t.monto||0); },0);
      totalIng += ing; totalGas += gas; totalTxs += txs.length;
      if(txs.length > 0) activos++;
      usuariosData.push({ u:u, ing:ing, gas:gas, txs:txs.length });
    } catch(e){ usuariosData.push({ u:u, ing:0, gas:0, txs:0 }); }
  }
  var totalUsuarios = (usuarios||[]).length;
  var solPend = 0;
  try {
    var sols = await DB.get('usala_solicitudes','estado=eq.pendiente');
    solPend = (sols||[]).length;
  } catch(e){}
  // Actividad reciente (últimas txs de todos)
  var hoy = today();
  var txsHoy = usuariosData.reduce(function(s,d){
    return s + d.txs; // simplificado — en futuro filtrar por fecha
  }, 0);
  var html = '';
  html += '<div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:14px;">';
  html += _adminMetric('👥 Usuarios', totalUsuarios, 'total registrados', 'var(--accent)');
  html += _adminMetric('🟢 Activos', activos, 'con transacciones', '#2d9e5f');
  html += _adminMetric('💰 Ingresos', fmt(totalIng), 'suma global', 'var(--accent2)');
  html += _adminMetric('💸 Gastos', fmt(totalGas), 'suma global', 'var(--danger)');
  html += '</div>';
  html += '<div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:14px;">';
  html += _adminMetric('🔄 Transacciones', totalTxs, 'movimientos totales', '#7c6fff');
  html += _adminMetric('📩 Solicitudes', solPend, 'esperando aprobación', solPend>0?'#ffb340':'var(--dim)');
  html += '</div>';
  var balance = totalIng - totalGas;
  html += '<div class="card" style="margin-bottom:14px;padding:14px 16px;background:linear-gradient(135deg,rgba(43,192,112,0.1),rgba(43,192,112,0.04));border:1px solid rgba(43,192,112,0.2);">'
    +'<div style="font-size:0.68rem;color:var(--dim);font-weight:700;">FLUJO NETO GLOBAL (todos los usuarios)</div>'
    +'<div style="font-size:1.5rem;font-weight:900;color:'+(balance>=0?'var(--accent)':'var(--danger)')+';">'
    +(balance>=0?'+':'')+fmt(balance)+'</div></div>';
  var topUsers = usuariosData.sort(function(a,b){ return b.txs-a.txs; }).slice(0,5);
  if(topUsers.length > 0){
    html += '<div style="font-size:0.72rem;font-weight:800;color:var(--dim);margin-bottom:8px;">🏆 USUARIOS MÁS ACTIVOS</div>';
    html += '<div class="card" style="padding:8px 14px;">';
    topUsers.forEach(function(d,i){
      var pct = totalTxs > 0 ? Math.round(d.txs/totalTxs*100) : 0;
      html += '<div style="display:flex;align-items:center;gap:10px;padding:8px 0;'+(i<topUsers.length-1?'border-bottom:1px solid var(--border);':'') +'">'
        +'<div style="width:28px;height:28px;border-radius:50%;background:var(--accent);display:flex;align-items:center;justify-content:center;font-size:0.75rem;font-weight:800;color:#fff;flex-shrink:0;">'+(d.u.nombre||'?').charAt(0).toUpperCase()+'</div>'
        +'<div style="flex:1;min-width:0;">'
        +'<div style="font-size:0.82rem;font-weight:700;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;">'+(d.u.nombre||d.u.codigo)+'</div>'
        +'<div style="font-size:0.65rem;color:var(--dim);">'+d.txs+' transacciones · '+pct+'% del total</div>'
        +'</div>'
        +'<div style="font-size:0.8rem;font-weight:800;color:var(--accent2);">'+fmt(d.ing)+'</div>'
        +'</div>';
    });
    html += '</div>';
  }
  body.innerHTML = html;
}

async function _adminRenderUsuarios(){
  var body = document.getElementById('adminPanelBody');
  if(!body) return;
  body.innerHTML = '<div style="text-align:center;padding:30px;color:var(--dim);">Cargando usuarios...</div>';
  var usuarios = [];
  try { usuarios = await DB.get('usala_usuarios','is_admin=eq.false&order=creado_en.desc'); }
  catch(e){ body.innerHTML = '<div class="card" style="text-align:center;padding:30px;color:var(--danger);">Error al cargar usuarios</div>'; return; }
  var hoy = new Date(); hoy.setHours(0,0,0,0);
  var buscador = '<input class="inp" id="adminBuscarUser" placeholder="🔍 Buscar usuario..." '
    +'oninput="_adminFiltrarUsers(this.value)" style="margin-bottom:12px;">';
  var lista = '<div id="adminUserLista">';
  (usuarios||[]).forEach(function(u, i){
    var venc   = u.vencimiento ? new Date(u.vencimiento) : null;
    var vencida = venc && venc < hoy;
    var bloq   = !u.activo;
    var estado = bloq ? '🔴 Bloqueado' : vencida ? '🟡 Vencido' : '🟢 Activo';
    var colorE = bloq ? 'var(--danger)' : vencida ? '#ffb340' : 'var(--accent)';
    lista += '<div class="card" style="margin-bottom:8px;padding:14px 16px;" data-user-nombre="'+(u.nombre||'').toLowerCase()+'" data-user-cod="'+(u.codigo||'').toLowerCase()+'">'
      +'<div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">'
      +'<div style="width:36px;height:36px;border-radius:50%;background:var(--accent);display:flex;align-items:center;justify-content:center;font-weight:900;font-size:1rem;color:#fff;flex-shrink:0;">'+(u.nombre||'?').charAt(0).toUpperCase()+'</div>'
      +'<div style="flex:1;min-width:0;">'
      +'<div style="font-weight:800;font-size:0.9rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;">'+(u.nombre||'Sin nombre')+'</div>'
      +'<div style="font-size:0.68rem;color:var(--dim);">'+u.codigo+(u.contacto?' · '+u.contacto:'')+'</div>'
      +'<div style="font-size:0.65rem;color:var(--dim);">Vence: '+(u.vencimiento||'Sin vencimiento')+(u.password_hash?' · 🔐':'')+'</div>'
      +'</div>'
      +'<span style="font-size:0.65rem;font-weight:700;color:'+colorE+';">'+estado+'</span>'
      +'</div>'
      +'<div style="display:grid;grid-template-columns:1fr 1fr;gap:6px;">'
      +'<button data-uid="'+u.codigo+'" data-unombre="'+encodeURIComponent(u.nombre||'')+'" data-uvenc="'+(u.vencimiento||'')+'" onclick="_adminEditarUser(this.dataset.uid, decodeURIComponent(this.dataset.unombre), this.dataset.uvenc)" '
      +'style="background:var(--inp);border:1px solid var(--border);border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.75rem;cursor:pointer;">✏️ Editar</button>'
      +(bloq
        ? '<button data-uid="'+u.codigo+'" onclick="_adminDesbloquear(this.dataset.uid)" style="background:rgba(43,192,112,0.1);border:1px solid rgba(43,192,112,0.3);border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.75rem;color:var(--accent);cursor:pointer;">🔓 Desbloquear</button>'
        : '<button data-uid="'+u.codigo+'" onclick="_adminBloquear(this.dataset.uid)" style="background:rgba(255,95,87,0.08);border:1px solid rgba(255,95,87,0.2);border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.75rem;color:var(--danger);cursor:pointer;">🔒 Bloquear</button>')
      +'<button data-uid="'+u.codigo+'" onclick="_adminResetNip(this.dataset.uid)" style="background:var(--inp);border:1px solid var(--border);border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.75rem;cursor:pointer;">🔑 Reset NIP</button>'
      +'<button data-uid="'+u.codigo+'" data-unombre="'+encodeURIComponent(u.nombre||'')+'" onclick="_adminEliminarUser(this.dataset.uid, decodeURIComponent(this.dataset.unombre))" style="background:rgba(255,95,87,0.08);border:1px solid rgba(255,95,87,0.2);border-radius:10px;padding:8px;font-family:Outfit,sans-serif;font-size:0.75rem;color:var(--danger);cursor:pointer;">🗑 Eliminar</button>'
      +'</div>'
      +'</div>';
  });
  lista += '</div>';
  if(!usuarios || usuarios.length === 0){
    lista = '<div class="card" style="text-align:center;padding:30px;color:var(--dim);">Sin usuarios registrados</div>';
  }
  body.innerHTML = buscador + lista;
}

function _adminRenderConfig(){
  var body = document.getElementById('adminPanelBody');
  if(!body) return;
  var cfgGlobal = JSON.parse(localStorage.getItem('usala_cfg_global')||'{}');
  body.innerHTML = ''
    +'<div style="font-size:0.72rem;font-weight:800;color:var(--dim);margin-bottom:8px;">⚙️ CONFIGURACIÓN GLOBAL</div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<div class="set-item" onclick="_adminCfgNombreApp()">'
    +'<div><div class="set-label">📛 Nombre de la app</div>'
    +'<div class="set-sub">'+(cfgGlobal.nombreApp||'USALA Finanzas')+'</div></div>'
    +'<div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="_adminCfgBienvenida()">'
    +'<div><div class="set-label">👋 Mensaje de bienvenida</div>'
    +'<div class="set-sub">'+(cfgGlobal.msgBienvenida||'Configura aquí')+'</div></div>'
    +'<div class="set-arrow">›</div></div>'
    +'<div class="set-item">'
    +'<div><div class="set-label">🔑 Registro abierto</div>'
    +'<div class="set-sub">Permitir solicitudes de nuevos usuarios</div></div>'
    +'<label style="position:relative;display:inline-block;width:42px;height:24px;flex-shrink:0;">'
    +'<input type="checkbox" id="cfgRegistroAbierto" '+(cfgGlobal.registroAbierto!==false?'checked':'')+' '
    +'onchange="_adminToggleCfg(\'registroAbierto\',this.checked)" style="opacity:0;width:0;height:0;">'
    +'<span onclick="this.previousElementSibling.click()" style="position:absolute;cursor:pointer;inset:0;background:'+(cfgGlobal.registroAbierto!==false?'var(--accent)':'#ccc')+';border-radius:24px;transition:0.2s;">'
    +'<span style="position:absolute;height:18px;width:18px;left:'+(cfgGlobal.registroAbierto!==false?'21px':'3px')+';bottom:3px;background:white;border-radius:50%;transition:0.2s;"></span></span>'
    +'</label></div>'
    +'<div class="set-item">'
    +'<div><div class="set-label">📊 Vigencia predeterminada</div>'
    +'<div class="set-sub">Al crear códigos nuevos</div></div>'
    +'<select class="inp" style="width:120px;" onchange="_adminToggleCfg(\'vigenciaDefault\',this.value)">'
    +['8','15','30','90','180','365','3650'].map(function(d){
        var labels={8:'8 días',15:'15 días',30:'1 mes',90:'3 meses',180:'6 meses',365:'1 año',3650:'Sin límite'};
        return '<option value="'+d+'"'+(String(cfgGlobal.vigenciaDefault||30)===d?' selected':'')+'>'+labels[d]+'</option>';
      }).join('')
    +'</select></div>'
    +'</div>'
    +'<div style="font-size:0.72rem;font-weight:800;color:var(--dim);margin:14px 0 8px;">🏷️ CATEGORÍAS DE GASTOS</div>'
    +'<div class="card" style="margin-bottom:14px;padding:14px 16px;">'
    +_adminListaCats('gasto')
    +'<button onclick="_adminNuevaCat(\'gasto\')" style="width:100%;margin-top:10px;padding:10px;background:var(--inp);border:1px dashed var(--border);border-radius:12px;font-family:Outfit,sans-serif;font-size:0.8rem;color:var(--dim);cursor:pointer;">+ Nueva categoría de gasto</button>'
    +'</div>'
    +'<div style="font-size:0.72rem;font-weight:800;color:var(--dim);margin-bottom:8px;">💰 CATEGORÍAS DE INGRESOS</div>'
    +'<div class="card" style="margin-bottom:14px;padding:14px 16px;">'
    +_adminListaCats('ingreso')
    +'<button onclick="_adminNuevaCat(\'ingreso\')" style="width:100%;margin-top:10px;padding:10px;background:var(--inp);border:1px dashed var(--border);border-radius:12px;font-family:Outfit,sans-serif;font-size:0.8rem;color:var(--dim);cursor:pointer;">+ Nueva categoría de ingreso</button>'
    +'</div>'
    +'<div style="font-size:0.72rem;font-weight:800;color:var(--danger);margin-bottom:8px;">⚠️ ZONA DE RIESGO</div>'
    +'<div class="card" style="border:1px solid rgba(255,95,87,0.2);padding:14px 16px;">'
    +'<div class="set-item" onclick="_adminCambiarPass()">'
    +'<div><div class="set-label" style="color:var(--danger);">🔐 Cambiar contraseña admin</div>'
    +'<div class="set-sub">Modifica la clave de administrador</div></div>'
    +'<div class="set-arrow">›</div></div>'
    +'</div>';
}

function _adminMetric(titulo, valor, sub, color){
  return '<div class="card" style="padding:14px;text-align:center;">'
    +'<div style="font-size:0.65rem;color:var(--dim);font-weight:700;margin-bottom:4px;">'+titulo+'</div>'
    +'<div style="font-size:1.3rem;font-weight:900;color:'+(color||'var(--text)')+';">'+valor+'</div>'
    +'<div style="font-size:0.62rem;color:var(--dim);margin-top:2px;">'+sub+'</div>'
    +'</div>';
}

function _adminFiltrarUsers(q){
  var cards = document.querySelectorAll('#adminUserLista .card');
  cards.forEach(function(c){
    var nombre = c.getAttribute('data-user-nombre')||'';
    var cod    = c.getAttribute('data-user-cod')||'';
    c.style.display = (nombre+cod).indexOf(q.toLowerCase()) > -1 ? '' : 'none';
  });
}

function _adminEditarUser(uid, nombre, vencActual){
  var modal = document.createElement('div');
  modal.id  = 'modalEditUser';
  modal.style.cssText = 'position:fixed;inset:0;z-index:9200;background:rgba(0,0,0,0.55);display:flex;align-items:flex-end;';
  modal.innerHTML = '<div style="background:var(--bg);border-radius:24px 24px 0 0;padding:24px 20px 40px;width:100%;max-width:480px;margin:0 auto;">'
    +'<div style="font-size:1rem;font-weight:900;margin-bottom:16px;">✏️ Editar usuario</div>'
    +'<label class="inp-label">Nombre</label>'
    +'<input class="inp" id="_euNombre" value="'+nombre+'" style="margin-bottom:10px;">'
    +'<label class="inp-label">Nuevo vencimiento</label>'
    +'<select class="inp" id="_euVence" style="margin-bottom:10px;">'
    +'<option value="">— Mantener actual ('+(vencActual||'sin límite')+') —</option>'
    +'<option value="8">+8 días desde hoy</option>'
    +'<option value="15">+15 días desde hoy</option>'
    +'<option value="30">+1 mes desde hoy</option>'
    +'<option value="90">+3 meses desde hoy</option>'
    +'<option value="180">+6 meses desde hoy</option>'
    +'<option value="365">+1 año desde hoy</option>'
    +'<option value="3650">Sin vencimiento</option>'
    +'</select>'
    +'<label class="inp-label">Resetear contraseña</label>'
    +'<div style="display:flex;align-items:center;gap:8px;margin-bottom:16px;">'
    +'<input type="checkbox" id="_euResetPass" style="width:18px;height:18px;">'
    +'<label for="_euResetPass" style="font-size:0.82rem;cursor:pointer;">Eliminar contraseña (usuario deberá crear una nueva)</label>'
    +'</div>'
    +'<button class="btn-main" onclick="_adminGuardarUser(\''+uid+'\')">💾 Guardar cambios</button>'
    +'<button onclick="document.getElementById(\'modalEditUser\').remove()" style="width:100%;margin-top:8px;background:none;border:none;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">Cancelar</button>'
    +'</div>';
  document.body.appendChild(modal);
}

async function _adminGuardarUser(uid){
  var nombre = document.getElementById('_euNombre').value.trim();
  var diasStr= document.getElementById('_euVence').value;
  var resetPw= document.getElementById('_euResetPass').checked;
  var data   = {};
  if(nombre) data.nombre = nombre;
  if(diasStr){
    var venc = new Date(); venc.setDate(venc.getDate()+parseInt(diasStr));
    data.vencimiento = venc.toISOString().split('T')[0]+'T23:59:59Z';
  }
  if(resetPw) data.password_hash = null;
  try {
    await DB.update('usala_usuarios','codigo=eq.'+encodeURIComponent(uid), data);
    var modal = document.getElementById('modalEditUser'); if(modal) modal.remove();
    showToast('✅ Usuario actualizado');
    _adminRenderUsuarios();
  } catch(e){ showToast('⚠ Error al guardar: '+e.message); }
}

async function _adminBloquear(uid){
  usalaConfirm('¿Bloquear acceso a este usuario?', async function(){
    try {
        await DB.update('usala_usuarios','codigo=eq.'+encodeURIComponent(uid),{activo:false});
        showToast('🔒 Usuario bloqueado');
        _adminRenderUsuarios();
      } catch(e){ showToast('⚠ Error: '+e.message); }
  });
}

async function _adminDesbloquear(uid){
  try {
    await DB.update('usala_usuarios','codigo=eq.'+encodeURIComponent(uid),{activo:true});
    showToast('🔓 Usuario desbloqueado');
    _adminRenderUsuarios();
  } catch(e){ showToast('⚠ Error: '+e.message); }
}

async function _adminResetNip(uid){
  usalaConfirm('¿Resetear el NIP de este usuario?', async function(){
    localStorage.removeItem('usala_nip_u_'+uid);
      showToast('🔑 NIP reseteado — el usuario podrá crear uno nuevo');
  });
}

async function _adminEliminarUser(uid, nombre){
  usalaConfirm('ELIMINAR a '+nombre+' permanentemente?\nEsto borra su acceso y todos sus datos.', async function(){
    try {
        await DB.update('usala_usuarios','codigo=eq.'+encodeURIComponent(uid),{activo:false, nombre:'[eliminado]'});
        showToast('🗑 Usuario eliminado');
        _adminRenderUsuarios();
      } catch(e){ showToast('⚠ Error: '+e.message); }
  });
}

function _adminToggleCfg(key, val){
  var cfg = JSON.parse(localStorage.getItem('usala_cfg_global')||'{}');
  cfg[key] = val;
  localStorage.setItem('usala_cfg_global', JSON.stringify(cfg));
  showToast('✓ Configuración guardada');
}

function _adminListaCats(tipo){
  var key = 'cats_'+tipo+'_custom';
  var defaults = tipo==='gasto'
    ? ['Alimentación','Transporte','Salud','Entretenimiento','Ropa','Servicios','Educación','Hogar']
    : ['Salario','Freelance','Negocio','Inversiones','Regalo','Otros'];
  var custom = load(key, []);
  var all = defaults.map(function(n){ return {nombre:n, default:true}; })
    .concat(custom.map(function(c){ return {nombre:c, default:false}; }));
  return all.map(function(c){
    return '<div style="display:flex;align-items:center;justify-content:space-between;padding:7px 0;border-bottom:1px solid var(--border);">'
      +'<span style="font-size:0.82rem;">'+c.nombre+'</span>'
      +(c.default
        ? '<span style="font-size:0.62rem;color:var(--dim);background:var(--inp);border-radius:6px;padding:2px 7px;">default</span>'
        : '<button data-tipo="'+tipo+'" data-cat="'+encodeURIComponent(c.nombre)+'" onclick="_adminBorrarCat(this.dataset.tipo, decodeURIComponent(this.dataset.cat))" style="background:none;border:none;color:var(--danger);cursor:pointer;font-size:0.8rem;padding:2px 6px;">✕</button>')
      +'</div>';
  }).join('');
}

function _adminNuevaCat(tipo){
  usalaPrompt('Nueva categoria de '+tipo+':', '', function(nombre){
    if(!nombre||!nombre.trim()) return;
    if(!nombre || !nombre.trim()) return;
      var key = 'cats_'+tipo+'_custom';
      var custom = load(key, []);
      if(custom.indexOf(nombre.trim()) > -1){ showToast('Ya existe esa categoría'); return; }
      custom.push(nombre.trim());
      save(key, custom);
      showToast('✓ Categoría "'+nombre.trim()+'" creada');
      _adminRenderConfig();
  });
}

function _adminBorrarCat(tipo, nombre){
  usalaConfirm('Eliminar la categoria "'+nombre+'"?', function(){
    var key = 'cats_'+tipo+'_custom';
      var custom = load(key, []).filter(function(c){ return c !== nombre; });
      save(key, custom);
      showToast('🗑 Categoría eliminada');
      _adminRenderConfig();
  });
}

function _adminCambiarPass(){
  usalaPrompt('Contrasena actual:', '', function(actual){
    var guardada = localStorage.getItem('usala_admin_pass')||'admin1234';
    if(actual !== guardada){ showToast('Contrasena incorrecta'); return; }
    usalaPrompt('Nueva contrasena (minimo 6 caracteres):', '', function(nueva){
      if(!nueva||nueva.length<6){ showToast('Minimo 6 caracteres'); return; }
      usalaPrompt('Confirmar nueva contrasena:', '', function(confirma){
        if(nueva!==confirma){ showToast('Las contrasenas no coinciden'); return; }
        localStorage.setItem('usala_admin_pass', nueva);
        showToast('Contrasena actualizada');
      },{type:'password',placeholder:'Repetir contrasena'});
    },{type:'password',placeholder:'Nueva contrasena'});
  },{type:'password',placeholder:'Contrasena actual'});
}

function actualizarBadgeSolicitudes(){
  var solicitudes = JSON.parse(localStorage.getItem('usala_solicitudes')||'[]');
  var pendientes = solicitudes.filter(function(s){ return s.estado==='pendiente'; }).length;
  var btn = document.getElementById('btnSolicitudes');
  var badge = document.getElementById('badgeSolicitudes');
  if(btn){
    btn.style.display = pendientes > 0 ? 'flex' : 'none';
    if(badge) badge.textContent = pendientes > 0 ? pendientes : '';
  }
}


async function renderDashboardAdmin(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  mc.innerHTML = '<div class="page-header">'
    + backSubBtn()
    + '<div class="page-title">📊 Dashboard Admin</div>'
    + '</div>'
    + '<div style="padding:20px;text-align:center;color:var(--dim);">'
    + '<div style="font-size:2rem;animation:consejeroFloat 1.5s ease-in-out infinite;">📊</div>'
    + '<div style="margin-top:10px;font-size:0.85rem;">Cargando datos de usuarios...</div>'
    + '</div>';
  try {
    // 1. Obtener todos los usuarios invitados
    var usuarios = await DB.get('usala_usuarios',
      'is_admin=eq.false&activo=eq.true&order=ultimo_acceso.desc');
    if(!usuarios) usuarios = [];
    var datosUsuarios = [];
    for(var i=0; i<usuarios.length; i++){
      var u = usuarios[i];
      try {
        var kvRows = await DB.get('usala_kv',
          'user_codigo=eq.' + encodeURIComponent(u.codigo));
        var kv = {};
        if(kvRows) kvRows.forEach(function(r){
          try{ kv[r.key] = JSON.parse(r.value); }catch(e){}
        });
        var txs     = kv.txs || [];
        var creds   = kv.creditos || [];
        var ing     = txs.filter(function(t){ return t.tipo==='ingreso'; })
                        .reduce(function(s,t){ return s+Number(t.monto||0); },0);
        var gas     = txs.filter(function(t){ return t.tipo==='gasto'; })
                        .reduce(function(s,t){ return s+Number(t.monto||0); },0);
        var debo    = creds.filter(function(c){ return c.tipo==='deuda'&&c.estado!=='pagado'; })
                        .reduce(function(s,c){ return s+Number((c.monto||0)-(c.abonado||0)); },0);
        var cobrar  = creds.filter(function(c){ return c.tipo==='prestamo'&&c.estado!=='pagado'; })
                        .reduce(function(s,c){ return s+Number((c.monto||0)-(c.abonado||0)); },0);
        var balance = ing - gas;
        var salud = 'ok';
        if(balance < 0 || debo > ing) salud = 'critico';
        else if(debo > 0 || (ing > 0 && (gas/ing) > 0.8)) salud = 'atencion';
        datosUsuarios.push({
          u: u, ing: ing, gas: gas, debo: debo,
          cobrar: cobrar, balance: balance,
          txCount: txs.length, salud: salud
        });
      } catch(e){
        datosUsuarios.push({ u: u, ing:0, gas:0, debo:0, cobrar:0, balance:0, txCount:0, salud:'sin_datos' });
      }
    }
    var totalIng    = datosUsuarios.reduce(function(s,d){ return s+d.ing; },0);
    var totalGas    = datosUsuarios.reduce(function(s,d){ return s+d.gas; },0);
    var totalDebo   = datosUsuarios.reduce(function(s,d){ return s+d.debo; },0);
    var totalCobrar = datosUsuarios.reduce(function(s,d){ return s+d.cobrar; },0);
    var criticos    = datosUsuarios.filter(function(d){ return d.salud==='critico'; }).length;
    var atencion    = datosUsuarios.filter(function(d){ return d.salud==='atencion'; }).length;
    var resumenGlobal = '<div class="sec-title">🌐 Resumen global</div>'
      + '<div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px;">'
      + _adminMetricCard('👥 Usuarios', usuarios.length + ' activos', 'var(--accent)')
      + _adminMetricCard('💰 Ingresos totales', fmt(totalIng), '#2bc070')
      + _adminMetricCard('💸 Gastos totales', fmt(totalGas), '#ff6057')
      + _adminMetricCard('🤝 Deudas totales', fmt(totalDebo), '#ffb340')
      + '</div>';
    var alertasHtml = '';
    if(criticos > 0 || atencion > 0){
      alertasHtml = '<div class="sec-title">⚠️ Alertas</div>'
        + '<div class="card" style="margin-bottom:14px;padding:12px 16px;">';
      if(criticos > 0) alertasHtml += '<div style="display:flex;align-items:center;gap:8px;margin-bottom:8px;">'
        + '<span style="background:#ff6057;color:#fff;border-radius:20px;padding:3px 10px;font-size:0.72rem;font-weight:800;">🚨 '+criticos+' en rojo</span>'
        + '<span style="font-size:0.78rem;color:var(--dim);">Gastos superan ingresos</span></div>';
      if(atencion > 0) alertasHtml += '<div style="display:flex;align-items:center;gap:8px;">'
        + '<span style="background:#ffb340;color:#fff;border-radius:20px;padding:3px 10px;font-size:0.72rem;font-weight:800;">⚠️ '+atencion+' con alerta</span>'
        + '<span style="font-size:0.78rem;color:var(--dim);">Requieren atención</span></div>';
      alertasHtml += '</div>';
    }
    var usuariosHtml = '<div class="sec-title">👤 Usuarios</div>';
    if(datosUsuarios.length === 0){
      usuariosHtml += '<div class="card" style="text-align:center;padding:28px;color:var(--dim);font-size:0.85rem;">Sin usuarios invitados aún</div>';
    } else {
      usuariosHtml += datosUsuarios.map(function(d){
        var saludColor = d.salud==='critico' ? '#ff6057' : d.salud==='atencion' ? '#ffb340' : d.salud==='sin_datos' ? 'var(--dim)' : '#2bc070';
        var saludIco   = d.salud==='critico' ? '🚨' : d.salud==='atencion' ? '⚠️' : d.salud==='sin_datos' ? '💤' : '✅';
        var ultimoAcc  = d.u.ultimo_acceso ? new Date(d.u.ultimo_acceso).toLocaleDateString('es-MX',{day:'2-digit',month:'short'}) : 'Nunca';
        var venc       = d.u.vencimiento ? new Date(d.u.vencimiento).toLocaleDateString('es-MX',{day:'2-digit',month:'short',year:'2-digit'}) : '—';
        var vencPasada = d.u.vencimiento && new Date(d.u.vencimiento) < new Date();
        return '<div class="card" style="margin-bottom:10px;padding:14px 16px;">'
          + '<div style="display:flex;align-items:center;gap:12px;margin-bottom:12px;">'
          + '<div style="width:40px;height:40px;border-radius:50%;background:linear-gradient(135deg,var(--accent),var(--accent2));display:flex;align-items:center;justify-content:center;font-weight:900;color:#fff;font-size:1rem;flex-shrink:0;">'
          + (d.u.nombre||'?').charAt(0).toUpperCase()
          + '</div>'
          + '<div style="flex:1;min-width:0;">'
          + '<div style="font-weight:800;font-size:0.9rem;color:var(--text);">' + (d.u.nombre||d.u.codigo) + '</div>'
          + '<div style="font-size:0.68rem;color:var(--dim);">'
          + d.u.codigo
          + (d.u.password_hash ? ' · 🔐' : ' · sin contraseña')
          + '</div>'
          + '</div>'
          + '<div style="text-align:right;">'
          + '<div style="font-size:1.1rem;">' + saludIco + '</div>'
          + '<div style="font-size:0.62rem;color:' + saludColor + ';font-weight:700;">'
          + (d.salud==='critico'?'En rojo':d.salud==='atencion'?'Atención':d.salud==='sin_datos'?'Sin datos':'Al día')
          + '</div>'
          + '</div>'
          + '</div>'
          + (d.txCount > 0 ? ''
            + '<div style="display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:10px;">'
            + '<div style="text-align:center;background:var(--inp);border-radius:10px;padding:8px 4px;">'
            + '<div style="font-size:0.65rem;color:var(--dim);">Ingresos</div>'
            + '<div style="font-size:0.82rem;font-weight:800;color:#2bc070;">' + fmt(d.ing) + '</div>'
            + '</div>'
            + '<div style="text-align:center;background:var(--inp);border-radius:10px;padding:8px 4px;">'
            + '<div style="font-size:0.65rem;color:var(--dim);">Gastos</div>'
            + '<div style="font-size:0.82rem;font-weight:800;color:#ff6057;">' + fmt(d.gas) + '</div>'
            + '</div>'
            + '<div style="text-align:center;background:var(--inp);border-radius:10px;padding:8px 4px;">'
            + '<div style="font-size:0.65rem;color:var(--dim);">Balance</div>'
            + '<div style="font-size:0.82rem;font-weight:800;color:' + (d.balance>=0?'#2bc070':'#ff6057') + ';">' + fmt(d.balance) + '</div>'
            + '</div>'
            + '</div>'
            + (d.debo > 0 ? '<div style="font-size:0.72rem;color:#ffb340;margin-bottom:6px;">🤝 Debe: <b>'+fmt(d.debo)+'</b></div>' : '')
            + (d.cobrar > 0 ? '<div style="font-size:0.72rem;color:#3dbf7a;margin-bottom:6px;">📥 Le deben: <b>'+fmt(d.cobrar)+'</b></div>' : '')
          : '<div style="font-size:0.75rem;color:var(--dim);text-align:center;padding:8px;">Sin transacciones registradas</div>')
          + '<div style="display:flex;justify-content:space-between;align-items:center;margin-top:8px;padding-top:8px;border-top:1px solid var(--border);">'
          + '<span style="font-size:0.65rem;color:var(--dim);">Último acceso: ' + ultimoAcc + '</span>'
          + '<span style="font-size:0.65rem;color:' + (vencPasada?'#ff6057':'var(--dim)') + ';">Vence: ' + venc + '</span>'
          + '</div>'
          + '</div>';
      }).join('');
    }
    mc.innerHTML = '<div class="page-header">'
      + backSubBtn()
      + '<div class="page-title">📊 Dashboard Admin</div>'
      + '<button onclick="renderDashboardAdmin()" style="background:var(--inp);border:1px solid var(--border);border-radius:10px;padding:6px 12px;font-size:0.75rem;color:var(--text);cursor:pointer;">🔄 Actualizar</button>'
      + '</div>'
      + resumenGlobal
      + alertasHtml
      + usuariosHtml;
  } catch(e){
    mc.innerHTML = '<div class="page-header">'+backSubBtn()+'<div class="page-title">📊 Dashboard Admin</div></div>'
      + '<div class="card" style="text-align:center;padding:28px;color:var(--dim);">'
      + '<div style="font-size:2rem;margin-bottom:10px;">😕</div>'
      + '<div>Error cargando datos<br><span style="font-size:0.75rem;">'+e.message+'</span></div>'
      + '<button class="btn-main" onclick="renderDashboardAdmin()" style="margin-top:16px;">Reintentar</button>'
      + '</div>';
    console.error('Dashboard admin:', e);
  }
}

function renderNoticiasAdmin(){
  var noticias = JSON.parse(localStorage.getItem('usala_noticias')||'[]');
  var html = '<div class="page-header">'+backSubBtn()+'<div class="page-title">📢 Noticias (Admin)</div></div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<div class="card-title">📝 Publicar noticia</div>'
    +'<label class="inp-label">Título</label>'
    +'<input class="inp" id="noticiasTitulo" placeholder="Título de la noticia" autocomplete="off">'
    +'<label class="inp-label">Mensaje</label>'
    +'<textarea class="inp" id="noticiasMsg" rows="3" placeholder="Contenido de la noticia..." style="resize:vertical;"></textarea>'
    +'<div class="form-row" style="margin-top:4px;">'
    +'<div><label class="inp-label">Tipo</label>'
    +'<select class="inp" id="noticiasTipo">'
    +'<option value="info">ℹ️ Info</option>'
    +'<option value="aviso">⚠️ Aviso</option>'
    +'<option value="promo">🎉 Promo</option>'
    +'<option value="update">🆕 Update</option>'
    +'</select></div>'
    +'<div style="display:flex;align-items:flex-end;">'
    +'<button class="btn-main" style="margin-bottom:0;" onclick="publicarNoticia()">📢 Publicar</button>'
    +'</div></div></div>'
    +'<div class="card"><div class="card-title">📋 Publicadas ('+noticias.length+')</div>';
  if(noticias.length===0){
    html += '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin noticias publicadas</div>';
  } else {
    noticias.slice().reverse().forEach(function(n,i){
      var ri = noticias.length-1-i;
      html += '<div class="tx-item" style="align-items:flex-start;gap:10px;">'
        +'<div style="font-size:1.1rem;margin-top:2px;">'+(n.tipo==='aviso'?'⚠️':n.tipo==='promo'?'🎉':n.tipo==='update'?'🆕':'ℹ️')+'</div>'
        +'<div style="flex:1;">'
        +'<div style="font-weight:700;font-size:0.88rem;">'+n.titulo+'</div>'
        +'<div style="font-size:0.78rem;color:var(--dim);margin-top:2px;">'+n.msg+'</div>'
        +'<div style="font-size:0.68rem;color:var(--dim);margin-top:4px;">'+n.fecha+'</div>'
        +'</div>'
        +'<button class="ic-btn" onclick="borrarNoticia('+ri+')" style="color:var(--danger);">🗑️</button>'
        +'</div>';
    });
  }
  html += '</div>';
  return html;
}

function publicarNoticia(){
  var titulo = document.getElementById('notTitulo').value.trim();
  var mensaje = document.getElementById('notMensaje').value.trim();
  var tipo = document.getElementById('notTipo').value;
  if(!titulo || !mensaje){ showToast('⚠ Escribe título y mensaje'); return; }
  var noticias = getNoticias();
  noticias.push({
    id: Date.now(),
    titulo: titulo,
    mensaje: mensaje,
    tipo: tipo,
    fecha: today()
  });
  saveNoticias(noticias);
  showToast('✅ Mensaje publicado para todos los invitados');
  goSub('noticias');
}

function borrarNoticia(i){
  var noticias = getNoticias();
  var _eliNot = JSON.parse(JSON.stringify(noticias[i]));
  noticias.splice(i, 1);
  saveNoticias(noticias);
  goSub('noticias');
  mostrarUndo('📢 Mensaje eliminado', function(){
    var n2=getNoticias(); n2.splice(i,0,_eliNot); saveNoticias(n2); goSub('noticias');
  });
}

function renderNoticias(){
  var isAdmin = S.user && S.user.isAdmin;
  var noticias = getNoticias();
  if(isAdmin){
    var lista = noticias.length ? noticias.slice().reverse().map(function(n,i){
      var ri = noticias.length - 1 - i;
      var leidas = JSON.parse(localStorage.getItem('usala_leidas_count_'+n.id)||'0');
      return '<div class="card" style="margin-bottom:8px;">'
        +'<div style="display:flex;justify-content:space-between;align-items:flex-start;gap:8px;">'
        +'<div style="flex:1;">'
        +'<div style="font-weight:800;font-size:0.88rem;">'+n.titulo+'</div>'
        +'<div style="font-size:0.75rem;color:var(--dim);margin-top:4px;line-height:1.5;">'+n.mensaje+'</div>'
        +'<div style="font-size:0.65rem;color:var(--dim);margin-top:6px;">📅 '+n.fecha+' &nbsp; 👁️ '+leidas+' lecturas</div>'
        +'</div>'
        +'<button class="ic-btn" onclick="borrarNoticia('+ri+')" style="flex-shrink:0;">🗑️</button>'
        +'</div></div>';
    }).join('') : '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin mensajes enviados</div>';
    return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">📢 Centro de Mensajes</div></div>'
      +'<div class="card" style="margin-bottom:14px;">'
      +'<div class="card-title">✍️ Nuevo mensaje</div>'
      +'<label class="inp-label">Título</label>'
      +'<input class="inp" id="notTitulo" placeholder="Ej: Nueva actualización disponible">'
      +'<label class="inp-label">Mensaje</label>'
      +'<textarea class="inp" id="notMensaje" rows="4" placeholder="Escribe aquí las novedades, mejoras o información importante para tus invitados..." style="resize:none;line-height:1.5;"></textarea>'
      +'<label class="inp-label">Tipo</label>'
      +'<select class="inp" id="notTipo">'
      +'<option value="📢">📢 Anuncio general</option>'
      +'<option value="🆕">🆕 Nueva función</option>'
      +'<option value="🔧">🔧 Mejora / corrección</option>'
      +'<option value="⚠️">⚠️ Aviso importante</option>'
      +'<option value="🎉">🎉 Celebración</option>'
      +'</select>'
      +'<button class="btn-main" onclick="publicarNoticia()">📤 Publicar para todos los invitados</button>'
      +'</div>'
      +'<div style="font-size:0.72rem;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;color:var(--dim);margin-bottom:8px;">Mensajes publicados ('+noticias.length+')</div>'
      + lista;
  } else {
    var leidas = JSON.parse(localStorage.getItem('usala_leidas_'+S.user.codigo)||'[]');
    var items = noticias.length ? noticias.slice().reverse().map(function(n){
      var yaLeida = leidas.indexOf(n.id) !== -1;
      if(!yaLeida){
        leidas.push(n.id);
        localStorage.setItem('usala_leidas_'+S.user.codigo, JSON.stringify(leidas));
        var cnt = parseInt(localStorage.getItem('usala_leidas_count_'+n.id)||'0');
        localStorage.setItem('usala_leidas_count_'+n.id, cnt+1);
      }
      return '<div class="card" style="margin-bottom:10px;'+(yaLeida?'':'border-left:3px solid var(--accent);')+'">'
        +'<div style="display:flex;align-items:center;gap:8px;margin-bottom:6px;">'
        +'<span style="font-size:1.2rem;">'+n.tipo+'</span>'
        +'<div style="font-weight:800;font-size:0.9rem;flex:1;">'+n.titulo+'</div>'
        +(yaLeida?'':'<span style="font-size:0.6rem;background:var(--accent);color:var(--navtext);padding:2px 7px;border-radius:10px;font-weight:700;">NUEVO</span>')
        +'</div>'
        +'<div style="font-size:0.8rem;color:var(--dim);line-height:1.6;">'+n.mensaje+'</div>'
        +'<div style="font-size:0.65rem;color:var(--dim);margin-top:8px;">'+n.fecha+'</div>'
        +'</div>';
    }).join('') : '<div style="text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;">📭 No hay mensajes aún</div>';
    return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">📢 Mensajes</div></div>'
      + items;
  }
}

function getNoticias(){ return JSON.parse(localStorage.getItem('usala_noticias')||'[]'); }


// ════════════════════════════════════════════════════
//  PANTALLA: Registro completado → redirige al login
// ════════════════════════════════════════════════════
function mostrarExitoRegistro(nombre, codigo){
  // Limpiar campos
  var campos = ['accNuevaPass','accPassword','accCodigo','accNombre'];
  campos.forEach(function(id){
    var el = document.getElementById(id);
    if(el) el.value = '';
  });
  var sb = document.getElementById('passStrengthBox');
  if(sb) sb.innerHTML = '';

  // Ocultar todos los paneles
  ['panelSesion','panelCodigo','panelSolicitud','panelEnviada'].forEach(function(id){
    var el = document.getElementById(id);
    if(el) el.style.display = 'none';
  });

  // Mostrar panel de éxito (si ya existe, limpiarlo; si no, crearlo)
  var container = document.querySelector('.lg-wrap');
  if(!container) { location.reload(); return; }

  // Eliminar panel anterior si existe
  var viejo = document.getElementById('panelRegistroOk');
  if(viejo) viejo.remove();

  var div = document.createElement('div');
  div.id = 'panelRegistroOk';
  div.className = 'lg-card';
  div.style.textAlign = 'center';
  div.innerHTML = ''
    + '<div style="font-size:3.5rem;margin-bottom:12px;animation:consejeroFloat 2s ease-in-out infinite;">🎉</div>'
    + '<div style="font-size:1.1rem;font-weight:900;color:#fff;margin-bottom:6px;letter-spacing:-0.02em;">'
    +   '¡Registro completado!'
    + '</div>'
    + '<div style="font-size:0.82rem;color:rgba(255,255,255,0.5);margin-bottom:6px;">'
    +   'Bienvenid@ a USALA, <b style="color:#fff;">' + (nombre||'').split(' ')[0] + '</b>'
    + '</div>'
    + '<div style="font-size:0.72rem;color:rgba(255,255,255,0.3);margin-bottom:24px;">'
    +   'Tu contraseña ha sido guardada de forma segura.'
    + '</div>'

    // Código visible
    + '<div style="background:rgba(43,192,112,0.08);border:1px solid rgba(43,192,112,0.2);'
    +   'border-radius:14px;padding:14px 20px;margin-bottom:20px;">'
    +   '<div style="font-size:0.62rem;color:rgba(43,192,112,0.7);font-weight:700;'
    +     'letter-spacing:0.1em;text-transform:uppercase;margin-bottom:4px;">Tu código de acceso</div>'
    +   '<div style="font-size:1.5rem;font-weight:900;letter-spacing:0.1em;color:#2bc070;">'
    +     codigo
    +   '</div>'
    +   '<div style="font-size:0.65rem;color:rgba(255,255,255,0.3);margin-top:4px;">'
    +     'Guárdalo — lo necesitarás para entrar'
    +   '</div>'
    + '</div>'

    // Checklist de lo que se configuró
    + '<div style="text-align:left;margin-bottom:20px;">'
    +   '<div style="font-size:0.68rem;font-weight:700;color:rgba(255,255,255,0.4);'
    +     'text-transform:uppercase;letter-spacing:0.08em;margin-bottom:8px;">Lo que configuraste</div>'
    +   '<div style="font-size:0.78rem;color:rgba(43,192,112,0.9);margin-bottom:4px;">✓ Código de acceso</div>'
    +   '<div style="font-size:0.78rem;color:rgba(43,192,112,0.9);margin-bottom:4px;">✓ Contraseña segura</div>'
    +   '<div style="font-size:0.78rem;color:rgba(255,255,255,0.3);">○ NIP (opcional — configúralo después)</div>'
    + '</div>'

    // Botón ir al login
    + '<button class="lg-btn" onclick="irAlLogin()">'
    +   '🔐 Iniciar sesión →'
    + '</button>'
    + '<div style="font-size:0.68rem;color:rgba(255,255,255,0.25);margin-top:10px;">'
    +   'Usa tu código + contraseña para entrar'
    + '</div>';

  container.appendChild(div);
  // Scroll al panel
  div.scrollIntoView({ behavior: 'smooth', block: 'start' });
}

// ── Ir al login limpio ────────────────────────────
function irAlLogin(){
  // Ocultar panel de éxito
  var ok = document.getElementById('panelRegistroOk');
  if(ok) ok.style.display = 'none';

  // Limpiar campos y errores
  var errEl = document.getElementById('accessErr');
  if(errEl){ errEl.textContent=''; errEl.style.display='none'; }
  var sb = document.getElementById('passStrengthBox');
  if(sb) sb.innerHTML='';

  // Restablecer estado
  _saltarPass = false;
  _accPassVerificada = false;

  // Mostrar el panel de código (login normal)
  var panelCodigo = document.getElementById('panelCodigo');
  var panelSesion = document.getElementById('panelSesion');
  if(panelCodigo){
    panelCodigo.style.display = 'block';
    // Ocultar rows opcionales
    var rows = ['accCrearPassRow','accPassRow'];
    rows.forEach(function(id){
      var el = document.getElementById(id);
      if(el) el.style.display = 'none';
    });
    // Mostrar el row de nombre
    var nr = document.getElementById('accNombreRow');
    if(nr) nr.style.display = 'block';
    // Mostrar el row de código
    var cr = document.getElementById('accCodigo');
    if(cr){ cr.value = ''; cr.focus(); }
  }
  if(panelSesion) panelSesion.style.display = 'none';

  // Texto del input de código con hint
  var codInp = document.getElementById('accCodigo');
  if(codInp) codInp.focus();

  // Toast guía
  showToast('Ingresa tu código y contraseña para entrar');
}


// ─────────────────────────────────────────────
//  USALA Suite — Transacciones
//  js/transacciones.js
// ─────────────────────────────────────────────

function getTxs(){
  var txs = load('txs',[]);
  var dirty = false;
  txs.forEach(function(t){
    var m = migrarCat(t.cat);
    if(m !== t.cat){ t.cat = m; dirty = true; }
  });
  if(dirty) save('txs', txs);
  return txs;
}

function saveTxs(txs){ save('txs',txs); }

function txItem(t, showEdit){
  var es = showEdit !== false;
  var isIng = t.tipo==='ingreso';
  var ico = isIng ? '💰' : (t.cat==='Comida'||t.cat==='Alimentación'?'🍽️':t.cat==='Transporte'?'🚗':t.cat==='Servicios'?'⚡':t.cat==='Salud'?'💊':t.cat==='Entretenimiento'?'🎬':t.cat==='Educación'?'📚':t.cat==='Pagos'?'📅':'💳');
  var fechaFmt = (function(){
    if(!t.fecha) return '';
    var p=t.fecha.split('-'); if(p.length<3) return t.fecha;
    var meses=['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'];
    return p[2]+' '+meses[+p[1]-1];
  })();
  return '<div class="tx-item">'
    +'<div class="tx-ico" style="background:'+(isIng?'rgba(43,192,112,0.12)':'rgba(255,95,87,0.1)')+';border-color:'+(isIng?'rgba(43,192,112,0.2)':'rgba(255,95,87,0.15)')+';font-size:1rem;">'+ico+'</div>'
    +'<div class="tx-info">'
    +'<div class="tx-name">'+t.desc+'</div>'
    +'<div class="tx-date">'+fechaFmt+(t.cat?' · <span style="color:var(--accent);opacity:0.7;">'+t.cat+'</span>':'')+'</div>'
    +'</div>'
    +'<div class="tx-right">'
    +'<div class="tx-amt '+(isIng?'ing':'gas')+'">'+(isIng?'+':'-')+fmt(t.monto)+'</div>'
    +(es?'<button class="ic-btn" onclick="editarTx(\"'+t.id+'\")" style="font-size:0.8rem;">✏️</button>':'')
    +(es?'<button class="ic-btn" onclick="borrarTx(\"'+t.id+'\")" style="font-size:0.8rem;">🗑️</button>':'')
    +'</div></div>';
}

function borrarTx(id){
  var txs = getTxs();
  // Comparar como string para soportar IDs 'tx_123' y numéricos
  var idStr = String(id);
  var eli = txs.find(function(t){ return String(t.id)===idStr; });
  if(!eli) return;
  if(eli.cuenta) revertirMovimientoCuenta(eli.cuenta, Number(eli.monto), eli.tipo);
  saveTxs(txs.filter(function(t){ return String(t.id)!==idStr; }));
  renderTab(S.tab);
  mostrarUndo('Transaccion eliminada', function(){
    var t2=getTxs();
    var eliId=String(eli.id);
    if(!t2.find(function(x){ return String(x.id)===eliId; })) t2.push(eli);
    saveTxs(t2);
    if(eli.cuenta) aplicarMovimientoCuenta(eli.cuenta, Number(eli.monto), eli.tipo, eli.desc, eli.fecha, eli.id);
    showToast('Restaurado'); renderTab(S.tab);
  });
}

function editarTx(id){
  var txs = getTxs();
  var idStr = String(id);
  var t = txs.find(function(x){ return String(x.id)===idStr; });
  if(!t) return;
  S.editTxId = t.id; // usar el id tal como está guardado
  document.getElementById('txModalTitle').textContent = 'Editar Transacción';
  document.getElementById('tipoSelector').style.display = 'none';
  document.getElementById('txDesc').value = t.desc;
  document.getElementById('txMonto').value = t.monto;
  document.getElementById('txFecha').value = t.fecha;
  document.getElementById('txSaveBtn').textContent = '💾 Guardar cambios';
  var _catMigrado = migrarCat(t.cat);
  var sel = document.getElementById('txCat');
  sel.innerHTML = t.tipo==='ingreso' ? buildIngresoCatSelect('txCat',_catMigrado) : buildGastoCatSelect('txCat',_catMigrado);
  poblarCuentas(t.cuenta||'');
  document.getElementById('txModal').classList.add('open');
  setTimeout(function(){ document.getElementById('txDesc').focus(); }, 400);
}

function guardarTx(){
  var desc  = document.getElementById('txDesc').value.trim();
  var monto = parseFloat(document.getElementById('txMonto').value);
  var cat   = document.getElementById('txCat').value;
  var fecha = document.getElementById('txFecha').value || today();
  var cuenta = document.getElementById('txCuenta').value;
  var tipo  = document.getElementById('tipoGasto').classList.contains('selected') ? 'gasto' : 'ingreso';
  if(!desc){ showToast('⚠ Escribe una descripción'); return; }
  if(!monto || monto<=0){ showToast('⚠ Escribe un monto válido'); return; }
  var txs = getTxs();
  if(S.editTxId){
    var _eid=String(S.editTxId); var ei = txs.findIndex(function(t){ return String(t.id)===_eid; });
    if(ei>-1){
      var prev = txs[ei];
      if(prev.cuenta) revertirMovimientoCuenta(prev.cuenta, Number(prev.monto), prev.tipo);
      tipo = prev.tipo;
      txs[ei] = Object.assign(prev, {desc:desc, monto:monto, cat:cat, fecha:fecha, cuenta:cuenta});
      if(cuenta) aplicarMovimientoCuenta(cuenta, monto, tipo, desc, fecha, S.editTxId);
    }
    showToast('✓ Actualizado correctamente');
  } else {
    var id = Date.now();
    txs.push({id:id, tipo:tipo, desc:desc, monto:monto, cat:cat, fecha:fecha, cuenta:cuenta});
    if(cuenta) aplicarMovimientoCuenta(cuenta, monto, tipo, desc, fecha, id);
    showToast('✓ '+( tipo==='ingreso'?'Ingreso':'Gasto')+' guardado'+(cuenta?' → '+nombreCuenta(cuenta):''));
  }
  saveTxs(txs);
  cerrarTxModal();
  renderTab(S.tab);
}

function guardarTxInline(tipo, cat){
  var sufijo = tipo==='ingreso' ? 'ingreso' : cat;
  var descEl  = document.getElementById('inDesc_'+sufijo);
  var montoEl = document.getElementById('inMonto_'+sufijo);
  var fechaEl = document.getElementById('inFecha_'+sufijo);
  var cuentaEl= document.getElementById('inCuenta_'+sufijo);
  if(!descEl||!montoEl){ showToast('⚠ Error de formulario'); return; }
  var desc  = descEl.value.trim();
  var monto = parseFloat(montoEl.value);
  var fecha = fechaEl ? fechaEl.value||today() : today();
  var cuenta = cuentaEl ? cuentaEl.value : '';
  var catFinal = tipo==='ingreso'
    ? (document.getElementById('inCat_ingreso') ? document.getElementById('inCat_ingreso').value : 'Salario')
    : cat;
  if(!desc){ showToast('⚠ Escribe una descripción'); return; }
  if(!monto||monto<=0){ showToast('⚠ Escribe un monto válido'); return; }
  var txs = getTxs();
  var id = Date.now();
  txs.push({id:id, tipo:tipo, desc:desc, monto:monto, cat:catFinal, fecha:fecha, cuenta:cuenta});
  saveTxs(txs);
  if(cuenta) aplicarMovimientoCuenta(cuenta, monto, tipo, desc, fecha, id);
  showToast('✓ Guardado'+(cuenta?' → '+nombreCuenta(cuenta):''));
  var mapSub = {Pagos:'pagos', Compras:'compras', Servicios:'servicios', ingreso:'activos'};
  var sub = mapSub[cat]||mapSub[tipo];
  if(sub) goSub(sub);
}

function aplicarMovimientoCuenta(cuentaVal, monto, tipo, desc, fecha, txId){
  if(!cuentaVal) return;
  var c = getCuentas();
  var delta = tipo==='ingreso' ? monto : -monto;
  if(cuentaVal==='efectivo'){
    c.movEfectivo = c.movEfectivo||[];
    c.movEfectivo.push({desc:desc, monto:Math.abs(delta), fecha:fecha, tipo:tipo==='ingreso'?'entrada':'salida', txId:txId});
    c.efectivo = (c.efectivo||0) + delta;
  } else if(cuentaVal.indexOf('cheque_')===0){
    var idx = parseInt(cuentaVal.replace('cheque_',''));
    if(c.cheques && c.cheques[idx]){
      c.cheques[idx].saldo = (c.cheques[idx].saldo||0) + delta;
    }
  } else if(cuentaVal.indexOf('tc_')===0){
    var ti = parseInt(cuentaVal.replace('tc_',''));
    if(c.tarjetas && c.tarjetas[ti]){
      var cambio = tipo==='gasto' ? monto : -monto;
      c.tarjetas[ti].balance = (Number(c.tarjetas[ti].balance)||0) + cambio;
    }
  }
  saveCuentas(c);
}

function revertirMovimientoCuenta(cuentaVal, monto, tipo){
  if(!cuentaVal) return;
  var c = getCuentas();
  var delta = tipo==='ingreso' ? -monto : monto;
  if(cuentaVal==='efectivo'){
    c.efectivo = (c.efectivo||0) + delta;
  } else if(cuentaVal.indexOf('cheque_')===0){
    var idx = parseInt(cuentaVal.replace('cheque_',''));
    if(c.cheques && c.cheques[idx]){
      c.cheques[idx].saldo = (c.cheques[idx].saldo||0) + delta;
    }
  } else if(cuentaVal.indexOf('tc_')===0){
    var ti = parseInt(cuentaVal.replace('tc_',''));
    if(c.tarjetas && c.tarjetas[ti]){
      var cambio = tipo==='gasto' ? -monto : monto;
      c.tarjetas[ti].balance = (Number(c.tarjetas[ti].balance)||0) + cambio;
    }
  }
  saveCuentas(c);
}

function nombreCuenta(val){
  if(!val) return '';
  if(val==='efectivo') return 'Efectivo';
  if(val.indexOf('cheque_')===0){
    var c=getCuentas(); var idx=parseInt(val.replace('cheque_',''));
    return c.cheques&&c.cheques[idx] ? c.cheques[idx].banco : 'Banco';
  }
  return val;
}

function renderGastos(){
  return '<div class="page-header" style="padding-top:4px;margin-bottom:16px;"><div style="font-size:1.05rem;font-weight:800;">💳 Gastos</div></div>'
    +'<div class="mod-list">'
    +'<div class="mod-item" onclick="goSub(\'pagos\')"><div class="mod-icon">💵</div><div><div class="mod-label">Pagos</div><div class="mod-sub">Facturas, servicios, rentas</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'compras\')"><div class="mod-icon">🛍️</div><div><div class="mod-label">Compras</div><div class="mod-sub">Productos y artículos</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'carrito\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,179,64,0.2),rgba(255,179,64,0.08));">🛒</div><div><div class="mod-label">Carrito inteligente</div><div class="mod-sub">Listas, precios e historial</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'servicios\')"><div class="mod-icon">⚡</div><div><div class="mod-label">Servicios</div><div class="mod-sub">Luz, agua, internet, etc.</div></div><div class="mod-arrow">›</div></div>'
    +'</div>';
}

function renderSubTxs(titulo, icono, cat){
  var txs = getTxs().filter(function(t){ return t.tipo==='gasto' && (cat==='all' || t.cat===cat); });
  var total = txs.reduce(function(s,t){ return s+Number(t.monto); },0);
  var items = txs.slice().reverse().map(function(t){
    var cuentaLabel = t.cuenta ? ' <span style="font-size:0.65rem;background:var(--inp);padding:2px 6px;border-radius:6px;color:var(--dim);">'+nombreCuenta(t.cuenta)+'</span>' : '';
    return txItem(t,true).replace('</div></div>','</div>'+cuentaLabel+'</div>');
  }).join('') || '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin registros</div>';
  var cuentaOpts = buildCuentaOpts('');
  return '<div class="page-header">'+backSubBtn()+'<div class="page-title">'+icono+' '+titulo+'</div></div>'
    +'<div class="card" style="margin-bottom:12px;"><div class="stat-label">Total gastado</div><div class="stat-val red">'+fmt(total)+'</div></div>'
    +'<div class="card" style="margin-bottom:14px;" id="formInline_'+cat+'">'
    +'<div class="card-title">+ Agregar gasto</div>'
    +'<label class="inp-label">Descripción</label><input class="inp" id="inDesc_'+cat+'" placeholder="Ej: Supermercado" autocomplete="off">'
    +'<div class="form-row"><div><label class="inp-label">Monto ($)</label><input class="inp" id="inMonto_'+cat+'" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'<div><label class="inp-label">Fecha</label><input class="inp" id="inFecha_'+cat+'" type="date" value="'+today()+'"></div></div>'
    +'<label class="inp-label">💼 ¿De qué cuenta sale?</label>'
    +'<select class="inp" id="inCuenta_'+cat+'">'+cuentaOpts+'</select>'
    +'<button class="btn-main" onclick="guardarTxInline(\'gasto\',\''+cat+'\')">💾 Guardar gasto</button>'
    +'</div>'
    +'<div class="card"><div class="card-title">Registros</div>'+items+'</div>';
}

function renderPagos(){ return renderSubTxs('Pagos','💵','Pagos'); }

function renderCompras(){ return renderSubTxs('Compras','🛍️','Compras'); }

function renderServicios(){ return renderSubTxs('Servicios','⚡','Servicios'); }

function renderIngresos(){
  return '<div class="page-header" style="padding-top:4px;margin-bottom:16px;"><div style="font-size:1.05rem;font-weight:800;">💰 Ingresos</div></div>'
    +'<div class="mod-list">'
    +'<div class="mod-item" onclick="goSub(\'ingresos_activos\')"><div class="mod-icon">📥</div><div><div class="mod-label">Activos</div><div class="mod-sub">Salario, rentas, negocios</div></div><div class="mod-arrow">›</div></div>'
    +'</div>';
}

function renderIngresosActivos(){
  var txs = getTxs().filter(function(t){ return t.tipo==='ingreso'; });
  var total = txs.reduce(function(s,t){ return s+Number(t.monto); },0);
  var items = txs.slice().reverse().map(function(t){
    var cuentaLabel = t.cuenta ? ' <span style="font-size:0.65rem;background:var(--inp);padding:2px 6px;border-radius:6px;color:var(--dim);">'+nombreCuenta(t.cuenta)+'</span>' : '';
    return txItem(t,true).replace('</div></div>','</div>'+cuentaLabel+'</div>');
  }).join('') || '<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin ingresos aún</div>';
  var cuentaOpts = buildCuentaOpts('');
  return '<div class="page-header">'+backSubBtn()+'<div class="page-title">📥 Activos</div></div>'
    +'<div class="card" style="margin-bottom:12px;"><div class="stat-label">Total ingresos</div><div class="stat-val">'+fmt(total)+'</div></div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<div class="card-title">+ Agregar ingreso</div>'
    +'<label class="inp-label">Descripción</label><input class="inp" id="inDesc_ingreso" placeholder="Ej: Salario quincenal" autocomplete="off">'
    +'<div class="form-row"><div><label class="inp-label">Monto ($)</label><input class="inp" id="inMonto_ingreso" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'<div><label class="inp-label">Categoría</label><select class="inp" id="inCat_ingreso"><option>Salario</option><option>Activos</option><option>Freelance</option><option>Renta</option><option>Inversión</option><option>Otros</option></select></div></div>'
    +'<label class="inp-label">💼 ¿A qué cuenta entra?</label>'
    +'<select class="inp" id="inCuenta_ingreso">'+cuentaOpts+'</select>'
    +'<label class="inp-label">Fecha</label><input class="inp" id="inFecha_ingreso" type="date" value="'+today()+'">'
    +'<button class="btn-main" onclick="guardarTxInline(\'ingreso\',\'ingreso\')">💾 Guardar ingreso</button>'
    +'</div>'
    +'<div class="card"><div class="card-title">Registros</div>'+items+'</div>';
}

function renderHistorial(){
  var txs = getTxs().slice().reverse();
  var filtro = window._histFiltro || 'todos';
  var txsFilt = txs.filter(function(t){
    if(filtro==='ingresos') return t.tipo==='ingreso';
    if(filtro==='gastos') return t.tipo==='gasto';
    return true;
  });
  function fmtFecha(f){
    if(!f) return '';
    var p=f.split('-');
    var meses=['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'];
    return p[2]+' '+meses[parseInt(p[1])-1]+' '+p[0];
  }
  var ing = txs.filter(function(t){ return t.tipo==='ingreso'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var gas = txs.filter(function(t){ return t.tipo==='gasto'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var items = txsFilt.length ? txsFilt.map(function(t){
    var cuentaLabel = t.cuenta ? '<span style="font-size:0.6rem;background:rgba(45,158,95,0.12);color:var(--accent2);padding:1px 5px;border-radius:8px;margin-left:4px;">'+nombreCuenta(t.cuenta)+'</span>' : '';
    return '<div class="tx-item" style="padding:12px 0;">'
      +'<div class="tx-ico" style="font-size:1.3rem;">'+(t.tipo==='ingreso'?'💰':'💸')+'</div>'
      +'<div class="tx-info" style="flex:1;">'
      +'<div class="tx-name" style="font-size:0.88rem;font-weight:700;">'+t.desc+cuentaLabel+'</div>'
      +'<div class="tx-date" style="font-size:0.7rem;margin-top:2px;">'+fmtFecha(t.fecha)+' · '+t.cat+'</div>'
      +'</div>'
      +'<div class="tx-right" style="align-items:flex-end;gap:6px;">'
      +'<div class="tx-amt '+(t.tipo==='ingreso'?'ing':'gas')+'" style="font-size:0.95rem;">'+(t.tipo==='ingreso'?'+':'-')+fmt(t.monto)+'</div>'
      +'<div style="display:flex;gap:4px;">'
      +'<button class="ic-btn" onclick="editarTx(\"'+t.id+'\")" title="Editar">✏️</button>'
      +'<button class="ic-btn" onclick="borrarTx(\"'+t.id+'\")" title="Eliminar">🗑️</button>'
      +'</div></div></div>';
  }).join('') : '<div style="text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;">Sin movimientos '+(filtro!=='todos'?'en esta categoría':'aún')+'</div>';
  function filtBtn(val, label){
    var act = filtro===val;
    return '<button onclick="window._histFiltro=\''+val+'\';goSub(\'historial\')" style="padding:7px 14px;border:none;border-radius:20px;font-family:\'Outfit\',sans-serif;font-size:0.75rem;font-weight:700;cursor:pointer;background:'+(act?'var(--accent)':'rgba(0,0,0,0.06)')+';color:'+(act?'var(--navtext)':'var(--dim)')+';">'+label+'</button>';
  }
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">📋 Historial</div></div>'
    +'<div class="stat-grid" style="margin-bottom:12px;">'
    +'<div class="stat-card" style="padding:12px;"><div class="stat-label" style="font-size:0.6rem;">💰 Total ingresos</div><div style="font-size:1rem;font-weight:900;color:var(--accent2);">'+fmt(ing)+'</div></div>'
    +'<div class="stat-card" style="padding:12px;"><div class="stat-label" style="font-size:0.6rem;">💸 Total gastos</div><div style="font-size:1rem;font-weight:900;color:var(--danger);">'+fmt(gas)+'</div></div>'
    +'</div>'
    +'<div style="display:flex;gap:8px;margin-bottom:12px;">'
    +filtBtn('todos','Todos ('+txs.length+')')
    +filtBtn('ingresos','💰 Ingresos')
    +filtBtn('gastos','💸 Gastos')
    +'</div>'
    +'<div class="card">'+items+'</div>';
}

function migrarCat(cat){
  return _CAT_MIGRA[cat] || cat;
}

function buildCuentaOpts(selVal){
  var c = getCuentas();
  var ops = '<option value="">— Sin asignar —</option>'
    +'<option value="efectivo"'+(selVal==='efectivo'?' selected':'')+'>💵 Efectivo</option>';
  (c.cheques||[]).forEach(function(ch, i){
    var val='cheque_'+i;
    ops+='<option value="'+val+'"'+(selVal===val?' selected':'')+'>🏧 '+ch.banco+' — '+ch.tipo+'</option>';
  });
  return ops;
}

function irPresupuesto(){
  var nbs=document.querySelectorAll('.nb');
  nbs.forEach(function(b){ b.classList.remove('active'); });
  if(nbs[4]) nbs[4].classList.add('active');
  S.tab='mas'; S.subtab='presupuesto';
  renderPresupuesto();
}

function irProgreso(){
  var nbs=document.querySelectorAll('.nb');
  nbs.forEach(function(b){ b.classList.remove('active'); });
  if(nbs[4]) nbs[4].classList.add('active');
  S.tab='mas'; S.subtab='progreso';
  renderProgreso();
}

function abrirTxModal(tipo){
  if(tipo === 'ingreso'){
    document.getElementById('ingresoTipoModal').classList.add('open');
    return;
  }
  if(tipo === 'gasto'){
    document.getElementById('gastoTipoModal').classList.add('open');
    return;
  }
  _abrirTxModalDirecto(tipo || 'gasto');
}

function cerrarTxModal(){ document.getElementById('txModal').classList.remove('open'); }

function carritoConfirmarFin(){
  var modal = document.getElementById('modalFinCarrito');
  var actual   = getCarritoActual();
  var comprados= actual.items.filter(function(i){ return i.comprado; });
  var total    = comprados.reduce(function(s,i){ return s+(i.precio||0)*(i.qty||1); },0);
  var regGasto = document.getElementById('finRegGasto').checked;
  var cuentaSel= document.getElementById('finCuentaGasto').value;
  var hist = getCarritoHistorial();
  var listaGuardar = JSON.parse(JSON.stringify(actual));
  listaGuardar.fechaFin = today();
  listaGuardar.totalReal = total;
  hist.unshift(listaGuardar);
  if(hist.length > 50) hist = hist.slice(0,50);
  saveCarritoHistorial(hist);
  comprados.forEach(function(i){
    if(i.precio) carritoRegistrarPrecio(i.nombre, i.precio, actual.tienda);
  });
  if(regGasto && total > 0){
    var cats = getCarritoCats();
    var cat  = cats.find(function(c){ return c.id===actual.catId; });
    var desc = (actual.nombre||'Compra') + (actual.tienda?' en '+actual.tienda:'');
    var txId = 'tx_'+Date.now();
    var tx = {
      id: txId,
      tipo: 'gasto',
      monto: total,
      cat: cat ? cat.nombre : 'Compras',
      desc: desc,
      fecha: today(),
      cuenta: cuentaSel,
      nota: comprados.length+' productos'
    };
    var txs = load('txs',[]);
    txs.push(tx);
    save('txs', txs);
    if(cuentaSel){
      aplicarMovimientoCuenta(cuentaSel, total, 'gasto', desc, today(), txId);
    }
  }
  saveCarritoActual({nombre:'',catId:'super',items:[],fecha:'',tienda:''});
  var _m = document.getElementById('modalFinCarrito'); if(_m) _m.remove();
  showToast('✅ Compra guardada'+(regGasto?' y registrada como gasto':''));
  S._carritoTab = 'historial';
  goSub('carrito');
}



// ─────────────────────────────────────────────
//  USALA Suite — Dashboard & UI
//  js/dashboard.js
// ─────────────────────────────────────────────

function renderInicio(){
  var txs = getTxs();
  var ing = txs.filter(function(t){ return t.tipo==='ingreso'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var gas = txs.filter(function(t){ return t.tipo==='gasto'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var creds = load('creditos',[]);
  var debo   = creds.filter(function(c){ return c.tipo==='deuda'&&c.estado!=='pagado'; }).reduce(function(s,c){ return s+Number(c.monto-(c.abonado||0)); },0);
  var meDebn = creds.filter(function(c){ return c.tipo==='prestamo'&&c.estado!=='pagado'; }).reduce(function(s,c){ return s+Number(c.monto-(c.abonado||0)); },0);
  var cu = getCuentas();
  var efec  = cu.efectivo || 0;
  var banco = (cu.cheques||[]).reduce(function(s,x){ return s+Number(x.saldo||0); },0);
  var deudaTC = (cu.tarjetas||[]).reduce(function(s,t){ return s+Number(t.balance||0); },0);
  var totalDisp = efec + banco;
  var actP = load('activos_personales',[]).reduce(function(s,a){ return s+(a.valor||0); },0);
  var pn = (efec+banco+actP)-(deudaTC+debo);
  var nombre = (S.user.nombre||'').split(' ')[0] || 'tú';
  var hora = new Date().getHours();
  var saludo = hora<12 ? '☀️ Buenos días' : hora<19 ? '👋 Buenas tardes' : '🌙 Buenas noches';
  var _u=S.user, _prefix=(_u?(_u.isAdmin?'usala_admin':'usala_u_'+_u.codigo)+'_snap_':'');
  var _mes=new Date().toISOString().slice(0,7);
  var _prevKeys=[]; for(var _k in localStorage){ if(_prefix&&_k.indexOf(_prefix)===0&&_k!==_prefix+_mes) _prevKeys.push(_k); }
  _prevKeys.sort(); var _prevSnap=null;
  if(_prevKeys.length){ try{ _prevSnap=JSON.parse(localStorage.getItem(_prevKeys[_prevKeys.length-1])); }catch(e){} }
  var _diff=_prevSnap?pn-_prevSnap.patrimonioNeto:null;
  var trendStr = _diff===null ? '' :
    (_diff>=0
      ? '<span style="font-size:0.7rem;color:rgba(255,255,255,0.75);margin-left:8px;">↑ '+fmt(Math.abs(_diff))+' vs mes ant.</span>'
      : '<span style="font-size:0.7rem;color:rgba(255,200,200,0.8);margin-left:8px;">↓ '+fmt(Math.abs(_diff))+' vs mes ant.</span>');
  var heroCard = '<div class="hero-card" onclick="irProgreso()">'
    +'<div style="position:relative;z-index:1;">'
    +'<div class="hero-label">'+saludo+', '+nombre+'</div>'
    +'<div class="hero-amount">'+fmt(totalDisp)+'</div>'
    +'<div class="hero-sub">Total disponible · Toca para ver progreso'+trendStr+'</div>'
    +'<div class="hero-pills">'
    +'<div class="hero-pill" onclick="event.stopPropagation();goSub(\'efectivo\');goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1])"><span class="hero-pill-ico">💵</span>'+fmt(efec)+'</div>'
    +'<div class="hero-pill" onclick="event.stopPropagation();goSub(\'cheques\');goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1])"><span class="hero-pill-ico">🏧</span>'+fmt(banco)+'</div>'
    +'</div>'
    +'</div>'
    +'</div>';
  var quickActions = '<div class="quick-grid">'
    +'<div class="quick-item" onclick="abrirTxModal(\'gasto\')">'
    +'<div class="quick-ico">➖</div>'
    +'<div class="quick-lbl">Nuevo gasto</div></div>'
    +'<div class="quick-item" onclick="abrirTxModal(\'ingreso\')">'
    +'<div class="quick-ico">➕</div>'
    +'<div class="quick-lbl">Ingreso</div></div>'
    +'<div class="quick-item" onclick="abrirPP()">'
    +'<div class="quick-ico" style="position:relative;">'
    +(function(){
      var _h=new Date(); _h.setHours(0,0,0,0);
      var _pp=loadPagosBase(),_pe=loadPagosEstado();
      var _nV=0;
      _pp.forEach(function(p){
        if(_pe[p.id]&&_pe[p.id].pagado) return;
        var _dia=Math.min(p.dia||1,28);
        var _f; if(p.proximoPago){ var _pts=p.proximoPago.split('-'); _f=new Date(+_pts[0],+_pts[1]-1,+_pts[2]); }
        else { _f=new Date(_h.getFullYear(),_h.getMonth(),_dia); } _f.setHours(0,0,0,0);
        if(Math.round((_f-_h)/86400000)<=7) _nV++;
      });
      return '⏰'+(_nV>0?'<div style="position:absolute;top:-4px;right:-4px;background:#ff5f57;color:#fff;font-size:0.55rem;font-weight:900;min-width:16px;height:16px;border-radius:50%;display:flex;align-items:center;justify-content:center;">'+_nV+'</div>':'');
    })()
    +'</div><div class="quick-lbl">Pagos</div></div>'
    +'<div class="quick-item" onclick="goTab(\'creditos\',document.querySelectorAll(\'.nb\')[2])">'
    +'<div class="quick-ico">🤝</div>'
    +'<div class="quick-lbl">Créditos</div></div>'
    +'<div class="quick-item" onclick="goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1]);setTimeout(function(){goSub(\'carrito\');},80)">'
    +'<div class="quick-ico">🛒</div>'
    +'<div class="quick-lbl">Lista del súper</div></div>'
    +'</div>';
  var noticiasBanner = '';
  if(!S.user.isAdmin){
    var noticias = JSON.parse(localStorage.getItem('usala_noticias')||'[]');
    var sinLeer = noticias.filter(function(n){
      var leidas = JSON.parse(localStorage.getItem('usala_leidas_'+S.user.codigo)||'[]');
      return leidas.indexOf(n.id) === -1;
    });
    if(sinLeer.length){
      noticiasBanner = '<div class="noticia-banner" onclick="goSub(\'noticias\')">'
        +'<div style="display:flex;align-items:center;gap:10px;">'
        +'<span style="font-size:1.4rem;">📢</span>'
        +'<div><div style="font-weight:800;font-size:0.85rem;color:var(--text);">'+sinLeer.length+' mensaje nuevo'+(sinLeer.length>1?'s':'')+' del admin</div>'
        +'<div style="font-size:0.7rem;color:var(--accent2);margin-top:2px;font-weight:600;">Toca para leer →</div></div>'
        +'</div></div>';
    }
  }
  var pnColor = pn>=0?'var(--accent2)':'var(--danger)';
  var insightCards = '<div class="insight-row">'
    +'<div class="insight-card accent" onclick="irProgreso()">'
    +'<span class="insight-ico">📈</span>'
    +'<div class="insight-label">Patrimonio Neto</div>'
    +'<div class="insight-val" style="color:'+pnColor+';">'+fmt(pn)+'</div>'
    +(_diff!==null?'<div class="insight-trend" style="color:'+(_diff>=0?'var(--accent2)':'var(--danger)')+';">'
      +(_diff>=0?'↑':'↓')+' '+fmt(Math.abs(_diff))+'</div>':'')
    +'</div>'
    +'<div class="insight-card danger" onclick="goTab(\'creditos\',document.querySelectorAll(\'.nb\')[2])">'
    +'<span class="insight-ico">🔴</span>'
    +'<div class="insight-label">Total Deudas</div>'
    +'<div class="insight-val" style="color:var(--danger);">'+fmt(deudaTC+debo)+'</div>'
    +'<div class="insight-trend" style="color:var(--dim);">'
    +'<span>💳'+fmt(deudaTC)+'</span></div>'
    +'</div>'
    +'</div>'
    +'<div class="insight-row">'
    +'<div class="insight-card" onclick="goSub(\'ingresos\');goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1])">'
    +'<span class="insight-ico">💚</span>'
    +'<div class="insight-label">Ingresos</div>'
    +'<div class="insight-val" style="color:var(--accent2);">'+fmt(ing)+'</div>'
    +'</div>'
    +'<div class="insight-card" onclick="goSub(\'gastos\');goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1])">'
    +'<span class="insight-ico">🔥</span>'
    +'<div class="insight-label">Gastos</div>'
    +'<div class="insight-val" style="color:var(--danger);">'+fmt(gas)+'</div>'
    +'</div>'
    +'</div>';
  var _pagosMes = load('pagos_mensuales',[]);
  var _estadoPagos = (function(){ try{ var mes=new Date().toISOString().slice(0,7); var u=S.user; var base=u.isAdmin?'usala_admin':'usala_u_'+u.codigo; return JSON.parse(localStorage.getItem(base+'_pagos_estado_'+mes)||'{}'); }catch(e){ return {}; } })();
  var _totalPagosMes = _pagosMes.reduce(function(s,p){ return s+(p.monto||0); },0);
  var _pagadosN = _pagosMes.filter(function(p){ return _estadoPagos[p.id]&&_estadoPagos[p.id].pagado; }).length;
  var _totalPagado = _pagosMes.filter(function(p){ return _estadoPagos[p.id]&&_estadoPagos[p.id].pagado; }).reduce(function(s,p){ return s+(_estadoPagos[p.id].montoPagado||p.monto||0); },0);
  var _pctPagos = _totalPagosMes>0?Math.min(100,Math.round((_totalPagado/_totalPagosMes)*100)):0;
  var secPagos = '';
  if(_pagosMes.length){
    var _col = _pctPagos>=100?'var(--accent2)':_pctPagos>=70?'var(--gold)':'var(--danger)';
    secPagos = '<div class="sec-title">📅 Pagos del mes</div>'
      +'<div class="insight-card full" onclick="goSub(\'pagos_mes\')" style="margin-bottom:10px;">'
      +'<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;">'
      +'<div><div class="insight-label">Este mes</div>'
      +'<div style="font-size:1.4rem;font-weight:900;color:var(--text);">'+fmt(_totalPagosMes)+'</div></div>'
      +'<div style="text-align:right;">'
      +'<div style="font-size:1.6rem;font-weight:900;color:'+_col+';">'+_pctPagos+'%</div>'
      +'<div style="font-size:0.65rem;color:var(--dim);">'+_pagadosN+' / '+_pagosMes.length+'</div>'
      +'</div></div>'
      +'<div class="prog-wrap" style="height:8px;margin-bottom:8px;"><div class="prog-bar" style="width:'+_pctPagos+'%;background:'+_col+';"></div></div>'
      +'<div style="display:flex;justify-content:space-between;font-size:0.72rem;">'
      +'<span style="color:var(--accent2);font-weight:700;">✅ '+fmt(_totalPagado)+'</span>'
      +(_pctPagos>=100?'<span style="color:var(--accent2);font-weight:800;">🎉 ¡Al corriente!</span>':'<span style="color:var(--danger);font-weight:600;">⏳ '+fmt(_totalPagosMes-_totalPagado)+' pendiente</span>')
      +'</div></div>';
  }
  var secPres = (function(){
    var pres=load('presupuesto',{});
    var mesAct=new Date().toISOString().slice(0,7);
    var txsP=getTxs().filter(function(t){ return t.tipo==='gasto'&&t.fecha&&t.fecha.slice(0,7)===mesAct; });
    var totalLim=0, totalGas=0, excedidos=0;
    ['Pagos','Compras','Servicios','Alimentación','Transporte','Salud','Entretenimiento','Educación','Otros'].forEach(function(c){
      var lim=pres[c]||0; if(!lim) return;
      var g=txsP.filter(function(t){ return t.cat===c; }).reduce(function(s,t){ return s+Number(t.monto||0); },0);
      totalLim+=lim; totalGas+=g;
      if(g>=lim) excedidos++;
    });
    if(!totalLim) return '';
    var pct=Math.min(100,Math.round((totalGas/totalLim)*100));
    var col=pct>=100?'var(--danger)':pct>=80?'var(--gold)':'var(--accent2)';
    return '<div class="sec-title">🗂️ Presupuesto</div>'
      +'<div class="insight-card full" onclick="irPresupuesto()" style="margin-bottom:10px;">'
      +'<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;">'
      +'<div><div class="insight-label">Gasto vs límite</div>'
      +'<div style="font-size:1.2rem;font-weight:900;color:var(--text);">'+fmt(totalGas)+' <span style="font-size:0.7rem;font-weight:500;color:var(--dim);">/ '+fmt(totalLim)+'</span></div></div>'
      +(excedidos?'<div style="background:rgba(255,95,87,0.15);border:1px solid rgba(255,95,87,0.25);border-radius:12px;padding:5px 10px;font-size:0.65rem;font-weight:800;color:var(--danger);">⚠️ '+excedidos+' excedido'+(excedidos>1?'s':'')+'</div>':'<div style="background:rgba(43,192,112,0.12);border:1px solid rgba(43,192,112,0.2);border-radius:12px;padding:5px 10px;font-size:0.65rem;font-weight:800;color:var(--accent2);">✅ En control</div>')
      +'</div>'
      +'<div class="prog-wrap" style="height:8px;"><div class="prog-bar" style="width:'+pct+'%;background:'+col+';"></div></div>'
      +'</div>';
  })();
  var invCard = '';
  if(S.user.isAdmin){
    var codigos = JSON.parse(localStorage.getItem('usala_codigos')||'[]');
    var hoy2 = new Date();
    var codActivos = codigos.filter(function(c){ return c.activo && c.vencimiento && new Date(c.vencimiento.split('-').join('/'))>=hoy2; });
    var codUsados  = codigos.filter(function(c){ return c.usado; });
    invCard = '<div class="sec-title">👥 Invitados</div>'
      +'<div class="insight-card full" onclick="goSub(\'codigos\')" style="margin-bottom:10px;">'
      +'<div style="display:flex;justify-content:space-between;align-items:center;">'
      +'<div style="display:flex;gap:20px;">'
      +'<div><div class="insight-label">Conectados</div><div class="insight-val" style="color:var(--accent2);">'+codUsados.length+'</div></div>'
      +'<div><div class="insight-label">Códigos activos</div><div class="insight-val">'+codActivos.length+'</div></div>'
      +'</div>'
      +'<div style="font-size:1.5rem;opacity:0.4;">›</div>'
      +'</div></div>';
  }
  var rec = txs.slice(-5).reverse().map(function(t){ return txItem(t,true); }).join('')
    || '<div style="text-align:center;padding:28px 20px;color:var(--dim);font-size:0.83rem;">Sin transacciones aún<br><span style="font-size:0.7rem;">Toca ➕ para agregar la primera</span></div>';
  var consejeroCard = renderConsejero(ing, gas, debo, totalDisp, pn);
  return ''
    + noticiasBanner
    + heroCard
    + quickActions
    + '<div class="sec-title">🤖 Mi Consejero</div>'
    + consejeroCard
    + '<div class="sec-title">📊 Resumen financiero</div>'
    + insightCards
    + secPagos
    + secPres
    + invCard
    +'<div style="margin-top:4px;">'
    +'<div class="tx-feed-header">'
    +'<div class="tx-feed-title">Últimas transacciones</div>'
    +'<span class="tx-feed-link" onclick="goSub(\'historial\');goTab(\'cuentas\',document.querySelectorAll(\'.nb\')[1])">Ver todas →</span>'
    +'</div>'
    +'<div class="card" style="padding:8px 16px;">'+rec+'</div>'
    +'</div>';
}


function renderMas(){
  var isAdmin = S.user && S.user.isAdmin;
  var inicialNombre = S.user && S.user.nombre ? S.user.nombre.charAt(0).toUpperCase() : '?';
  var rolLabel = isAdmin ? 'Administrador' : 'Invitado';
  var rolBadge = isAdmin ? '👑 Admin' : '🔑 Invitado';
  var profileSection = '<div class="profile-header">'
    +'<div class="profile-avatar">'+inicialNombre+'</div>'
    +'<div><div class="profile-name">'+(S.user&&S.user.nombre?S.user.nombre:'Usuario')+'</div>'
    +'<div class="profile-role">'+rolLabel+' · USALA Finanzas</div></div>'
    +'<div class="profile-badge">'+rolBadge+'</div>'
    +'</div>';
  var secHerramientas = '<div class="mod-section">'
    +'<div class="mod-section-title">Herramientas</div>'
    +'<div class="mod-list">'
    +'<div class="mod-item" onclick="irProgreso()"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(43,192,112,0.2),rgba(43,192,112,0.08));">📈</div><div><div class="mod-label">Mi Progreso Financiero</div><div class="mod-sub">Patrimonio, gráficas y salud</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'activos\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,179,64,0.2),rgba(255,179,64,0.08));">🏦</div><div><div class="mod-label">Mis Activos</div><div class="mod-sub">Casa, carro, inversiones...</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'presupuesto\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(56,170,255,0.2),rgba(56,170,255,0.08));">🗂️</div><div><div class="mod-label">Presupuesto mensual</div><div class="mod-sub">Límites por categoría</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'metas\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,95,87,0.2),rgba(255,95,87,0.08));">🎯</div><div><div class="mod-label">Metas de ahorro</div><div class="mod-sub">Progreso hacia tus objetivos</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'alertas\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,179,64,0.2),rgba(255,179,64,0.08));">🔔</div><div><div class="mod-label">Alertas financieras</div><div class="mod-sub">Notificaciones personalizadas</div></div><div class="mod-arrow">›</div></div>'
    +'</div></div>';
  var secExtras = '<div class="mod-section">'
    +'<div class="mod-section-title">Extras</div>'
    +'<div class="mod-list">'
    +'<div class="mod-item" onclick="goSub(\'conversor\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(43,192,112,0.15),rgba(43,192,112,0.06));">💱</div><div><div class="mod-label">Conversor de monedas</div><div class="mod-sub">Tipos de cambio en tiempo real</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'noticias\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(56,170,255,0.15),rgba(56,170,255,0.06));">📢</div><div><div class="mod-label">Mensajes del admin</div><div class="mod-sub">Noticias y comunicados</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'ayuda\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,255,255,0.12),rgba(255,255,255,0.04));">❓</div><div><div class="mod-label">Ayuda y soporte</div><div class="mod-sub">Guía de uso y preguntas frecuentes</div></div><div class="mod-arrow">›</div></div>'
    +'</div></div>';
  var secAdmin = '';
  if(isAdmin){
    secAdmin = '<div class="mod-section">'
      +'<div class="mod-section-title">Administración</div>'
      +'<div class="mod-list">'
      +'<div class="mod-item" onclick="goSub(\'codigos\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,179,64,0.2),rgba(255,179,64,0.08));">🔑</div><div><div class="mod-label">Códigos de acceso</div><div class="mod-sub">Gestionar invitados y solicitudes</div></div><div class="mod-arrow">›</div></div>'
      +'<div class="mod-item" onclick="goSub(\'noticias_admin\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(56,170,255,0.2),rgba(56,170,255,0.08));">📝</div><div><div class="mod-label">Enviar mensajes</div><div class="mod-sub">Comunicados a todos los usuarios</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'panel_admin\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(100,100,255,0.22),rgba(100,100,255,0.08));">🛡️</div><div><div class="mod-label">Panel Administrador</div><div class="mod-sub">Usuarios, métricas y configuración</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="goSub(\'dashboard_admin\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(43,192,112,0.2),rgba(43,192,112,0.08));">📊</div><div><div class="mod-label">Dashboard usuarios</div><div class="mod-sub">Resumen financiero de todos</div></div><div class="mod-arrow">›</div></div>'
      +'<div class="mod-item" onclick="goSub(\'version\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,255,255,0.1),rgba(255,255,255,0.04));">ℹ️</div><div><div class="mod-label">Versión y estado</div><div class="mod-sub">Info técnica de la app</div></div><div class="mod-arrow">›</div></div>'
      +'</div></div>';
  }
  var secCuenta = '<div class="mod-section">'
    +'<div class="mod-section-title">Cuenta</div>'
    +'<div class="mod-list">'
    +'<div class="mod-item" onclick="goSub(\'config\')"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,255,255,0.1),rgba(255,255,255,0.04));">⚙️</div><div><div class="mod-label">Configuración</div><div class="mod-sub">Tema, moneda, NIP y privacidad</div></div><div class="mod-arrow">›</div></div>'
    +'<div class="mod-item" onclick="cerrarSesion()" style="cursor:pointer;"><div class="mod-icon" style="background:linear-gradient(135deg,rgba(255,95,87,0.2),rgba(255,95,87,0.08));">🚪</div><div><div class="mod-label" style="color:var(--danger);">Cerrar sesión</div><div class="mod-sub">Volver a la pantalla de inicio</div></div></div>'
    +'</div></div>';
  return profileSection + secHerramientas + secExtras + secAdmin + secCuenta;
}

function renderTab(tab){
  var map = {
    inicio: renderInicio,
    cuentas: renderCuentas,
    creditos: renderCreditos,
    reportes: renderReportes,
    mas: renderMas
  };
  var fn = map[tab] || function(){ return '<p>En construcción</p>'; };
  document.getElementById('mainContent').innerHTML = fn();
}

function goTab(tab, btn){
  S.tab = tab; S.subtab = null;
  document.querySelectorAll('.nb').forEach(function(b){ b.classList.remove('active'); });
  if(btn) btn.classList.add('active');
  var mc = document.getElementById('mainContent');
  mc.style.opacity = '0';
  mc.style.transform = 'translateY(8px)';
  mc.style.transition = 'none';
  renderTab(tab);
  requestAnimationFrame(function(){
    requestAnimationFrame(function(){
      mc.style.transition = 'opacity 0.28s ease, transform 0.28s cubic-bezier(0.16,1,0.3,1)';
      mc.style.opacity = '1';
      mc.style.transform = 'translateY(0)';
    });
  });
}

function goSub(sub){
  S.subtab = sub;
  if(sub && sub.indexOf('banco_')===0){
    var idx = parseInt(sub.replace('banco_',''));
    document.getElementById('mainContent').innerHTML = renderBancoDetalle(idx);
    return;
  }
  // ── Rutas que manejan su propio mc.innerHTML ──
  if(sub==='tarjetas_credito')  { renderTarjetasCredito(); return; }
  if(sub==='creditos_debo')     { renderCreditosDebo(); return; }
  if(sub==='creditos_cobrar')   { renderCreditosCobrar(); return; }
  if(sub==='cxc')               { renderCxC(); return; }
  if(sub==='nueva_tc'){
    document.getElementById('mainContent').innerHTML = renderFormTC(null); return;
  }
  if(sub==='nueva_tarjeta'){
    document.getElementById('mainContent').innerHTML = renderFormTC(null); return;
  }
  if(sub==='nueva_deuda'){
    document.getElementById('mainContent').innerHTML = renderFormCredito('deuda', null); return;
  }
  if(sub==='nuevo_prestamo'){
    document.getElementById('mainContent').innerHTML = renderFormCredito('prestamo', null); return;
  }
  if(sub==='nueva_cxc')         { renderNuevaCxC(); return; }

  var renders = {
    efectivo: renderEfectivo, cheques: renderCheques,
    pagos_mes:       renderPagosMes,
    activos:         renderActivos,
    progreso:        renderProgreso,
    ingresos_activos: renderIngresosActivos,
    metas: renderMetas, alertas: renderAlertas,
    historial: renderHistorial, conversor: renderConversor,
    reportes: renderReportes,
    codigos: null, config: renderConfig, ayuda: renderAyuda,
    version: renderVersion, noticias: renderNoticias,
    carrito: renderCarrito
  };
  if(sub==='ingresos_activos'){ document.getElementById('mainContent').innerHTML=renderIngresosActivos(); return; }
  if(sub==='presupuesto'){ renderPresupuesto(); return; }
  if(sub==='dashboard_admin'){ renderDashboardAdmin(); return; }
  if(sub==='panel_admin')     { renderAdminPanel(); return; }
  if(sub==='codigos')         { renderCodigos(); return; }
  if(sub==='autolock')        { abrirConfigAutolock(); return; }
  if(sub==='config_nip')      { goTab('mas',document.querySelectorAll('.nb')[4]); setTimeout(function(){ goSub('config'); setTimeout(abrirConfigNip,120); },80); return; }
  // ── Rutas adicionales ──
  if(sub==='gastos')          { _renderMainContent(renderGastos()); return; }
  if(sub==='compras')         { _renderMainContent(renderCompras()); return; }
  if(sub==='pagos')           { _renderMainContent(renderPagos()); return; }
  if(sub==='servicios')       { _renderMainContent(renderServicios()); return; }
  if(sub==='ingresos')        { _renderMainContent(renderIngresos()); return; }
  if(sub==='noticias_admin')  { _renderMainContent(renderNoticiasAdmin()); return; }
  var fn = renders[sub];
  if(fn){
    var _mc = document.getElementById('mainContent');
    _mc.style.cssText += ';opacity:0;transform:translateY(6px);transition:none;';
    _mc.innerHTML = fn();
    requestAnimationFrame(function(){ requestAnimationFrame(function(){
      _mc.style.transition = 'opacity 0.24s ease,transform 0.24s cubic-bezier(0.16,1,0.3,1)';
      _mc.style.opacity = '1'; _mc.style.transform = 'translateY(0)';
    }); });
  }
}

function _renderMainContent(htmlStr){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  mc.style.cssText += ';opacity:0;transform:translateY(6px);transition:none;';
  mc.innerHTML = htmlStr;
  requestAnimationFrame(function(){ requestAnimationFrame(function(){
    mc.style.transition = 'opacity 0.22s ease,transform 0.22s cubic-bezier(0.16,1,0.3,1)';
    mc.style.opacity = '1'; mc.style.transform = 'translateY(0)';
  }); });
}

function renderReportes(){
  var txs = getTxs();
  var ing = txs.filter(function(t){ return t.tipo==='ingreso'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var gas = txs.filter(function(t){ return t.tipo==='gasto'; }).reduce(function(s,t){ return s+Number(t.monto); },0);
  var bal = ing - gas;
  var mesAct = new Date().toISOString().slice(0,7);
  var porCat = {};
  txs.filter(function(t){ return t.tipo==='gasto'; }).forEach(function(t){
    porCat[t.cat] = (porCat[t.cat]||0) + Number(t.monto);
  });
  var cats = Object.keys(porCat).sort(function(a,b){ return porCat[b]-porCat[a]; }).slice(0,6);
  var maxCat = cats.length ? Math.max.apply(null, cats.map(function(c){ return porCat[c]; })) : 1;
  var barChart = cats.length ? (
    '<div class="bar-chart">'
    + cats.map(function(c){
        var h = Math.max(8, Math.round((porCat[c]/maxCat)*80));
        var pct = gas>0?Math.round((porCat[c]/gas)*100):0;
        return '<div class="bar-col">'
          +'<div class="bar-fill danger" style="height:'+h+'px;" title="'+c+': '+fmt(porCat[c])+'"></div>'
          +'<div class="bar-lbl">'+c.slice(0,5)+'</div>'
          +'</div>';
      }).join('')
    +'</div>'
  ) : '';
  var catItems = cats.map(function(cat){
    var pct = gas>0 ? Math.round((porCat[cat]/gas)*100) : 0;
    return '<div style="margin-bottom:12px;">'
      +'<div style="display:flex;justify-content:space-between;font-size:0.82rem;margin-bottom:5px;">'
      +'<span style="font-weight:700;color:var(--text);">'+cat+'</span>'
      +'<span style="font-weight:800;color:var(--danger);font-family:JetBrains Mono,monospace;">'+fmt(porCat[cat])+' <span style="font-weight:500;color:var(--dim);font-family:Outfit,sans-serif;">'+pct+'%</span></span>'
      +'</div>'
      +'<div class="prog-wrap"><div class="prog-bar danger" style="width:'+pct+'%;background:var(--danger);opacity:0.8;"></div></div>'
      +'</div>';
  }).join('') || '<div style="color:var(--dim);font-size:0.82rem;text-align:center;padding:20px;">Sin gastos registrados</div>';
  var meses6 = [];
  for(var i=5;i>=0;i--){
    var d=new Date(); d.setMonth(d.getMonth()-i);
    var m=d.toISOString().slice(0,7);
    var label=['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'][d.getMonth()];
    var g=txs.filter(function(t){ return t.tipo==='gasto'&&t.fecha&&t.fecha.slice(0,7)===m; }).reduce(function(s,t){ return s+Number(t.monto); },0);
    var ing2=txs.filter(function(t){ return t.tipo==='ingreso'&&t.fecha&&t.fecha.slice(0,7)===m; }).reduce(function(s,t){ return s+Number(t.monto); },0);
    meses6.push({m:m,label:label,gas:g,ing:ing2,act:m===mesAct});
  }
  var maxMes = Math.max.apply(null, meses6.map(function(m){ return Math.max(m.gas,m.ing); }))||1;
  var mesChart = '<div class="bar-chart" style="height:110px;">'
    + meses6.map(function(m){
        var hg = Math.max(4, Math.round((m.gas/maxMes)*90));
        var hi = Math.max(4, Math.round((m.ing/maxMes)*90));
        return '<div class="bar-col">'
          +'<div style="display:flex;gap:2px;align-items:flex-end;height:90px;">'
          +'<div class="bar-fill danger" style="height:'+hg+'px;flex:1;opacity:'+(m.act?1:0.5)+';"></div>'
          +'<div class="bar-fill" style="height:'+hi+'px;flex:1;opacity:'+(m.act?1:0.5)+';"></div>'
          +'</div>'
          +'<div class="bar-lbl" style="color:'+(m.act?'var(--text)':'var(--dim)')+';">'+m.label+'</div>'
          +'</div>';
    }).join('')
    +'</div>'
    +'<div style="display:flex;gap:14px;margin-top:8px;">'
    +'<div style="display:flex;align-items:center;gap:5px;font-size:0.68rem;color:var(--dim);"><div style="width:10px;height:10px;border-radius:3px;background:var(--danger);"></div>Gastos</div>'
    +'<div style="display:flex;align-items:center;gap:5px;font-size:0.68rem;color:var(--dim);"><div style="width:10px;height:10px;border-radius:3px;background:var(--accent);"></div>Ingresos</div>'
    +'</div>';
  return ''
    +'<div class="insight-row" style="margin-bottom:10px;">'
    +'<div class="insight-card accent">'
    +'<span class="insight-ico">💚</span>'
    +'<div class="insight-label">Ingresos totales</div>'
    +'<div class="insight-val" style="color:var(--accent2);">'+fmt(ing)+'</div>'
    +'</div>'
    +'<div class="insight-card danger">'
    +'<span class="insight-ico">🔥</span>'
    +'<div class="insight-label">Gastos totales</div>'
    +'<div class="insight-val" style="color:var(--danger);">'+fmt(gas)+'</div>'
    +'</div>'
    +'</div>'
    +'<div class="insight-card full" style="margin-bottom:16px;">'
    +'<div class="insight-label">Balance neto</div>'
    +'<div style="font-size:1.6rem;font-weight:900;color:'+(bal>=0?'var(--accent2)':'var(--danger)')+';">'+fmt(bal)+'</div>'
    +'<div class="insight-trend" style="color:var(--dim);">'+(bal>=0?'✅ Positivo — gastas menos de lo que ganas':'⚠️ Negativo — gastas más de lo que ingresas')+'</div>'
    +'</div>'
    +'<div class="sec-title">📅 Evolución 6 meses</div>'
    +'<div class="card">'+mesChart+'</div>'
    +'<div class="sec-title">📊 Gastos por categoría</div>'
    +'<div class="card">'
    + barChart
    + catItems
    +'</div>';
}

function kpi(label,val,ant,inv){
    var diff=ant!==null&&ant!==undefined?val-ant:null;
    var pct=(diff!==null&&ant!==0)?Math.round((diff/Math.abs(ant))*100):null;
    var sube=diff!==null?diff>0:null;
    var pos=inv?(sube===null?null:!sube):sube;
    var col=pos===null?'var(--dim)':pos?'#2d9e5f':'var(--danger)';
    var flecha=sube===null?'':sube?'↑':'↓';
    var d=document.createElement('div');
    d.style.cssText='background:var(--card);border-radius:14px;padding:12px 13px;border:1.5px solid var(--border);';
    d.innerHTML='<div style="font-size:0.67rem;color:var(--dim);font-weight:700;text-transform:uppercase;letter-spacing:0.04em;margin-bottom:4px;">'+label+'</div>'
      +'<div style="font-size:1.05rem;font-weight:900;color:var(--text);">'+fmt(val)+'</div>'
      +(diff!==null
        ?'<div style="font-size:0.7rem;margin-top:3px;color:'+col+';">'+flecha+' '+fmt(Math.abs(diff))+(pct!==null?' ('+Math.abs(pct)+'%)':'')+'</div>'
        :'<div style="font-size:0.7rem;color:var(--dim);margin-top:3px;">Primer registro</div>');
    return d;
  }

function renderConversor(){
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">💱 Conversor</div></div>'
    +'<div class="card">'
    +'<label class="inp-label">Monto</label><input class="inp" id="convMonto" type="number" placeholder="0.00" oninput="convertir()">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">De</label><select class="inp" id="convDe" onchange="convertir()"><option value="1">MXN</option><option value="0.05">USD</option><option value="0.046">EUR</option><option value="7.8">CNY</option></select></div>'
    +'<div><label class="inp-label">A</label><select class="inp" id="convA" onchange="convertir()"><option value="0.05">USD</option><option value="1">MXN</option><option value="0.046">EUR</option><option value="7.8">CNY</option></select></div>'
    +'</div>'
    +'<div id="convResult" style="text-align:center;padding:16px;font-size:1.6rem;font-weight:900;color:var(--accent);font-family:\'JetBrains Mono\',monospace;"></div>'
    +'<div style="font-size:0.65rem;color:var(--dim);text-align:center;">Tasas aproximadas de referencia</div>'
    +'</div>';
}

function convertir(){
  var m=parseFloat(document.getElementById('convMonto').value)||0;
  var de=parseFloat(document.getElementById('convDe').value);
  var a=parseFloat(document.getElementById('convA').value);
  var res=(m/de)*a;
  document.getElementById('convResult').textContent=res.toLocaleString('es-MX',{minimumFractionDigits:2,maximumFractionDigits:4});
}

function renderMetas(){
  var metas=load('metas',[]);
  var items=metas.length?metas.map(function(m,i){
    var pct=m.meta>0?Math.min(100,Math.round((m.actual/m.meta)*100)):0;
    return '<div class="card" style="margin-bottom:8px;">'
      +'<div style="display:flex;justify-content:space-between;margin-bottom:6px;"><div style="font-weight:700;">'+m.nombre+'</div><span style="font-size:0.75rem;color:var(--dim);">'+pct+'%</span></div>'
      +'<div class="prog-wrap"><div class="prog-bar" style="width:'+pct+'%;'+(pct>=100?'background:#2d9e5f;':'')+'"></div></div>'
      +'<div style="display:flex;justify-content:space-between;font-size:0.72rem;color:var(--dim);margin-top:5px;margin-bottom:10px;"><span>'+fmt(m.actual)+'</span><span>Meta: '+fmt(m.meta)+'</span></div>'
      +'<div style="display:flex;gap:6px;">'
      +'<button class="cred-btn success" style="flex:2;" onclick="abonarMeta('+i+')">+ Abonar</button>'
      +'<button class="cred-btn" onclick="editarMeta('+i+')">✏️</button>'
      +'<button class="cred-btn danger" onclick="borrarMeta('+i+')">🗑️</button>'
      +'</div></div>';
  }).join(''):'<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin metas aún</div>';
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">🎯 Metas de Ahorro</div></div>'
    +'<div class="card" style="margin-bottom:14px;">'
    +'<label class="inp-label">Nombre de la meta</label><input class="inp" id="metaNombre" placeholder="Ej: Fondo de emergencia">'
    +'<div class="form-row"><div><label class="inp-label">Objetivo ($)</label><input class="inp" id="metaObjetivo" type="number" placeholder="0.00"></div><div><label class="inp-label">Ya tengo ($)</label><input class="inp" id="metaActual" type="number" placeholder="0.00"></div></div>'
    +'<button class="btn-main" onclick="guardarMeta()">+ Agregar meta</button>'
    +'</div>'+items;
}

function guardarMeta(){
  var n=document.getElementById('metaNombre').value.trim();
  var o=parseFloat(document.getElementById('metaObjetivo').value);
  var a=parseFloat(document.getElementById('metaActual').value)||0;
  if(!n||!o){ showToast('⚠ Completa nombre y objetivo'); return; }
  var m=load('metas',[]); m.push({nombre:n,meta:o,actual:a}); save('metas',m);
  showToast('✓ Meta agregada'); goSub('metas');
}

function borrarMeta(i){ var m=load('metas',[]); var e=m[i]; m.splice(i,1); save('metas',m); goSub('metas'); mostrarUndo('Meta eliminada',function(){ var m2=load('metas',[]); m2.splice(i,0,e); save('metas',m2); goSub('metas'); }); }

function renderAlertas(){
  var alertas=load('alertas',[]);
  var txs=getTxs();
  var items=alertas.length?alertas.map(function(a,i){
    var gastado=txs.filter(function(t){ return t.tipo==='gasto' && t.cat===a.nombre; }).reduce(function(s,t){ return s+Number(t.monto); },0);
    var pct=a.limite>0?Math.min(100,Math.round((gastado/a.limite)*100)):0;
    var color=pct>=100?'var(--danger)':pct>=75?'#f59e0b':'var(--accent2)';
    return '<div class="card" style="margin-bottom:10px;padding:14px;">'
      +'<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;">'
      +'<div style="font-weight:800;font-size:0.9rem;">'+(pct>=100?'🔴':pct>=75?'⚡':'🟢')+' '+a.nombre+'</div>'
      +'<div style="display:flex;gap:6px;">'
      +'<button class="ic-btn" onclick="editarAlerta('+i+')">✏️</button>'
      +'<button class="ic-btn" onclick="borrarAlerta('+i+')">🗑️</button>'
      +'</div></div>'
      +'<div style="font-size:0.75rem;color:var(--dim);margin-bottom:6px;">'+fmt(gastado)+' de '+fmt(a.limite)+' · Vence: '+a.fecha+'</div>'
      +'<div style="background:rgba(0,0,0,0.08);border-radius:8px;height:7px;overflow:hidden;">'
      +'<div style="height:100%;border-radius:8px;background:'+color+';width:'+pct+'%;transition:width 0.4s;"></div></div>'
      +'</div>';
  }).join(''):'<div style="text-align:center;padding:20px;color:var(--dim);font-size:0.83rem;">Sin alertas configuradas</div>';
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">🔔 Alertas de Gasto</div></div>'
    +'<div class="card" style="margin-bottom:14px;" id="alertaForm">'
    +'<div class="card-title">+ Nueva alerta</div>'
    +'<label class="inp-label">Nombre / Categoría a vigilar</label>'
    +'<input class="inp" id="alNombre" placeholder="Ej: Alimentación, Entretenimiento...">'
    +'<div class="form-row">'
    +'<div><label class="inp-label">Límite ($)</label><input class="inp" id="alLimite" type="number" inputmode="decimal" placeholder="0.00"></div>'
    +'<div><label class="inp-label">Fecha límite</label><input class="inp" id="alFecha" type="date" value="'+today()+'"></div>'
    +'</div>'
    +'<button class="btn-main" id="alSaveBtn" onclick="guardarAlerta()">+ Agregar alerta</button>'
    +'</div>'+items;
}

function guardarAlerta(){
  var n=document.getElementById('alNombre').value.trim();
  var l=parseFloat(document.getElementById('alLimite').value);
  var f=document.getElementById('alFecha').value;
  if(!n||!l||!f){ showToast('⚠ Completa todos los campos'); return; }
  var alertas=load('alertas',[]);
  if(window._editAlerta!==undefined){
    alertas[window._editAlerta]=Object.assign(alertas[window._editAlerta],{nombre:n,limite:l,fecha:f});
    delete window._editAlerta; showToast('✓ Alerta actualizada');
  } else {
    alertas.push({nombre:n,limite:l,fecha:f,activa:true});
    showToast('✓ Alerta guardada');
  }
  save('alertas',alertas); goSub('alertas');
}

function borrarAlerta(i){ var a=load('alertas',[]); var e=a[i]; a.splice(i,1); save('alertas',a); goSub('alertas'); mostrarUndo('Alerta eliminada',function(){ var a2=load('alertas',[]); a2.splice(i,0,e); save('alertas',a2); goSub('alertas'); }); }

function renderPresupuesto(){
  var mc = document.getElementById('mainContent');
  if(!mc) return;
  mc.innerHTML = '';
  var pres    = load('presupuesto', {});
  var mesAct  = new Date().toISOString().slice(0,7);
  var txs     = getTxs().filter(function(t){
    return t.tipo==='gasto' && t.fecha && t.fecha.slice(0,7)===mesAct;
  });
  var cats = getPresCats();
  var totalLimite = 0, totalGastado = 0;
  var catData = cats.map(function(c){
    var lim = pres[c.id] || 0;
    var gas = txs.filter(function(t){ return t.cat === c.id; })
                 .reduce(function(s,t){ return s + Number(t.monto||0); }, 0);
    totalLimite  += lim;
    totalGastado += gas;
    var pct    = lim>0 ? Math.min(100, Math.round((gas/lim)*100)) : (gas>0?100:0);
    var estado = lim===0 ? 'sin-limite' : pct>=100 ? 'excedido' : pct>=80 ? 'alerta' : 'ok';
    return { id:c.id, color:c.color||'#78909c', lim:lim, gas:gas, pct:pct, estado:estado };
  });
  var conLimite = catData.filter(function(c){ return c.lim>0; }).length;
  var pctTotal  = totalLimite>0 ? Math.min(100, Math.round((totalGastado/totalLimite)*100)) : 0;
  var heroCol   = pctTotal>=100 ? '#e53935' : pctTotal>=80 ? '#f57c00' : '#2d9e5f';
  var libre     = totalLimite - totalGastado;
  var mesLabel = new Date(mesAct+'-02').toLocaleString('es-MX',{month:'long',year:'numeric'});
  mesLabel = mesLabel.charAt(0).toUpperCase() + mesLabel.slice(1);
  var hdr = document.createElement('div');
  hdr.innerHTML = '<div class="page-header">'+backBtn('mas',4)
    +'<div class="page-title">🗂️ Presupuesto Mensual</div></div>';
  mc.appendChild(hdr);
  var hero = document.createElement('div');
  hero.style.cssText = 'border-radius:20px;padding:20px;margin-bottom:14px;'
    +'background:linear-gradient(135deg,var(--card) 0%,var(--inp) 100%);'
    +'border:1.5px solid var(--border);position:relative;overflow:hidden;';
  hero.innerHTML =
     '<div style="position:absolute;top:-24px;right:-24px;width:110px;height:110px;border-radius:50%;background:'+heroCol+';opacity:0.08;"></div>'
    +'<div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:12px;">'
      +'<div>'
        +'<div style="font-size:0.68rem;font-weight:800;text-transform:uppercase;letter-spacing:0.09em;color:var(--dim);margin-bottom:4px;">'+mesLabel+'</div>'
        +'<div style="font-size:1.7rem;font-weight:900;color:var(--text);line-height:1;">'+fmt(totalGastado)+'</div>'
        +'<div style="font-size:0.73rem;color:var(--dim);margin-top:3px;">de <b>'+fmt(totalLimite)+'</b> presupuestado</div>'
      +'</div>'
      +'<div style="text-align:right;">'
        +'<div style="font-size:2.2rem;font-weight:900;color:'+heroCol+';line-height:1;">'+pctTotal+'%</div>'
        +'<div style="font-size:0.68rem;color:var(--dim);">usado</div>'
      +'</div>'
    +'</div>'
    +'<div style="background:var(--border);border-radius:999px;height:8px;margin-bottom:12px;overflow:hidden;">'
      +'<div style="height:100%;border-radius:999px;background:'+heroCol+';width:'+pctTotal+'%;"></div>'
    +'</div>'
    +'<div style="display:flex;gap:20px;flex-wrap:wrap;">'
      +(totalLimite>0 ? '<div style="font-size:0.72rem;"><span style="color:var(--dim);">Libre: </span>'
        +'<b style="color:'+heroCol+';">'+fmt(Math.max(0,libre))+'</b></div>' : '')
      +'<div style="font-size:0.72rem;"><span style="color:var(--dim);">Con límite: </span>'
        +'<b>'+conLimite+' / '+cats.length+'</b></div>'
    +'</div>';
  mc.appendChild(hero);
  if(conLimite === 0){
    var empty = document.createElement('div');
    empty.style.cssText = 'text-align:center;padding:28px 20px;background:var(--card);border-radius:16px;border:1.5px dashed var(--border);margin-bottom:12px;';
    empty.innerHTML = '<div style="font-size:2rem;margin-bottom:8px;">🎯</div>'
      +'<div style="font-weight:800;margin-bottom:6px;">Sin límites configurados</div>'
      +'<div style="font-size:0.78rem;color:var(--dim);">Escribe un límite en cada categoría<br>para empezar a controlar tus gastos</div>';
    mc.appendChild(empty);
  }
  var excedidos  = catData.filter(function(c){ return c.estado==='excedido'; });
  var enAlerta   = catData.filter(function(c){ return c.estado==='alerta'; });
  if(excedidos.length || enAlerta.length){
    var ab = document.createElement('div');
    ab.style.cssText = 'border-radius:14px;padding:12px 14px;margin-bottom:12px;'
      +'background:rgba(229,57,53,0.06);border:1.5px solid rgba(229,57,53,0.22);';
    var msgs = excedidos.map(function(c){
      return '<span style="color:#e53935;font-weight:700;">⚠️ '+c.id+' ('+c.pct+'%)</span>';
    }).concat(enAlerta.map(function(c){
      return '<span style="color:#f57c00;font-weight:700;">🔶 '+c.id+' ('+c.pct+'%)</span>';
    }));
    ab.innerHTML = '<div style="font-size:0.75rem;line-height:2;">'+msgs.join(' &nbsp;·&nbsp; ')+'</div>';
    mc.appendChild(ab);
  }
  var lbl = document.createElement('div');
  lbl.style.cssText = 'font-size:0.68rem;font-weight:800;text-transform:uppercase;'
    +'letter-spacing:0.08em;color:var(--dim);margin-bottom:8px;';
  lbl.textContent = 'Control por categoría';
  mc.appendChild(lbl);
  catData.forEach(function(c){
    var borderCol = c.estado==='excedido' ? '#e53935'
                  : c.estado==='alerta'   ? '#f57c00'
                  : c.estado==='ok'       ? c.color
                  : 'var(--border)';
    var card = document.createElement('div');
    card.style.cssText = 'background:var(--card);border-radius:16px;padding:14px 16px;'
      +'margin-bottom:8px;border:1.5px solid var(--border);border-left:3.5px solid '+borderCol+';';
    var topRow = document.createElement('div');
    topRow.style.cssText = 'display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;';
    var nameEl = document.createElement('div');
    nameEl.style.cssText = 'font-weight:700;font-size:0.9rem;';
    nameEl.textContent = c.id;
    var badge = document.createElement('div');
    badge.style.cssText = 'font-size:0.7rem;font-weight:800;padding:2px 8px;border-radius:20px;'
      +'background:'+borderCol+'22;color:'+borderCol+';white-space:nowrap;';
    badge.textContent = c.lim>0 ? c.pct+'%' : (c.gas>0 ? fmt(c.gas) : 'Sin límite');
    topRow.appendChild(nameEl);
    topRow.appendChild(badge);
    card.appendChild(topRow);
    var botRow = document.createElement('div');
    botRow.style.cssText = 'display:flex;justify-content:space-between;align-items:center;'
      +'font-size:0.75rem;color:var(--dim);margin-bottom:'+(c.lim>0?'8':'0')+'px;';
    var gasEl = document.createElement('span');
    gasEl.innerHTML = 'Gastado: <b style="color:var(--text);">'+fmt(c.gas)+'</b>';
    var limWrap = document.createElement('div');
    limWrap.style.cssText = 'display:flex;align-items:center;gap:5px;';
    var limLbl = document.createElement('span');
    limLbl.textContent = 'Límite:';
    var inp = document.createElement('input');
    inp.type = 'number'; inp.min = '0';
    inp.value = c.lim || '';
    inp.placeholder = '—';
    inp.style.cssText = 'width:82px;padding:4px 8px;background:var(--inp);'
      +'border:1px solid var(--border);border-radius:8px;'
      +'font-family:\'Outfit\',sans-serif;font-size:0.76rem;color:var(--text);text-align:right;';
    (function(catId){
      inp.onchange = function(){
        var p = load('presupuesto',{});
        p[catId] = parseFloat(this.value) || 0;
        save('presupuesto', p);
        showToast('✓ Límite guardado');
        renderPresupuesto();
      };
    })(c.id);
    limWrap.appendChild(limLbl);
    limWrap.appendChild(inp);
    botRow.appendChild(gasEl);
    botRow.appendChild(limWrap);
    card.appendChild(botRow);
    if(c.lim > 0){
      var barWrap = document.createElement('div');
      barWrap.style.cssText = 'background:var(--border);border-radius:999px;height:5px;overflow:hidden;';
      var bar = document.createElement('div');
      bar.style.cssText = 'height:100%;border-radius:999px;background:'+borderCol+';width:0%;'
        +'transition:width 0.6s cubic-bezier(.4,0,.2,1);';
      barWrap.appendChild(bar);
      card.appendChild(barWrap);
      setTimeout((function(b, pct){ return function(){ b.style.width = pct+'%'; }; })(bar, c.pct), 80);
    }
    mc.appendChild(card);
  });
  var tip = document.createElement('div');
  tip.style.cssText = 'text-align:center;padding:16px;font-size:0.73rem;color:var(--dim);';
  tip.innerHTML = '💡 Los gastos se clasifican automáticamente<br>según la categoría que eliges al registrarlos';
  mc.appendChild(tip);
}

function renderProgreso(){
  var mc=document.getElementById('mainContent');
  mc.innerHTML='';
  var hdr=document.createElement('div');
  hdr.innerHTML='<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">📈 Mi Progreso Financiero</div></div>';
  mc.appendChild(hdr);
  var mes=new Date().toISOString().slice(0,7);
  var key=_snapKey()+mes;
  localStorage.removeItem(key);
  _forzarSnapshot(mes, key);
  var snaps=getSnapshots();
  var ultimo=snaps.length?snaps[snaps.length-1]:null;
  var penultimo=snaps.length>1?snaps[snaps.length-2]:null;
  if(!ultimo){
    var empty=document.createElement('div'); empty.className='card';
    empty.innerHTML='<div style="text-align:center;padding:24px;color:var(--dim);font-size:0.85rem;">Sin datos todavía.<br>Agrega cuentas o transacciones y regresa aquí.</div>';
    mc.appendChild(empty); return;
  }
  var score=0;
  if(penultimo){
    if(ultimo.patrimonioNeto>penultimo.patrimonioNeto) score++;
    if(ultimo.totalDeudas<penultimo.totalDeudas) score++;
    if(ultimo.ingresos>ultimo.gastos) score++;
  } else {
    if(ultimo.patrimonioNeto>0) score++;
    if(ultimo.ingresos>ultimo.gastos) score++;
    score=Math.min(score,2);
  }
  var si=score>=3
    ?{emoji:'🟢',label:'Progresando',  color:'#2d9e5f', bg:'rgba(45,158,95,0.08)'}
    :score>=2
    ?{emoji:'🟡',label:'Estable',      color:'#e07b00', bg:'rgba(224,123,0,0.08)'}
    :{emoji:'🔴',label:'Atención',     color:'var(--danger)',bg:'rgba(229,57,53,0.08)'};
  var salud=document.createElement('div');
  salud.style.cssText='border-radius:16px;padding:14px 16px;margin-bottom:12px;background:'+si.bg+';border:1.5px solid '+si.color+';';
  salud.innerHTML='<div style="display:flex;align-items:center;gap:12px;">'
    +'<div style="font-size:2rem;">'+si.emoji+'</div>'
    +'<div><div style="font-size:1rem;font-weight:900;color:'+si.color+';">'+si.label+'</div>'
    +'<div style="font-size:0.74rem;color:var(--dim);margin-top:2px;">Salud financiera · '+new Date().toLocaleString('es-MX',{month:'long',year:'numeric'})+'</div></div></div>';
  mc.appendChild(salud);
  
  var grid=document.createElement('div');
  grid.style.cssText='display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:12px;';
  var p=penultimo;
  grid.appendChild(kpi('🏛 Patrimonio neto', ultimo.patrimonioNeto, p?p.patrimonioNeto:null, false));
  grid.appendChild(kpi('💰 Efectivo+Banco',  ultimo.efectivo+ultimo.banco, p?p.efectivo+p.banco:null, false));
  grid.appendChild(kpi('🔴 Total deudas',    ultimo.totalDeudas, p?p.totalDeudas:null, true));
  grid.appendChild(kpi('🏦 Activos',         ultimo.totalActivos, p?p.totalActivos:null, false));
  grid.appendChild(kpi('📥 Ingresos mes',    ultimo.ingresos, p?p.ingresos:null, false));
  grid.appendChild(kpi('📤 Gastos mes',      ultimo.gastos, p?p.gastos:null, true));
  mc.appendChild(grid);
  var ultimos6=snaps.slice(-6);
  if(ultimos6.length>=1){
    var secG=document.createElement('div'); secG.className='card'; secG.style.marginBottom='12px';
    var titG=document.createElement('div'); titG.style.cssText='font-size:0.8rem;font-weight:800;margin-bottom:10px;'; titG.textContent='📈 Evolución del Patrimonio Neto';
    secG.appendChild(titG);
    var vals=ultimos6.map(function(s){ return s.patrimonioNeto; });
    var minV=Math.min.apply(null,vals), maxV=Math.max.apply(null,vals);
    var rango=maxV-minV||1;
    var W=300,H=90,px=12,py=10;
    var n=ultimos6.length;
    var pts=vals.map(function(v,i){
      var x=n>1?px+(i/(n-1))*(W-2*px):W/2;
      var y=H-py-((v-minV)/rango)*(H-2*py);
      return x.toFixed(1)+','+y.toFixed(1);
    }).join(' ');
    var lc=vals[vals.length-1]>=vals[0]?'#2d9e5f':'#e53935';
    var svg='<svg viewBox="0 0 '+W+' '+H+'" style="width:100%;height:90px;overflow:visible;">';
    if(minV<0&&maxV>0){
      var yz=H-py-((-minV)/rango)*(H-2*py);
      svg+='<line x1="'+px+'" y1="'+yz.toFixed(1)+'" x2="'+(W-px)+'" y2="'+yz.toFixed(1)+'" stroke="var(--border)" stroke-width="1" stroke-dasharray="4,3"/>';
    }
    if(n>1) svg+='<polyline points="'+pts+'" fill="none" stroke="'+lc+'" stroke-width="2.5" stroke-linejoin="round" stroke-linecap="round"/>';
    vals.forEach(function(v,i){
      var x=n>1?px+(i/(n-1))*(W-2*px):W/2;
      var y=H-py-((v-minV)/rango)*(H-2*py);
      svg+='<circle cx="'+x.toFixed(1)+'" cy="'+y.toFixed(1)+'" r="4" fill="'+lc+'" stroke="var(--card)" stroke-width="1.5"/>';
      var anchor=i===0?'start':i===n-1?'end':'middle';
      svg+='<text x="'+x.toFixed(1)+'" y="'+(y-7).toFixed(1)+'" text-anchor="'+anchor+'" font-size="8" fill="var(--dim)">'+fmt(v)+'</text>';
    });
    svg+='</svg>';
    var labelsRow=document.createElement('div');
    labelsRow.style.cssText='display:flex;justify-content:space-between;font-size:0.63rem;color:var(--dim);margin-top:2px;';
    ultimos6.forEach(function(s){
      var sp=document.createElement('span');
      sp.textContent=new Date(s.mes+'-02').toLocaleString('es-MX',{month:'short',year:'2-digit'});
      labelsRow.appendChild(sp);
    });
    secG.innerHTML+=svg;
    secG.appendChild(labelsRow);
    mc.appendChild(secG);
  }
  var secT=document.createElement('div'); secT.className='card'; secT.style.marginBottom='12px';
  var titT=document.createElement('div'); titT.style.cssText='font-size:0.8rem;font-weight:800;margin-bottom:10px;'; titT.textContent='📋 Historial mes a mes';
  secT.appendChild(titT);
  snaps.slice(-6).reverse().forEach(function(s){
    var idx2=snaps.indexOf(s);
    var prev=idx2>0?snaps[idx2-1]:null;
    var diff2=prev?s.patrimonioNeto-prev.patrimonioNeto:null;
    var col2=diff2===null?'var(--dim)':diff2>=0?'#2d9e5f':'var(--danger)';
    var fl2=diff2===null?'':diff2>=0?' ↑':' ↓';
    var mesLabel=new Date(s.mes+'-02').toLocaleString('es-MX',{month:'long',year:'numeric'});
    mesLabel=mesLabel.charAt(0).toUpperCase()+mesLabel.slice(1);
    var fila=document.createElement('div');
    fila.style.cssText='padding:9px 0;border-bottom:1px solid var(--border);font-size:0.75rem;';
    fila.innerHTML='<div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:4px;">'
      +'<span style="font-weight:700;">'+mesLabel+'</span>'
      +'<span style="color:'+col2+';font-weight:800;">'+fmt(s.patrimonioNeto)+fl2+'</span>'
      +'</div>'
      +'<div style="display:flex;gap:10px;color:var(--dim);flex-wrap:wrap;">'
      +'<span>💰 '+fmt(s.efectivo+s.banco)+'</span>'
      +'<span style="color:var(--danger);">🔴 '+fmt(s.totalDeudas)+'</span>'
      +'<span style="color:var(--accent2);">🏦 '+fmt(s.totalActivos)+'</span>'
      +'<span>📥 '+fmt(s.ingresos)+'</span>'
      +'<span>📤 '+fmt(s.gastos)+'</span>'
      +'</div>';
    secT.appendChild(fila);
  });
  mc.appendChild(secT);
  var bSnap=document.createElement('button');
  bSnap.style.cssText='width:100%;padding:12px;background:var(--inp);color:var(--text);border:1.5px solid var(--border);border-radius:12px;font-family:\'Outfit\',sans-serif;font-weight:700;cursor:pointer;margin-bottom:14px;font-size:0.85rem;';
  bSnap.textContent='🔄 Actualizar datos ahora';
  bSnap.onclick=function(){
    var m2=new Date().toISOString().slice(0,7);
    localStorage.removeItem(_snapKey()+m2);
    _forzarSnapshot(m2,_snapKey()+m2);
    showToast('✓ Datos actualizados');
    renderProgreso();
  };
  mc.appendChild(bSnap);
}

function renderActivos(){
  var mc = document.getElementById('mainContent');
  mc.innerHTML = '';
  var activos = load('activos_personales',[]);
  var totalActivos = activos.reduce(function(s,a){ return s+(a.valor||0); },0);
  var hdr = document.createElement('div');
  hdr.innerHTML = '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">🏦 Mis Activos</div></div>';
  mc.appendChild(hdr);
  var res = document.createElement('div');
  res.className='card'; res.style.marginBottom='10px';
  res.innerHTML = '<div style="display:flex;justify-content:space-between;align-items:center;">'
    +'<div><div style="font-size:0.75rem;color:var(--dim);">Valor total de activos</div>'
    +'<div style="font-size:1.5rem;font-weight:900;color:var(--accent2);">'+fmt(totalActivos)+'</div></div>'
    +'<div style="font-size:2rem;">🏦</div></div>';
  mc.appendChild(res);
  var bAdd = document.createElement('button');
  bAdd.style.cssText='width:100%;padding:13px;background:var(--accent);color:var(--navtext);border:none;border-radius:12px;font-family:\'Outfit\',sans-serif;font-weight:700;cursor:pointer;margin-bottom:14px;font-size:0.95rem;';
  bAdd.textContent='+ Registrar activo';
  bAdd.onclick=function(){ renderFormActivo(null); };
  mc.appendChild(bAdd);
  if(!activos.length){
    var empty=document.createElement('div');
    empty.style.cssText='text-align:center;padding:30px;color:var(--dim);font-size:0.83rem;';
    empty.textContent='Sin activos registrados. Agrega casa, carro, inversiones, etc.';
    mc.appendChild(empty); return;
  }
  var grupos={};
  activos.forEach(function(a){ var c=a.categoria||'📦 Otros'; if(!grupos[c]) grupos[c]=[]; grupos[c].push(a); });
  getActivosCats().forEach(function(cat){
    if(!grupos[cat]) return;
    var tit=document.createElement('div');
    tit.style.cssText='font-size:0.72rem;font-weight:800;color:var(--dim);text-transform:uppercase;letter-spacing:0.06em;margin:10px 0 6px;';
    tit.textContent=cat; mc.appendChild(tit);
    grupos[cat].forEach(function(a){
      var idx=activos.indexOf(a);
      var card=document.createElement('div');
      card.style.cssText='background:var(--card);border-radius:14px;padding:12px 14px;margin-bottom:8px;border:1.5px solid var(--border);';
      var row=document.createElement('div');
      row.style.cssText='display:flex;justify-content:space-between;align-items:flex-start;';
      var left=document.createElement('div'); left.style.flex='1';
      var nom=document.createElement('div'); nom.style.cssText='font-weight:700;font-size:0.9rem;'; nom.textContent=a.nombre; left.appendChild(nom);
      var meta=document.createElement('div'); meta.style.cssText='font-size:0.72rem;color:var(--dim);margin-top:2px;';
      meta.textContent=(a.descripcion||'')+(a.fecha?' · Desde '+a.fecha:''); left.appendChild(meta);
      var right=document.createElement('div'); right.style.cssText='display:flex;flex-direction:column;align-items:flex-end;gap:6px;';
      var val=document.createElement('div'); val.style.cssText='font-weight:800;font-size:0.95rem;color:var(--accent2);'; val.textContent=fmt(a.valor); right.appendChild(val);
      var btns=document.createElement('div'); btns.style.cssText='display:flex;gap:5px;';
      var bEd=document.createElement('button'); bEd.style.cssText='border:1px solid var(--border);border-radius:8px;padding:4px 8px;font-size:0.75rem;cursor:pointer;background:none;color:var(--accent);'; bEd.textContent='✏️';
      (function(i_){ bEd.onclick=function(){ renderFormActivo(i_); }; })(idx); btns.appendChild(bEd);
      var bDel=document.createElement('button'); bDel.style.cssText='border:1px solid rgba(229,57,53,0.3);border-radius:8px;padding:4px 8px;font-size:0.75rem;cursor:pointer;background:none;color:var(--danger);'; bDel.textContent='🗑';
      (function(i_){ bDel.onclick=function(){ borrarActivo(i_); }; })(idx); btns.appendChild(bDel);
      right.appendChild(btns); row.appendChild(left); row.appendChild(right); card.appendChild(row); mc.appendChild(card);
    });
  });
}

function borrarActivo(i){
  var aa=load('activos_personales',[]);
  if(!aa[i]) return;
  var eli=JSON.parse(JSON.stringify(aa[i]));
  aa.splice(i,1); save('activos_personales',aa);
  renderActivos();
  mostrarUndo('🏦 '+eli.nombre+' eliminado', function(){
    var aa2=load('activos_personales',[]); aa2.splice(i,0,eli); save('activos_personales',aa2); renderActivos();
  });
}

function renderConsejero(ing, gas, debo, totalDisp, pn){
  var nombre = S && S.user && S.user.nombre ? S.user.nombre.split(' ')[0] : 'tú';
  var balance      = ing - gas;           // flujo neto del periodo
  var balanceLibre = ing - gas - debo;    // flujo descontando deudas
  var tasaAhorro = ing > 0 ? (balance / ing) * 100 : (balance > 0 ? 100 : -100);
  var cargaDeuda = ing > 0 ? (debo / ing) * 100 : (debo > 0 ? 999 : 0);
  var cobertura = gas > 0 ? (totalDisp / gas) : (totalDisp > 0 ? 3 : 0);
  var puntos = 0;
  if(tasaAhorro >= 20)       puntos += 45;
  else if(tasaAhorro >= 10)  puntos += 32;
  else if(tasaAhorro >= 1)   puntos += 18;
  else if(tasaAhorro >= -10) puntos += 8;
  else                       puntos += 0;  // gasta mucho más de lo que gana
  if(cargaDeuda === 0)       puntos += 35;
  else if(cargaDeuda < 20)   puntos += 28;
  else if(cargaDeuda < 50)   puntos += 18;
  else if(cargaDeuda < 100)  puntos += 8;
  else                       puntos += 0;  // debe más de lo que gana
  if(cobertura >= 3)         puntos += 20;
  else if(cobertura >= 1)    puntos += 13;
  else if(cobertura >= 0.5)  puntos += 6;
  else                       puntos += 0;
  puntos = Math.min(100, Math.round(puntos));
  var expresion, colorBarra, tituloCard, mensaje, chips;
  if(puntos >= 78){
    expresion  = 'feliz';
    colorBarra = 'linear-gradient(90deg,#2bc070,#52d48e)';
    tituloCard = '¡Flujo de dinero sano! 🏆';
    mensaje    = '¡Excelente manejo, '+nombre+'! '
      + 'Tus ingresos superan tus gastos por '+fmt(balance)+' '
      + 'y tu carga de deuda es '+(cargaDeuda===0?'cero':'del '+Math.round(cargaDeuda)+'% de tus ingresos')+'. '
      + (cobertura >= 2 ? 'Tienes cobertura para ~'+Math.round(cobertura)+' meses sin ingresos. ' : '')
      + (balanceLibre > 0 ? '¡Con '+fmt(balanceLibre)+' libres podrías considerar invertir! 🚀' : '');
    chips = [
      {label:'Ahorro '+Math.round(Math.max(0,tasaAhorro))+'%', cls:'chip-verde'},
      debo===0 ? {label:'Sin deudas 🎉', cls:'chip-verde'} : {label:'Deuda manejable', cls:'chip-gold'},
      balanceLibre > 0 ? {label:'Invertir posible', cls:'chip-azul'} : null,
    ];
  } else if(puntos >= 55){
    expresion  = 'contento';
    colorBarra = 'linear-gradient(90deg,#3dbf7a,#ffb340)';
    tituloCard = 'Buen camino 👍';
    mensaje    = '¡Vas bien, '+nombre+'! '
      + (balance >= 0 ? 'Tu flujo es positivo: ingresas '+fmt(ing)+' y gastas '+fmt(gas)+'. '
                      : 'Tus gastos ('+fmt(gas)+') superan ligeramente tus ingresos ('+fmt(ing)+'). ')
      + (debo > 0 ? 'Tienes deudas por '+fmt(debo)+' — abónalas antes de gastar en extras. ' : '')
      + 'Con disciplina puedes llegar a una tasa de ahorro del 20%. 💪';
    chips = [
      {label:'Balance '+fmt(balance), cls: balance>=0?'chip-verde':'chip-rojo'},
      debo>0 ? {label:'Reduce deuda: '+fmt(debo), cls:'chip-gold'} : {label:'Sin deudas 🎉', cls:'chip-verde'},
      {label:'Meta: ahorro 20%', cls:'chip-azul'},
    ];
  } else if(puntos >= 28){
    expresion  = 'preocupado';
    colorBarra = 'linear-gradient(90deg,#ffb340,#ff6057)';
    tituloCard = 'Hay que ajustar ⚠️';
    mensaje    = (balance < 0
      ? '¡Cuidado, '+nombre+'! Gastaste '+fmt(Math.abs(balance))+' más de lo que ingresaste. '
      : 'Tu flujo es ajustado, '+nombre+'. Apenas queda '+fmt(balance)+' de margen. ')
      + (debo > 0 ? 'Más tus deudas de '+fmt(debo)+' — eso pesa fuerte. ' : '')
      + 'Detén gastos no esenciales esta semana y haz una lista de lo que debes. 🛑';
    chips = [
      balance < 0 ? {label:'Déficit '+fmt(Math.abs(balance)), cls:'chip-rojo'} : {label:'Margen ajustado', cls:'chip-gold'},
      debo > 0 ? {label:'Deuda: '+fmt(debo), cls:'chip-rojo'} : null,
      {label:'Cortar gastos ya', cls:'chip-gold'},
    ];
  } else {
    expresion  = 'triste';
    colorBarra = 'linear-gradient(90deg,#ff6057,#ff2010)';
    tituloCard = 'Flujo en rojo 🚨';
    mensaje    = '¡Necesitas actuar hoy, '+nombre+'! '
      + 'Gastas '+fmt(gas)+' pero solo ingresas '+fmt(ing)
      + (debo > 0 ? ', y además debes '+fmt(debo) : '')
      + '. Cada día que pasa el hoyo crece. '
      + 'Prioridad #1: detener el sangrado de gastos. Prioridad #2: generar un ingreso extra, aunque sea pequeño. ❤️';
    chips = [
      {label:'Déficit '+fmt(Math.abs(balance)), cls:'chip-rojo'},
      debo > 0 ? {label:'Deuda urgente: '+fmt(debo), cls:'chip-rojo'} : null,
      {label:'Plan de emergencia', cls:'chip-azul'},
    ];
  }
  var svg = _consejeroSVG(expresion);
  var chipsHtml = (chips||[]).filter(Boolean).map(function(c){
    return '<span class="consejero-chip '+c.cls+'">'+c.label+'</span>';
  }).join('');
  var barId = 'saludBar_' + Date.now();
  setTimeout(function(){
    var el = document.getElementById(barId);
    if(el) el.style.width = puntos + '%';
  }, 300);
  var nota = '<div style="font-size:0.68rem;color:var(--dim);margin-top:8px;padding:6px 10px;'
    +'background:rgba(0,0,0,0.05);border-radius:8px;border-left:2px solid var(--accent);">'
    +'ℹ️ Este análisis usa solo tu <b>flujo de dinero real</b> (ingresos, gastos y deudas). '
    +'El Patrimonio Neto <b>no se considera</b> para darte una lectura más honesta.'
    +'</div>';
  return '<div class="consejero-card" onclick="renderConsejeroDetalle()">'    +'<div class="consejero-avatar">'+svg+'</div>'    +'<div class="consejero-body">'    +'<div class="consejero-titulo">💡 Consejero Financiero</div>'    +'<div class="consejero-estado">'+tituloCard+'</div>'    +'<div class="consejero-msg">'+mensaje+'</div>'    +'<div class="consejero-chips">'+chipsHtml+'</div>'    +'<div style="margin-top:8px;">'    +'<div style="display:flex;justify-content:space-between;font-size:0.68rem;color:var(--dim);margin-bottom:4px;">'    +'<span>Salud de flujo (sin patrimonio)</span>'    +'<span style="font-weight:700;color:var(--text);">'+puntos+'/100</span>'    +'</div>'    +'<div class="salud-bar-wrap"><div class="salud-bar-fill" id="'+barId+'" style="width:0%;background:'+colorBarra+';"></div></div>'    +'</div>'    +nota    +'</div>'    +'</div>';
}


function actualizarUMenu(){
  var c = getCuentas();
  var efectivo = Number(c.efectivo||0);
  var banco = (c.cheques||[]).reduce(function(s,x){ return s+Number(x.saldo||0); },0);
  var deudaTC = (c.tarjetas||[]).reduce(function(s,t){ return s+Number(t.balance||0); },0);
  var ef = document.getElementById('uMenuEfectivo');
  var ba = document.getElementById('uMenuBanco');
  var tc = document.getElementById('uMenuTC');
  if(ef) ef.textContent = '$' + efectivo.toLocaleString('es-MX', {minimumFractionDigits:2});
  if(ba) ba.textContent = '$' + banco.toLocaleString('es-MX', {minimumFractionDigits:2});
  if(tc) tc.textContent = 'Deuda: $' + deudaTC.toLocaleString('es-MX', {minimumFractionDigits:2});
}

function cerrarUMenu(){
  var menu = document.getElementById('uFabMenu');
  var btn  = document.getElementById('uFabBtn');
  if(!menu) return;
  menu.style.opacity = '0';
  menu.style.transform = 'scale(0.85) translateY(-10px)';
  setTimeout(function(){ menu.style.display = 'none'; }, 220);
  if(btn) btn.style.background = 'linear-gradient(135deg,var(--accent),var(--accent2))';
}

function toggleUMenu(){
  var menu = document.getElementById('uFabMenu');
  var btn  = document.getElementById('uFabBtn');
  if(!menu) return;
  var abierto = menu.style.display === 'block';
  if(abierto){
    cerrarUMenu();
  } else {
    actualizarUMenu();
    menu.style.display = 'block';
    requestAnimationFrame(function(){
      menu.style.opacity = '1';
      menu.style.transform = 'scale(1) translateY(0)';
    });
    if(btn) btn.style.background = 'var(--accent2,#4f8ef7)';
    setTimeout(function(){
      function cerrarFuera(e){
        var dentroMenu = menu.contains(e.target);
        var esBtn = btn && (btn === e.target || btn.contains(e.target));
        if(!dentroMenu && !esBtn){
          cerrarUMenu();
          document.removeEventListener('touchstart', cerrarFuera);
          document.removeEventListener('click', cerrarFuera);
        }
      }
      document.addEventListener('touchstart', cerrarFuera, {passive:true});
      document.addEventListener('click', cerrarFuera);
    }, 300);
  }
}

function abrirMenu(){ toggleUMenu(); }

function menuAccion(accion){
  document.getElementById('menuModal').classList.remove('open');
  var nbs = document.querySelectorAll('.nb');
  function irMas(sub){
    nbs.forEach(function(b){ b.classList.remove('active'); });
    nbs[4].classList.add('active');
    S.tab='mas'; S.subtab=sub;
    var renders = {config:renderConfig, codigos:renderCodigos, noticias:renderNoticias};
    document.getElementById('mainContent').innerHTML = renders[sub] ? renders[sub]() : '';
  }
  if(accion==='tema'){ pickTema(); }
  else if(accion==='salir'){ cerrarSesion(); }
  else if(accion==='config'){ irMas('config'); }
  else if(accion==='codigos'){ irMas('codigos'); }
  else if(accion==='noticias'){ irMas('noticias'); }
}

function cerrarMenu(){ var m=document.getElementById('menuModal'); if(m) m.classList.remove('open'); }

function renderConfig(){
  var isAdmin=S.user&&S.user.isAdmin;
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">⚙️ Configuración</div></div>'
    +'<div class="card">'
    +'<div class="set-item" onclick="pickTema()"><div><div class="set-label">🎨 Cambiar tema</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="abrirSelectorMoneda()"><div><div class="set-label">💱 Moneda de la app</div><div class="set-sub">'+_getMonedaApp()+'</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="abrirConfigNip()"><div><div class="set-label">🔒 NIP de seguridad</div><div class="set-sub">'+(localStorage.getItem('usala_nip_'+(S.user&&S.user.isAdmin?'admin':'u_'+(S.user&&S.user.codigo)))?'Activado ✓':'Sin NIP')+'</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="abrirConfigAutolock()"><div><div class="set-label">⏱ Bloqueo automático</div><div class="set-sub" id="autolockSubLabel">'
    +(function(){ var m=getLockTimeout(); var op=LOCK_OPCIONES.find(function(o){return o.val===m;}); return op?op.label:'Desactivado'; })()
    +'</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="restablecerMic()"><div><div class="set-label">🎤 Restablecer micrófono</div><div class="set-sub" id="micEstadoLabel">'+_getMicEstado()+'</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="goSub(\'version\')"><div><div class="set-label">📋 Versión</div><div class="set-sub">v'+APP_VERSION+'</div></div><div class="set-arrow">›</div></div>'
    +'<div class="set-item" onclick="cerrarSesion()"><div><div class="set-label" style="color:var(--danger);">🚪 Cerrar sesión</div></div><div class="set-arrow">›</div></div>'
    +'</div>'
    +(isAdmin?'<div class="card" style="margin-top:12px;"><div class="card-title">Admin</div>'
    +'<div class="set-item"><div><div class="set-label">🔐 Nueva contraseña</div></div></div>'
    +'<input class="inp" id="np1" type="password" placeholder="Nueva contraseña" style="margin-bottom:8px;">'
    +'<input class="inp" id="np2" type="password" placeholder="Confirmar contraseña" style="margin-bottom:10px;">'
    +'<button class="btn-main" onclick="cambiarPass()">Cambiar contraseña</button>'
    +'</div>':'')
    +'<div class="card" style="margin-top:12px;">'
    +'<div class="card-title" style="margin-top:14px;">🏷️ Mis categorías</div>'
  +'<div style="font-size:0.75rem;color:var(--dim);margin-bottom:10px;">Categorías personalizadas en toda la app</div>'
  +'<div style="display:flex;flex-wrap:wrap;gap:8px;margin-bottom:10px;">'
  +'<button class="cat-add-btn" onclick="abrirCatModal(\'gasto\',null)">💸 Gastos</button>'
  +'<button class="cat-add-btn" onclick="abrirCatModal(\'ingreso\',null)">💰 Ingresos</button>'
  +'<button class="cat-add-btn" onclick="abrirCatModal(\'activos\',null)">🏦 Activos</button>'
  +'<button class="cat-add-btn" onclick="abrirCatModal(\'pagos\',null)">📅 Pagos fijos</button>'
  +'</div>'
  +'<div class="danger-zone">'
    +'<div class="danger-title">⚠️ Zona de peligro</div>'
    +'<button class="danger-btn" onclick="resetTxs()">🗑️ Borrar mis transacciones</button>'
    +'<button class="danger-btn" onclick="resetCuenta()">♻️ Restablecer toda mi cuenta</button>'
    +'</div></div>';
}

function renderAyuda(){
  var st = _getSecurityStatus();
  var nipOk   = st.nip;
  var lockOk  = st.autolock;
  var ambos   = nipOk && lockOk;
  var secCard = '<div style="border-radius:18px;padding:16px;margin-bottom:16px;'
    +(ambos
      ? 'background:rgba(45,158,95,0.08);border:1.5px solid rgba(45,158,95,0.25);'
      : 'background:rgba(229,57,53,0.06);border:1.5px solid rgba(229,57,53,0.2);')
    +'">'
    +'<div style="display:flex;align-items:center;gap:12px;margin-bottom:12px;">'
      +'<div style="font-size:2rem;line-height:1;">'+(ambos?'🛡️':'⚠️')+'</div>'
      +'<div>'
        +'<div style="font-weight:900;font-size:0.9rem;">'
          +(ambos?'Tu cuenta está protegida ✓':'Tu seguridad necesita atención')
        +'</div>'
        +'<div style="font-size:0.72rem;color:var(--dim);margin-top:2px;">'
          +(ambos?'NIP activo + bloqueo automático configurado':'Configura NIP y bloqueo para proteger tus datos')
        +'</div>'
      +'</div>'
    +'</div>'
    +'<div style="display:flex;gap:8px;flex-wrap:wrap;margin-bottom:12px;">'
      +'<div style="display:flex;align-items:center;gap:5px;font-size:0.72rem;font-weight:700;padding:5px 10px;border-radius:20px;'
        +(nipOk?'background:rgba(45,158,95,0.12);color:#2d7a4f;':'background:rgba(229,57,53,0.1);color:#c62828;')
        +'">'+( nipOk?'✅':'❌')+' NIP de seguridad</div>'
      +'<div style="display:flex;align-items:center;gap:5px;font-size:0.72rem;font-weight:700;padding:5px 10px;border-radius:20px;'
        +(lockOk?'background:rgba(45,158,95,0.12);color:#2d7a4f;':'background:rgba(229,57,53,0.1);color:#c62828;')
        +'">'+( lockOk?'✅':'❌')+' Bloqueo automático</div>'
    +'</div>';
  if(!ambos){
    secCard += '<div style="display:flex;gap:8px;flex-wrap:wrap;">'
      +(!nipOk?'<button onclick="goSub(\'config_nip\')" style="background:#c62828;color:#fff;border:none;border-radius:20px;padding:7px 14px;font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:800;cursor:pointer;">🔒 Activar NIP</button>':'')
      +(!lockOk?'<button onclick="abrirConfigAutolock()" style="background:#e65100;color:#fff;border:none;border-radius:20px;padding:7px 14px;font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:800;cursor:pointer;">⏱ Bloqueo auto</button>':'')
    +'</div>';
  }
  secCard += '</div>';
  var html = '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">❓ Ayuda</div></div>'
    + secCard
    +'<div style="position:relative;margin-bottom:16px;">'
      +'<input class="inp" id="ayudaBusca" placeholder="🔍 Buscar en la ayuda..." oninput="filtrarAyuda()" style="padding-left:16px;">'
    +'</div>'
    +'<div style="display:flex;gap:7px;overflow-x:auto;padding-bottom:8px;margin-bottom:10px;scrollbar-width:none;">'
      +'<div style="display:flex;gap:7px;overflow-x:auto;padding-bottom:8px;margin-bottom:10px;scrollbar-width:none;">'
      +'<button class="ayuda-chip active" id="chip_todos" data-cat="" onclick="ayudaChipEv(this)">Todos</button>'
      +'<button class="ayuda-chip" data-cat="Seguridad" onclick="ayudaChipEv(this)">🔐 Seguridad</button>'
      +'<button class="ayuda-chip" data-cat="Pagos" onclick="ayudaChipEv(this)">📅 Pagos</button>'
      +'<button class="ayuda-chip" data-cat="Cuentas" onclick="ayudaChipEv(this)">🏦 Cuentas</button>'
      +'<button class="ayuda-chip" data-cat="Créditos" onclick="ayudaChipEv(this)">🤝 Créditos</button>'
      +'<button class="ayuda-chip" data-cat="Voz" onclick="ayudaChipEv(this)">🎙️ Voz</button>'
      +'<button class="ayuda-chip" data-cat="Config" onclick="ayudaChipEv(this)">⚙️ Config</button>'
    +'</div>'
    +'<div id="ayudaLista">'+renderFaqs('')+'</div>';
  return html;
}

function renderVersion(){
  var isAdmin=S.user&&S.user.isAdmin;
  return '<div class="page-header">'+backBtn('mas',4)+'<div class="page-title">📋 Versión</div></div>'
    +'<div class="card" style="text-align:center;padding:28px 20px;">'
    +'<div style="font-size:2rem;font-weight:900;color:var(--accent);font-family:\'JetBrains Mono\',monospace;">v'+APP_VERSION+'</div>'
    +'<div style="font-size:0.8rem;color:var(--dim);margin-top:8px;">'+APP_NOTAS+'</div>'
    +'</div>'
    +(isAdmin?'<div class="card"><div class="card-title">Editar versión</div>'
    +'<label class="inp-label">Número</label><input class="inp" id="vNum" value="'+APP_VERSION+'">'
    +'<label class="inp-label">Notas</label><textarea class="inp" id="vNotas" rows="3" style="resize:none;">'+APP_NOTAS+'</textarea>'
    +'<button class="btn-main" onclick="guardarVersion()">💾 Guardar</button>'
    +'</div>':'');
}


function backBtn(tab, idx){
  return '<button class="back-btn" onclick="goTab(\''+tab+'\',document.querySelectorAll(\'.nb\')['+idx+'])" style="width:36px;height:36px;border-radius:50%;background:var(--inp);border:1px solid var(--border);backdrop-filter:blur(8px);display:flex;align-items:center;justify-content:center;font-size:1.2rem;color:var(--text);cursor:pointer;flex-shrink:0;transition:background 0.15s;">‹</button>';
}

function backSubBtn(label){
  return '<button class="back-btn" onclick="goTab(S.tab,document.querySelector(\'.nb.active\'))" style="width:36px;height:36px;border-radius:50%;background:var(--inp);border:1px solid var(--border);backdrop-filter:blur(8px);display:flex;align-items:center;justify-content:center;font-size:1.2rem;color:var(--text);cursor:pointer;flex-shrink:0;transition:background 0.15s;">‹</button>';
}

function showScreen(id){
  document.querySelectorAll('.screen').forEach(function(s){ s.classList.remove('active'); });
  document.getElementById(id).classList.add('active');
}

function showToast(msg){ var t=document.createElement('div'); t.className='toast'; t.textContent=msg; document.body.appendChild(t); setTimeout(function(){ t.remove(); },2500); }

function mostrarUndo(msg, fn){
  if(_undoTimer) clearTimeout(_undoTimer);
  var old = document.getElementById('undoBar'); if(old) old.remove();
  _undoFn = fn;
  setTimeout(function(){
    var d = document.createElement('div'); d.id='undoBar'; d.className='undo-bar';
    d.innerHTML = '<div style="display:flex;align-items:center;gap:8px;flex:1;">'
      +'<span style="flex:1;">'+msg+'</span>'
      +'<button class="undo-btn" onclick="ejecutarUndo()">↩ Deshacer</button>'
      +'</div>'
      +'<div class="undo-prog" id="undoProg"></div>';
    document.body.appendChild(d);
    requestAnimationFrame(function(){
      requestAnimationFrame(function(){
        var p=document.getElementById('undoProg'); if(p) p.style.width='0%';
      });
    });
    _undoTimer = setTimeout(function(){
      var u=document.getElementById('undoBar'); if(u){ u.style.opacity='0'; u.style.transform='translateY(10px)'; u.style.transition='opacity 0.3s,transform 0.3s'; setTimeout(function(){ if(u.parentNode) u.remove(); },300); } _undoFn=null;
    }, 7000);
  }, 0);
}

function ejecutarUndo(){
  if(_undoTimer) clearTimeout(_undoTimer);
  var u=document.getElementById('undoBar'); if(u) u.remove();
  if(_undoFn){ _undoFn(); _undoFn=null; }
}


</script>
</body>
</html>
