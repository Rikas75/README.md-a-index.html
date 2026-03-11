<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>USALA · Finanzas</title>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
:root {
  --bg: #f0f4f0;
  --card: #ffffff;
  --text: #1a2e1a;
  --dim: #7a9a7a;
  --accent: #1e6b3c;
  --accent2: #2d9e5f;
  --danger: #e53935;
  --gold: #c9841a;
  --border: rgba(30,107,60,0.12);
  --nav: #1a2e1a;
  --navtext: #ffffff;
  --shadow: 0 4px 24px rgba(30,107,60,0.10);
  --radius: 18px;
  --inp: #f5f9f5;
}
[data-theme="dark"] {
  --bg: #0d1a0d;
  --card: #162016;
  --text: #e8f5e8;
  --dim: #5a8a5a;
  --accent: #2d9e5f;
  --accent2: #3dce7a;
  --border: rgba(45,158,95,0.15);
  --nav: #0a120a;
  --shadow: 0 4px 24px rgba(0,0,0,0.4);
  --inp: #1e2e1e;
}
[data-theme="gold"] {
  --bg: #0a0800;
  --card: #140f00;
  --text: #f5e6c0;
  --dim: #8a7040;
  --accent: #c9841a;
  --accent2: #f0a830;
  --border: rgba(201,132,26,0.2);
  --nav: #0a0800;
  --navtext: #f5e6c0;
  --shadow: 0 4px 24px rgba(0,0,0,0.5);
  --inp: #1a1200;
}
[data-theme="ocean"] {
  --bg: #e8f4fd;
  --card: #ffffff;
  --text: #0d2d4a;
  --dim: #5a8aaa;
  --accent: #0066cc;
  --accent2: #0099ee;
  --border: rgba(0,102,204,0.12);
  --nav: #0d2d4a;
  --navtext: #ffffff;
  --shadow: 0 4px 24px rgba(0,102,204,0.12);
  --inp: #f0f8ff;
}
[data-theme="rose"] {
  --bg: #fff5f7;
  --card: #ffffff;
  --text: #3d0a14;
  --dim: #aa6070;
  --accent: #c02040;
  --accent2: #e84060;
  --border: rgba(192,32,64,0.12);
  --nav: #3d0a14;
  --navtext: #ffffff;
  --shadow: 0 4px 24px rgba(192,32,64,0.10);
  --inp: #fff0f2;
}

*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body{height:100%;font-family:Outfit,sans-serif;background:var(--bg);color:var(--text);overflow:hidden;}

/* ── SCREENS ── */
.screen{display:none;position:fixed;inset:0;background:var(--bg);}
.screen.active{display:flex;flex-direction:column;}

/* ── THEME PICKER ── */
#themePicker{align-items:center;justify-content:center;padding:32px 24px;}
.tp-logo{font-size:2.4rem;font-weight:900;letter-spacing:-0.03em;color:var(--accent);margin-bottom:6px;}
.tp-sub{font-size:0.82rem;color:var(--dim);margin-bottom:36px;text-align:center;}
.tp-title{font-size:0.72rem;font-weight:700;letter-spacing:0.12em;text-transform:uppercase;color:var(--dim);margin-bottom:16px;}
.themes-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;width:100%;}
.theme-card{padding:20px 16px;border-radius:16px;cursor:pointer;border:2px solid transparent;transition:all 0.2s;text-align:left;}
.theme-card:active{transform:scale(0.97);}
.theme-card.selected{border-color:currentColor;}
.tc-name{font-weight:700;font-size:0.9rem;margin-top:8px;}
.tc-dot{width:28px;height:28px;border-radius:50%;}
.tp-btn{margin-top:24px;width:100%;padding:16px;background:var(--accent);color:var(--navtext);border:none;border-radius:14px;font-family:Outfit,sans-serif;font-size:1rem;font-weight:700;cursor:pointer;letter-spacing:0.02em;}

/* ── ACCESS SCREEN ── */
#accessScreen{
  align-items:center;justify-content:start;padding:24px 20px 40px;
  background:linear-gradient(160deg,#dceeff 0%,#eef5ff 60%,#f5f9ff 100%) !important;
  min-height:100vh;overflow-y:auto;
}
.access-logo{
  font-size:3.4rem;font-weight:900;
  color:#1a3a8f;
  margin-bottom:2px;letter-spacing:-0.03em;
  text-shadow: 0 2px 8px rgba(26,58,143,0.12);
}
.access-logo-sub{
  font-size:0.85rem;color:#6b8abf;font-weight:500;
  margin-bottom:32px;letter-spacing:0.01em;
}
.access-icon{font-size:2.2rem;margin-bottom:8px;}
.access-card{
  background:#ffffff;border-radius:28px;
  padding:32px 26px 28px;width:100%;
  box-shadow:0 8px 40px rgba(26,58,143,0.10), 0 2px 8px rgba(0,0,0,0.04);
}
.access-title{font-size:1.2rem;font-weight:900;margin-bottom:4px;color:#1a2b4a;}
.access-sub{font-size:0.8rem;color:#7a90b8;margin-bottom:24px;line-height:1.6;}
.inp-label{
  font-size:0.72rem;font-weight:800;color:#2355c9;
  letter-spacing:0.1em;text-transform:uppercase;
  margin-bottom:8px;display:block;
}
.inp{
  width:100%;padding:17px 20px;
  background:#f0f4fc;border:2px solid #e2eaf8;
  border-radius:18px;font-family:Outfit,sans-serif;
  font-size:1rem;color:#1a2b4a;outline:none;margin-bottom:18px;
  transition:border-color 0.2s,background 0.2s;
  box-sizing:border-box;
}
.inp::placeholder{color:#a8b8d8;}
.inp:focus{border-color:#2355c9;background:#fff;}
.btn-main{
  width:100%;padding:18px;
  background:linear-gradient(135deg,#2355c9,#3a72f0);
  color:#fff;border:none;border-radius:18px;
  font-family:Outfit,sans-serif;font-size:1.05rem;
  font-weight:800;cursor:pointer;margin-top:6px;
  letter-spacing:0.02em;
  box-shadow:0 6px 20px rgba(35,85,201,0.35);
  transition:transform 0.15s,box-shadow 0.15s;
}
.btn-main:active{transform:scale(0.98);box-shadow:0 3px 10px rgba(35,85,201,0.25);}
.access-err{display:none;padding:10px 14px;background:rgba(229,57,53,0.08);border:1px solid rgba(229,57,53,0.25);border-radius:12px;font-size:0.8rem;color:var(--danger);margin-bottom:14px;}
.admin-link{text-align:center;margin-top:16px;font-size:0.72rem;color:var(--dim);cursor:pointer;text-decoration:underline;}
.admin-modal{display:none;position:fixed;inset:0;z-index:200;background:rgba(0,0,0,0.5);align-items:flex-end;}
.admin-modal.open{display:flex;}
.admin-box{background:var(--card);border-radius:24px 24px 0 0;padding:28px 24px 40px;width:100%;}
.admin-handle{width:36px;height:4px;background:var(--border);border-radius:2px;margin:0 auto 20px;}
.admin-title{font-size:1rem;font-weight:800;margin-bottom:16px;text-align:center;}
.admin-hint{text-align:center;font-size:0.7rem;color:var(--dim);margin-top:12px;}
.admin-recover{text-align:center;margin-top:8px;font-size:0.68rem;color:var(--dim);text-decoration:underline;cursor:pointer;background:none;border:none;font-family:Outfit,sans-serif;width:100%;}

/* ── DASHBOARD ── */
#dashboard{display:none;flex-direction:column;}
#dashboard.active{display:flex;}
.topbar{display:flex;align-items:center;padding:12px 16px 8px;gap:10px;background:var(--bg);}
.top-logo{font-size:1rem;font-weight:900;color:var(--accent);flex:1;letter-spacing:-0.02em;}
.top-ver{font-size:0.58rem;font-weight:800;opacity:1;margin-left:6px;color:var(--navtext);background:var(--accent);padding:2px 8px;border-radius:10px;vertical-align:middle;letter-spacing:0.02em;}
.top-icon{width:36px;height:36px;border-radius:50%;background:var(--inp);border:none;cursor:pointer;font-size:1rem;display:flex;align-items:center;justify-content:center;color:var(--text);}
.top-avatar{width:36px;height:36px;border-radius:50%;background:var(--accent);color:var(--navtext);font-weight:800;font-size:0.85rem;display:flex;align-items:center;justify-content:center;cursor:pointer;}
.content{flex:1;overflow-y:auto;padding:0 16px 90px;}
.bot-nav{position:fixed;bottom:0;left:0;right:0;background:var(--nav);display:flex;border-top:1px solid rgba(255,255,255,0.06);z-index:50;padding-bottom:env(safe-area-inset-bottom);}
.nb{flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:10px 2px 8px;border:none;background:none;color:var(--navtext);opacity:0.4;cursor:pointer;font-family:Outfit,sans-serif;transition:opacity 0.2s;}
.nb.active{opacity:1;}
.nb-ico{font-size:1.15rem;margin-bottom:2px;}
.nb-lbl{font-size:0.46rem;font-weight:700;letter-spacing:0.04em;text-transform:uppercase;}

/* ── CARDS & UI ── */
.card{background:var(--card);border-radius:var(--radius);padding:18px;margin-bottom:12px;box-shadow:var(--shadow);}
.card-title{font-size:0.72rem;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:var(--dim);margin-bottom:14px;}
.stat-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px;}
.stat-card{background:var(--card);border-radius:14px;padding:14px;box-shadow:var(--shadow);cursor:pointer;}
.stat-card.full{grid-column:1/-1;}
.stat-label{font-size:0.65rem;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;color:var(--dim);margin-bottom:4px;}
.stat-val{font-size:1.15rem;font-weight:800;color:var(--accent);}
.stat-val.red{color:var(--danger);}
.stat-val.gold{color:var(--gold);}

/* ── TRANSACCIONES ── */
.tx-item{display:flex;align-items:center;gap:12px;padding:12px 0;border-bottom:1px solid var(--border);}
.tx-item:last-child{border-bottom:none;}
.tx-ico{width:38px;height:38px;border-radius:12px;background:var(--inp);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0;}
.tx-info{flex:1;min-width:0;}
.tx-name{font-weight:600;font-size:0.88rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.tx-date{font-size:0.68rem;color:var(--dim);margin-top:2px;}
.tx-right{display:flex;align-items:center;gap:6px;flex-shrink:0;}
.tx-amt{font-weight:800;font-size:0.88rem;font-family:JetBrains Mono,monospace;}
.ing{color:var(--accent2);}
.gas{color:var(--danger);}
.ic-btn{background:none;border:none;cursor:pointer;font-size:0.95rem;padding:4px;opacity:0.6;}
.ic-btn:active{opacity:1;}

/* ── MÓDULOS ── */
.mod-list{display:flex;flex-direction:column;gap:2px;}
.mod-item{display:flex;align-items:center;gap:14px;padding:15px 16px;background:var(--card);border-radius:14px;cursor:pointer;margin-bottom:6px;box-shadow:var(--shadow);}
.mod-item:active{opacity:0.8;}
.mod-icon{font-size:1.4rem;width:42px;height:42px;background:var(--inp);border-radius:12px;display:flex;align-items:center;justify-content:center;flex-shrink:0;}
.mod-label{font-weight:700;font-size:0.9rem;}
.mod-sub{font-size:0.7rem;color:var(--dim);margin-top:2px;}
.mod-arrow{margin-left:auto;color:var(--dim);font-size:1.1rem;}

/* ── FORMS ── */
.form-section{margin-bottom:16px;}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.btn-sec{width:100%;padding:15px;background:var(--inp);color:var(--accent);border:1.5px solid var(--border);border-radius:12px;font-family:Outfit,sans-serif;font-size:0.88rem;font-weight:700;cursor:pointer;margin-bottom:8px;}
.back-btn{background:none;border:none;font-size:1.4rem;cursor:pointer;color:var(--text);padding:0 10px 0 0;line-height:1;}
.page-header{display:flex;align-items:center;margin-bottom:18px;padding-top:4px;}
.page-title{font-size:1.05rem;font-weight:800;}

/* ── PROGRESS BAR ── */
.prog-wrap{background:var(--inp);border-radius:6px;height:7px;overflow:hidden;margin:8px 0;}
.prog-bar{height:100%;background:var(--accent);border-radius:6px;transition:width 0.4s;}

/* ── ALERTAS ── */
.alerta-item{display:flex;align-items:flex-start;gap:10px;padding:14px;background:var(--card);border-radius:14px;margin-bottom:8px;box-shadow:var(--shadow);}
.alerta-info{flex:1;min-width:0;}
.alerta-nombre{font-weight:700;font-size:0.88rem;}
.alerta-meta{font-size:0.68rem;color:var(--dim);margin-top:3px;}
.alerta-actions{display:flex;gap:6px;flex-shrink:0;}

/* ── CRÉDITOS ── */
.cred-item{background:var(--card);border-radius:14px;padding:16px;margin-bottom:10px;box-shadow:var(--shadow);}
.cred-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:8px;}
.cred-persona{font-weight:800;font-size:0.9rem;}
.cred-desc{font-size:0.7rem;color:var(--dim);margin-top:2px;}
.cred-badge{font-size:0.65rem;padding:3px 10px;border-radius:20px;font-weight:700;}
.badge-pend{background:rgba(255,152,0,0.12);color:#f57c00;}
.badge-pagado{background:rgba(45,158,95,0.12);color:var(--accent2);}
.badge-vencido{background:rgba(229,57,53,0.10);color:var(--danger);}
.cred-amounts{display:flex;justify-content:space-between;font-size:0.72rem;color:var(--dim);margin-bottom:6px;}
.cred-btns{display:flex;gap:6px;margin-top:10px;}
.cred-btn{flex:1;padding:8px 6px;border-radius:10px;border:1.5px solid var(--border);background:var(--inp);font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;cursor:pointer;color:var(--accent);}
.cred-btn.danger{color:var(--danger);border-color:rgba(229,57,53,0.2);}
.cred-btn.success{color:var(--accent2);border-color:rgba(45,158,95,0.2);}

/* ── MODAL TRANSACCIÓN ── */
.modal{display:none;position:fixed;inset:0;z-index:100;background:rgba(0,0,0,0.5);align-items:flex-end;}
.modal.open{display:flex;}
.modal-box{background:var(--card);border-radius:24px 24px 0 0;padding:20px 20px 36px;width:100%;max-height:90vh;overflow-y:auto;}
.modal-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:18px;}
.modal-title{font-size:1rem;font-weight:800;}
.modal-close{background:var(--inp);border:none;width:32px;height:32px;border-radius:50%;font-size:1.1rem;cursor:pointer;color:var(--dim);display:flex;align-items:center;justify-content:center;}
.tipo-selector{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:16px;}
.tipo-opt{padding:12px;border-radius:12px;border:2px solid var(--border);background:var(--inp);text-align:center;cursor:pointer;font-weight:700;font-size:0.88rem;transition:all 0.15s;}
.tipo-opt.selected{border-color:var(--accent);background:rgba(30,107,60,0.08);color:var(--accent);}

/* ── TOAST & UNDO ── */
.toast{position:fixed;top:20px;left:50%;transform:translateX(-50%);background:#1a2e1a;color:#fff;padding:10px 20px;border-radius:20px;font-size:0.82rem;font-weight:600;z-index:999;white-space:nowrap;box-shadow:0 4px 20px rgba(0,0,0,0.3);animation:toastIn 0.3s ease;}
@keyframes toastIn{from{opacity:0;transform:translateX(-50%) translateY(-10px);}to{opacity:1;transform:translateX(-50%) translateY(0);}}
@keyframes gradShift{0%{background-position:0% 50%;}50%{background-position:100% 50%;}100%{background-position:0% 50%;}}
@keyframes float1{0%,100%{transform:translateY(0) scale(1);}50%{transform:translateY(-12px) scale(1.05);}}
@keyframes float2{0%,100%{transform:translateY(0) rotate(0deg);}50%{transform:translateY(-8px) rotate(8deg);}}
@keyframes popIn{0%{transform:scale(0) rotate(-15deg);opacity:0;}70%{transform:scale(1.2) rotate(5deg);}100%{transform:scale(1) rotate(0deg);opacity:1;}}
@keyframes slideUp{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
/* ── PANEL PAGOS PENDIENTES ── */
.pp-overlay{position:fixed;inset:0;background:rgba(0,0,0,0.5);z-index:8000;display:flex;align-items:flex-end;justify-content:center;animation:fadeIn 0.18s;}
.pp-panel{background:var(--card);border-radius:24px 24px 0 0;width:100%;max-width:520px;max-height:90vh;display:flex;flex-direction:column;animation:slideUp 0.28s cubic-bezier(.4,0,.2,1);}
.pp-handle{width:36px;height:4px;background:var(--border);border-radius:99px;margin:12px auto 0;}
.pp-head{padding:16px 18px 0;}
.pp-title{font-size:1.05rem;font-weight:900;margin-bottom:2px;}
.pp-subtitle{font-size:0.72rem;color:var(--dim);margin-bottom:12px;}
.pp-tabs{display:flex;gap:6px;padding:0 18px 12px;overflow-x:auto;-webkit-overflow-scrolling:touch;}
.pp-tab{padding:6px 14px;border-radius:20px;border:1.5px solid var(--border);background:var(--inp);font-family:Outfit,sans-serif;font-size:0.76rem;font-weight:700;cursor:pointer;white-space:nowrap;color:var(--dim);transition:all 0.15s;}
.pp-tab.active{background:var(--accent);border-color:var(--accent);color:var(--navtext);}
.pp-body{flex:1;overflow-y:auto;padding:0 18px 32px;}
.pp-empty{text-align:center;padding:32px 20px;color:var(--dim);font-size:0.82rem;}
.pp-item{display:flex;align-items:center;gap:12px;padding:12px 0;border-bottom:1px solid var(--border);}
.pp-item:last-child{border-bottom:none;}
.pp-dot{width:10px;height:10px;border-radius:50%;flex-shrink:0;}
.pp-ico{width:40px;height:40px;border-radius:13px;background:var(--inp);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0;}
.pp-info{flex:1;min-width:0;}
.pp-name{font-weight:700;font-size:0.88rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.pp-when{font-size:0.68rem;color:var(--dim);margin-top:2px;}
.pp-amt{font-weight:900;font-size:0.92rem;font-family:JetBrains Mono,monospace;flex-shrink:0;}
.pp-badge{font-size:0.62rem;font-weight:800;padding:2px 7px;border-radius:20px;margin-left:4px;flex-shrink:0;}
.pp-section-title{font-size:0.62rem;font-weight:800;text-transform:uppercase;letter-spacing:0.09em;color:var(--dim);padding:12px 0 6px;}
.pp-btn-abrir{display:flex;flex-direction:column;align-items:center;justify-content:center;background:var(--card);border-radius:14px;padding:14px 10px;box-shadow:var(--shadow);cursor:pointer;border:1.5px solid var(--border);gap:2px;transition:all 0.15s;}
.pp-btn-abrir:active{transform:scale(0.96);}
/* ── AUTOLOCK ── */
.lock-screen{position:fixed;inset:0;z-index:99999;display:flex;flex-direction:column;align-items:center;justify-content:center;background:var(--bg);animation:fadeIn 0.3s;}
.lock-card{background:var(--card);border-radius:28px;padding:32px 28px;width:90%;max-width:340px;box-shadow:0 24px 60px rgba(0,0,0,0.25);text-align:center;}
.lock-avatar{width:72px;height:72px;border-radius:50%;background:var(--accent);display:flex;align-items:center;justify-content:center;font-size:2rem;margin:0 auto 14px;box-shadow:0 8px 24px rgba(0,0,0,0.15);}
.lock-nombre{font-size:1.1rem;font-weight:900;margin-bottom:4px;}
.lock-sub{font-size:0.75rem;color:var(--dim);margin-bottom:22px;}
.lock-dots{display:flex;justify-content:center;gap:12px;margin-bottom:20px;}
.lock-dot{width:14px;height:14px;border-radius:50%;background:var(--border);transition:background 0.15s;}
.lock-dot.filled{background:var(--accent);}
.lock-dot.error{background:#e53935;}
.lock-pad{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;max-width:240px;margin:0 auto;}
.lock-key{height:56px;border-radius:16px;border:1.5px solid var(--border);background:var(--inp);font-family:Outfit,sans-serif;font-size:1.2rem;font-weight:700;cursor:pointer;color:var(--text);transition:all 0.1s;}
.lock-key:active{transform:scale(0.92);background:var(--accent);color:var(--navtext);}
.lock-key.del{font-size:1rem;}
.lock-timeout-badge{display:inline-block;font-size:0.65rem;font-weight:800;padding:3px 10px;border-radius:20px;background:var(--accent);color:var(--navtext);margin-bottom:16px;}
.ayuda-chip{flex-shrink:0;border:1.5px solid var(--border);border-radius:20px;padding:6px 14px;font-family:Outfit,sans-serif;font-size:0.72rem;font-weight:700;background:var(--card);color:var(--dim);cursor:pointer;transition:all 0.15s;}
.ayuda-chip.active,.ayuda-chip:active{background:var(--accent);color:var(--navtext);border-color:var(--accent);}
.cat-add-btn{display:inline-flex;align-items:center;gap:4px;padding:5px 10px;border-radius:20px;border:1.5px dashed var(--accent);background:transparent;color:var(--accent);font-family:Outfit,sans-serif;font-size:0.74rem;font-weight:700;cursor:pointer;margin-top:5px;transition:all 0.18s;}
.cat-add-btn:hover{background:var(--accent);color:var(--navtext);}
.cat-modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,0.45);z-index:10000;display:flex;align-items:flex-end;justify-content:center;animation:fadeIn 0.15s;}
.cat-modal-box{background:var(--card);border-radius:24px 24px 0 0;padding:20px 18px 32px;width:100%;max-width:480px;animation:slideUp 0.25s cubic-bezier(.4,0,.2,1);}
.cat-modal-title{font-size:1rem;font-weight:900;margin-bottom:4px;}
.cat-modal-sub{font-size:0.75rem;color:var(--dim);margin-bottom:14px;}
.cat-chips-wrap{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:14px;max-height:160px;overflow-y:auto;}
.cat-chip{display:inline-flex;align-items:center;gap:5px;padding:5px 12px;border-radius:20px;border:1.5px solid var(--border);background:var(--inp);font-size:0.78rem;font-weight:600;cursor:default;}
.cat-chip .del-chip{background:none;border:none;cursor:pointer;color:var(--dim);font-size:0.8rem;padding:0;line-height:1;}
.cat-chip .del-chip:hover{color:var(--danger);}
.cat-new-row{display:flex;gap:8px;align-items:center;}
.cat-new-inp{flex:1;padding:10px 12px;border-radius:10px;border:1.5px solid var(--border);background:var(--inp);color:var(--text);font-family:Outfit,sans-serif;font-size:0.85rem;}
.cat-new-inp:focus{outline:none;border-color:var(--accent);}
.cat-save-btn{padding:10px 16px;border-radius:10px;border:none;background:var(--accent);color:var(--navtext);font-family:Outfit,sans-serif;font-weight:700;font-size:0.85rem;cursor:pointer;white-space:nowrap;}
.undo-bar{position:fixed;bottom:86px;left:10px;right:10px;background:var(--nav);color:var(--navtext);padding:14px 16px;border-radius:16px;font-size:0.84rem;font-weight:600;z-index:9999;display:flex;flex-direction:column;gap:8px;box-shadow:0 6px 28px rgba(0,0,0,0.35);animation:undoSlideIn 0.25s cubic-bezier(.4,0,.2,1);}
.undo-btn{background:var(--accent);border:none;color:var(--navtext);padding:7px 16px;border-radius:10px;font-family:Outfit,sans-serif;font-weight:700;cursor:pointer;font-size:0.8rem;}
.undo-prog{position:absolute;bottom:0;left:0;height:4px;background:var(--accent);border-radius:0 0 16px 16px;transition:width 7s linear;width:100%;}

/* ── CONFIG / DANGER ── */
.danger-zone{border:1.5px solid rgba(229,57,53,0.25);border-radius:14px;padding:16px;margin-top:12px;}
.danger-title{font-size:0.78rem;font-weight:700;color:var(--danger);margin-bottom:12px;letter-spacing:0.05em;text-transform:uppercase;}
.danger-btn{width:100%;padding:12px;background:rgba(229,57,53,0.06);border:1.5px solid rgba(229,57,53,0.2);border-radius:10px;color:var(--danger);font-family:Outfit,sans-serif;font-size:0.82rem;font-weight:600;cursor:pointer;margin-bottom:8px;text-align:left;}
.danger-btn:last-child{margin-bottom:0;}

/* ── CHIPS & TAGS ── */
.chip{display:inline-flex;align-items:center;gap:4px;padding:4px 10px;border-radius:20px;font-size:0.68rem;font-weight:700;}
.chip-green{background:rgba(45,158,95,0.1);color:var(--accent2);}
.chip-red{background:rgba(229,57,53,0.1);color:var(--danger);}
.chip-orange{background:rgba(255,152,0,0.1);color:#f57c00;}

/* ── CÓDIGOS ── */
.code-item{background:var(--card);border-radius:12px;padding:14px;margin-bottom:8px;box-shadow:var(--shadow);display:flex;align-items:center;gap:12px;}
.code-text{font-family:JetBrains Mono,monospace;font-weight:700;font-size:0.9rem;color:var(--accent);flex:1;}
.code-info{font-size:0.68rem;color:var(--dim);}

/* ── SETTINGS ── */
.set-item{display:flex;align-items:center;justify-content:space-between;padding:16px 0;border-bottom:1px solid var(--border);}
.set-item:last-child{border-bottom:none;}
.set-label{font-weight:600;font-size:0.88rem;}
.set-sub{font-size:0.7rem;color:var(--dim);margin-top:2px;}
.set-arrow{color:var(--dim);}

/* ── BANNER ADMIN ── */
.admin-banner{background:rgba(45,158,95,0.12);border:1px solid rgba(45,158,95,0.25);border-radius:12px;padding:10px 14px;margin-bottom:12px;font-size:0.75rem;color:var(--accent2);font-weight:600;text-align:center;}

/* ── PRESUPUESTO ── */
.pres-item{display:flex;align-items:center;gap:10px;padding:12px 0;border-bottom:1px solid var(--border);}
.pres-item:last-child{border-bottom:none;}
.pres-name{flex:1;font-size:0.85rem;font-weight:600;}
.pres-val{font-family:JetBrains Mono,monospace;font-size:0.8rem;font-weight:700;}

select.inp{appearance:none;-webkit-appearance:none;}
.ck{padding:16px 6px;border:none;background:rgba(255,255,255,0.08);color:#fff;font-family:Outfit,sans-serif;font-size:1.15rem;font-weight:600;cursor:pointer;transition:background 0.1s,transform 0.08s;-webkit-tap-highlight-color:transparent;border-radius:4px;}
.ck:active{background:rgba(255,255,255,0.22);transform:scale(0.93);}
.ck-fn{background:rgba(160,174,200,0.15);color:#a0aec8;font-size:0.95rem;font-weight:700;}
.ck-fn:active{background:rgba(160,174,200,0.3);}
.ck-op{background:rgba(255,159,10,0.18);color:#ffb347;font-size:1.2rem;font-weight:700;}
.ck-op:active{background:rgba(255,159,10,0.4);}
.ck-eq{background:linear-gradient(135deg,#ff9f0a,#ff6b00);color:#fff;font-size:1.25rem;font-weight:800;border-radius:4px;}
.ck-eq:active{filter:brightness(0.85);}
.ck-del{background:rgba(255,80,80,0.15);color:#ff6b6b;font-size:1rem;}
.ck-del:active{background:rgba(255,80,80,0.35);}

50%{transform:scaleY(1.8);}}
</style>
</head>
<body>

<!-- ══ ACCESS SCREEN ══ -->
<div class="screen active" id="accessScreen">
  <div style="width:100%;max-width:420px;margin:0 auto;padding:16px 0 60px;">
    <!-- Logo USALA -->
    <div style="text-align:center;">
      <div class="access-logo">USALA</div>
      <div class="access-logo-sub">Finanzas Personales</div>
    </div>

    <!-- ── PANEL: Sesión recordada ── -->
    <div class="access-card" id="panelSesion" style="display:none;">
      <div style="text-align:center;margin-bottom:20px;">
        <div id="sesionAvatar" style="width:76px;height:76px;border-radius:50%;background:linear-gradient(135deg,var(--accent),var(--accent2));margin:0 auto 14px;display:flex;align-items:center;justify-content:center;font-size:2.2rem;box-shadow:0 6px 24px rgba(45,106,255,0.35);">👤</div>
        <div style="font-size:0.65rem;color:var(--dim);font-weight:700;text-transform:uppercase;letter-spacing:0.1em;margin-bottom:6px;">Bienvenid@ de vuelta</div>
        <div id="sesionNombre" style="font-size:1.5rem;font-weight:900;color:var(--text);"></div>
      </div>
      <!-- NIP: solo visible si el usuario tiene NIP configurado -->
      <div id="nipZona" style="display:none;margin-bottom:16px;">
        <div style="font-size:0.78rem;color:var(--dim);text-align:center;margin-bottom:10px;">🔒 Ingresa tu NIP de seguridad</div>
        <div style="display:flex;gap:10px;justify-content:center;margin-bottom:8px;">
          <input id="nip1" type="password" inputmode="numeric" maxlength="1" class="inp" style="width:52px;height:56px;text-align:center;font-size:1.5rem;font-weight:800;padding:0;" oninput="nipSig(this,'nip2')" onkeydown="nipBack(event,this,null)">
          <input id="nip2" type="password" inputmode="numeric" maxlength="1" class="inp" style="width:52px;height:56px;text-align:center;font-size:1.5rem;font-weight:800;padding:0;" oninput="nipSig(this,'nip3')" onkeydown="nipBack(event,this,'nip1')">
          <input id="nip3" type="password" inputmode="numeric" maxlength="1" class="inp" style="width:52px;height:56px;text-align:center;font-size:1.5rem;font-weight:800;padding:0;" oninput="nipSig(this,'nip4')" onkeydown="nipBack(event,this,'nip2')">
          <input id="nip4" type="password" inputmode="numeric" maxlength="1" class="inp" style="width:52px;height:56px;text-align:center;font-size:1.5rem;font-weight:800;padding:0;" oninput="nipSig(this,null)" onkeydown="nipBack(event,this,'nip3')">
        </div>
        <div id="nipErr" style="display:none;font-size:0.75rem;color:#e53;text-align:center;margin-bottom:6px;">NIP incorrecto, intenta de nuevo</div>
        <button onclick="verificarNip()" style="width:100%;padding:15px;background:linear-gradient(135deg,var(--accent),var(--accent2));color:var(--navtext);border:none;border-radius:16px;font-family:Outfit,sans-serif;font-size:1rem;font-weight:800;cursor:pointer;box-shadow:0 6px 20px rgba(45,106,255,0.3);margin-bottom:10px;">
          Entrar 🔓
        </button>
      </div>
      <!-- Sin NIP: botón directo -->
      <div id="sinNipZona">
        <button onclick="entrarSesionGuardada()" style="width:100%;padding:16px;background:linear-gradient(135deg,var(--accent),var(--accent2));color:var(--navtext);border:none;border-radius:16px;font-family:Outfit,sans-serif;font-size:1.05rem;font-weight:800;cursor:pointer;box-shadow:0 6px 20px rgba(45,106,255,0.35);margin-bottom:12px;letter-spacing:0.01em;">
          ¡Continuar! →
        </button>
      </div>
      <button onclick="mostrarPanelCodigo(true)" style="width:100%;padding:13px;background:none;border:1.5px solid var(--border);border-radius:14px;font-family:Outfit,sans-serif;font-size:0.85rem;color:var(--dim);cursor:pointer;">
        No soy yo — ingresar con otro código
      </button>
      <div style="text-align:center;margin-top:16px;">
        <span onclick="abrirAdminModal()" style="font-size:0.78rem;color:var(--dim);cursor:pointer;text-decoration:underline;text-underline-offset:3px;">🔐 Acceso administrador</span>
      </div>
    </div>

    <!-- ── PANEL: Código ── -->
    <div class="access-card" id="panelCodigo" style="display:none;">
      <!-- Ícono + título centrado -->
      <div style="display:flex;align-items:center;gap:12px;margin-bottom:22px;">
        <div style="font-size:2.4rem;line-height:1;">🔑</div>
        <div>
          <div id="accTitulo" style="font-size:1.2rem;font-weight:900;color:#1a2b4a;line-height:1.2;">Código de acceso</div>
          <div id="accSubtitulo" style="font-size:0.8rem;color:#7a90b8;margin-top:3px;line-height:1.4;">Ingresa el código que te compartieron</div>
        </div>
      </div>
      <!-- Saludo de regreso (se muestra cuando el nombre ya está guardado) -->
      <div id="accSaludo" style="display:none;background:#f0f7ff;border-radius:12px;padding:12px 14px;margin-bottom:14px;border:1.5px solid #c8deff;">
        <div style="font-size:0.75rem;color:#7a90b8;font-weight:700;">👋 ¡Bienvenid@ de regreso!</div>
        <div id="accSaludoNombre" style="font-size:1rem;font-weight:900;color:#1a2b4a;margin-top:2px;"></div>
      </div>
      <div id="accessErr" class="access-err">Código incorrecto o vencido</div>
      <!-- Campo nombre: solo visible si es primera vez -->
      <div id="accNombreRow">
        <label class="inp-label">Tu nombre</label>
        <input class="inp" id="accNombre" placeholder="¿Cómo te llamas?" autocomplete="off">
      </div>
      <label class="inp-label">Código</label>
      <input class="inp" id="accCodigo" placeholder="Ej: FIN-2026" autocomplete="off" style="font-family:JetBrains Mono,monospace;letter-spacing:0.08em;"
        oninput="accCodigoLookup(this.value)"
        onkeydown="if(event.key==='Enter')verificarCodigo()">
      <button class="btn-main" onclick="verificarCodigo()">Entrar →</button>
      <div style="display:flex;align-items:center;gap:10px;margin:20px 0 10px;">
        <div style="flex:1;height:1.5px;background:#e2eaf8;"></div>
        <span style="font-size:0.72rem;color:#7a90b8;font-weight:700;letter-spacing:0.05em;">¿No tienes código?</span>
        <div style="flex:1;height:1.5px;background:#e2eaf8;"></div>
      </div>
      <button onclick="mostrarPanelSolicitud()" style="width:100%;padding:16px;border:2.5px dashed #2355c9;background:rgba(35,85,201,0.04);color:#2355c9;border-radius:18px;font-family:Outfit,sans-serif;font-size:0.92rem;font-weight:800;cursor:pointer;letter-spacing:0.01em;">
        📩 Solicitar acceso al administrador
      </button>
      <div style="text-align:center;margin-top:20px;padding:14px;background:rgba(35,85,201,0.06);border-radius:14px;">
        <span onclick="abrirAdminModal()" style="font-size:0.9rem;color:#2355c9;cursor:pointer;font-weight:700;letter-spacing:0.01em;">🔒 Acceso administrador</span>
      </div>
    </div>

    <!-- Panel: Solicitar acceso -->
    <div class="access-card" id="panelSolicitud" style="display:none;">
      <div class="access-icon" style="text-align:center;">📩</div>
      <div class="access-title" style="text-align:center;">Solicitar acceso</div>
      <div class="access-sub" style="text-align:center;">El administrador recibirá tu solicitud y te enviará un código si la aprueba</div>
      <div id="solicitudMsg" class="access-err" style="display:none;"></div>
      <label class="inp-label">Tu nombre completo</label>
      <input class="inp" id="solNombre" placeholder="¿Cómo te llamas?" autocomplete="off">
      <label class="inp-label">¿Para qué quieres usar USALA?</label>
      <textarea class="inp" id="solMotivo" placeholder="Ej: Quiero llevar control de mis gastos personales..." style="height:80px;resize:none;"></textarea>
      <label class="inp-label">Tu contacto (WhatsApp, email, etc.)</label>
      <input class="inp" id="solContacto" placeholder="Para que el admin te envíe el código">
      <button class="btn-main" onclick="enviarSolicitud()">📩 Enviar solicitud</button>
      <button onclick="mostrarPanelCodigo()" style="width:100%;padding:12px;background:none;border:none;color:var(--dim);font-family:Outfit,sans-serif;font-size:0.83rem;cursor:pointer;margin-top:4px;">← Ya tengo un código</button>
    </div>

    <!-- Panel: Solicitud enviada -->
    <div class="access-card" id="panelEnviada" style="display:none;text-align:center;padding:32px 20px;">
      <div style="font-size:3rem;margin-bottom:12px;">✅</div>
      <div class="access-title">¡Solicitud enviada!</div>
      <div class="access-sub" style="margin-top:8px;">El administrador revisará tu solicitud y te contactará para darte acceso.<br><br>Cuando tengas tu código, regresa aquí e ingrésalo.</div>
      <button onclick="mostrarPanelCodigo()" style="margin-top:20px;width:100%;padding:13px;background:var(--accent);color:var(--navtext);border:none;border-radius:14px;font-family:Outfit,sans-serif;font-size:0.88rem;font-weight:700;cursor:pointer;">← Volver al login</button>
    </div>
  </div>
</div>

<!-- ══ ADMIN MODAL ══ -->
<div class="admin-modal" id="adminModal">
  <div style="position:absolute;inset:0;" onclick="cerrarAdminModal()"></div>
  <div class="admin-box" style="position:relative;">
    <div class="admin-handle"></div>
    <div style="text-align:center;font-size:2rem;margin-bottom:8px;">🔐</div>
    <div class="admin-title">Acceso Administrador</div>
    <div id="adminErr" class="access-err">Contraseña incorrecta</div>
    <label class="inp-label">Contraseña</label>
    <input class="inp" id="adminPass" type="password" placeholder="Contraseña de administrador" onkeydown="if(event.key==='Enter')verificarAdmin()">
    <button class="btn-main" onclick="verificarAdmin()">Entrar como Admin →</button>
    <div class="admin-hint">¿Primera vez? Usa la clave que te fue asignada</div>
    <button class="admin-recover" onclick="recuperarAdmin()">¿Olvidaste tu contraseña? Restablecer</button>
  </div>
</div>

<!-- ══ DASHBOARD ══ -->
<div class="screen" id="dashboard">
  <div class="topbar">
    <div class="top-logo">USALA <span class="top-ver" id="verBadge"></span></div>
    <div id="topUserName" style="font-size:0.72rem;font-weight:700;color:var(--dim);flex:1;text-align:right;padding-right:10px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;"></div>
    <button class="top-icon" id="btnSolicitudes" onclick="goTab('mas',document.querySelectorAll('.nb')[4]);setTimeout(function(){goSub('codigos');},50);" title="Solicitudes" style="display:none;position:relative;">
      📩
      <span id="badgeSolicitudes" style="position:absolute;top:2px;right:2px;background:#ff3b30;color:#fff;font-size:0.45rem;font-weight:800;width:14px;height:14px;border-radius:50%;display:flex;align-items:center;justify-content:center;"></span>
    </button>
    <!-- Botón U acceso rápido cuentas -->
    <button id="uFabBtn" class="top-icon" onclick="toggleUMenu()" title="Mis cuentas" style="display:none;background:linear-gradient(135deg,var(--accent),var(--accent2));color:#fff;font-weight:900;font-size:0.95rem;letter-spacing:-0.5px;transition:transform 0.2s ease;">U</button>
    <button class="top-icon" id="btnVoz" onclick="toggleVoz()" title="Comando de voz" style="display:none;">🎙️</button>
    <button class="top-icon" onclick="abrirCalc()" title="Calculadora">🔢</button>
    <button class="top-icon" onclick="goTab('mas',document.querySelectorAll('.nb')[4]);setTimeout(function(){goSub('ayuda');},50);" title="Ayuda">❓</button>
  </div>
  <div class="content" id="mainContent"></div>
  <nav class="bot-nav">
    <button class="nb active" onclick="goTab('inicio',this)"><div class="nb-ico">🏠</div><div class="nb-lbl">Inicio</div></button>
    <button class="nb" onclick="goTab('cuentas',this)"><div class="nb-ico">🏦</div><div class="nb-lbl">Cuentas</div></button>
    <button class="nb" onclick="goTab('creditos',this)"><div class="nb-ico">🤝</div><div class="nb-lbl">Créditos</div></button>
    <button class="nb" onclick="goTab('reportes',this)"><div class="nb-ico">📊</div><div class="nb-lbl">Reportes</div></button>
    <button class="nb" onclick="goTab('mas',this)"><div class="nb-ico">⋯</div><div class="nb-lbl">Más</div></button>
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
        <div style="font-size:1rem;font-weight:900;background:linear-gradient(135deg,#667eea,#764ba2);-webkit-background-clip:text;-webkit-text-fill-color:transpar
