<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ComedorU · Gestión del Comedor Universitario</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700;800&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.4/chart.umd.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf-autotable/3.8.2/jspdf.plugin.autotable.min.js"></script>
<style>
/* =========================================================
   TOKENS
========================================================= */
:root{
  --blue-dark:#1E3A8A;
  --blue-dark-2:#16296b;
  --blue-soft:#EEF2FF;
  --green:#22C55E;
  --green-dark:#16A34A;
  --white:#FFFFFF;
  --gray-50:#F8FAFC;
  --gray-100:#F3F4F6;
  --gray-200:#E5E7EB;
  --gray-400:#9CA3AF;
  --text:#111827;
  --text-soft:#6B7280;
  --yellow:#FACC15;
  --yellow-bg:#FEF9C3;
  --red:#EF4444;
  --red-bg:#FEE2E2;
  --green-bg:#DCFCE7;
  --radius-lg:18px;
  --radius-md:12px;
  --radius-sm:8px;
  --shadow-sm:0 1px 2px rgba(16,24,40,.06);
  --shadow-md:0 4px 16px rgba(16,24,40,.08);
  --shadow-lg:0 12px 32px rgba(16,24,40,.12);
  --font-display:'Poppins',sans-serif;
  --font-body:'Inter',sans-serif;
  --bg:var(--gray-50);
  --surface:var(--white);
  --border:var(--gray-200);
  --text-main:var(--text);
  --text-muted:var(--text-soft);
}
html.dark{
  --bg:#0B1220;
  --surface:#141B2D;
  --border:#243046;
  --text-main:#F1F5F9;
  --text-muted:#94A3B8;
  --blue-soft:#1A2340;
  --gray-100:#1A2338;
  --gray-200:#243046;
  --yellow-bg:#3a3312;
  --red-bg:#3a1616;
  --green-bg:#0f2a1c;
}
*{box-sizing:border-box;}
body{
  margin:0;
  background:var(--bg);
  color:var(--text-main);
  font-family:var(--font-body);
  transition:background .3s ease, color .3s ease;
  -webkit-font-smoothing:antialiased;
}
h1,h2,h3,h4,.display{font-family:var(--font-display);}
button{font-family:inherit;cursor:pointer;}
input,select{font-family:inherit;}
::selection{background:var(--green);color:#fff;}

/* Scrollbar */
::-webkit-scrollbar{width:8px;height:8px;}
::-webkit-scrollbar-thumb{background:var(--gray-200);border-radius:8px;}

/* =========================================================
   LAYOUT SHELL
========================================================= */
.app{min-height:100vh;display:flex;flex-direction:column;}

.topbar{
  display:flex;align-items:center;justify-content:space-between;
  padding:16px 28px;background:var(--surface);border-bottom:1px solid var(--border);
  position:sticky;top:0;z-index:40;
}
.brand{display:flex;align-items:center;gap:10px;cursor:pointer;}
.brand-mark{
  width:38px;height:38px;border-radius:10px;
  background:linear-gradient(135deg,var(--blue-dark),var(--green));
  display:flex;align-items:center;justify-content:center;font-size:19px;
  box-shadow:var(--shadow-sm);
}
.brand-name{font-family:var(--font-display);font-weight:700;font-size:17px;letter-spacing:.2px;}
.brand-sub{font-size:11px;color:var(--text-muted);margin-top:-2px;}

.topbar-actions{display:flex;align-items:center;gap:10px;}
.icon-btn{
  width:38px;height:38px;border-radius:50%;border:1px solid var(--border);
  background:var(--surface);display:flex;align-items:center;justify-content:center;
  font-size:16px;transition:all .2s ease;
}
.icon-btn:hover{background:var(--gray-100);transform:translateY(-1px);}

.pill-btn{
  display:flex;align-items:center;gap:6px;
  border:1px solid var(--border);background:var(--surface);
  padding:8px 14px;border-radius:999px;font-size:13px;font-weight:600;color:var(--text-main);
  transition:all .2s ease;
}
.pill-btn:hover{background:var(--gray-100);}

main{flex:1;display:flex;flex-direction:column;}

.view{display:none;animation:fadeSlide .45s cubic-bezier(.22,1,.36,1);}
.view.active{display:block;}
@keyframes fadeSlide{
  from{opacity:0;transform:translateY(10px);}
  to{opacity:1;transform:translateY(0);}
}

/* =========================================================
   LANDING
========================================================= */
.landing-wrap{
  max-width:1000px;margin:0 auto;padding:64px 24px 80px;text-align:center;
}
.landing-eyebrow{
  display:inline-flex;align-items:center;gap:8px;background:var(--blue-soft);
  color:var(--blue-dark);padding:6px 14px;border-radius:999px;font-size:12.5px;font-weight:600;
  margin-bottom:22px;
}
html.dark .landing-eyebrow{color:#93a5f5;}
.landing-title{font-size:38px;font-weight:800;margin:0 0 12px;line-height:1.15;letter-spacing:-.5px;}
.landing-title span{color:var(--green);}
.landing-desc{color:var(--text-muted);font-size:16px;max-width:560px;margin:0 auto 48px;line-height:1.6;}

.portal-grid{
  display:grid;grid-template-columns:1fr 1fr;gap:24px;text-align:left;
}
@media(max-width:760px){.portal-grid{grid-template-columns:1fr;}}

.portal-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);
  padding:32px;box-shadow:var(--shadow-sm);position:relative;overflow:hidden;
  transition:transform .35s cubic-bezier(.22,1,.36,1),box-shadow .35s ease;
}
.portal-card:hover{transform:translateY(-6px);box-shadow:var(--shadow-lg);}
.portal-card::after{
  content:'';position:absolute;inset:0;opacity:0;transition:opacity .35s ease;
  background:radial-gradient(circle at 85% 15%, rgba(34,197,94,.12), transparent 60%);
  pointer-events:none;
}
.portal-card:hover::after{opacity:1;}
.portal-icon{
  width:58px;height:58px;border-radius:16px;display:flex;align-items:center;justify-content:center;
  font-size:28px;margin-bottom:20px;
}
.portal-icon.student{background:var(--blue-soft);}
.portal-icon.cook{background:var(--green-bg);}
.portal-card h3{font-size:20px;margin:0 0 8px;}
.portal-card p{color:var(--text-muted);font-size:14px;line-height:1.6;margin:0 0 24px;}
.btn{
  border:none;border-radius:var(--radius-sm);padding:12px 20px;font-weight:600;font-size:14px;
  display:inline-flex;align-items:center;gap:8px;transition:all .2s ease;
}
.btn-primary{background:var(--blue-dark);color:#fff;}
.btn-primary:hover{background:var(--blue-dark-2);transform:translateY(-1px);box-shadow:var(--shadow-md);}
.btn-green{background:var(--green);color:#fff;}
.btn-green:hover{background:var(--green-dark);transform:translateY(-1px);box-shadow:var(--shadow-md);}
.btn-outline{background:transparent;border:1px solid var(--border);color:var(--text-main);}
.btn-outline:hover{background:var(--gray-100);}
.btn-block{width:100%;justify-content:center;}
.btn:disabled{opacity:.55;cursor:not-allowed;transform:none !important;box-shadow:none !important;}

/* =========================================================
   SHARED PAGE HEADER (with back button)
========================================================= */
.page-shell{max-width:1180px;margin:0 auto;padding:28px 24px 60px;width:100%;}
.page-head{display:flex;align-items:center;gap:14px;margin-bottom:26px;}
.back-btn{
  width:36px;height:36px;border-radius:50%;border:1px solid var(--border);background:var(--surface);
  display:flex;align-items:center;justify-content:center;font-size:15px;flex-shrink:0;
}
.back-btn:hover{background:var(--gray-100);}
.page-title{font-size:22px;font-weight:700;margin:0;}
.page-sub{color:var(--text-muted);font-size:13.5px;margin-top:2px;}

/* =========================================================
   FORM (estudiante)
========================================================= */
.form-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);
  padding:32px;max-width:640px;margin:0 auto;box-shadow:var(--shadow-sm);
}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px;}
@media(max-width:600px){.form-grid{grid-template-columns:1fr;}}
.field{display:flex;flex-direction:column;gap:6px;margin-bottom:4px;}
.field.full{grid-column:1/-1;}
.field label{font-size:13px;font-weight:600;color:var(--text-main);}
.field label .opt{color:var(--text-muted);font-weight:400;font-size:11.5px;}
.field input, .field select{
  padding:11px 13px;border:1.5px solid var(--border);border-radius:var(--radius-sm);
  background:var(--bg);color:var(--text-main);font-size:14px;transition:border-color .2s ease, box-shadow .2s ease;
}
.field input:focus, .field select:focus{
  outline:none;border-color:var(--blue-dark);box-shadow:0 0 0 3px rgba(30,58,138,.12);
}
.field.error input, .field.error select{border-color:var(--red);}
.field-error-msg{color:var(--red);font-size:12px;display:none;align-items:center;gap:4px;}
.field.error .field-error-msg{display:flex;}
.form-actions{display:flex;gap:12px;margin-top:22px;}

/* =========================================================
   LOGIN (cocinera)
========================================================= */
.login-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);
  padding:36px;max-width:400px;margin:40px auto 0;box-shadow:var(--shadow-sm);text-align:center;
}
.login-card .portal-icon{margin:0 auto 18px;}
.login-hint{font-size:12px;color:var(--text-muted);background:var(--gray-100);border-radius:var(--radius-sm);padding:10px 12px;margin-top:16px;line-height:1.5;}

/* =========================================================
   MENÚ DEL DÍA / RESERVA
========================================================= */
.menu-section{max-width:640px;margin:0 auto 28px;}
.menu-section h3{font-size:16px;margin:0 0 4px;display:flex;align-items:center;gap:8px;}
.menu-section .menu-sub{font-size:13px;color:var(--text-muted);margin:0 0 16px;}
.menu-options{display:grid;grid-template-columns:1fr 1fr;gap:16px;}
@media(max-width:600px){.menu-options{grid-template-columns:1fr;}}
.menu-option-card{
  background:var(--surface);border:2px solid var(--border);border-radius:var(--radius-md);
  padding:18px;cursor:pointer;transition:all .25s cubic-bezier(.22,1,.36,1);position:relative;
}
.menu-option-card:hover{border-color:var(--green);transform:translateY(-2px);box-shadow:var(--shadow-md);}
.menu-option-card.selected{border-color:var(--green);background:var(--green-bg);}
.menu-option-card .mo-tag{
  display:inline-block;font-size:11px;font-weight:700;color:var(--blue-dark);background:var(--blue-soft);
  padding:3px 9px;border-radius:999px;margin-bottom:10px;
}
html.dark .menu-option-card .mo-tag{color:#93a5f5;}
.menu-option-card .mo-check{
  position:absolute;top:14px;right:14px;width:22px;height:22px;border-radius:50%;border:2px solid var(--border);
  display:flex;align-items:center;justify-content:center;font-size:12px;background:var(--surface);transition:all .2s ease;
}
.menu-option-card.selected .mo-check{background:var(--green);border-color:var(--green);color:#fff;}
.menu-option-card dl{margin:0;font-size:13px;color:var(--text-main);line-height:1.85;}
.menu-option-card dl b{font-weight:600;color:var(--text-muted);font-size:11.5px;text-transform:uppercase;letter-spacing:.3px;display:block;margin-top:8px;}
.menu-option-card dl b:first-child{margin-top:0;}
.menu-empty{
  border:1.5px dashed var(--border);border-radius:var(--radius-md);padding:26px;text-align:center;
  color:var(--text-muted);font-size:13.5px;background:var(--gray-100);
}
.menu-cook-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
@media(max-width:760px){.menu-cook-grid{grid-template-columns:1fr;}}
.menu-cook-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);padding:22px;box-shadow:var(--shadow-sm);}
.menu-cook-card h4{margin:0 0 14px;font-size:14.5px;}
.reserva-tag{
  display:inline-flex;align-items:center;gap:4px;font-size:11px;font-weight:700;color:var(--green-dark);
  background:var(--green-bg);padding:3px 8px;border-radius:999px;margin-top:4px;
}

/* =========================================================
   DASHBOARD
========================================================= */
.tabs{display:flex;gap:6px;border-bottom:1px solid var(--border);margin-bottom:24px;flex-wrap:wrap;}
.tab-btn{
  padding:10px 16px;background:none;border:none;font-size:13.5px;font-weight:600;color:var(--text-muted);
  border-bottom:2.5px solid transparent;margin-bottom:-1px;transition:all .2s ease;
}
.tab-btn:hover{color:var(--text-main);}
.tab-btn.active{color:var(--blue-dark);border-color:var(--green);}
html.dark .tab-btn.active{color:#8ea3ff;}
.tab-panel{display:none;}
.tab-panel.active{display:block;animation:fadeSlide .35s ease;}

.stat-grid{
  display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:26px;
}
@media(max-width:900px){.stat-grid{grid-template-columns:repeat(2,1fr);}}
@media(max-width:480px){.stat-grid{grid-template-columns:1fr;}}
.stat-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-md);
  padding:18px 20px;box-shadow:var(--shadow-sm);position:relative;overflow:hidden;
}
.stat-label{font-size:12px;color:var(--text-muted);font-weight:600;text-transform:uppercase;letter-spacing:.4px;}
.stat-value{font-size:28px;font-weight:800;font-family:var(--font-display);margin-top:6px;}
.stat-card.accent-blue .stat-value{color:var(--blue-dark);}
.stat-card.accent-green .stat-value{color:var(--green-dark);}
.stat-card.accent-yellow .stat-value{color:#a16207;}
html.dark .stat-card.accent-yellow .stat-value{color:var(--yellow);}
.stat-card.accent-purple .stat-value{color:#7c3aed;}

/* signature "plate" progress ring */
.plate-hero{
  display:flex;align-items:center;gap:28px;background:var(--surface);border:1px solid var(--border);
  border-radius:var(--radius-lg);padding:24px 28px;margin-bottom:26px;box-shadow:var(--shadow-sm);flex-wrap:wrap;
}
.plate-ring-wrap{position:relative;width:118px;height:118px;flex-shrink:0;}
.plate-ring-wrap svg{transform:rotate(-90deg);}
.plate-ring-bg{fill:none;stroke:var(--gray-200);stroke-width:11;}
.plate-ring-fg{fill:none;stroke:var(--green);stroke-width:11;stroke-linecap:round;transition:stroke-dashoffset .8s cubic-bezier(.22,1,.36,1);}
.plate-ring-label{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;}
.plate-ring-label .pct{font-size:22px;font-weight:800;font-family:var(--font-display);}
.plate-ring-label .txt{font-size:10px;color:var(--text-muted);}
.plate-copy h3{margin:0 0 6px;font-size:17px;}
.plate-copy p{margin:0;color:var(--text-muted);font-size:13.5px;max-width:420px;line-height:1.55;}

.toolbar{display:flex;gap:12px;margin-bottom:18px;flex-wrap:wrap;align-items:center;justify-content:space-between;}
.search-box{position:relative;flex:1;min-width:220px;max-width:360px;}
.search-box input{
  width:100%;padding:10px 14px 10px 36px;border:1.5px solid var(--border);border-radius:999px;
  background:var(--surface);color:var(--text-main);font-size:13.5px;
}
.search-box input:focus{outline:none;border-color:var(--blue-dark);}
.search-box .ico{position:absolute;left:13px;top:50%;transform:translateY(-50%);font-size:13px;color:var(--text-muted);}
.filter-group{display:flex;gap:6px;background:var(--gray-100);padding:4px;border-radius:999px;}
.filter-chip{
  padding:7px 14px;border:none;background:none;border-radius:999px;font-size:12.5px;font-weight:600;
  color:var(--text-muted);transition:all .2s ease;
}
.filter-chip.active{background:var(--surface);color:var(--blue-dark);box-shadow:var(--shadow-sm);}
html.dark .filter-chip.active{color:#8ea3ff;}
.export-group{display:flex;gap:8px;}

.table-wrap{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);overflow:hidden;
  box-shadow:var(--shadow-sm);
}
table{width:100%;border-collapse:collapse;font-size:13.5px;}
thead th{
  text-align:left;padding:13px 16px;background:var(--gray-100);color:var(--text-muted);
  font-size:11.5px;text-transform:uppercase;letter-spacing:.4px;font-weight:700;
}
tbody td{padding:13px 16px;border-top:1px solid var(--border);}
tbody tr{transition:background .15s ease;}
tbody tr:hover{background:var(--gray-100);}
.cell-name{font-weight:600;}
.cell-sub{font-size:11.5px;color:var(--text-muted);}
.badge{
  display:inline-flex;align-items:center;gap:5px;padding:4px 10px;border-radius:999px;
  font-size:11.5px;font-weight:700;
}
.badge.pending{background:var(--yellow-bg);color:#92660a;}
html.dark .badge.pending{color:var(--yellow);}
.badge.done{background:var(--green-bg);color:var(--green-dark);}
.deliver-btn{
  padding:7px 14px;border-radius:var(--radius-sm);border:none;font-size:12.5px;font-weight:700;
  background:var(--blue-dark);color:#fff;transition:all .2s ease;
}
.deliver-btn:hover:not(:disabled){background:var(--blue-dark-2);}
.deliver-btn:disabled{background:var(--gray-200);color:var(--text-muted);cursor:not-allowed;}
.empty-state{padding:60px 24px;text-align:center;color:var(--text-muted);}
.empty-state .em-icon{font-size:34px;margin-bottom:10px;}

/* charts */
.chart-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
@media(max-width:900px){.chart-grid{grid-template-columns:1fr;}}
.chart-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);
  padding:22px;box-shadow:var(--shadow-sm);
}
.chart-card h4{margin:0 0 4px;font-size:14.5px;}
.chart-card .chart-sub{font-size:12px;color:var(--text-muted);margin-bottom:14px;}
.chart-card canvas{max-height:260px;}

.history-controls{display:flex;gap:10px;margin-bottom:18px;flex-wrap:wrap;align-items:center;}
.date-input{
  padding:9px 12px;border:1.5px solid var(--border);border-radius:var(--radius-sm);
  background:var(--surface);color:var(--text-main);font-size:13px;
}

/* =========================================================
   TOAST
========================================================= */
#toast-stack{
  position:fixed;bottom:24px;right:24px;display:flex;flex-direction:column;gap:10px;z-index:200;
  max-width:340px;
}
.toast{
  background:var(--surface);border:1px solid var(--border);border-left:4px solid var(--green);
  padding:14px 16px;border-radius:var(--radius-md);box-shadow:var(--shadow-lg);
  display:flex;align-items:flex-start;gap:10px;font-size:13.5px;
  animation:toastIn .35s cubic-bezier(.22,1,.36,1);
}
.toast.error{border-left-color:var(--red);}
.toast.info{border-left-color:var(--blue-dark);}
.toast .t-icon{font-size:17px;line-height:1;}
.toast .t-body b{display:block;margin-bottom:2px;}
.toast .t-body span{color:var(--text-muted);font-size:12px;}
@keyframes toastIn{from{opacity:0;transform:translateX(30px);}to{opacity:1;transform:translateX(0);}}
.toast.leaving{animation:toastOut .3s ease forwards;}
@keyframes toastOut{to{opacity:0;transform:translateX(30px);}}

/* =========================================================
   LOADER
========================================================= */
#loader-overlay{
  position:fixed;inset:0;background:var(--bg);display:flex;flex-direction:column;align-items:center;justify-content:center;
  z-index:500;gap:16px;transition:opacity .4s ease;
}
.spinner{
  width:42px;height:42px;border-radius:50%;border:4px solid var(--gray-200);border-top-color:var(--green);
  animation:spin .8s linear infinite;
}
@keyframes spin{to{transform:rotate(360deg);}}
#loader-overlay p{color:var(--text-muted);font-size:13.5px;font-weight:600;}

footer.app-footer{
  text-align:center;padding:22px;color:var(--text-muted);font-size:11.5px;border-top:1px solid var(--border);
}
.small-note{font-size:12px;color:var(--text-muted);}
</style>
</head>
<body>

<div id="loader-overlay">
  <div class="spinner"></div>
  <p id="loader-text">Cargando comedor universitario…</p>
</div>

<div class="app" id="app" style="display:none;">

  <div class="topbar">
    <div class="brand" onclick="ir('landing')">
      <div class="brand-mark">🍽️</div>
      <div>
        <div class="brand-name">ComedorU</div>
        <div class="brand-sub">Gestión de beneficiarios</div>
      </div>
    </div>
    <div class="topbar-actions">
      <span id="session-pill" class="pill-btn" style="display:none;">
        👩‍🍳 <span id="session-label"></span>
      </span>
      <button class="icon-btn" onclick="toggleTheme()" id="theme-toggle" title="Cambiar tema">🌙</button>
    </div>
  </div>

  <main>

    <!-- ================= LANDING ================= -->
    <section class="view active" id="view-landing">
      <div class="landing-wrap">
        <div class="landing-eyebrow">🎓 Sistema de comedor universitario</div>
        <h1 class="landing-title">Almuerzos entregados con <span>orden y a tiempo</span></h1>
        <p class="landing-desc">Registra a los estudiantes beneficiarios y controla la entrega diaria de almuerzos en tiempo real, sin duplicados y con estadísticas al instante.</p>

        <div class="portal-grid">
          <div class="portal-card">
            <div class="portal-icon student">👨‍🎓</div>
            <h3>Soy estudiante</h3>
            <p>Regístrate como beneficiario del comedor con tu código universitario y datos académicos.</p>
            <button class="btn btn-primary btn-block" onclick="ir('estudiante')">Registrarme <span>→</span></button>
          </div>
          <div class="portal-card">
            <div class="portal-icon cook">👩‍🍳</div>
            <h3>Soy cocinera / administración</h3>
            <p>Ingresa al panel de control para entregar almuerzos, ver estadísticas e historial.</p>
            <button class="btn btn-green btn-block" onclick="ir('login')">Ingresar al panel <span>→</span></button>
          </div>
        </div>
      </div>
    </section>

    <!-- ================= ESTUDIANTE ================= -->
    <section class="view" id="view-estudiante">
      <div class="page-shell" style="max-width:720px;">
        <div class="page-head">
          <button class="back-btn" onclick="ir('landing')">←</button>
          <div>
            <h2 class="page-title">Registro de beneficiario</h2>
            <div class="page-sub">Completa tus datos para acceder al almuerzo de hoy</div>
          </div>
        </div>

        <div class="menu-section">
          <h3>🍛 Menú de hoy</h3>
          <p class="menu-sub">Elige el menú que quieres reservar. Se guardará junto con tu registro.</p>
          <div id="menu-hoy-render"></div>
        </div>

        <div class="form-card">
          <form id="form-estudiante" novalidate>
            <div class="form-grid">
              <div class="field" id="f-codigo">
                <label>Código universitario</label>
                <input type="text" id="in-codigo" placeholder="Ej. 2021045896" autocomplete="off">
                <div class="field-error-msg">⚠️ Ingresa tu código universitario</div>
              </div>
              <div class="field" id="f-nombre">
                <label>Nombre completo</label>
                <input type="text" id="in-nombre" placeholder="Ej. María Fernández Ruiz">
                <div class="field-error-msg">⚠️ Ingresa tu nombre completo</div>
              </div>
              <div class="field" id="f-facultad">
                <label>Facultad</label>
                <select id="in-facultad">
                  <option value="">Selecciona tu facultad</option>
                  <option>Ingeniería</option>
                  <option>Ciencias de la Salud</option>
                  <option>Ciencias Administrativas</option>
                  <option>Derecho y Ciencias Políticas</option>
                  <option>Educación</option>
                  <option>Ciencias Sociales</option>
                  <option>Arquitectura</option>
                </select>
                <div class="field-error-msg">⚠️ Selecciona tu facultad</div>
              </div>
              <div class="field" id="f-carrera">
                <label>Carrera</label>
                <input type="text" id="in-carrera" placeholder="Ej. Ingeniería de Sistemas">
                <div class="field-error-msg">⚠️ Ingresa tu carrera</div>
              </div>
              <div class="field" id="f-ciclo">
                <label>Ciclo</label>
                <select id="in-ciclo">
                  <option value="">Selecciona tu ciclo</option>
                  <script>document.write(Array.from({length:10},(_,i)=>`<option>${i+1}° ciclo</option>`).join(''))</script>
                </select>
                <div class="field-error-msg">⚠️ Selecciona tu ciclo</div>
              </div>
              <div class="field" id="f-correo">
                <label>Correo institucional <span class="opt">(opcional)</span></label>
                <input type="email" id="in-correo" placeholder="nombre@universidad.edu.pe">
                <div class="field-error-msg">⚠️ Ingresa un correo válido</div>
              </div>
            </div>
            <div class="form-actions">
              <button type="submit" class="btn btn-primary btn-block" id="btn-registrar">✅ Confirmar registro</button>
            </div>
          </form>
        </div>
      </div>
    </section>

    <!-- ================= LOGIN COCINERA ================= -->
    <section class="view" id="view-login">
      <div class="page-shell" style="max-width:500px;">
        <div class="page-head">
          <button class="back-btn" onclick="ir('landing')">←</button>
          <div>
            <h2 class="page-title">Acceso del personal</h2>
            <div class="page-sub">Panel de cocinera / administración</div>
          </div>
        </div>
        <div class="login-card">
          <div class="portal-icon cook" style="margin:0 auto 18px;">👩‍🍳</div>
          <form id="form-login">
            <div class="field" style="text-align:left;margin-bottom:14px;">
              <label>Usuario</label>
              <input type="text" id="in-user" placeholder="cocinera" autocomplete="off">
            </div>
            <div class="field" style="text-align:left;" id="f-pass">
              <label>Contraseña</label>
              <input type="password" id="in-pass" placeholder="••••••••">
              <div class="field-error-msg">⚠️ Usuario o contraseña incorrectos</div>
            </div>
            <button type="submit" class="btn btn-green btn-block" style="margin-top:18px;">Ingresar al panel</button>
          </form>
          <div class="login-hint">🔐 Acceso de demostración — usuario <b>cocinera</b> / contraseña <b>comedor2026</b>. En producción se recomienda autenticación real en el servidor (bcrypt + JWT) con una base de datos como Firebase o MySQL.</div>
        </div>
      </div>
    </section>

    <!-- ================= DASHBOARD COCINERA ================= -->
    <section class="view" id="view-dashboard">
      <div class="page-shell">
        <div class="page-head">
          <button class="back-btn" onclick="cerrarSesion()">←</button>
          <div>
            <h2 class="page-title">Panel de cocinera</h2>
            <div class="page-sub" id="fecha-hoy"></div>
          </div>
        </div>

        <div class="tabs">
          <button class="tab-btn active" data-tab="resumen" onclick="cambiarTab('resumen')">📊 Resumen</button>
          <button class="tab-btn" data-tab="entregas" onclick="cambiarTab('entregas')">🍽️ Entrega de almuerzos</button>
          <button class="tab-btn" data-tab="menu" onclick="cambiarTab('menu')">🍛 Menú del día</button>
          <button class="tab-btn" data-tab="estadisticas" onclick="cambiarTab('estadisticas')">📈 Estadísticas</button>
          <button class="tab-btn" data-tab="historial" onclick="cambiarTab('historial')">🗂️ Historial</button>
        </div>

        <!-- RESUMEN -->
        <div class="tab-panel active" id="tab-resumen">
          <div class="plate-hero">
            <div class="plate-ring-wrap">
              <svg width="118" height="118" viewBox="0 0 118 118">
                <circle class="plate-ring-bg" cx="59" cy="59" r="50"></circle>
                <circle class="plate-ring-fg" id="plate-ring" cx="59" cy="59" r="50" stroke-dasharray="314" stroke-dashoffset="314"></circle>
              </svg>
              <div class="plate-ring-label"><span class="pct" id="plate-pct">0%</span><span class="txt">del plato servido</span></div>
            </div>
            <div class="plate-copy">
              <h3>Avance de entregas de hoy</h3>
              <p id="plate-desc">Aún no hay registros para el día de hoy.</p>
            </div>
          </div>

          <div class="stat-grid">
            <div class="stat-card accent-blue"><div class="stat-label">Estudiantes registrados</div><div class="stat-value" id="st-total">0</div></div>
            <div class="stat-card accent-green"><div class="stat-label">Almuerzos entregados</div><div class="stat-value" id="st-entregados">0</div></div>
            <div class="stat-card accent-yellow"><div class="stat-label">Almuerzos pendientes</div><div class="stat-value" id="st-pendientes">0</div></div>
            <div class="stat-card accent-purple"><div class="stat-label">% de entregas</div><div class="stat-value" id="st-porcentaje">0%</div></div>
          </div>
        </div>

        <!-- ENTREGAS -->
        <div class="tab-panel" id="tab-entregas">
          <div class="toolbar">
            <div class="search-box">
              <span class="ico">🔎</span>
              <input type="text" id="in-buscar" placeholder="Buscar por código, nombre o facultad…" oninput="renderTabla()">
            </div>
            <div class="filter-group" id="filtros">
              <button class="filter-chip active" data-f="todos" onclick="setFiltro('todos')">Todos</button>
              <button class="filter-chip" data-f="pendiente" onclick="setFiltro('pendiente')">Pendientes</button>
              <button class="filter-chip" data-f="entregado" onclick="setFiltro('entregado')">Entregados</button>
            </div>
          </div>
          <div class="table-wrap">
            <table>
              <thead>
                <tr><th>Código</th><th>Estudiante</th><th>Facultad / Carrera</th><th>Menú reservado</th><th>Estado</th><th>Hora de entrega</th><th>Acción</th></tr>
              </thead>
              <tbody id="tbody-estudiantes"></tbody>
            </table>
            <div class="empty-state" id="empty-tabla" style="display:none;">
              <div class="em-icon">🍽️</div>
              <div>No se encontraron estudiantes con ese criterio.</div>
            </div>
          </div>
        </div>

        <!-- MENU DEL DIA -->
        <div class="tab-panel" id="tab-menu">
          <p class="small-note" style="margin-bottom:16px;">Configura las opciones de menú disponibles para hoy (<span id="menu-fecha-label"></span>). Los estudiantes las verán al registrarse y podrán reservar la que prefieran.</p>
          <div class="menu-cook-grid">
            <div class="menu-cook-card">
              <h4>🅰️ Menú A</h4>
              <div class="field"><label>Entrada</label><input type="text" id="menuA-entrada" placeholder="Ej. Crema de zapallo"></div>
              <div class="field"><label>Plato de fondo</label><input type="text" id="menuA-fondo" placeholder="Ej. Lomo saltado"></div>
              <div class="field"><label>Postre</label><input type="text" id="menuA-postre" placeholder="Ej. Gelatina"></div>
              <div class="field"><label>Bebida</label><input type="text" id="menuA-bebida" placeholder="Ej. Chicha morada"></div>
            </div>
            <div class="menu-cook-card">
              <h4>🅱️ Menú B</h4>
              <div class="field"><label>Entrada</label><input type="text" id="menuB-entrada" placeholder="Ej. Ensalada rusa"></div>
              <div class="field"><label>Plato de fondo</label><input type="text" id="menuB-fondo" placeholder="Ej. Tallarines verdes"></div>
              <div class="field"><label>Postre</label><input type="text" id="menuB-postre" placeholder="Ej. Fruta"></div>
              <div class="field"><label>Bebida</label><input type="text" id="menuB-bebida" placeholder="Ej. Refresco de maracuyá"></div>
            </div>
          </div>
          <div class="form-actions" style="max-width:640px;">
            <button class="btn btn-green" onclick="guardarMenu()">💾 Guardar menú de hoy</button>
          </div>
        </div>

        <!-- ESTADISTICAS -->
        <div class="tab-panel" id="tab-estadisticas">
          <div class="chart-grid">
            <div class="chart-card">
              <h4>Entregados vs. pendientes</h4>
              <div class="chart-sub">Estado actual de los almuerzos de hoy</div>
              <canvas id="chart-donut"></canvas>
            </div>
            <div class="chart-card">
              <h4>Facultades con más beneficiarios</h4>
              <div class="chart-sub">Total de estudiantes registrados por facultad</div>
              <canvas id="chart-facultades"></canvas>
            </div>
            <div class="chart-card" style="grid-column:1/-1;">
              <h4>Entregas por hora</h4>
              <div class="chart-sub">Distribución de entregas a lo largo del día de hoy</div>
              <canvas id="chart-horas"></canvas>
            </div>
          </div>
        </div>

        <!-- HISTORIAL -->
        <div class="tab-panel" id="tab-historial">
          <div class="history-controls">
            <div class="filter-group" id="filtros-historial">
              <button class="filter-chip active" data-hf="dia" onclick="setFiltroHistorial('dia')">Día</button>
              <button class="filter-chip" data-hf="semana" onclick="setFiltroHistorial('semana')">Semana</button>
              <button class="filter-chip" data-hf="mes" onclick="setFiltroHistorial('mes')">Mes</button>
            </div>
            <input type="date" class="date-input" id="in-fecha-historial">
            <div style="flex:1;"></div>
            <div class="export-group">
              <button class="btn btn-outline" onclick="exportar('csv')">⬇️ CSV</button>
              <button class="btn btn-outline" onclick="exportar('excel')">⬇️ Excel</button>
              <button class="btn btn-outline" onclick="exportar('pdf')">⬇️ PDF</button>
            </div>
          </div>
          <div class="table-wrap">
            <table>
              <thead><tr><th>Código</th><th>Estudiante</th><th>Facultad</th><th>Fecha</th><th>Hora de entrega</th></tr></thead>
              <tbody id="tbody-historial"></tbody>
            </table>
            <div class="empty-state" id="empty-historial" style="display:none;">
              <div class="em-icon">🗂️</div>
              <div>No hay entregas registradas en este rango de fechas.</div>
            </div>
          </div>
        </div>

      </div>
    </section>

  </main>

  <footer class="app-footer">
    ComedorU · Proyecto de gestión de comedor universitario · Datos almacenados de forma persistente y compartida
  </footer>
</div>

<div id="toast-stack"></div>

<script>
/* =========================================================
   ESTADO GLOBAL
========================================================= */
const FACULTADES_ORDEN = ['Ingeniería','Ciencias de la Salud','Ciencias Administrativas','Derecho y Ciencias Políticas','Educación','Ciencias Sociales','Arquitectura'];
const CRED_KEY = 'cocinera-credenciales';
const DATA_KEY = 'comedor-data';

let DB = { students: [], deliveries: [], menu: null }; // students = beneficiarios; deliveries = log histórico; menu = opciones del día
let filtroActual = 'todos';
let filtroHistorial = 'dia';
let charts = {};
let sesionActiva = false;
let menuSeleccionado = null; // id de la opción de menú elegida por el estudiante en el formulario actual

/* =========================================================
   UTILIDADES
========================================================= */
function hoyISO(){ return new Date().toISOString().slice(0,10); }
function horaAhora(){ return new Date().toLocaleTimeString('es-PE',{hour:'2-digit',minute:'2-digit',second:'2-digit'}); }
function fechaLegible(){
  return new Date().toLocaleDateString('es-PE',{weekday:'long',year:'numeric',month:'long',day:'numeric'});
}
function escapeHtml(s){ return String(s).replace(/[&<>"']/g, c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c])); }

function mostrarToast(msg, tipo='success', titulo=''){
  const stack = document.getElementById('toast-stack');
  const div = document.createElement('div');
  div.className = 'toast ' + (tipo==='success'?'':tipo);
  const icons = {success:'✅', error:'⚠️', info:'ℹ️'};
  div.innerHTML = `<span class="t-icon">${icons[tipo]||'✅'}</span><div class="t-body">${titulo?`<b>${escapeHtml(titulo)}</b>`:''}<span>${escapeHtml(msg)}</span></div>`;
  stack.appendChild(div);
  setTimeout(()=>{
    div.classList.add('leaving');
    setTimeout(()=>div.remove(),300);
  }, 3800);
}

/* =========================================================
   PERSISTENCIA (Storage API — hace de "base de datos" compartida)
========================================================= */
async function cargarDatos(){
  try{
    const res = await window.storage.get(DATA_KEY, true);
    if(res && res.value){ DB = JSON.parse(res.value); }
  }catch(e){ /* aún no existe la clave -> usamos DB vacío */ }

  try{
    const cred = await window.storage.get(CRED_KEY, true);
    if(!cred){ throw new Error('sin credenciales'); }
  }catch(e){
    // primera vez: crear credenciales por defecto
    try{ await window.storage.set(CRED_KEY, JSON.stringify({user:'cocinera', pass:'comedor2026'}), true); }catch(err){}
  }
}

async function guardarDatos(){
  try{
    const ok = await window.storage.set(DATA_KEY, JSON.stringify(DB), true);
    if(!ok) mostrarToast('No se pudo guardar la información. Intenta nuevamente.','error','Error de almacenamiento');
  }catch(e){
    mostrarToast('Error de conexión con el almacenamiento.','error','Error');
  }
}

/* =========================================================
   NAVEGACIÓN
========================================================= */
function ir(vista){
  document.querySelectorAll('.view').forEach(v=>v.classList.remove('active'));
  document.getElementById('view-'+vista).classList.add('active');
  window.scrollTo({top:0,behavior:'smooth'});
  if(vista==='dashboard'){ renderTodoElPanel(); }
  if(vista==='estudiante'){ menuSeleccionado = null; renderMenuHoy(); }
}

/* =========================================================
   MENÚ DEL DÍA (vista estudiante)
========================================================= */
function renderMenuHoy(){
  const cont = document.getElementById('menu-hoy-render');
  const hoy = hoyISO();
  if(!DB.menu || DB.menu.fecha !== hoy || !DB.menu.opciones || DB.menu.opciones.every(o=>!o.fondo)){
    cont.innerHTML = `<div class="menu-empty">🍽️ El menú de hoy aún no ha sido publicado por el comedor. Puedes registrarte y tu almuerzo será el del día.</div>`;
    return;
  }
  cont.innerHTML = `<div class="menu-options">` + DB.menu.opciones.map(o=>{
    if(!o.fondo) return '';
    const sel = menuSeleccionado===o.id;
    return `
    <div class="menu-option-card ${sel?'selected':''}" onclick="elegirMenu('${o.id}')">
      <div class="mo-check">${sel?'✓':''}</div>
      <span class="mo-tag">${escapeHtml(o.nombre)}</span>
      <dl>
        ${o.entrada?`<b>Entrada</b>${escapeHtml(o.entrada)}`:''}
        ${o.fondo?`<b>Plato de fondo</b>${escapeHtml(o.fondo)}`:''}
        ${o.postre?`<b>Postre</b>${escapeHtml(o.postre)}`:''}
        ${o.bebida?`<b>Bebida</b>${escapeHtml(o.bebida)}`:''}
      </dl>
    </div>`;
  }).join('') + `</div>`;
}

function elegirMenu(id){
  menuSeleccionado = (menuSeleccionado===id) ? null : id;
  renderMenuHoy();
}

function cerrarSesion(){
  sesionActiva = false;
  document.getElementById('session-pill').style.display='none';
  ir('landing');
}

/* =========================================================
   TEMA CLARO / OSCURO
========================================================= */
function toggleTheme(){
  const html = document.documentElement;
  html.classList.toggle('dark');
  const isDark = html.classList.contains('dark');
  document.getElementById('theme-toggle').textContent = isDark ? '☀️' : '🌙';
  localStorage_safe_set('comedor-theme', isDark?'dark':'light');
  refrescarGraficos();
}
// Nota: para la preferencia de tema (no datos del comedor) usamos una variable en memoria,
// ya que localStorage no está disponible de forma fiable en este entorno de artefactos.
let temaMemoria = 'light';
function localStorage_safe_set(k,v){ temaMemoria = v; }

/* =========================================================
   VALIDACIÓN Y REGISTRO DE ESTUDIANTE
========================================================= */
document.getElementById('form-estudiante').addEventListener('submit', async function(e){
  e.preventDefault();
  const codigo = document.getElementById('in-codigo').value.trim();
  const nombre = document.getElementById('in-nombre').value.trim();
  const facultad = document.getElementById('in-facultad').value;
  const carrera = document.getElementById('in-carrera').value.trim();
  const ciclo = document.getElementById('in-ciclo').value;
  const correo = document.getElementById('in-correo').value.trim();

  let valido = true;
  const marcar = (id, ok) => {
    const el = document.getElementById(id);
    el.classList.toggle('error', !ok);
    if(!ok) valido = false;
  };

  marcar('f-codigo', codigo.length>0);
  marcar('f-nombre', nombre.length>0);
  marcar('f-facultad', facultad.length>0);
  marcar('f-carrera', carrera.length>0);
  marcar('f-ciclo', ciclo.length>0);
  const correoValido = correo.length===0 || /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(correo);
  marcar('f-correo', correoValido);

  if(!valido){
    mostrarToast('Revisa los campos marcados en rojo antes de continuar.','error','Faltan datos obligatorios');
    return;
  }

  if(DB.students.some(s => s.codigo === codigo)){
    marcar('f-codigo', false);
    mostrarToast('Ese código universitario ya está registrado en el comedor.','error','Código duplicado');
    return;
  }

  const hayMenuPublicado = DB.menu && DB.menu.fecha===hoyISO() && DB.menu.opciones && DB.menu.opciones.some(o=>o.fondo);
  if(hayMenuPublicado && !menuSeleccionado){
    mostrarToast('Elige uno de los menús disponibles antes de registrarte.','error','Falta reservar tu menú');
    return;
  }
  const menuElegidoObj = hayMenuPublicado ? DB.menu.opciones.find(o=>o.id===menuSeleccionado) : null;

  const btn = document.getElementById('btn-registrar');
  btn.disabled = true; btn.textContent = 'Registrando…';

  const nuevo = {
    codigo, nombre, facultad, carrera, ciclo, correo,
    estado: 'pendiente',
    fechaRegistro: hoyISO(),
    horaRegistro: horaAhora(),
    fechaAlmuerzo: hoyISO(),
    horaEntrega: 'Sin entregar',
    menuReservado: menuElegidoObj ? menuElegidoObj.nombre : 'No especificado'
  };
  DB.students.push(nuevo);
  await guardarDatos();

  btn.disabled = false; btn.textContent = '✅ Confirmar registro';
  this.reset();
  document.querySelectorAll('#form-estudiante .field').forEach(f=>f.classList.remove('error'));
  menuSeleccionado = null;
  renderMenuHoy();

  mostrarToast(`${nombre} quedó registrado con ${nuevo.menuReservado==='No especificado'?'el almuerzo del día':'su '+nuevo.menuReservado+' reservado'}.`, 'success', '¡Registro exitoso!');
});

/* =========================================================
   LOGIN COCINERA
========================================================= */
document.getElementById('form-login').addEventListener('submit', async function(e){
  e.preventDefault();
  const user = document.getElementById('in-user').value.trim();
  const pass = document.getElementById('in-pass').value;
  let cred = {user:'cocinera', pass:'comedor2026'};
  try{
    const res = await window.storage.get(CRED_KEY, true);
    if(res && res.value) cred = JSON.parse(res.value);
  }catch(err){}

  const passField = document.getElementById('f-pass');
  if(user === cred.user && pass === cred.pass){
    passField.classList.remove('error');
    sesionActiva = true;
    document.getElementById('session-pill').style.display='flex';
    document.getElementById('session-label').textContent = cred.user;
    this.reset();
    ir('dashboard');
    mostrarToast('Bienvenida al panel del comedor.','success','Sesión iniciada');
  }else{
    passField.classList.add('error');
    mostrarToast('Verifica tu usuario y contraseña.','error','Acceso denegado');
  }
});

/* =========================================================
   PANEL: TABS
========================================================= */
function cambiarTab(tab){
  document.querySelectorAll('.tab-btn').forEach(b=>b.classList.toggle('active', b.dataset.tab===tab));
  document.querySelectorAll('.tab-panel').forEach(p=>p.classList.remove('active'));
  document.getElementById('tab-'+tab).classList.add('active');
  if(tab==='estadisticas') setTimeout(renderGraficos, 60);
  if(tab==='historial') renderHistorial();
  if(tab==='menu') cargarFormularioMenu();
}

/* =========================================================
   MENÚ DEL DÍA (panel cocinera)
========================================================= */
function cargarFormularioMenu(){
  document.getElementById('menu-fecha-label').textContent = fechaLegible();
  const hoy = hoyISO();
  const vigente = (DB.menu && DB.menu.fecha===hoy) ? DB.menu : null;
  const A = vigente ? (vigente.opciones.find(o=>o.id==='A')||{}) : {};
  const B = vigente ? (vigente.opciones.find(o=>o.id==='B')||{}) : {};
  document.getElementById('menuA-entrada').value = A.entrada||'';
  document.getElementById('menuA-fondo').value = A.fondo||'';
  document.getElementById('menuA-postre').value = A.postre||'';
  document.getElementById('menuA-bebida').value = A.bebida||'';
  document.getElementById('menuB-entrada').value = B.entrada||'';
  document.getElementById('menuB-fondo').value = B.fondo||'';
  document.getElementById('menuB-postre').value = B.postre||'';
  document.getElementById('menuB-bebida').value = B.bebida||'';
}

async function guardarMenu(){
  const leer = id => document.getElementById(id).value.trim();
  const opA = { id:'A', nombre:'Menú A', entrada:leer('menuA-entrada'), fondo:leer('menuA-fondo'), postre:leer('menuA-postre'), bebida:leer('menuA-bebida') };
  const opB = { id:'B', nombre:'Menú B', entrada:leer('menuB-entrada'), fondo:leer('menuB-fondo'), postre:leer('menuB-postre'), bebida:leer('menuB-bebida') };

  if(!opA.fondo && !opB.fondo){
    mostrarToast('Ingresa al menos el plato de fondo de una opción para publicar el menú.','error','Faltan datos del menú');
    return;
  }

  DB.menu = { fecha: hoyISO(), opciones:[opA, opB] };
  await guardarDatos();
  mostrarToast('Los estudiantes ya pueden ver y reservar el menú de hoy.','success','Menú publicado');
}

function setFiltro(f){
  filtroActual = f;
  document.querySelectorAll('#filtros .filter-chip').forEach(b=>b.classList.toggle('active', b.dataset.f===f));
  renderTabla();
}
function setFiltroHistorial(f){
  filtroHistorial = f;
  document.querySelectorAll('#filtros-historial .filter-chip').forEach(b=>b.classList.toggle('active', b.dataset.hf===f));
  renderHistorial();
}
document.getElementById('in-fecha-historial').addEventListener('change', renderHistorial);

/* =========================================================
   RENDER: RESUMEN / STATS
========================================================= */
function renderResumen(){
  document.getElementById('fecha-hoy').textContent = fechaLegible();
  const hoy = hoyISO();
  const deHoy = DB.students.filter(s=>s.fechaAlmuerzo===hoy);
  const total = deHoy.length;
  const entregados = deHoy.filter(s=>s.estado==='entregado').length;
  const pendientes = total - entregados;
  const pct = total>0 ? Math.round((entregados/total)*100) : 0;

  document.getElementById('st-total').textContent = total;
  document.getElementById('st-entregados').textContent = entregados;
  document.getElementById('st-pendientes').textContent = pendientes;
  document.getElementById('st-porcentaje').textContent = pct+'%';

  const ring = document.getElementById('plate-ring');
  const circunferencia = 314;
  ring.style.strokeDashoffset = circunferencia - (circunferencia*pct/100);
  document.getElementById('plate-pct').textContent = pct+'%';
  document.getElementById('plate-desc').textContent = total===0
    ? 'Aún no hay registros para el día de hoy.'
    : `${entregados} de ${total} estudiantes ya recogieron su almuerzo. Quedan ${pendientes} por atender.`;
}

/* =========================================================
   RENDER: TABLA DE ENTREGAS
========================================================= */
function estudiantesFiltrados(){
  const q = document.getElementById('in-buscar').value.trim().toLowerCase();
  const hoy = hoyISO();
  return DB.students
    .filter(s=>s.fechaAlmuerzo===hoy)
    .filter(s=>{
      if(filtroActual==='pendiente') return s.estado==='pendiente';
      if(filtroActual==='entregado') return s.estado==='entregado';
      return true;
    })
    .filter(s=>{
      if(!q) return true;
      return s.codigo.toLowerCase().includes(q) || s.nombre.toLowerCase().includes(q) || s.facultad.toLowerCase().includes(q);
    })
    .sort((a,b)=> a.nombre.localeCompare(b.nombre));
}

function renderTabla(){
  const lista = estudiantesFiltrados();
  const tbody = document.getElementById('tbody-estudiantes');
  const empty = document.getElementById('empty-tabla');
  tbody.innerHTML = '';
  empty.style.display = lista.length===0 ? 'block' : 'none';

  lista.forEach(s=>{
    const tr = document.createElement('tr');
    const badge = s.estado==='entregado'
      ? `<span class="badge done">🟢 Recibido</span>`
      : `<span class="badge pending">🟡 Pendiente</span>`;
    const accion = s.estado==='entregado'
      ? `<button class="deliver-btn" disabled>Ya entregado</button>`
      : `<button class="deliver-btn" onclick="entregarAlmuerzo('${s.codigo}')">Entregar almuerzo</button>`;
    tr.innerHTML = `
      <td>${escapeHtml(s.codigo)}</td>
      <td><div class="cell-name">${escapeHtml(s.nombre)}</div><div class="cell-sub">${escapeHtml(s.ciclo||'')}</div></td>
      <td>${escapeHtml(s.facultad)}<div class="cell-sub">${escapeHtml(s.carrera)}</div></td>
      <td><span class="reserva-tag">🍛 ${escapeHtml(s.menuReservado||'No especificado')}</span></td>
      <td>${badge}</td>
      <td>${escapeHtml(s.horaEntrega)}</td>
      <td>${accion}</td>`;
    tbody.appendChild(tr);
  });
}

async function entregarAlmuerzo(codigo){
  const est = DB.students.find(s=>s.codigo===codigo);
  if(!est) return;
  if(est.estado==='entregado'){
    mostrarToast('Este estudiante ya recibió su almuerzo.','error','Entrega duplicada');
    return;
  }
  est.estado = 'entregado';
  est.horaEntrega = horaAhora();
  DB.deliveries.push({
    codigo: est.codigo, nombre: est.nombre, facultad: est.facultad,
    fecha: hoyISO(), hora: est.horaEntrega
  });
  await guardarDatos();
  renderTodoElPanel();
  mostrarToast(`Almuerzo entregado a ${est.nombre}.`,'success','Entrega registrada');
}

/* =========================================================
   RENDER: GRÁFICOS
========================================================= */
function coloresTema(){
  const dark = document.documentElement.classList.contains('dark');
  return {
    text: dark ? '#94A3B8' : '#6B7280',
    grid: dark ? '#243046' : '#E5E7EB'
  };
}

function renderGraficos(){
  const hoy = hoyISO();
  const deHoy = DB.students.filter(s=>s.fechaAlmuerzo===hoy);
  const entregados = deHoy.filter(s=>s.estado==='entregado').length;
  const pendientes = deHoy.length - entregados;
  const c = coloresTema();

  // Donut entregados vs pendientes
  if(charts.donut) charts.donut.destroy();
  charts.donut = new Chart(document.getElementById('chart-donut'), {
    type:'doughnut',
    data:{ labels:['Entregados','Pendientes'], datasets:[{ data:[entregados,pendientes], backgroundColor:['#22C55E','#FACC15'], borderWidth:0 }] },
    options:{ plugins:{ legend:{ position:'bottom', labels:{color:c.text} } }, cutout:'68%' }
  });

  // Facultades con más beneficiarios
  const porFacultad = {};
  DB.students.forEach(s=>{ porFacultad[s.facultad] = (porFacultad[s.facultad]||0)+1; });
  const labelsFac = Object.keys(porFacultad).sort((a,b)=>porFacultad[b]-porFacultad[a]);
  if(charts.facultades) charts.facultades.destroy();
  charts.facultades = new Chart(document.getElementById('chart-facultades'), {
    type:'bar',
    data:{ labels:labelsFac, datasets:[{ label:'Estudiantes', data:labelsFac.map(f=>porFacultad[f]), backgroundColor:'#1E3A8A', borderRadius:6, maxBarThickness:34 }] },
    options:{ plugins:{legend:{display:false}}, scales:{ x:{ticks:{color:c.text},grid:{display:false}}, y:{ticks:{color:c.text},grid:{color:c.grid}} } }
  });

  // Entregas por hora (hoy)
  const porHora = {};
  DB.deliveries.filter(d=>d.fecha===hoy).forEach(d=>{
    const h = d.hora.split(':')[0]+':00';
    porHora[h] = (porHora[h]||0)+1;
  });
  const horasOrdenadas = Object.keys(porHora).sort();
  if(charts.horas) charts.horas.destroy();
  charts.horas = new Chart(document.getElementById('chart-horas'), {
    type:'bar',
    data:{ labels:horasOrdenadas, datasets:[{ label:'Entregas', data:horasOrdenadas.map(h=>porHora[h]), backgroundColor:'#22C55E', borderRadius:6, maxBarThickness:40 }] },
    options:{ plugins:{legend:{display:false}}, scales:{ x:{ticks:{color:c.text},grid:{display:false}}, y:{ticks:{color:c.text},grid:{color:c.grid}} } }
  });
}
function refrescarGraficos(){
  if(document.getElementById('tab-estadisticas').classList.contains('active')) renderGraficos();
}

/* =========================================================
   RENDER: HISTORIAL
========================================================= */
function rangoFechas(){
  const base = document.getElementById('in-fecha-historial').value || hoyISO();
  const d = new Date(base+'T00:00:00');
  let desde = new Date(d), hasta = new Date(d);
  if(filtroHistorial==='semana'){
    const dia = d.getDay();
    desde.setDate(d.getDate()-dia);
    hasta.setDate(desde.getDate()+6);
  }else if(filtroHistorial==='mes'){
    desde = new Date(d.getFullYear(), d.getMonth(), 1);
    hasta = new Date(d.getFullYear(), d.getMonth()+1, 0);
  }
  return {desde: desde.toISOString().slice(0,10), hasta: hasta.toISOString().slice(0,10)};
}

function entregasEnRango(){
  const {desde, hasta} = rangoFechas();
  return DB.deliveries.filter(d => d.fecha>=desde && d.fecha<=hasta).sort((a,b)=> (a.fecha+a.hora) < (b.fecha+b.hora) ? 1 : -1);
}

function renderHistorial(){
  const lista = entregasEnRango();
  const tbody = document.getElementById('tbody-historial');
  const empty = document.getElementById('empty-historial');
  tbody.innerHTML = '';
  empty.style.display = lista.length===0 ? 'block' : 'none';
  lista.forEach(d=>{
    const tr = document.createElement('tr');
    tr.innerHTML = `<td>${escapeHtml(d.codigo)}</td><td>${escapeHtml(d.nombre)}</td><td>${escapeHtml(d.facultad)}</td><td>${escapeHtml(d.fecha)}</td><td>${escapeHtml(d.hora)}</td>`;
    tbody.appendChild(tr);
  });
}

/* =========================================================
   EXPORTACIÓN
========================================================= */
function exportar(tipo){
  const datos = entregasEnRango();
  if(datos.length===0){
    mostrarToast('No hay datos en este rango para exportar.','error','Sin datos');
    return;
  }
  const filas = datos.map(d=>({Codigo:d.codigo, Estudiante:d.nombre, Facultad:d.facultad, Fecha:d.fecha, Hora:d.hora}));

  if(tipo==='csv'){
    const encabezado = Object.keys(filas[0]).join(',');
    const cuerpo = filas.map(f=>Object.values(f).map(v=>`"${String(v).replace(/"/g,'""')}"`).join(',')).join('\n');
    const blob = new Blob([encabezado+'\n'+cuerpo], {type:'text/csv;charset=utf-8;'});
    descargarBlob(blob, 'historial-comedor.csv');
  }else if(tipo==='excel'){
    const ws = XLSX.utils.json_to_sheet(filas);
    const wb = XLSX.utils.book_new();
    XLSX.utils.book_append_sheet(wb, ws, 'Historial');
    XLSX.writeFile(wb, 'historial-comedor.xlsx');
  }else if(tipo==='pdf'){
    const { jsPDF } = window.jspdf;
    const doc = new jsPDF();
    doc.setFontSize(14);
    doc.text('Historial de entregas — Comedor Universitario', 14, 16);
    doc.autoTable({
      startY: 22,
      head: [['Código','Estudiante','Facultad','Fecha','Hora']],
      body: filas.map(f=>Object.values(f)),
      styles:{fontSize:9},
      headStyles:{fillColor:[30,58,138]}
    });
    doc.save('historial-comedor.pdf');
  }
  mostrarToast('Archivo generado correctamente.','success','Exportación lista');
}
function descargarBlob(blob, nombre){
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url; a.download = nombre; a.click();
  URL.revokeObjectURL(url);
}

/* =========================================================
   RENDER GENERAL DEL PANEL
========================================================= */
function renderTodoElPanel(){
  renderResumen();
  renderTabla();
  if(document.getElementById('tab-estadisticas').classList.contains('active')) renderGraficos();
  if(document.getElementById('tab-historial').classList.contains('active')) renderHistorial();
}

/* =========================================================
   INICIO
========================================================= */
(async function init(){
  document.getElementById('in-fecha-historial').value = hoyISO();
  await cargarDatos();
  document.getElementById('loader-overlay').style.display='none';
  document.getElementById('app').style.display='flex';
})();
</script>
</body>
</html>
