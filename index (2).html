<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SmartTask — Modern Task Management</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700&family=DM+Mono:ital,wght@0,300;0,400;0,500;1,400&display=swap" rel="stylesheet" />

  <style>
    /* ============================================================
       CSS VARIABLES & RESET
    ============================================================ */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --navy:       #0F172A;
      --navy-800:   #1E293B;
      --navy-700:   #293548;
      --navy-600:   #334155;
      --sky:        #38BDF8;
      --sky-dark:   #0EA5E9;
      --teal:       #0D9488;
      --teal-light: #14B8A6;
      --white:      #F8FAFC;
      --muted:      #94A3B8;
      --danger:     #F43F5E;
      --warning:    #F59E0B;
      --success:    #22C55E;

      /* Category colors */
      --cat-work:     #38BDF8;
      --cat-personal: #A78BFA;
      --cat-study:    #34D399;

      /* Status colors */
      --status-pending:    #F59E0B;
      --status-progress:   #38BDF8;
      --status-done:       #22C55E;

      --radius:   12px;
      --radius-sm: 8px;
      --shadow:   0 4px 24px rgba(0,0,0,0.35);
      --shadow-sm:0 2px 12px rgba(0,0,0,0.25);
      --transition: 0.22s cubic-bezier(0.4,0,0.2,1);
    }

    html { font-size: 16px; scroll-behavior: smooth; }

    body {
      font-family: 'Sora', sans-serif;
      background: var(--navy);
      color: var(--white);
      min-height: 100vh;
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    /* ============================================================
       SCROLLBAR
    ============================================================ */
    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: var(--navy-800); }
    ::-webkit-scrollbar-thumb { background: var(--navy-600); border-radius: 3px; }
    ::-webkit-scrollbar-thumb:hover { background: var(--sky-dark); }

    /* ============================================================
       TYPOGRAPHY HELPERS
    ============================================================ */
    .mono { font-family: 'DM Mono', monospace; }
    .text-muted { color: var(--muted); }
    .text-sky   { color: var(--sky); }
    .text-teal  { color: var(--teal-light); }
    .text-danger { color: var(--danger); }

    /* ============================================================
       LAYOUT WRAPPERS
    ============================================================ */
    #auth-screen, #app-screen {
      min-height: 100vh;
      transition: opacity 0.35s ease;
    }
    .hidden { display: none !important; }

    /* ============================================================
       AUTH SCREEN
    ============================================================ */
    #auth-screen {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
      position: relative;
      overflow: hidden;
    }

    /* Animated background grid */
    #auth-screen::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image:
        linear-gradient(rgba(56,189,248,0.04) 1px, transparent 1px),
        linear-gradient(90deg, rgba(56,189,248,0.04) 1px, transparent 1px);
      background-size: 40px 40px;
      pointer-events: none;
      z-index: 0;
    }

    /* Glow blobs */
    #auth-screen::after {
      content: '';
      position: fixed;
      width: 500px; height: 500px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(13,148,136,0.15) 0%, transparent 70%);
      top: -100px; right: -100px;
      pointer-events: none;
      z-index: 0;
    }

    .auth-blob {
      position: fixed;
      width: 400px; height: 400px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(56,189,248,0.1) 0%, transparent 70%);
      bottom: -80px; left: -80px;
      pointer-events: none;
      z-index: 0;
    }

    .auth-card {
      background: var(--navy-800);
      border: 1px solid rgba(56,189,248,0.12);
      border-radius: 20px;
      padding: 48px 44px;
      width: 100%;
      max-width: 440px;
      box-shadow: 0 8px 48px rgba(0,0,0,0.5);
      position: relative;
      z-index: 1;
      animation: slideUp 0.45s cubic-bezier(0.16,1,0.3,1) both;
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(32px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    .auth-logo {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 32px;
    }
    .auth-logo-icon {
      width: 40px; height: 40px;
      background: linear-gradient(135deg, var(--sky), var(--teal));
      border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      font-size: 20px;
    }
    .auth-logo-text {
      font-size: 22px;
      font-weight: 700;
      letter-spacing: -0.5px;
    }
    .auth-logo-text span { color: var(--sky); }

    .auth-tabs {
      display: flex;
      background: var(--navy-700);
      border-radius: var(--radius-sm);
      padding: 4px;
      margin-bottom: 28px;
    }
    .auth-tab {
      flex: 1;
      padding: 8px;
      text-align: center;
      border-radius: 6px;
      cursor: pointer;
      font-size: 14px;
      font-weight: 500;
      color: var(--muted);
      transition: var(--transition);
      border: none;
      background: transparent;
    }
    .auth-tab.active {
      background: var(--navy-800);
      color: var(--white);
      box-shadow: var(--shadow-sm);
    }

    .auth-form { display: flex; flex-direction: column; gap: 16px; }
    .auth-form.hidden { display: none !important; }

    .form-group { display: flex; flex-direction: column; gap: 6px; }
    .form-label {
      font-size: 13px;
      font-weight: 500;
      color: var(--muted);
      letter-spacing: 0.4px;
      text-transform: uppercase;
    }
    .form-input, .form-select, .form-textarea {
      background: var(--navy-700);
      border: 1px solid rgba(148,163,184,0.15);
      border-radius: var(--radius-sm);
      color: var(--white);
      font-family: 'Sora', sans-serif;
      font-size: 15px;
      padding: 11px 14px;
      width: 100%;
      transition: var(--transition);
      outline: none;
    }
    .form-input:focus, .form-select:focus, .form-textarea:focus {
      border-color: var(--sky);
      background: var(--navy-600);
      box-shadow: 0 0 0 3px rgba(56,189,248,0.12);
    }
    .form-input.error, .form-select.error { border-color: var(--danger); }
    .form-textarea { resize: vertical; min-height: 80px; }
    .form-select { cursor: pointer; }
    .form-select option { background: var(--navy-800); }

    .error-msg {
      font-size: 12px;
      color: var(--danger);
      display: none;
      margin-top: 2px;
    }
    .error-msg.visible { display: block; }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 12px 20px;
      border: none;
      border-radius: var(--radius-sm);
      font-family: 'Sora', sans-serif;
      font-size: 15px;
      font-weight: 600;
      cursor: pointer;
      transition: var(--transition);
      text-decoration: none;
      white-space: nowrap;
    }
    .btn-primary {
      background: linear-gradient(135deg, var(--sky-dark), var(--teal));
      color: #fff;
    }
    .btn-primary:hover {
      opacity: 0.9;
      transform: translateY(-1px);
      box-shadow: 0 4px 16px rgba(56,189,248,0.3);
    }
    .btn-primary:active { transform: translateY(0); }

    .btn-ghost {
      background: var(--navy-700);
      color: var(--muted);
      border: 1px solid rgba(148,163,184,0.15);
    }
    .btn-ghost:hover { background: var(--navy-600); color: var(--white); }

    .btn-danger {
      background: rgba(244,63,94,0.12);
      color: var(--danger);
      border: 1px solid rgba(244,63,94,0.2);
    }
    .btn-danger:hover { background: var(--danger); color: #fff; }

    .btn-sm { padding: 7px 12px; font-size: 13px; }
    .btn-full { width: 100%; }

    .auth-switch {
      text-align: center;
      margin-top: 8px;
      font-size: 14px;
      color: var(--muted);
    }
    .auth-switch a { color: var(--sky); text-decoration: none; cursor: pointer; }
    .auth-switch a:hover { text-decoration: underline; }

    /* ============================================================
       APP SCREEN
    ============================================================ */
    #app-screen { display: flex; flex-direction: column; min-height: 100vh; }

    /* ---- HEADER ---- */
    .app-header {
      background: var(--navy-800);
      border-bottom: 1px solid rgba(56,189,248,0.08);
      padding: 16px 24px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(10px);
    }

    .header-logo {
      display: flex; align-items: center; gap: 10px;
      text-decoration: none; flex-shrink: 0;
    }
    .header-logo-icon {
      width: 34px; height: 34px;
      background: linear-gradient(135deg, var(--sky), var(--teal));
      border-radius: 8px;
      display: flex; align-items: center; justify-content: center;
      font-size: 16px;
    }
    .header-logo-text {
      font-size: 18px; font-weight: 700; color: var(--white);
      letter-spacing: -0.3px;
    }
    .header-logo-text span { color: var(--sky); }

    .header-stats {
      display: flex;
      align-items: center;
      gap: 20px;
      flex: 1;
      justify-content: center;
    }
    .stat-pill {
      display: flex;
      align-items: center;
      gap: 6px;
      background: var(--navy-700);
      border: 1px solid rgba(148,163,184,0.1);
      border-radius: 100px;
      padding: 5px 14px;
      font-size: 13px;
      color: var(--muted);
    }
    .stat-pill strong { color: var(--white); }
    .stat-pill.today strong { color: var(--sky); }
    .stat-pill .dot {
      width: 7px; height: 7px;
      border-radius: 50%;
      background: var(--teal-light);
      flex-shrink: 0;
    }
    .stat-pill.today .dot { background: var(--sky); }

    .header-right {
      display: flex; align-items: center; gap: 12px; flex-shrink: 0;
    }
    .user-badge {
      display: flex; align-items: center; gap: 8px;
      background: var(--navy-700);
      border: 1px solid rgba(148,163,184,0.1);
      border-radius: 100px;
      padding: 5px 14px 5px 5px;
    }
    .user-avatar {
      width: 26px; height: 26px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--sky), var(--teal));
      display: flex; align-items: center; justify-content: center;
      font-size: 12px;
      font-weight: 700;
      color: #fff;
      flex-shrink: 0;
    }
    .user-name { font-size: 13px; font-weight: 500; }

    /* ---- MAIN LAYOUT ---- */
    .app-main {
      flex: 1;
      max-width: 1100px;
      width: 100%;
      margin: 0 auto;
      padding: 32px 24px;
    }

    /* ---- CONTROLS BAR ---- */
    .controls-bar {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      align-items: center;
      margin-bottom: 24px;
    }
    .search-wrap {
      position: relative;
      flex: 1;
      min-width: 180px;
    }
    .search-icon {
      position: absolute;
      left: 12px; top: 50%;
      transform: translateY(-50%);
      color: var(--muted);
      font-size: 16px;
      pointer-events: none;
    }
    .search-input {
      background: var(--navy-800);
      border: 1px solid rgba(148,163,184,0.15);
      border-radius: var(--radius-sm);
      color: var(--white);
      font-family: 'Sora', sans-serif;
      font-size: 14px;
      padding: 9px 12px 9px 38px;
      width: 100%;
      outline: none;
      transition: var(--transition);
    }
    .search-input:focus {
      border-color: var(--sky);
      box-shadow: 0 0 0 3px rgba(56,189,248,0.1);
    }
    .search-input::placeholder { color: var(--muted); }

    .filter-group {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
    }
    .filter-select {
      background: var(--navy-800);
      border: 1px solid rgba(148,163,184,0.15);
      border-radius: var(--radius-sm);
      color: var(--white);
      font-family: 'Sora', sans-serif;
      font-size: 13px;
      padding: 8px 12px;
      cursor: pointer;
      outline: none;
      transition: var(--transition);
    }
    .filter-select:focus { border-color: var(--sky); }
    .filter-select option { background: var(--navy-800); }

    /* ---- TASK GRID ---- */
    .tasks-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 16px;
    }

    /* ---- TASK CARD ---- */
    .task-card {
      background: var(--navy-800);
      border: 1px solid rgba(148,163,184,0.1);
      border-radius: var(--radius);
      padding: 20px;
      display: flex;
      flex-direction: column;
      gap: 14px;
      transition: var(--transition);
      position: relative;
      overflow: hidden;
      animation: cardIn 0.3s cubic-bezier(0.16,1,0.3,1) both;
    }
    @keyframes cardIn {
      from { opacity: 0; transform: scale(0.96); }
      to   { opacity: 1; transform: scale(1); }
    }
    .task-card::before {
      content: '';
      position: absolute;
      left: 0; top: 0; bottom: 0;
      width: 3px;
      border-radius: 12px 0 0 12px;
    }
    .task-card[data-category="Work"]::before     { background: var(--cat-work); }
    .task-card[data-category="Personal"]::before { background: var(--cat-personal); }
    .task-card[data-category="Study"]::before    { background: var(--cat-study); }

    .task-card:hover {
      border-color: rgba(56,189,248,0.2);
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(0,0,0,0.3);
    }
    .task-card.completed { opacity: 0.7; }
    .task-card.completed .task-title { text-decoration: line-through; color: var(--muted); }

    .task-top {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 8px;
    }

    .task-title {
      font-size: 16px;
      font-weight: 600;
      line-height: 1.4;
      flex: 1;
    }

    .task-meta {
      display: flex;
      align-items: center;
      gap: 8px;
      flex-wrap: wrap;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 3px 9px;
      border-radius: 100px;
      font-size: 11.5px;
      font-weight: 600;
      letter-spacing: 0.3px;
    }
    .badge-cat-Work     { background: rgba(56,189,248,0.12);  color: var(--cat-work); }
    .badge-cat-Personal { background: rgba(167,139,250,0.12); color: var(--cat-personal); }
    .badge-cat-Study    { background: rgba(52,211,153,0.12);  color: var(--cat-study); }

    .status-badge {
      cursor: pointer;
      transition: var(--transition);
      user-select: none;
    }
    .status-badge:hover { opacity: 0.8; transform: scale(1.05); }
    .status-Pending     { background: rgba(245,158,11,0.12);  color: var(--status-pending); }
    .status-In\ Progress { background: rgba(56,189,248,0.12); color: var(--status-progress); }
    .status-Completed   { background: rgba(34,197,94,0.12);   color: var(--status-done); }

    .task-desc {
      font-size: 13.5px;
      color: var(--muted);
      line-height: 1.6;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
      display: -webkit-box;
    }

    .task-footer {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 8px;
      padding-top: 12px;
      border-top: 1px solid rgba(148,163,184,0.08);
    }

    .task-due {
      font-size: 12px;
      font-family: 'DM Mono', monospace;
      color: var(--muted);
      display: flex;
      align-items: center;
      gap: 5px;
    }
    .task-due.overdue { color: var(--danger); }
    .task-due.today   { color: var(--warning); }

    .task-actions { display: flex; gap: 6px; }
    .task-action-btn {
      width: 30px; height: 30px;
      border: none;
      border-radius: 6px;
      background: var(--navy-700);
      color: var(--muted);
      font-size: 14px;
      cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      transition: var(--transition);
    }
    .task-action-btn:hover { background: var(--navy-600); color: var(--white); }
    .task-action-btn.del:hover { background: rgba(244,63,94,0.15); color: var(--danger); }

    /* ---- EMPTY STATE ---- */
    .empty-state {
      grid-column: 1/-1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 80px 24px;
      text-align: center;
      gap: 16px;
    }
    .empty-svg { opacity: 0.6; margin-bottom: 8px; }
    .empty-title { font-size: 20px; font-weight: 600; color: var(--muted); }
    .empty-sub { font-size: 14px; color: var(--navy-600); max-width: 280px; }

    /* ---- FAB (Add Task) ---- */
    .fab {
      position: fixed;
      bottom: 32px;
      right: 32px;
      width: 56px; height: 56px;
      border-radius: 16px;
      background: linear-gradient(135deg, var(--sky-dark), var(--teal));
      border: none;
      color: #fff;
      font-size: 26px;
      cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      box-shadow: 0 6px 24px rgba(14,165,233,0.35);
      transition: var(--transition);
      z-index: 200;
    }
    .fab:hover {
      transform: scale(1.08) rotate(90deg);
      box-shadow: 0 10px 32px rgba(14,165,233,0.5);
    }
    .fab:active { transform: scale(0.96); }

    /* ---- MODAL ---- */
    .modal-backdrop {
      position: fixed; inset: 0;
      background: rgba(15,23,42,0.8);
      backdrop-filter: blur(6px);
      z-index: 300;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
      opacity: 0;
      animation: fadeIn 0.2s ease forwards;
    }
    @keyframes fadeIn { to { opacity: 1; } }

    .modal {
      background: var(--navy-800);
      border: 1px solid rgba(56,189,248,0.12);
      border-radius: 18px;
      padding: 36px 32px;
      width: 100%;
      max-width: 520px;
      box-shadow: 0 24px 80px rgba(0,0,0,0.6);
      transform: scale(0.95) translateY(12px);
      animation: modalIn 0.28s cubic-bezier(0.16,1,0.3,1) forwards;
      max-height: 90vh;
      overflow-y: auto;
    }
    @keyframes modalIn { to { transform: scale(1) translateY(0); } }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 24px;
    }
    .modal-title { font-size: 20px; font-weight: 700; }
    .modal-close {
      width: 32px; height: 32px;
      border: none;
      background: var(--navy-700);
      color: var(--muted);
      border-radius: 8px;
      cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      font-size: 18px;
      transition: var(--transition);
    }
    .modal-close:hover { background: var(--navy-600); color: var(--white); }

    .modal-form { display: flex; flex-direction: column; gap: 18px; }
    .modal-footer {
      display: flex;
      gap: 10px;
      justify-content: flex-end;
      margin-top: 8px;
    }

    /* ---- TOAST ---- */
    .toast-container {
      position: fixed;
      bottom: 100px;
      right: 24px;
      display: flex;
      flex-direction: column;
      gap: 8px;
      z-index: 500;
    }
    .toast {
      background: var(--navy-700);
      border: 1px solid rgba(148,163,184,0.15);
      border-radius: var(--radius-sm);
      padding: 12px 18px;
      font-size: 14px;
      font-weight: 500;
      display: flex;
      align-items: center;
      gap: 10px;
      box-shadow: var(--shadow);
      animation: toastIn 0.3s cubic-bezier(0.16,1,0.3,1) both,
                 toastOut 0.3s ease 2.8s forwards;
      max-width: 300px;
    }
    @keyframes toastIn  { from { opacity:0; transform: translateX(20px); } to { opacity:1; transform: translateX(0); } }
    @keyframes toastOut { to   { opacity:0; transform: translateX(20px); } }
    .toast.success { border-left: 3px solid var(--success); }
    .toast.error   { border-left: 3px solid var(--danger);  }
    .toast.info    { border-left: 3px solid var(--sky);     }

    /* ============================================================
       CONFIRM DIALOG
    ============================================================ */
    .confirm-box {
      background: var(--navy-800);
      border: 1px solid rgba(244,63,94,0.2);
      border-radius: var(--radius);
      padding: 28px;
      width: 100%;
      max-width: 360px;
      text-align: center;
      box-shadow: 0 24px 80px rgba(0,0,0,0.6);
      transform: scale(0.95);
      animation: modalIn 0.28s cubic-bezier(0.16,1,0.3,1) forwards;
    }
    .confirm-box h3 { margin-bottom: 8px; }
    .confirm-box p  { color: var(--muted); font-size: 14px; margin-bottom: 20px; }
    .confirm-actions { display: flex; gap: 10px; justify-content: center; }

    /* ============================================================
       SECTION HEADER
    ============================================================ */
    .section-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 20px;
    }
    .section-title {
      font-size: 14px;
      font-weight: 500;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.8px;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .task-count-badge {
      background: var(--navy-700);
      color: var(--sky);
      font-size: 12px;
      font-family: 'DM Mono', monospace;
      padding: 2px 8px;
      border-radius: 100px;
    }

    /* ============================================================
       RESPONSIVE
    ============================================================ */
    @media (max-width: 768px) {
      .header-stats { display: none; }
      .app-main { padding: 20px 16px; }
      .auth-card { padding: 32px 24px; }
      .modal { padding: 28px 20px; }
      .tasks-grid { grid-template-columns: 1fr; }
      .controls-bar { flex-direction: column; align-items: stretch; }
      .filter-group { flex-wrap: wrap; }
      .fab { bottom: 24px; right: 20px; }
    }

    @media (max-width: 480px) {
      .user-name { display: none; }
      .stat-pill span.label { display: none; }
    }

    /* ============================================================
       INPUT DATE CALENDAR ICON OVERRIDE
    ============================================================ */
    input[type="date"]::-webkit-calendar-picker-indicator {
      filter: invert(0.7);
      cursor: pointer;
    }
    input[type="date"] { color-scheme: dark; }

    /* ============================================================
       LOADING SPINNER
    ============================================================ */
    .spinner {
      width: 18px; height: 18px;
      border: 2px solid rgba(255,255,255,0.3);
      border-top-color: #fff;
      border-radius: 50%;
      animation: spin 0.7s linear infinite;
      display: inline-block;
    }
    @keyframes spin { to { transform: rotate(360deg); } }
  </style>
</head>
<body>

  <!-- ============================================================
       AUTH SCREEN
  ============================================================ -->
  <div id="auth-screen">
    <div class="auth-blob"></div>

    <div class="auth-card">
      <div class="auth-logo">
        <div class="auth-logo-icon">✦</div>
        <div class="auth-logo-text">Smart<span>Task</span></div>
      </div>

      <!-- Tabs -->
      <div class="auth-tabs">
        <button class="auth-tab active" id="tab-login" onclick="switchAuthTab('login')">Sign In</button>
        <button class="auth-tab" id="tab-register" onclick="switchAuthTab('register')">Register</button>
      </div>

      <!-- LOGIN FORM -->
      <form class="auth-form" id="login-form" onsubmit="handleLogin(event)">
        <div class="form-group">
          <label class="form-label">Email</label>
          <input type="email" id="login-email" class="form-input" placeholder="you@example.com" autocomplete="email" />
          <span class="error-msg" id="login-email-err"></span>
        </div>
        <div class="form-group">
          <label class="form-label">Password</label>
          <input type="password" id="login-pwd" class="form-input" placeholder="••••••••" autocomplete="current-password" />
          <span class="error-msg" id="login-pwd-err"></span>
        </div>
        <span class="error-msg visible" id="login-general-err" style="text-align:center;"></span>
        <button type="submit" class="btn btn-primary btn-full" style="margin-top:4px;">Sign In</button>
        <div class="auth-switch">
          No account? <a onclick="switchAuthTab('register')">Create one</a>
        </div>
      </form>

      <!-- REGISTER FORM -->
      <form class="auth-form hidden" id="register-form" onsubmit="handleRegister(event)">
        <div class="form-group">
          <label class="form-label">Email</label>
          <input type="email" id="reg-email" class="form-input" placeholder="you@example.com" autocomplete="email" />
          <span class="error-msg" id="reg-email-err"></span>
        </div>
        <div class="form-group">
          <label class="form-label">Password <span class="text-muted" style="font-size:11px;text-transform:none;">(min 6 chars)</span></label>
          <input type="password" id="reg-pwd" class="form-input" placeholder="Choose a strong password" autocomplete="new-password" />
          <span class="error-msg" id="reg-pwd-err"></span>
        </div>
        <div class="form-group">
          <label class="form-label">Confirm Password</label>
          <input type="password" id="reg-pwd2" class="form-input" placeholder="Repeat password" autocomplete="new-password" />
          <span class="error-msg" id="reg-pwd2-err"></span>
        </div>
        <span class="error-msg visible" id="reg-general-err" style="text-align:center;"></span>
        <button type="submit" class="btn btn-primary btn-full" style="margin-top:4px;">Create Account</button>
        <div class="auth-switch">
          Already have an account? <a onclick="switchAuthTab('login')">Sign in</a>
        </div>
      </form>
    </div>
  </div>

  <!-- ============================================================
       APP SCREEN
  ============================================================ -->
  <div id="app-screen" class="hidden">

    <!-- HEADER -->
    <header class="app-header">
      <div class="header-logo">
        <div class="header-logo-icon">✦</div>
        <div class="header-logo-text">Smart<span>Task</span></div>
      </div>

      <div class="header-stats">
        <div class="stat-pill">
          <span class="dot"></span>
          <span class="label">Total:</span>
          <strong id="stat-total">0</strong>
        </div>
        <div class="stat-pill today">
          <span class="dot"></span>
          <span class="label">Due today:</span>
          <strong id="stat-today">0</strong>
        </div>
        <div class="stat-pill">
          <span class="dot" style="background:var(--success)"></span>
          <span class="label">Done:</span>
          <strong id="stat-done">0</strong>
        </div>
      </div>

      <div class="header-right">
        <div class="user-badge">
          <div class="user-avatar" id="user-avatar">U</div>
          <span class="user-name" id="user-name-label">User</span>
        </div>
        <button class="btn btn-ghost btn-sm" onclick="handleLogout()">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M9 21H5a2 2 0 01-2-2V5a2 2 0 012-2h4M16 17l5-5-5-5M21 12H9"/></svg>
          Logout
        </button>
      </div>
    </header>

    <!-- MAIN CONTENT -->
    <main class="app-main">

      <!-- Controls Bar -->
      <div class="controls-bar">
        <div class="search-wrap">
          <span class="search-icon">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="M21 21l-4.35-4.35"/></svg>
          </span>
          <input type="text" class="search-input" id="search-input" placeholder="Search tasks by title or description…" oninput="renderTasks()" />
        </div>
        <div class="filter-group">
          <select class="filter-select" id="filter-status" onchange="renderTasks()">
            <option value="">All Status</option>
            <option value="Pending">Pending</option>
            <option value="In Progress">In Progress</option>
            <option value="Completed">Completed</option>
          </select>
          <select class="filter-select" id="filter-cat" onchange="renderTasks()">
            <option value="">All Categories</option>
            <option value="Work">Work</option>
            <option value="Personal">Personal</option>
            <option value="Study">Study</option>
          </select>
          <select class="filter-select" id="sort-order" onchange="renderTasks()">
            <option value="asc">Due Date ↑</option>
            <option value="desc">Due Date ↓</option>
          </select>
        </div>
      </div>

      <!-- Section Header -->
      <div class="section-header">
        <div class="section-title">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>
          My Tasks
          <span class="task-count-badge" id="visible-count">0</span>
        </div>
      </div>

      <!-- Task Grid -->
      <div class="tasks-grid" id="tasks-grid"></div>

    </main>

    <!-- FAB -->
    <button class="fab" id="fab" onclick="openTaskModal()" title="Add new task" aria-label="Add new task">+</button>

  </div>

  <!-- ============================================================
       TASK MODAL
  ============================================================ -->
  <!-- Rendered dynamically by JS -->

  <!-- Toast Container -->
  <div class="toast-container" id="toast-container"></div>

  <!-- ============================================================
       JAVASCRIPT
  ============================================================ -->
  <script>
    /* ============================================================
       UTILITIES
    ============================================================ */

    /**
     * Simple hash function (NOT cryptographic — simulated auth only).
     * Converts a string to a deterministic numeric hash string.
     */
    function simpleHash(str) {
      let hash = 5381;
      for (let i = 0; i < str.length; i++) {
        hash = ((hash << 5) + hash) ^ str.charCodeAt(i);
        hash = hash >>> 0; // keep unsigned 32-bit
      }
      return hash.toString(36);
    }

    /** Generate a UUID-like unique ID */
    function uid() {
      return Date.now().toString(36) + Math.random().toString(36).slice(2, 8);
    }

    /** Format a date string (YYYY-MM-DD) to locale-aware display */
    function formatDate(dateStr) {
      if (!dateStr) return '';
      // Parse as local date (avoid UTC offset shifting the day)
      const [y, m, d] = dateStr.split('-').map(Number);
      const date = new Date(y, m - 1, d);
      return date.toLocaleDateString(undefined, { year: 'numeric', month: 'short', day: 'numeric' });
    }

    /** Get today's date string YYYY-MM-DD in the user's local timezone */
    function todayStr() {
      const now = new Date();
      const y = now.getFullYear();
      const m = String(now.getMonth() + 1).padStart(2, '0');
      const d = String(now.getDate()).padStart(2, '0');
      return `${y}-${m}-${d}`;
    }

    /** Check if a date string is in the past (before today) */
    function isPast(dateStr) {
      return dateStr < todayStr();
    }

    /** Check if a date string is today */
    function isToday(dateStr) {
      return dateStr === todayStr();
    }

    /* ============================================================
       LOCALSTORAGE HELPERS
    ============================================================ */
    const LS_USERS   = 'smarttask_users';
    const LS_SESSION = 'smarttask_session';

    function getUsers()       { return JSON.parse(localStorage.getItem(LS_USERS)  || '{}'); }
    function saveUsers(u)     { localStorage.setItem(LS_USERS, JSON.stringify(u)); }
    function getSession()     { return localStorage.getItem(LS_SESSION); }
    function setSession(uid)  { localStorage.setItem(LS_SESSION, uid); }
    function clearSession()   { localStorage.removeItem(LS_SESSION); }

    /** Per-user task storage key */
    function taskKey(userEmail) { return `smarttask_tasks_${simpleHash(userEmail)}`; }

    function getTasks(email) {
      return JSON.parse(localStorage.getItem(taskKey(email)) || '[]');
    }
    function saveTasks(email, tasks) {
      localStorage.setItem(taskKey(email), JSON.stringify(tasks));
    }

    /* ============================================================
       APP STATE
    ============================================================ */
    let currentUser = null; // { email, name }
    let editingTaskId = null;

    /* ============================================================
       AUTH LOGIC
    ============================================================ */

    /** Switch between login / register tabs */
    function switchAuthTab(tab) {
      document.getElementById('login-form').classList.toggle('hidden', tab !== 'login');
      document.getElementById('register-form').classList.toggle('hidden', tab !== 'register');
      document.getElementById('tab-login').classList.toggle('active', tab === 'login');
      document.getElementById('tab-register').classList.toggle('active', tab === 'register');
      clearAuthErrors();
    }

    function clearAuthErrors() {
      document.querySelectorAll('.error-msg').forEach(el => {
        el.textContent = '';
        el.classList.remove('visible');
      });
      document.querySelectorAll('.form-input').forEach(el => el.classList.remove('error'));
    }

    function showError(id, msg) {
      const el = document.getElementById(id);
      if (el) { el.textContent = msg; el.classList.add('visible'); }
    }

    function handleRegister(e) {
      e.preventDefault();
      clearAuthErrors();
      const email = document.getElementById('reg-email').value.trim();
      const pwd   = document.getElementById('reg-pwd').value;
      const pwd2  = document.getElementById('reg-pwd2').value;
      let valid   = true;

      if (!email || !/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email)) {
        showError('reg-email-err', 'Please enter a valid email.');
        document.getElementById('reg-email').classList.add('error');
        valid = false;
      }
      if (pwd.length < 6) {
        showError('reg-pwd-err', 'Password must be at least 6 characters.');
        document.getElementById('reg-pwd').classList.add('error');
        valid = false;
      }
      if (pwd !== pwd2) {
        showError('reg-pwd2-err', 'Passwords do not match.');
        document.getElementById('reg-pwd2').classList.add('error');
        valid = false;
      }
      if (!valid) return;

      const users = getUsers();
      if (users[email]) {
        showError('reg-general-err', 'An account with this email already exists.');
        return;
      }

      // Store hashed password
      users[email] = { email, hash: simpleHash(pwd) };
      saveUsers(users);

      showToast('Account created! Please sign in.', 'success');
      switchAuthTab('login');
      document.getElementById('login-email').value = email;
    }

    function handleLogin(e) {
      e.preventDefault();
      clearAuthErrors();
      const email = document.getElementById('login-email').value.trim();
      const pwd   = document.getElementById('login-pwd').value;
      let valid   = true;

      if (!email) {
        showError('login-email-err', 'Email is required.');
        document.getElementById('login-email').classList.add('error');
        valid = false;
      }
      if (!pwd) {
        showError('login-pwd-err', 'Password is required.');
        document.getElementById('login-pwd').classList.add('error');
        valid = false;
      }
      if (!valid) return;

      const users = getUsers();
      if (!users[email] || users[email].hash !== simpleHash(pwd)) {
        showError('login-general-err', 'Invalid email or password.');
        return;
      }

      setSession(email);
      loginUser(email);
    }

    function loginUser(email) {
      currentUser = { email };
      setSession(email);

      // Update header
      const label = email.split('@')[0];
      document.getElementById('user-name-label').textContent = label;
      document.getElementById('user-avatar').textContent = label[0].toUpperCase();

      // Show app
      document.getElementById('auth-screen').classList.add('hidden');
      document.getElementById('app-screen').classList.remove('hidden');

      renderTasks();
      showToast(`Welcome back, ${label}! 👋`, 'info');
    }

    function handleLogout() {
      currentUser = null;
      clearSession();
      document.getElementById('app-screen').classList.add('hidden');
      document.getElementById('auth-screen').classList.remove('hidden');
      // Reset search/filters
      document.getElementById('search-input').value   = '';
      document.getElementById('filter-status').value  = '';
      document.getElementById('filter-cat').value     = '';
      clearAuthErrors();
    }

    /* ============================================================
       TASK MODAL
    ============================================================ */

    function openTaskModal(taskId = null) {
      editingTaskId = taskId;
      const tasks   = getTasks(currentUser.email);
      const task    = taskId ? tasks.find(t => t.id === taskId) : null;

      // Remove existing modal
      const existing = document.getElementById('task-modal-backdrop');
      if (existing) existing.remove();

      const backdrop = document.createElement('div');
      backdrop.className   = 'modal-backdrop';
      backdrop.id          = 'task-modal-backdrop';
      backdrop.innerHTML   = `
        <div class="modal" role="dialog" aria-modal="true" aria-label="Task form">
          <div class="modal-header">
            <h2 class="modal-title">${task ? '✏️ Edit Task' : '＋ New Task'}</h2>
            <button class="modal-close" onclick="closeTaskModal()" aria-label="Close">✕</button>
          </div>
          <form class="modal-form" id="task-form" onsubmit="handleSaveTask(event)">

            <div class="form-group">
              <label class="form-label">Title <span style="color:var(--danger)">*</span></label>
              <input type="text" id="task-title" class="form-input"
                     placeholder="What needs to be done?" maxlength="100"
                     value="${task ? escHtml(task.title) : ''}" />
              <span class="error-msg" id="task-title-err"></span>
            </div>

            <div class="form-group">
              <label class="form-label">Description</label>
              <textarea id="task-desc" class="form-textarea"
                        placeholder="Add details (optional)…">${task ? escHtml(task.description) : ''}</textarea>
            </div>

            <div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;">
              <div class="form-group">
                <label class="form-label">Due Date <span style="color:var(--danger)">*</span></label>
                <input type="date" id="task-due" class="form-input"
                       value="${task ? task.dueDate : ''}"
                       min="${todayStr()}" />
                <span class="error-msg" id="task-due-err"></span>
              </div>
              <div class="form-group">
                <label class="form-label">Category</label>
                <select id="task-cat" class="form-select">
                  <option value="Work"     ${task && task.category === 'Work'     ? 'selected' : ''}>💼 Work</option>
                  <option value="Personal" ${task && task.category === 'Personal' ? 'selected' : ''}>🏠 Personal</option>
                  <option value="Study"    ${task && task.category === 'Study'    ? 'selected' : ''}>📚 Study</option>
                </select>
              </div>
            </div>

            ${task ? `
            <div class="form-group">
              <label class="form-label">Status</label>
              <select id="task-status" class="form-select">
                <option value="Pending"     ${task.status === 'Pending'     ? 'selected' : ''}>🟡 Pending</option>
                <option value="In Progress" ${task.status === 'In Progress' ? 'selected' : ''}>🔵 In Progress</option>
                <option value="Completed"   ${task.status === 'Completed'   ? 'selected' : ''}>🟢 Completed</option>
              </select>
            </div>` : ''}

            <span class="error-msg visible" id="task-general-err" style="text-align:center;"></span>

            <div class="modal-footer">
              <button type="button" class="btn btn-ghost" onclick="closeTaskModal()">Cancel</button>
              <button type="submit" class="btn btn-primary">${task ? 'Save Changes' : 'Add Task'}</button>
            </div>
          </form>
        </div>
      `;

      // Close on backdrop click
      backdrop.addEventListener('click', (ev) => {
        if (ev.target === backdrop) closeTaskModal();
      });

      document.body.appendChild(backdrop);
      // Focus first input after animation
      setTimeout(() => document.getElementById('task-title').focus(), 100);
    }

    function closeTaskModal() {
      const el = document.getElementById('task-modal-backdrop');
      if (el) el.remove();
      editingTaskId = null;
    }

    /** HTML-escape a string to prevent XSS in innerHTML */
    function escHtml(str) {
      return (str || '').replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;');
    }

    function handleSaveTask(e) {
      e.preventDefault();

      // Clear previous errors
      document.querySelectorAll('#task-form .error-msg').forEach(el => { el.textContent = ''; el.classList.remove('visible'); });
      document.querySelectorAll('#task-form .form-input, #task-form .form-select').forEach(el => el.classList.remove('error'));

      const title   = document.getElementById('task-title').value.trim();
      const desc    = document.getElementById('task-desc').value.trim();
      const dueDate = document.getElementById('task-due').value;
      const cat     = document.getElementById('task-cat').value;
      const statusEl = document.getElementById('task-status');
      const status  = statusEl ? statusEl.value : 'Pending';

      let valid = true;

      // Validate title
      if (!title) {
        document.getElementById('task-title-err').textContent = 'Title is required.';
        document.getElementById('task-title-err').classList.add('visible');
        document.getElementById('task-title').classList.add('error');
        valid = false;
      }

      // Validate due date — DR1: Cannot save a task with a due date in the past
      if (!dueDate) {
        document.getElementById('task-due-err').textContent = 'Due date is required.';
        document.getElementById('task-due-err').classList.add('visible');
        document.getElementById('task-due').classList.add('error');
        valid = false;
      } else if (isPast(dueDate)) {
        document.getElementById('task-due-err').textContent = '⚠️ Due date cannot be in the past.';
        document.getElementById('task-due-err').classList.add('visible');
        document.getElementById('task-due').classList.add('error');
        valid = false;
      }

      if (!valid) return;

      const tasks = getTasks(currentUser.email);

      if (editingTaskId) {
        // Edit existing task
        const idx = tasks.findIndex(t => t.id === editingTaskId);
        if (idx !== -1) {
          tasks[idx] = { ...tasks[idx], title, description: desc, dueDate, category: cat, status, updatedAt: Date.now() };
        }
        saveTasks(currentUser.email, tasks);
        showToast('Task updated successfully!', 'success');
      } else {
        // Create new task
        const newTask = {
          id: uid(),
          title,
          description: desc,
          dueDate,
          category: cat,
          status: 'Pending',
          createdAt: Date.now(),
          updatedAt: Date.now()
        };
        tasks.push(newTask);
        saveTasks(currentUser.email, tasks);
        showToast('Task created!', 'success');
      }

      closeTaskModal();
      renderTasks();
    }

    /* ============================================================
       TASK ACTIONS
    ============================================================ */

    /** Cycle task status: Pending → In Progress → Completed → Pending */
    function cycleStatus(taskId) {
      const tasks = getTasks(currentUser.email);
      const task  = tasks.find(t => t.id === taskId);
      if (!task) return;

      const cycle = ['Pending', 'In Progress', 'Completed'];
      const next  = cycle[(cycle.indexOf(task.status) + 1) % cycle.length];
      task.status    = next;
      task.updatedAt = Date.now();

      saveTasks(currentUser.email, tasks);
      renderTasks();
      showToast(`Status → ${next}`, 'info');
    }

    /** Open confirm dialog then delete */
    function deleteTask(taskId) {
      const existing = document.getElementById('confirm-backdrop');
      if (existing) existing.remove();

      const backdrop = document.createElement('div');
      backdrop.className = 'modal-backdrop';
      backdrop.id        = 'confirm-backdrop';
      backdrop.innerHTML = `
        <div class="confirm-box">
          <div style="font-size:32px;margin-bottom:12px;">🗑️</div>
          <h3>Delete this task?</h3>
          <p>This action cannot be undone.</p>
          <div class="confirm-actions">
            <button class="btn btn-ghost" onclick="document.getElementById('confirm-backdrop').remove()">Cancel</button>
            <button class="btn btn-danger" onclick="confirmDelete('${taskId}')">Delete</button>
          </div>
        </div>
      `;
      backdrop.addEventListener('click', ev => { if (ev.target === backdrop) backdrop.remove(); });
      document.body.appendChild(backdrop);
    }

    function confirmDelete(taskId) {
      const tasks = getTasks(currentUser.email).filter(t => t.id !== taskId);
      saveTasks(currentUser.email, tasks);
      document.getElementById('confirm-backdrop').remove();
      renderTasks();
      showToast('Task deleted.', 'error');
    }

    /* ============================================================
       RENDER TASKS
    ============================================================ */
    function renderTasks() {
      if (!currentUser) return;

      const allTasks   = getTasks(currentUser.email);
      const query      = (document.getElementById('search-input').value || '').toLowerCase();
      const filterStat = document.getElementById('filter-status').value;
      const filterCat  = document.getElementById('filter-cat').value;
      const sortOrder  = document.getElementById('sort-order').value;

      // Filter
      let tasks = allTasks.filter(t => {
        const matchQ   = !query || t.title.toLowerCase().includes(query) || (t.description || '').toLowerCase().includes(query);
        const matchSt  = !filterStat || t.status === filterStat;
        const matchCat = !filterCat  || t.category === filterCat;
        return matchQ && matchSt && matchCat;
      });

      // Sort
      tasks.sort((a, b) => {
        if (sortOrder === 'asc') return a.dueDate.localeCompare(b.dueDate);
        return b.dueDate.localeCompare(a.dueDate);
      });

      // Stats (from ALL tasks, not filtered)
      const today     = todayStr();
      const totalDone = allTasks.filter(t => t.status === 'Completed').length;
      const dueToday  = allTasks.filter(t => t.dueDate === today && t.status !== 'Completed').length;
      document.getElementById('stat-total').textContent = allTasks.length;
      document.getElementById('stat-today').textContent = dueToday;
      document.getElementById('stat-done').textContent  = totalDone;
      document.getElementById('visible-count').textContent = tasks.length;

      const grid = document.getElementById('tasks-grid');
      grid.innerHTML = '';

      if (tasks.length === 0) {
        grid.innerHTML = `
          <div class="empty-state">
            <svg class="empty-svg" width="120" height="120" viewBox="0 0 120 120" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="20" y="15" width="80" height="90" rx="10" fill="rgba(56,189,248,0.06)" stroke="rgba(56,189,248,0.15)" stroke-width="1.5"/>
              <rect x="35" y="35" width="50" height="6" rx="3" fill="rgba(56,189,248,0.2)"/>
              <rect x="35" y="50" width="38" height="6" rx="3" fill="rgba(56,189,248,0.12)"/>
              <rect x="35" y="65" width="44" height="6" rx="3" fill="rgba(56,189,248,0.12)"/>
              <circle cx="60" cy="85" r="12" fill="rgba(13,148,136,0.15)" stroke="rgba(13,148,136,0.3)" stroke-width="1.5"/>
              <text x="60" y="90" text-anchor="middle" font-size="12" fill="rgba(13,148,136,0.7)">+</text>
            </svg>
            <div class="empty-title">No tasks yet</div>
            <div class="empty-sub text-muted">
              ${query || filterStat || filterCat
                ? 'No tasks match your current filters. Try adjusting the search or filters.'
                : 'Hit the + button to create your first task and get things done!'}
            </div>
          </div>
        `;
        return;
      }

      tasks.forEach(task => {
        const card = createTaskCard(task);
        grid.appendChild(card);
      });
    }

    /** Build a single task card DOM element */
    function createTaskCard(task) {
      const div = document.createElement('div');
      div.className = `task-card${task.status === 'Completed' ? ' completed' : ''}`;
      div.dataset.category = task.category;
      div.dataset.id       = task.id;

      const catIcons = { Work: '💼', Personal: '🏠', Study: '📚' };
      const catIcon  = catIcons[task.category] || '';

      let dueClass = '';
      let dueLabel = '';
      if (isToday(task.dueDate))      { dueClass = 'today';   dueLabel = '📅 Due today'; }
      else if (isPast(task.dueDate))  { dueClass = 'overdue'; dueLabel = '⚠️ Overdue';   }

      const statusDot = { Pending: '🟡', 'In Progress': '🔵', Completed: '🟢' };

      div.innerHTML = `
        <div class="task-top">
          <div class="task-title">${escHtml(task.title)}</div>
        </div>
        <div class="task-meta">
          <span class="badge badge-cat-${task.category}">${catIcon} ${task.category}</span>
          <span class="badge status-badge status-${task.status}"
                onclick="cycleStatus('${task.id}')"
                title="Click to change status">
            ${statusDot[task.status] || ''} ${task.status}
          </span>
        </div>
        ${task.description ? `<div class="task-desc">${escHtml(task.description)}</div>` : ''}
        <div class="task-footer">
          <div class="task-due ${dueClass}">
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
            ${dueLabel || formatDate(task.dueDate)}
          </div>
          <div class="task-actions">
            <button class="task-action-btn" onclick="openTaskModal('${task.id}')" title="Edit task" aria-label="Edit">
              <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M11 4H4a2 2 0 00-2 2v14a2 2 0 002 2h14a2 2 0 002-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 013 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>
            </button>
            <button class="task-action-btn del" onclick="deleteTask('${task.id}')" title="Delete task" aria-label="Delete">
              <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><polyline points="3 6 5 6 21 6"/><path d="M19 6l-1 14a2 2 0 01-2 2H8a2 2 0 01-2-2L5 6"/><path d="M10 11v6M14 11v6"/><path d="M9 6V4a1 1 0 011-1h4a1 1 0 011 1v2"/></svg>
            </button>
          </div>
        </div>
      `;
      return div;
    }

    /* ============================================================
       TOAST NOTIFICATIONS
    ============================================================ */
    function showToast(message, type = 'info') {
      const icons = { success: '✅', error: '🗑️', info: 'ℹ️' };
      const container = document.getElementById('toast-container');
      const toast = document.createElement('div');
      toast.className = `toast ${type}`;
      toast.innerHTML = `<span>${icons[type] || ''}</span><span>${message}</span>`;
      container.appendChild(toast);
      setTimeout(() => toast.remove(), 3200);
    }

    /* ============================================================
       KEYBOARD SHORTCUTS
    ============================================================ */
    document.addEventListener('keydown', (e) => {
      // Escape closes modals
      if (e.key === 'Escape') {
        const modal   = document.getElementById('task-modal-backdrop');
        const confirm = document.getElementById('confirm-backdrop');
        if (modal)   modal.remove();
        if (confirm) confirm.remove();
      }
      // Ctrl/Cmd + N opens new task modal when logged in
      if ((e.ctrlKey || e.metaKey) && e.key === 'n' && currentUser) {
        e.preventDefault();
        openTaskModal();
      }
    });

    /* ============================================================
       INIT — Check for existing session on load
    ============================================================ */
    (function init() {
      const savedEmail = getSession();
      if (savedEmail) {
        const users = getUsers();
        if (users[savedEmail]) {
          loginUser(savedEmail);
          return;
        }
        clearSession();
      }
      // Show auth screen
      document.getElementById('auth-screen').classList.remove('hidden');
      document.getElementById('app-screen').classList.add('hidden');
    })();
  </script>
</body>
</html>
