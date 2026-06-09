<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Turnos Junio · AgroPets Las Violetas</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');
  :root {
    --viola: #5B2D8E; --viola-light: #7B4DB8; --viola-pale: #F0E8FF;
    --viola-mid: #D8C4F5; --magenta: #C2185B; --amber: #F59E0B;
    --cream: #FDFAF5; --green: #22C55E; --green-pale: #DCFCE7;
    --red: #EF4444; --red-pale: #FEE2E2; --text: #1E0A3C; --muted: #7C6FA0;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'Poppins', sans-serif; background: var(--cream); color: var(--text); min-height: 100vh; }

  header {
    background: linear-gradient(135deg, var(--viola) 0%, var(--viola-light) 100%);
    color: white; padding: 18px 24px 16px; text-align: center;
  }
  header .brand-icon { font-size: 36px; margin-bottom: 4px; }
  header h1 { font-size: 18px; font-weight: 700; letter-spacing: 0.5px; }
  header h1 span { display: block; font-size: 11px; font-weight: 500; opacity: 0.8; letter-spacing: 2px; text-transform: uppercase; margin-top: 3px; }
  header .sub { font-size: 11px; opacity: 0.7; margin-top: 6px; }

  #selector { display: flex; flex-direction: column; align-items: center; padding: 40px 24px; gap: 16px; }
  #selector h2 { font-size: 16px; font-weight: 600; color: var(--viola); margin-bottom: 4px; }
  .worker-btn {
    width: 100%; max-width: 320px; padding: 18px 24px;
    border: 2.5px solid var(--viola-mid); border-radius: 16px; background: white;
    cursor: pointer; display: flex; align-items: center; gap: 16px;
    transition: all 0.2s; box-shadow: 0 2px 8px rgba(91,45,142,0.08);
  }
  .worker-btn:hover { border-color: var(--viola); background: var(--viola-pale); transform: translateY(-2px); box-shadow: 0 6px 20px rgba(91,45,142,0.18); }
  .worker-avatar { width: 48px; height: 48px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 20px; font-weight: 700; color: white; flex-shrink: 0; }
  .worker-info { text-align: left; }
  .worker-info .name { font-size: 15px; font-weight: 600; }
  .worker-info .count { font-size: 12px; color: var(--muted); margin-top: 2px; }

  #turnos-view { display: none; padding: 0 0 60px; }
  .worker-header { background: linear-gradient(135deg, var(--viola) 0%, var(--viola-light) 100%); color: white; padding: 20px 24px; display: flex; align-items: center; gap: 16px; }
  .back-btn { background: rgba(255,255,255,0.2); border: none; border-radius: 10px; color: white; padding: 8px 12px; cursor: pointer; font-size: 16px; font-family: 'Poppins', sans-serif; transition: background 0.2s; }
  .back-btn:hover { background: rgba(255,255,255,0.35); }
  .worker-header-info h2 { font-size: 18px; font-weight: 700; }
  .worker-header-info p { font-size: 12px; opacity: 0.8; }

  .stats-bar { display: flex; gap: 12px; padding: 16px 20px; background: white; border-bottom: 1px solid var(--viola-mid); }
  .stat-box { flex: 1; text-align: center; padding: 10px 8px; border-radius: 12px; background: var(--viola-pale); }
  .stat-box .val { font-size: 20px; font-weight: 700; color: var(--viola); }
  .stat-box .lbl { font-size: 10px; color: var(--muted); margin-top: 2px; }
  .stat-box.done { background: var(--green-pale); }
  .stat-box.done .val { color: #16A34A; }
  .stat-box.late { background: var(--red-pale); }
  .stat-box.late .val { color: var(--red); }

  .progress-wrap { padding: 14px 20px 0; }
  .progress-label { font-size: 11px; color: var(--muted); margin-bottom: 6px; display: flex; justify-content: space-between; }
  .progress-track { height: 8px; background: var(--viola-mid); border-radius: 8px; overflow: hidden; }
  .progress-fill { height: 100%; background: linear-gradient(90deg, var(--viola), var(--magenta)); border-radius: 8px; transition: width 0.4s ease; }

  .turnos-list { padding: 16px 20px; display: flex; flex-direction: column; gap: 12px; }
  .section-title { font-size: 11px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; color: var(--muted); padding: 16px 20px 4px; }

  .turno-card { background: white; border-radius: 16px; border: 2px solid var(--viola-mid); overflow: hidden; box-shadow: 0 2px 8px rgba(91,45,142,0.07); transition: all 0.3s; }
  .turno-card.confirmed { border-color: #86EFAC; background: #F0FDF4; }
  .turno-card.confirmed.is-late { border-color: #FCA5A5; background: #FFF5F5; }
  .turno-card.today-card { border-color: var(--amber); box-shadow: 0 4px 16px rgba(245,158,11,0.25); }

  .card-top { display: flex; align-items: stretch; min-height: 72px; }
  .date-badge { width: 60px; flex-shrink: 0; background: var(--viola); display: flex; flex-direction: column; align-items: center; justify-content: center; color: white; padding: 10px 4px; }
  .turno-card.confirmed .date-badge { background: #16A34A; }
  .turno-card.confirmed.is-late .date-badge { background: var(--red); }
  .turno-card.today-card .date-badge { background: var(--amber); }
  .date-badge .day-num { font-size: 22px; font-weight: 700; line-height: 1; }
  .date-badge .day-name { font-size: 8px; letter-spacing: 1px; text-transform: uppercase; opacity: 0.85; margin-top: 2px; }
  .date-badge .month { font-size: 9px; opacity: 0.75; }

  .card-body { flex: 1; padding: 10px 14px; display: flex; flex-direction: column; justify-content: center; gap: 4px; }
  .sede-tag { display: inline-block; font-size: 10px; font-weight: 600; letter-spacing: 0.5px; text-transform: uppercase; padding: 2px 8px; border-radius: 20px; background: var(--viola-pale); color: var(--viola); width: fit-content; }
  .turno-card.confirmed .sede-tag { background: #DCFCE7; color: #15803D; }
  .turno-card.confirmed.is-late .sede-tag { background: var(--red-pale); color: var(--red); }
  .horario { font-size: 14px; font-weight: 600; color: var(--text); margin-top: 2px; }

  .tag-row { display: flex; align-items: center; gap: 6px; flex-wrap: wrap; }
  .today-pill { display: inline-flex; align-items: center; gap: 4px; background: var(--amber); color: white; font-size: 9px; font-weight: 700; letter-spacing: 1px; text-transform: uppercase; padding: 2px 8px; border-radius: 20px; }
  .confirmed-stamp { display: inline-flex; align-items: center; gap: 4px; font-size: 10px; color: #15803D; font-weight: 600; }
  .late-stamp { display: inline-flex; align-items: center; gap: 4px; font-size: 10px; color: var(--red); font-weight: 600; }

  .card-action { padding: 8px 14px 10px; display: flex; gap: 8px; }
  .btn-confirm { flex: 1; padding: 9px; border: none; border-radius: 10px; font-family: 'Poppins', sans-serif; font-size: 12px; font-weight: 600; cursor: pointer; transition: all 0.2s; }
  .btn-confirm.pending { background: var(--viola); color: white; }
  .btn-confirm.pending:hover { background: var(--viola-light); }
  .btn-confirm.done-btn { background: var(--green-pale); color: #15803D; cursor: default; }
  .btn-confirm.done-late { background: var(--red-pale); color: var(--red); cursor: default; }
  .btn-undo { padding: 9px 12px; border: 1.5px solid #86EFAC; border-radius: 10px; background: white; color: #16A34A; font-family: 'Poppins', sans-serif; font-size: 11px; cursor: pointer; transition: all 0.2s; }
  .btn-undo:hover { background: #DCFCE7; }
  .btn-undo.red { border-color: #FCA5A5; color: var(--red); }
  .btn-undo.red:hover { background: var(--red-pale); }

  /* ── TARDANZA MODAL ── */
  .modal-overlay { display: none; position: fixed; inset: 0; background: rgba(0,0,0,0.5); z-index: 200; align-items: flex-end; justify-content: center; }
  .modal-overlay.open { display: flex; }
  .modal-box { background: white; border-radius: 24px 24px 0 0; padding: 28px 24px 40px; width: 100%; max-width: 480px; animation: slideUp 0.3s ease; }
  @keyframes slideUp { from { transform: translateY(100%); } to { transform: translateY(0); } }
  .modal-handle { width: 40px; height: 4px; background: var(--viola-mid); border-radius: 4px; margin: 0 auto 20px; }
  .modal-title { font-size: 17px; font-weight: 700; color: var(--text); margin-bottom: 6px; }
  .modal-sub { font-size: 12px; color: var(--muted); margin-bottom: 24px; }
  .modal-sub strong { color: var(--viola); }

  .late-options { display: flex; flex-direction: column; gap: 10px; margin-bottom: 20px; }
  .late-opt-btn {
    padding: 14px 18px; border-radius: 12px; border: 2px solid var(--viola-mid);
    background: white; font-family: 'Poppins', sans-serif; font-size: 13px;
    font-weight: 600; color: var(--text); cursor: pointer; transition: all 0.2s;
    display: flex; align-items: center; gap: 10px;
  }
  .late-opt-btn:hover { border-color: var(--viola); background: var(--viola-pale); }
  .late-opt-btn.selected { border-color: var(--red); background: var(--red-pale); color: var(--red); }
  .late-opt-btn .dot { width: 18px; height: 18px; border-radius: 50%; border: 2px solid currentColor; flex-shrink: 0; display: flex; align-items: center; justify-content: center; }
  .late-opt-btn.selected .dot::after { content: ''; width: 8px; height: 8px; border-radius: 50%; background: var(--red); display: block; }

  .custom-min-row { display: flex; gap: 10px; align-items: center; margin-bottom: 20px; }
  .min-input { flex: 1; padding: 12px 16px; border: 2px solid var(--viola-mid); border-radius: 12px; font-family: 'Poppins', sans-serif; font-size: 15px; font-weight: 600; color: var(--text); outline: none; }
  .min-input:focus { border-color: var(--viola); }
  .min-label { font-size: 13px; color: var(--muted); font-weight: 500; }

  .modal-actions { display: flex; gap: 10px; }
  .btn-modal-cancel { flex: 1; padding: 13px; border: 2px solid var(--viola-mid); border-radius: 12px; background: white; font-family: 'Poppins', sans-serif; font-size: 13px; font-weight: 600; color: var(--muted); cursor: pointer; }
  .btn-modal-cancel:hover { border-color: var(--viola); color: var(--viola); }
  .btn-modal-save { flex: 2; padding: 13px; border: none; border-radius: 12px; background: var(--viola); color: white; font-family: 'Poppins', sans-serif; font-size: 13px; font-weight: 700; cursor: pointer; transition: background 0.2s; }
  .btn-modal-save:hover { background: var(--viola-light); }
  .btn-modal-save:disabled { background: var(--viola-mid); cursor: not-allowed; }

  /* TOAST */
  #toast { position: fixed; bottom: 24px; left: 50%; transform: translateX(-50%) translateY(80px); background: var(--viola); color: white; padding: 12px 24px; border-radius: 30px; font-size: 13px; font-weight: 500; box-shadow: 0 8px 24px rgba(91,45,142,0.4); transition: transform 0.3s ease; z-index: 999; white-space: nowrap; }
  #toast.show { transform: translateX(-50%) translateY(0); }
  #toast.red { background: var(--red); }
</style>
</head>
<body>

<header>
  <div class="brand-icon">🐾</div>
  <h1>Turnos AGROPETS<span>Auxiliares Veterinarias · Junio 2026</span></h1>
  <div class="sub">Confirma tu asistencia cada día</div>
</header>

<div id="selector">
  <h2>¿Quién eres?</h2>
  <button class="worker-btn" onclick="openWorker('dahyana')">
    <div class="worker-avatar" style="background:#5B2D8E;">D</div>
    <div class="worker-info"><div class="name">Dahyana</div><div class="count" id="count-dahyana">Cargando...</div></div>
  </button>
  <button class="worker-btn" onclick="openWorker('julieth')">
    <div class="worker-avatar" style="background:#C2185B;">J</div>
    <div class="worker-info"><div class="name">Julieth</div><div class="count" id="count-julieth">Cargando...</div></div>
  </button>
  <button class="worker-btn" onclick="openWorker('mariana')">
    <div class="worker-avatar" style="background:#7B4DB8;">M</div>
    <div class="worker-info"><div class="name">Mariana</div><div class="count" id="count-mariana">Cargando...</div></div>
  </button>
</div>

<div id="turnos-view">
  <div class="worker-header">
    <button class="back-btn" onclick="goBack()">← Volver</button>
    <div class="worker-header-info">
      <h2 id="wh-name">Nombre</h2>
      <p id="wh-sub">Turnos de junio</p>
    </div>
  </div>
  <div class="stats-bar">
    <div class="stat-box">
      <div class="val" id="st-total">-</div>
      <div class="lbl">Turnos</div>
    </div>
    <div class="stat-box done">
      <div class="val" id="st-done">-</div>
      <div class="lbl">Confirmados</div>
    </div>
    <div class="stat-box late">
      <div class="val" id="st-late">-</div>
      <div class="lbl">Tardanzas</div>
    </div>
  </div>
  <div class="progress-wrap">
    <div class="progress-label"><span>Progreso del mes</span><span id="pct-lbl">0%</span></div>
    <div class="progress-track"><div class="progress-fill" id="prog-fill" style="width:0%"></div></div>
  </div>
  <div class="turnos-list" id="turnos-list"></div>
</div>

<!-- MODAL TARDANZA -->
<div class="modal-overlay" id="tardanza-modal">
  <div class="modal-box">
    <div class="modal-handle"></div>
    <div class="modal-title">⏰ ¿Llegaste tarde?</div>
    <div class="modal-sub">Turno del <strong id="modal-fecha-label"></strong></div>
    <div class="late-options">
      <button class="late-opt-btn" onclick="selectLate(0)" id="opt-0">
        <span class="dot"></span> Llegué a tiempo ✅
      </button>
      <button class="late-opt-btn" onclick="selectLate(15)" id="opt-15">
        <span class="dot"></span> 15 minutos tarde
      </button>
      <button class="late-opt-btn" onclick="selectLate(30)" id="opt-30">
        <span class="dot"></span> 30 minutos tarde
      </button>
      <button class="late-opt-btn" onclick="selectLate(60)" id="opt-60">
        <span class="dot"></span> 1 hora tarde
      </button>
      <button class="late-opt-btn" onclick="selectLate('custom')" id="opt-custom">
        <span class="dot"></span> Otro tiempo...
      </button>
    </div>
    <div class="custom-min-row" id="custom-row" style="display:none;">
      <input class="min-input" type="number" min="1" max="480" id="custom-min-input" placeholder="ej. 45">
      <span class="min-label">minutos de tardanza</span>
    </div>
    <div class="modal-actions">
      <button class="btn-modal-cancel" onclick="closeModal()">Cancelar</button>
      <button class="btn-modal-save" id="btn-save-modal" onclick="saveFromModal()" disabled>Guardar</button>
    </div>
  </div>
</div>

<div id="toast"></div>

<script>
const DATA = {
  dahyana: {
    nombre: "Dahyana", color: "#5B2D8E",
    turnos: [
      { fecha: "2026-06-10", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-11", dia: "Jueves", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-13", dia: "Sábado", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-14", dia: "Domingo", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "5:00 p.m." },
      { fecha: "2026-06-16", dia: "Martes", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-17", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-18", dia: "Jueves", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-20", dia: "Sábado", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-22", dia: "Lunes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-23", dia: "Martes", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-24", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-25", dia: "Jueves", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-27", dia: "Sábado", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-30", dia: "Martes", sede: "San Pedro", entrada: "8:00 a.m.", salida: "8:00 p.m." },
    ]
  },
  julieth: {
    nombre: "Julieth", color: "#C2185B",
    turnos: [
      { fecha: "2026-06-10", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-11", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-12", dia: "Viernes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-15", dia: "Lunes festivo", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "5:00 p.m." },
      { fecha: "2026-06-16", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-17", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-18", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-19", dia: "Viernes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-21", dia: "Domingo", sede: "San Pedro", entrada: "8:00 a.m.", salida: "4:00 p.m." },
      { fecha: "2026-06-22", dia: "Lunes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-23", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-24", dia: "Miércoles", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-25", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-26", dia: "Viernes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "7:00 p.m." },
      { fecha: "2026-06-29", dia: "Lunes festivo", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "5:00 p.m." },
      { fecha: "2026-06-30", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
    ]
  },
  mariana: {
    nombre: "Mariana", color: "#7B4DB8",
    turnos: [
      { fecha: "2026-06-11", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-12", dia: "Viernes", sede: "Medellín / Belén", entrada: "11:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-13", dia: "Sábado", sede: "Medellín / Belén", entrada: "10:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-15", dia: "Lunes festivo", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "3:00 p.m." },
      { fecha: "2026-06-16", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-18", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-19", dia: "Viernes", sede: "Medellín / Belén", entrada: "11:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-20", dia: "Sábado", sede: "Medellín / Belén", entrada: "10:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-23", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-25", dia: "Jueves", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-26", dia: "Viernes", sede: "Medellín / Belén", entrada: "11:00 a.m.", salida: "9:00 p.m." },
      { fecha: "2026-06-27", dia: "Sábado", sede: "Medellín / Belén", entrada: "10:00 a.m.", salida: "8:00 p.m." },
      { fecha: "2026-06-28", dia: "Domingo", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "5:00 p.m." },
      { fecha: "2026-06-30", dia: "Martes", sede: "Medellín / Belén", entrada: "9:00 a.m.", salida: "9:00 p.m." },
    ]
  }
};

let currentWorker = null;
let modalFecha = null;
let selectedLateVal = null;

// In-memory state (works on all devices including iOS)
const STATE = {};

function getWorkerData(w) { return STATE[w] || {}; }

function setTurno(worker, fecha, minutosLate) {
  if (!STATE[worker]) STATE[worker] = {};
  STATE[worker][fecha] = {
    hora: new Date().toLocaleTimeString('es-CO', {hour:'2-digit', minute:'2-digit'}),
    minutos: minutosLate
  };
}
function removeTurno(worker, fecha) {
  if (STATE[worker]) delete STATE[worker][fecha];
}

function getTodayStr() {
  const n = new Date();
  return `${n.getFullYear()}-${String(n.getMonth()+1).padStart(2,'0')}-${String(n.getDate()).padStart(2,'0')}`;
}
function formatFechaLabel(fecha) {
  const [,m,d] = fecha.split('-');
  const meses = ['','ene','feb','mar','abr','may','jun','jul','ago','sep','oct','nov','dic'];
  return `${parseInt(d)} de ${meses[parseInt(m)]}`;
}

// ── SELECTOR COUNTS ──
function initCounts() {
  ['dahyana','julieth','mariana'].forEach(w => {
    const wd = getWorkerData(w);
    const total = DATA[w].turnos.length;
    const done = Object.keys(wd).length;
    const tardanzas = Object.values(wd).filter(v => v.minutos > 0).length;
    let txt = `${total} turnos este mes`;
    if (done > 0) txt += ` · ✓ ${done} confirmados`;
    if (tardanzas > 0) txt += ` · ⏰ ${tardanzas} tardanza${tardanzas>1?'s':''}`;
    document.getElementById(`count-${w}`).textContent = txt;
  });
}

// ── NAVIGATION ──
function openWorker(key) {
  currentWorker = key;
  document.getElementById('selector').style.display = 'none';
  document.getElementById('turnos-view').style.display = 'block';
  document.getElementById('wh-name').textContent = DATA[key].nombre;
  renderTurnos();
}
function goBack() {
  currentWorker = null;
  document.getElementById('turnos-view').style.display = 'none';
  document.getElementById('selector').style.display = 'flex';
  initCounts();
}

// ── RENDER ──
function renderTurnos() {
  const data = DATA[currentWorker];
  const wd = getWorkerData(currentWorker);
  const today = getTodayStr();
  const total = data.turnos.length;
  const done = Object.keys(wd).length;
  const tardanzas = Object.values(wd).filter(v => v.minutos > 0).length;
  const pct = Math.round((done / total) * 100);

  document.getElementById('st-total').textContent = total;
  document.getElementById('st-done').textContent = done;
  document.getElementById('st-late').textContent = tardanzas;
  document.getElementById('prog-fill').style.width = pct + '%';
  document.getElementById('pct-lbl').textContent = pct + '%';
  document.getElementById('wh-sub').textContent = `${done} de ${total} turnos confirmados`;

  const list = document.getElementById('turnos-list');
  list.innerHTML = '';

  const past = data.turnos.filter(t => t.fecha < today);
  const todayArr = data.turnos.filter(t => t.fecha === today);
  const future = data.turnos.filter(t => t.fecha > today);

  if (todayArr.length) {
    appendSection(list, '📍 Hoy');
    todayArr.forEach(t => list.appendChild(buildCard(t, wd, true)));
  }
  if (future.length) {
    appendSection(list, '📅 Próximos turnos');
    future.forEach(t => list.appendChild(buildCard(t, wd, false)));
  }
  if (past.length) {
    appendSection(list, '📋 Turnos anteriores');
    past.forEach(t => list.appendChild(buildCard(t, wd, false)));
  }
}

function appendSection(list, label) {
  const el = document.createElement('div');
  el.className = 'section-title';
  el.textContent = label;
  list.appendChild(el);
}

function buildCard(t, wd, isToday) {
  const rec = wd[t.fecha];
  const isConfirmed = !!rec;
  const isLate = isConfirmed && rec.minutos > 0;
  const dayNum = t.fecha.split('-')[2].replace(/^0/,'');

  const card = document.createElement('div');
  card.className = 'turno-card'
    + (isConfirmed ? ' confirmed' : '')
    + (isLate ? ' is-late' : '')
    + (isToday ? ' today-card' : '');

  let actionHtml;
  if (isConfirmed) {
    const undoClass = isLate ? 'btn-undo red' : 'btn-undo';
    const doneClass = isLate ? 'btn-confirm done-late' : 'btn-confirm done-btn';
    const doneLabel = isLate ? `⏰ ${rec.minutos} min tarde` : '✓ A tiempo';
    actionHtml = `
      <button class="${doneClass}" disabled>${doneLabel}</button>
      <button class="${undoClass}" onclick="undoTurno('${t.fecha}')">Editar</button>`;
  } else {
    actionHtml = `<button class="btn-confirm pending" onclick="openModal('${t.fecha}','${t.dia} ${t.fecha.split('-')[2]}/${t.fecha.split('-')[1]}','${t.entrada}')">Confirmar asistencia</button>`;
  }

  const lateStamp = isLate ? `<span class="late-stamp">⏰ ${rec.minutos} min tarde</span>` : '';
  const confirmedStamp = isConfirmed && !isLate ? `<span class="confirmed-stamp">✅ Confirmado ${rec.hora}</span>` : '';
  const confirmedLateStamp = isLate ? `<span class="late-stamp">Llegada: ${rec.hora}</span>` : '';

  card.innerHTML = `
    <div class="card-top">
      <div class="date-badge">
        <span class="day-num">${dayNum}</span>
        <span class="day-name">${t.dia.substring(0,3)}</span>
        <span class="month">jun</span>
      </div>
      <div class="card-body">
        <div class="tag-row">
          <span class="sede-tag">${t.sede}</span>
          ${isToday ? '<span class="today-pill">⚡ Hoy</span>' : ''}
          ${confirmedStamp}
          ${isLate ? confirmedLateStamp : ''}
        </div>
        <div class="horario">${t.entrada} – ${t.salida}</div>
        ${lateStamp}
      </div>
    </div>
    <div class="card-action">${actionHtml}</div>`;
  return card;
}

// ── MODAL ──
function openModal(fecha, diaLabel, entrada) {
  modalFecha = fecha;
  selectedLateVal = null;
  document.getElementById('modal-fecha-label').textContent = `${diaLabel} · Entrada ${entrada}`;
  document.getElementById('custom-row').style.display = 'none';
  document.getElementById('custom-min-input').value = '';
  document.getElementById('btn-save-modal').disabled = true;
  [0,15,30,60,'custom'].forEach(v => {
    document.getElementById(`opt-${v}`).classList.remove('selected');
  });
  document.getElementById('tardanza-modal').classList.add('open');
}
function closeModal() {
  document.getElementById('tardanza-modal').classList.remove('open');
  modalFecha = null;
  selectedLateVal = null;
}
function selectLate(val) {
  selectedLateVal = val;
  [0,15,30,60,'custom'].forEach(v => document.getElementById(`opt-${v}`).classList.remove('selected'));
  document.getElementById(`opt-${val}`).classList.add('selected');
  const customRow = document.getElementById('custom-row');
  if (val === 'custom') {
    customRow.style.display = 'flex';
    document.getElementById('btn-save-modal').disabled = true;
    document.getElementById('custom-min-input').focus();
  } else {
    customRow.style.display = 'none';
    document.getElementById('btn-save-modal').disabled = false;
  }
}
document.getElementById('custom-min-input').addEventListener('input', function() {
  document.getElementById('btn-save-modal').disabled = !this.value || parseInt(this.value) < 1;
});
function saveFromModal() {
  let minutos = 0;
  if (selectedLateVal === 'custom') {
    minutos = parseInt(document.getElementById('custom-min-input').value) || 0;
  } else {
    minutos = selectedLateVal;
  }
  setTurno(currentWorker, modalFecha, minutos);
  closeModal();
  renderTurnos();
  if (minutos === 0) {
    showToast('✅ ¡Asistencia confirmada!', false);
  } else {
    showToast(`⏰ Tardanza de ${minutos} min registrada`, true);
  }
}
function undoTurno(fecha) {
  removeTurno(currentWorker, fecha);
  renderTurnos();
}

// ── TOAST ──
let toastTimer;
function showToast(msg, isRed) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.className = isRed ? 'red show' : 'show';
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => { t.className = ''; }, 2800);
}

// ── CLOSE MODAL ON OVERLAY CLICK ──
document.getElementById('tardanza-modal').addEventListener('click', function(e) {
  if (e.target === this) closeModal();
});

initCounts();
</script>
</body>
</html>
