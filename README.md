<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>سكر وورد | مستلزمات الحلويات والتغليف</title>

  <style>
    :root {
      --purple: #7542a8;
      --purple-dark: #3d1d5b;
      --purple-light: #f1e8f8;
      --pink: #ef83b9;
      --pink-light: #fff0f7;
      --ink: #2d1d3c;
      --muted: #81768b;
      --line: #eee6f2;
      --surface: #ffffff;
      --page: #fdfafd;
      --green: #388468;
      --shadow: 0 16px 45px rgba(62, 29, 91, .10);
      --radius: 22px;
    }

    * { box-sizing: border-box; }

    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      background: var(--page);
      color: var(--ink);
      font-family: Tahoma, Arial, sans-serif;
    }

    body.no-scroll { overflow: hidden; }

    button, input, select, textarea { font: inherit; }
    button { cursor: pointer; }
    a { color: inherit; text-decoration: none; }
    .hidden { display: none !important; }

    .announcement {
      padding: 9px 16px;
      color: #fff;
      background: var(--purple-dark);
      text-align: center;
      font-size: 13px;
    }

    .site-header {
      position: sticky;
      top: 0;
      z-index: 20;
      min-height: 78px;
      padding: 12px max(22px, calc((100vw - 1180px) / 2));
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      background: rgba(255, 255, 255, .94);
      border-bottom: 1px solid rgba(238, 230, 242, .8);
      backdrop-filter: blur(12px);
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 11px;
      flex-shrink: 0;
    }

    .brand-mark {
      width: 46px;
      height: 46px;
      display: grid;
      place-items: center;
      border-radius: 16px;
      color: #fff;
      font-size: 24px;
      background: linear-gradient(145deg, var(--pink), var(--purple));
      box-shadow: 0 8px 18px rgba(117, 66, 168, .2);
    }

    .brand-copy strong {
      display: block;
      font-size: 20px;
      letter-spacing: -.4px;
    }

    .brand-copy strong b { color: var(--purple); }
    .brand-copy small {
      display: block;
      margin-top: 3px;
      color: var(--muted);
      font-size: 11px;
    }

    .main-nav {
      display: flex;
      align-items: center;
      gap: 28px;
      color: #655970;
      font-size: 14px;
    }

    .main-nav a:hover { color: var(--purple); }
    .admin-mode .main-nav { display: none; }

    .header-actions {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .admin-button, .cart-button, .btn {
      border: 0;
      border-radius: 13px;
      padding: 12px 16px;
      font-weight: 700;
      transition: .2s ease;
    }

    .admin-button {
      color: var(--purple);
      background: var(--purple-light);
    }

    .admin-button:hover { background: #e7d8f3; }

    .cart-button {
      position: relative;
      display: flex;
      align-items: center;
      gap: 8px;
      color: #fff;
      background: var(--purple);
    }

    .cart-button:hover, .btn-primary:hover { background: var(--purple-dark); }

    .cart-count {
      min-width: 22px;
      height: 22px;
      padding-inline: 5px;
      display: grid;
      place-items: center;
      border-radius: 50px;
      color: var(--purple-dark);
      background: #fff;
      font-size: 12px;
    }

    .container {
      width: min(1180px, calc(100% - 40px));
      margin-inline: auto;
    }

    .hero {
      position: relative;
      isolation: isolate;
      overflow: hidden;
      min-height: 425px;
      margin: 26px auto 30px;
      padding: clamp(30px, 6vw, 72px);
      display: grid;
      grid-template-columns: 1.06fr .94fr;
      align-items: center;
      gap: 24px;
      color: #fff;
      border-radius: 34px;
      background:
        radial-gradient(circle at 78% 10%, rgba(239, 131, 185, .25), transparent 29%),
        linear-gradient(120deg, #392052 0%, #61368a 58%, #8b4f9b 100%);
      box-shadow: var(--shadow);
    }

    .hero::before, .hero::after {
      position: absolute;
      z-index: -1;
      content: "";
      border: 1px solid rgba(255, 255, 255, .12);
      border-radius: 50%;
    }

    .hero::before {
      width: 420px;
      height: 420px;
      inset-inline-start: -190px;
      top: -240px;
    }

    .hero::after {
      width: 320px;
      height: 320px;
      inset-inline-start: -140px;
      bottom: -235px;
    }

    .hero-copy { position: relative; z-index: 2; }

    .hero-label {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 9px 13px;
      border: 1px solid rgba(255, 255, 255, .22);
      border-radius: 30px;
      color: #ffe5f1;
      background: rgba(255, 255, 255, .08);
      font-size: 13px;
    }

    .hero-copy h1 {
      max-width: 620px;
      margin: 20px 0 14px;
      font-size: clamp(34px, 5vw, 57px);
      line-height: 1.25;
      letter-spacing: -1.4px;
    }

    .hero-copy h1 em {
      color: #ffc1de;
      font-style: normal;
    }

    .hero-copy > p {
      max-width: 520px;
      margin: 0;
      color: #eee4f6;
      font-size: 16px;
      line-height: 1.9;
    }

    .hero-actions {
      margin-top: 27px;
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 14px;
    }

    .btn {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      gap: 8px;
    }

    .btn-white {
      color: var(--purple-dark);
      background: #fff;
    }

    .btn-white:hover { background: #fff0f7; }
    .hero-note { color: #eee4f6; font-size: 13px; }

    .hero-art {
      position: relative;
      min-height: 300px;
      display: grid;
      place-items: center;
    }

    .hero-art-circle {
      width: min(290px, 70vw);
      height: min(290px, 70vw);
      display: grid;
      place-items: center;
      border: 1px solid rgba(255, 255, 255, .23);
      border-radius: 50%;
      background: radial-gradient(circle, rgba(255, 255, 255, .2), rgba(255, 255, 255, .04) 68%);
      box-shadow: inset 0 0 55px rgba(255, 255, 255, .08);
    }

    .hero-cupcake {
      filter: drop-shadow(0 16px 18px rgba(25, 9, 38, .25));
      font-size: 142px;
      transform: rotate(-7deg);
    }

    .floating-note {
      position: absolute;
      display: flex;
      align-items: center;
      gap: 10px;
      padding: 12px 16px;
      color: var(--ink);
      border: 1px solid rgba(255, 255, 255, .7);
      border-radius: 17px;
      background: rgba(255, 255, 255, .96);
      box-shadow: 0 14px 30px rgba(31, 12, 46, .18);
    }

    .floating-note span { font-size: 27px; }
    .floating-note strong { display: block; font-size: 13px; }
    .floating-note small { display: block; margin-top: 4px; color: var(--muted); font-size: 11px; }
    .note-top { top: 30px; inset-inline-end: 0; }
    .note-bottom { bottom: 25px; inset-inline-start: 0; }

    .benefits {
      margin: 0 auto 74px;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 15px;
    }

    .benefit {
      padding: 19px;
      display: flex;
      align-items: center;
      gap: 13px;
      border: 1px solid var(--line);
      border-radius: 18px;
      background: var(--surface);
    }

    .benefit-icon {
      width: 45px;
      height: 45px;
      flex-shrink: 0;
      display: grid;
      place-items: center;
      border-radius: 14px;
      background: var(--pink-light);
      font-size: 21px;
    }

    .benefit strong { display: block; font-size: 14px; }
    .benefit small { display: block; margin-top: 5px; color: var(--muted); font-size: 12px; }

    .section-heading {
      margin-bottom: 24px;
      display: flex;
      justify-content: space-between;
      align-items: end;
      gap: 20px;
    }

    .eyebrow {
      color: var(--purple);
      font-size: 13px;
      font-weight: 700;
    }

    .section-heading h2 {
      margin: 8px 0 8px;
      font-size: clamp(27px, 3vw, 36px);
      letter-spacing: -.7px;
    }

    .section-heading p { margin: 0; color: var(--muted); line-height: 1.7; }

    .search-box {
      width: min(300px, 100%);
      padding: 0 14px;
      display: flex;
      align-items: center;
      gap: 9px;
      border: 1px solid var(--line);
      border-radius: 14px;
      background: #fff;
    }

    .search-box span { color: var(--purple); font-size: 21px; }
    .search-box input {
      width: 100%;
      height: 46px;
      border: 0;
      outline: 0;
      color: var(--ink);
      background: transparent;
    }

    .filter-row {
      margin-bottom: 19px;
      display: flex;
      flex-wrap: wrap;
      gap: 9px;
    }

    .filter-chip {
      padding: 10px 16px;
      border: 1px solid var(--line);
      border-radius: 30px;
      color: #695b77;
      background: #fff;
      font-size: 13px;
    }

    .filter-chip:hover, .filter-chip.active {
      color: #fff;
      border-color: var(--purple);
      background: var(--purple);
    }

    .results-line {
      margin: 0 0 14px;
      color: var(--muted);
      font-size: 13px;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 18px;
    }

    .product-card {
      overflow: hidden;
      border: 1px solid var(--line);
      border-radius: 20px;
      background: #fff;
      transition: transform .2s ease, box-shadow .2s ease;
    }

    .product-card:hover {
      transform: translateY(-4px);
      box-shadow: var(--shadow);
    }

    .product-art {
      position: relative;
      min-height: 178px;
      display: grid;
      place-items: center;
      overflow: hidden;
    }

    .art-0 { background: linear-gradient(145deg, #fff0f7, #f1e8f8); }
    .art-1 { background: linear-gradient(145deg, #f3eafd, #fce9f3); }
    .art-2 { background: linear-gradient(145deg, #fff4e9, #f9e9f5); }
    .art-3 { background: linear-gradient(145deg, #f3efff, #e8f3fb); }

    .product-emoji {
      filter: drop-shadow(0 9px 9px rgba(71, 38, 91, .12));
      font-size: 77px;
      transition: transform .2s ease;
    }

    .product-card:hover .product-emoji { transform: scale(1.08) rotate(-4deg); }

    .product-category-tag {
      position: absolute;
      top: 12px;
      inset-inline-start: 12px;
      max-width: 75%;
      padding: 7px 10px;
      overflow: hidden;
      border-radius: 20px;
      color: var(--purple-dark);
      background: rgba(255, 255, 255, .85);
      font-size: 11px;
      text-overflow: ellipsis;
      white-space: nowrap;
    }

    .product-info { padding: 16px; }
    .product-info h3 { margin: 10px 0 7px; font-size: 16px; }
    .product-info p {
      min-height: 39px;
      margin: 0;
      color: var(--muted);
      font-size: 12px;
      line-height: 1.7;
    }

    .stock-text { margin-top: 10px; color: var(--green); font-size: 11px; }
    .stock-text.out { color: #ba4568; }

    .product-bottom {
      margin-top: 13px;
      padding-top: 12px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 8px;
      border-top: 1px solid #f2edf4;
    }

    .product-price { color: var(--purple-dark); font-size: 16px; font-weight: 800; }

    .add-button {
      padding: 9px 11px;
      border: 0;
      border-radius: 11px;
      color: #fff;
      background: var(--purple);
      font-size: 12px;
      font-weight: 700;
    }

    .add-button:hover { background: var(--purple-dark); }
    .add-button:disabled { cursor: not-allowed; opacity: .45; }

    .empty-state {
      grid-column: 1 / -1;
      padding: 44px 20px;
      color: var(--muted);
      border: 1px dashed #dacde4;
      border-radius: 18px;
      text-align: center;
      background: #fff;
    }

    .about-band {
      margin: 75px auto;
      padding: 28px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 24px;
      border: 1px solid #f2dce9;
      border-radius: 24px;
      background: linear-gradient(100deg, #fff3f9, #f5effb);
    }

    .about-band h2 { margin: 0 0 8px; font-size: 22px; }
    .about-band p { max-width: 720px; margin: 0; color: var(--muted); line-height: 1.8; }
    .about-decoration { font-size: 54px; }

    .site-footer {
      padding: 28px 20px;
      color: #e9dff0;
      background: var(--purple-dark);
    }

    .footer-inner {
      width: min(1180px, 100%);
      margin: auto;
      display: flex;
      justify-content: space-between;
      gap: 20px;
      font-size: 13px;
    }

    /* لوحة الإدارة */
    .admin-page {
      width: min(1180px, calc(100% - 40px));
      margin: 38px auto 70px;
    }

    .admin-heading {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      margin-bottom: 20px;
    }

    .admin-heading h1 { margin: 7px 0; font-size: 32px; }
    .admin-heading p { margin: 0; color: var(--muted); line-height: 1.7; }

    .btn-primary { color: #fff; background: var(--purple); }

    .demo-warning {
      margin-bottom: 22px;
      padding: 14px 17px;
      color: #704c16;
      border: 1px solid #f4dfb2;
      border-radius: 14px;
      background: #fff9e9;
      font-size: 13px;
      line-height: 1.7;
    }

    .stats-grid {
      margin-bottom: 22px;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 14px;
    }

    .stat-card {
      padding: 18px;
      border: 1px solid var(--line);
      border-radius: 17px;
      background: #fff;
    }

    .stat-card span { color: var(--muted); font-size: 12px; }
    .stat-card strong {
      display: block;
      margin-top: 9px;
      color: var(--purple-dark);
      font-size: 23px;
    }

    .admin-panel {
      margin-top: 20px;
      padding: 22px;
      border: 1px solid var(--line);
      border-radius: 20px;
      background: #fff;
      box-shadow: 0 8px 28px rgba(62, 29, 91, .04);
    }

    .panel-heading {
      margin-bottom: 17px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 15px;
    }

    .panel-heading h2 { margin: 0; font-size: 20px; }
    .panel-heading p { margin: 6px 0 0; color: var(--muted); font-size: 12px; }

    .admin-form {
      margin-bottom: 20px;
      padding: 17px;
      border-radius: 16px;
      background: #fcf9fd;
    }

    .form-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 13px;
    }

    .field label, .checkout-field label {
      display: block;
      margin-bottom: 7px;
      color: #554662;
      font-size: 12px;
      font-weight: 700;
    }

    .field input, .field select, .checkout-field input, .checkout-field textarea {
      width: 100%;
      min-height: 43px;
      padding: 10px 12px;
      border: 1px solid #e7deeb;
      border-radius: 11px;
      outline: 0;
      color: var(--ink);
      background: #fff;
    }

    .field input:focus, .field select:focus,
    .checkout-field input:focus, .checkout-field textarea:focus {
      border-color: var(--purple);
      box-shadow: 0 0 0 3px rgba(117, 66, 168, .1);
    }

    .form-actions { margin-top: 14px; display: flex; gap: 9px; }
    .btn-secondary { color: var(--purple); background: var(--purple-light); }
    .btn-secondary:hover { background: #e7d8f3; }

    .table-wrap {
      width: 100%;
      overflow-x: auto;
      border: 1px solid var(--line);
      border-radius: 13px;
    }

    table {
      width: 100%;
      min-width: 720px;
      border-collapse: collapse;
      text-align: right;
      font-size: 13px;
    }

    th, td {
      padding: 13px 14px;
      border-bottom: 1px solid #f1ebf4;
      vertical-align: middle;
    }

    th {
      color: #6d5f79;
      background: #faf7fc;
      font-size: 12px;
      white-space: nowrap;
    }

    tr:last-child td { border-bottom: 0; }
    td small { display: block; margin-top: 5px; color: var(--muted); font-size: 11px; }

    .table-actions { display: flex; gap: 7px; }
    .table-action {
      padding: 7px 9px;
      border: 0;
      border-radius: 9px;
      color: var(--purple);
      background: var(--purple-light);
      font-size: 11px;
    }

    .table-action.delete { color: #a33658; background: #fff0f3; }

    .status-select {
      min-width: 125px;
      padding: 8px;
      border: 1px solid #e7deeb;
      border-radius: 9px;
      color: var(--purple-dark);
      background: #fff;
    }

    /* السلة */
    .drawer-overlay {
      position: fixed;
      z-index: 39;
      inset: 0;
      visibility: hidden;
      opacity: 0;
      background: rgba(31, 17, 42, .4);
      transition: .2s ease;
    }

    .drawer-overlay.active { visibility: visible; opacity: 1; }

    .cart-drawer {
      position: fixed;
      z-index: 40;
      inset-block: 0;
      right: 0;
      width: min(440px, 94vw);
      padding: 20px;
      display: flex;
      flex-direction: column;
      background: #fff;
      box-shadow: -15px 0 45px rgba(31, 17, 42, .15);
      transform: translateX(110%);
      transition: transform .25s ease;
    }

    .cart-drawer.open { transform: translateX(0); }

    .drawer-head {
      padding-bottom: 15px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid var(--line);
    }

    .drawer-head h2 { margin: 0; font-size: 21px; }
    .close-button {
      width: 38px;
      height: 38px;
      border: 0;
      border-radius: 12px;
      color: var(--purple-dark);
      background: var(--purple-light);
      font-size: 20px;
    }

    .cart-items { flex: 1; overflow-y: auto; padding-block: 12px; }

    .cart-line {
      padding: 13px 0;
      display: grid;
      grid-template-columns: 55px 1fr auto;
      align-items: center;
      gap: 12px;
      border-bottom: 1px solid #f1ebf4;
    }

    .cart-line-art {
      width: 55px;
      height: 55px;
      display: grid;
      place-items: center;
      border-radius: 14px;
      background: var(--pink-light);
      font-size: 29px;
    }

    .cart-line h3 { margin: 0 0 6px; font-size: 13px; }
    .cart-line small { color: var(--muted); font-size: 11px; }
    .qty-controls { margin-top: 8px; display: flex; align-items: center; gap: 8px; }
    .qty-controls button {
      width: 25px;
      height: 25px;
      border: 1px solid var(--line);
      border-radius: 8px;
      color: var(--purple);
      background: #fff;
    }

    .remove-item {
      padding: 5px;
      border: 0;
      color: #a33658;
      background: transparent;
      font-size: 11px;
    }

    .empty-cart {
      flex: 1;
      display: grid;
      place-items: center;
      color: var(--muted);
      text-align: center;
      line-height: 1.8;
    }

    .cart-summary {
      padding-top: 14px;
      border-top: 1px solid var(--line);
    }

    .summary-total {
      margin-bottom: 14px;
      display: flex;
      justify-content: space-between;
      font-weight: 800;
    }

    .checkout-form { display: grid; gap: 10px; }
    .checkout-field input, .checkout-field textarea { min-height: 42px; font-size: 13px; }
    .checkout-field textarea { min-height: 66px; resize: vertical; }
    .checkout-submit { width: 100%; border: 0; }
    .checkout-hint { margin: 0; color: var(--muted); font-size: 11px; text-align: center; }

    .toast {
      position: fixed;
      z-index: 60;
      right: 50%;
      bottom: 22px;
      max-width: calc(100% - 30px);
      padding: 13px 18px;
      color: #fff;
      border-radius: 13px;
      background: var(--purple-dark);
      box-shadow: var(--shadow);
      opacity: 0;
      pointer-events: none;
      transform: translate(50%, 15px);
      transition: .2s ease;
      font-size: 13px;
    }

    .toast.show { opacity: 1; transform: translate(50%, 0); }

    @media (max-width: 950px) {
      .main-nav { gap: 16px; }
      .product-grid { grid-template-columns: repeat(3, minmax(0, 1fr)); }
      .hero { grid-template-columns: 1fr .8fr; }
    }

    @media (max-width: 760px) {
      .site-header { min-height: 70px; padding-inline: 16px; }
      .main-nav { display: none; }
      .hero { grid-template-columns: 1fr; padding: 35px 26px; }
      .hero-art { min-height: 260px; }
      .hero-art-circle { width: 230px; height: 230px; }
      .hero-cupcake { font-size: 115px; }
      .benefits { grid-template-columns: 1fr; margin-bottom: 55px; }
      .section-heading { align-items: stretch; flex-direction: column; }
      .search-box { width: 100%; }
      .product-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
      .stats-grid { grid-template-columns: repeat(2, 1fr); }
      .form-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
      .about-band { align-items: flex-start; }
      .footer-inner { flex-direction: column; }
    }

    @media (max-width: 480px) {
      .brand-copy small { display: none; }
      .brand-copy strong { font-size: 17px; }
      .brand-mark { width: 40px; height: 40px; }
      .header-actions { gap: 6px; }
      .admin-button, .cart-button { padding: 10px; font-size: 12px; }
      .container, .admin-page { width: min(100% - 24px, 1180px); }
      .hero { margin-top: 14px; border-radius: 24px; }
      .hero-copy h1 { font-size: 34px; }
      .floating-note { padding: 9px 11px; }
      .product-grid { gap: 10px; }
      .product-art { min-height: 135px; }
      .product-emoji { font-size: 60px; }
      .product-info { padding: 12px; }
      .product-info h3 { font-size: 14px; }
      .product-bottom { align-items: flex-start; flex-direction: column; }
      .add-button { width: 100%; }
      .form-grid { grid-template-columns: 1fr; }
      .admin-heading { align-items: flex-start; flex-direction: column; }
      .admin-panel { padding: 15px; }
      .about-band { padding: 20px; }
      .about-decoration { display: none; }
    }
  </style>
</head>

<body>
  <div class="announcement">كل ما تحتاجينه لصناعة حلويات جميلة وتغليفها بذوق ✨</div>

  <header class="site-header">
    <a class="brand" href="#home" aria-label="سكر وورد - الرئيسية">
      <span class="brand-mark">✿</span>
      <span class="brand-copy">
        <strong>سكر <b>وورد</b></strong>
        <small>مستلزمات الحلويات والتغليف</small>
      </span>
    </a>

    <nav class="main-nav" aria-label="التنقل الرئيسي">
      <a href="#home">الرئيسية</a>
      <a href="#products">المنتجات</a>
      <a href="#about">عن المتجر</a>
    </nav>

    <div class="header-actions">
      <button class="admin-button" id="adminToggle" type="button">⚙️ لوحة التحكم</button>
      <button class="cart-button" id="cartToggle" type="button">
        <span>🛍️</span><span>السلة</span><b class="cart-count" id="cartCount">0</b>
      </button>
    </div>
  </header>

  <div id="storeView">
    <main>
      <section class="hero container" id="home">
        <div class="hero-copy">
          <span class="hero-label">🧁 مستلزمات الخَبز، التزيين والتغليف</span>
          <h1>كل ما يحتاجه <em>حلاك</em><br>في مكان واحد</h1>
          <p>اختاري أدواتك وتغليفك المفضل، وابدئي بصناعة تفاصيل حلوة تستحق أن تُهدى وتُشارك.</p>
          <div class="hero-actions">
            <a class="btn btn-white" href="#products">تصفحي المنتجات <span>←</span></a>
            <span class="hero-note">أفكار جميلة لمناسباتك ومشاريعك</span>
          </div>
        </div>

        <div class="hero-art" aria-hidden="true">
          <div class="hero-art-circle"><span class="hero-cupcake">🧁</span></div>
          <div class="floating-note note-top">
            <span>🎀</span><div><strong>تغليف أنيق</strong><small>لمسة جميلة لكل هدية</small></div>
          </div>
          <div class="floating-note note-bottom">
            <span>🍰</span><div><strong>تفاصيل تصنع الفرق</strong><small>اختاري ما يناسب إبداعك</small></div>
          </div>
        </div>
      </section>

      <section class="benefits container" aria-label="مميزات المتجر">
        <div class="benefit">
          <span class="benefit-icon">🎂</span>
          <div><strong>مستلزمات متنوعة</strong><small>للخبز والتزيين والتغليف</small></div>
        </div>
        <div class="benefit">
          <span class="benefit-icon">🎨</span>
          <div><strong>خيارات تناسب ذوقك</strong><small>اختاري الألوان والأشكال التي تحبينها</small></div>
        </div>
        <div class="benefit">
          <span class="benefit-icon">💝</span>
          <div><strong>لكل مناسبة حلوة</strong><small>أفكار لمشاريعك وهداياك</small></div>
        </div>
      </section>

      <section class="container" id="products">
        <div class="section-heading">
          <div>
            <span class="eyebrow">تسوقي حسب احتياجك</span>
            <h2>منتجاتنا</h2>
            <p>تصفحي التشكيلة واختاري ما يلهم إبداعاتك.</p>
          </div>
          <label class="search-box">
            <span>⌕</span>
            <input id="productSearch" type="search" placeholder="ابحثي عن منتج..." aria-label="ابحثي عن منتج">
          </label>
        </div>

        <div class="filter-row" id="categoryFilters"></div>
        <div class="results-line" id="productCount"></div>
        <div class="product-grid" id="productGrid"></div>
      </section>

      <section class="about-band container" id="about">
        <div>
          <h2>كل تفصيلة صغيرة تصنع حلاوة أكبر 💜</h2>
          <p>جمعنا في «سكر وورد» مستلزمات تساعدك على الخَبز والتزيين وتقديم منتجاتك بطريقة جميلة. أضيفي المنتجات إلى السلة لإرسال طلب تجريبي.</p>
        </div>
        <span class="about-decoration" aria-hidden="true">🎁</span>
      </section>
    </main>

    <footer class="site-footer">
      <div class="footer-inner">
        <span>© <span id="year"></span> سكر وورد</span>
        <span>مستلزمات الحلويات والتغليف — كل الحقوق محفوظة</span>
      </div>
    </footer>
  </div>

  <section class="admin-view hidden" id="adminView">
    <main class="admin-page">
      <div class="admin-heading">
        <div>
          <span class="eyebrow">إدارة المتجر</span>
          <h1>لوحة التحكم</h1>
          <p>أضيفي المنتجات وعدّلي الأسعار والمخزون، وتابعي الطلبات وحالاتها.</p>
        </div>
        <button class="btn btn-primary" id="backToStore" type="button">العودة إلى المتجر</button>
      </div>

      <div class="demo-warning">
        <strong>تنبيه:</strong> هذه لوحة تجريبية تحفظ البيانات في هذا المتصفح فقط. لا تستخدميها لحفظ بيانات عملاء حقيقية أو كلوحة إدارة منشورة للعامة.
      </div>

      <div class="stats-grid" id="adminStats"></div>

      <section class="admin-panel">
        <div class="panel-heading">
          <div>
            <h2>إدارة المنتجات</h2>
            <p>أضيفي منتجًا جديدًا أو عدّلي بيانات منتج موجود.</p>
          </div>
        </div>

        <form class="admin-form" id="productForm">
          <input type="hidden" id="editProductId">
          <div class="form-grid">
            <div class="field">
              <label for="productName">اسم المنتج</label>
              <input id="productName" required maxlength="80" placeholder="مثال: علبة كيك شفافة">
            </div>
            <div class="field">
              <label for="productCategory">التصنيف</label>
              <input id="productCategory" list="categoriesList" required maxlength="40" placeholder="اختاري أو اكتبي تصنيفًا">
              <datalist id="categoriesList"></datalist>
            </div>
            <div class="field">
              <label for="productPrice">السعر</label>
              <input id="productPrice" type="number" min="0" step="1" required placeholder="مثال: 500">
            </div>
            <div class="field">
              <label for="productStock">الكمية المتوفرة</label>
              <input id="productStock" type="number" min="0" step="1" required placeholder="مثال: 20">
            </div>
            <div class="field">
              <label for="productEmoji">رمز العرض (إيموجي)</label>
              <input id="productEmoji" maxlength="8" value="🧁" placeholder="🧁">
            </div>
            <div class="field">
              <label for="productDescription">وصف قصير</label>
              <input id="productDescription" maxlength="120" placeholder="وصف بسيط للمنتج">
            </div>
          </div>
          <div class="form-actions">
            <button class="btn btn-primary" id="saveProductButton" type="submit">إضافة المنتج</button>
            <button class="btn btn-secondary hidden" id="cancelEdit" type="button">إلغاء التعديل</button>
          </div>
        </form>

        <div class="table-wrap">
          <table>
            <thead>
              <tr>
                <th>المنتج</th>
                <th>التصنيف</th>
                <th>السعر</th>
                <th>المخزون</th>
                <th>الإجراءات</th>
              </tr>
            </thead>
            <tbody id="adminProductsBody"></tbody>
          </table>
        </div>
      </section>

      <section class="admin-panel">
        <div class="panel-heading">
          <div>
            <h2>معالجة الطلبات</h2>
            <p>راجعي تفاصيل الطلب وغيّري حالته من القائمة.</p>
          </div>
        </div>
        <div class="table-wrap">
          <table>
            <thead>
              <tr>
                <th>رقم الطلب</th>
                <th>العميل</th>
                <th>المنتجات</th>
                <th>الإجمالي</th>
                <th>الحالة</th>
              </tr>
            </thead>
            <tbody id="adminOrdersBody"></tbody>
          </table>
        </div>
      </section>
    </main>
  </section>

  <div class="drawer-overlay" id="drawerOverlay"></div>

  <aside class="cart-drawer" id="cartDrawer" aria-label="سلة المشتريات" aria-hidden="true">
    <div class="drawer-head">
      <h2>سلة المشتريات</h2>
      <button class="close-button" id="closeCart" type="button" aria-label="إغلاق السلة">×</button>
    </div>

    <div class="cart-items" id="cartItems"></div>
    <div class="empty-cart" id="emptyCart">سلتك فارغة حاليًا 🛍️<br>أضيفي بعض المنتجات لتبدئي طلبك.</div>

    <div class="cart-summary hidden" id="cartSummary">
      <div class="summary-total"><span>الإجمالي</span><span id="cartTotal">0</span></div>
      <form class="checkout-form" id="checkoutForm">
        <div class="checkout-field">
          <label for="customerName">الاسم</label>
          <input id="customerName" required maxlength="80" placeholder="اسم صاحب الطلب">
        </div>
        <div class="checkout-field">
          <label for="customerPhone">رقم الهاتف</label>
          <input id="customerPhone" type="tel" required maxlength="30" placeholder="رقم للتواصل">
        </div>
        <div class="checkout-field">
          <label for="customerAddress">العنوان</label>
          <textarea id="customerAddress" required maxlength="180" placeholder="المدينة والعنوان"></textarea>
        </div>
        <button class="btn btn-primary checkout-submit" type="submit">إرسال الطلب</button>
        <p class="checkout-hint">سيظهر الطلب في لوحة التحكم التجريبية.</p>
      </form>
    </div>
  </aside>

  <div class="toast" id="toast" role="status" aria-live="polite"></div>

  <script>
    const CURRENCY = "د.ج";

    const seedProducts = [
      { id: "p1", name: "قوالب كب كيك ورقية", category: "أدوات الخَبز", price: 520, stock: 32, emoji: "🧁", description: "قوالب عملية لتقديم الكب كيك بشكل جميل." },
      { id: "p2", name: "علبة كيك شفافة", category: "التغليف", price: 350, stock: 25, emoji: "🎂", description: "علبة أنيقة لحفظ الكيك وتقديمه." },
      { id: "p3", name: "مجموعة رؤوس تزيين", category: "تزيين الكيك", price: 1200, stock: 18, emoji: "🍰", description: "أشكال متنوعة لإضافة لمساتك الخاصة." },
      { id: "p4", name: "أكياس حلواني", category: "أدوات الخَبز", price: 680, stock: 30, emoji: "🍥", description: "مناسبة لتزيين الكيك والحلويات بالكريمة." },
      { id: "p5", name: "قوالب سيليكون", category: "أدوات الخَبز", price: 950, stock: 14, emoji: "🍮", description: "قوالب متعددة الاستخدامات بأشكال جميلة." },
      { id: "p6", name: "شرائط ساتان للتغليف", category: "التغليف", price: 300, stock: 40, emoji: "🎀", description: "لمسة نهائية أنيقة لصناديق الهدايا." },
      { id: "p7", name: "رشات تزيين ملونة", category: "مكونات وتزيين", price: 450, stock: 24, emoji: "🌈", description: "زيني بها الكيك والكب كيك والحلويات." },
      { id: "p8", name: "شموع عيد ميلاد", category: "مستلزمات المناسبات", price: 250, stock: 35, emoji: "🕯️", description: "تفاصيل بسيطة تضيف بهجة للمناسبة." }
    ];

    const KEYS = {
      products: "sukar-ward-products-v1",
      orders: "sukar-ward-orders-v1",
      cart: "sukar-ward-cart-v1"
    };

    function readStorage(key, fallback) {
      try {
        const value = localStorage.getItem(key);
        return value === null ? fallback : JSON.parse(value);
      } catch {
        return fallback;
      }
    }

    const savedProducts = readStorage(KEYS.products, seedProducts);
    const savedOrders = readStorage(KEYS.orders, []);
    const savedCart = readStorage(KEYS.cart, {});

    let products = Array.isArray(savedProducts) ? savedProducts : seedProducts;
    let orders = Array.isArray(savedOrders) ? savedOrders : [];
    let cart = savedCart && typeof savedCart === "object" && !Array.isArray(savedCart) ? savedCart : {};
    let activeCategory = "الكل";
    let searchTerm = "";
    let toastTimer;

    const statusLabels = {
      new: "جديد",
      processing: "قيد التجهيز",
      shipped: "تم الشحن",
      completed: "مكتمل",
      cancelled: "ملغي"
    };

    function saveState() {
      try {
        localStorage.setItem(KEYS.products, JSON.stringify(products));
        localStorage.setItem(KEYS.orders, JSON.stringify(orders));
        localStorage.setItem(KEYS.cart, JSON.stringify(cart));
      } catch (error) {
        console.error("تعذر حفظ البيانات محليًا:", error);
      }
    }

    function escapeHTML(value) {
      return String(value ?? "").replace(/[&<>"']/g, char => ({
        "&": "&amp;",
        "<": "&lt;",
        ">": "&gt;",
        '"': "&quot;",
        "'": "&#39;"
      })[char]);
    }

    function formatPrice(value) {
      const amount = Number(value) || 0;
      return `${new Intl.NumberFormat("fr-DZ", { maximumFractionDigits: 0 }).format(amount)} ${CURRENCY}`;
    }

    function showToast(message) {
      const toast = document.getElementById("toast");
      toast.textContent = message;
      toast.classList.add("show");
      clearTimeout(toastTimer);
      toastTimer = setTimeout(() => toast.classList.remove("show"), 2500);
    }

    function renderCategories() {
      const container = document.getElementById("categoryFilters");
      const categories = ["الكل", ...new Set(products.map(p => p.category).filter(Boolean))];

      if (!categories.includes(activeCategory)) activeCategory = "الكل";

      container.innerHTML = categories.map(category => `
        <button class="filter-chip ${category === activeCategory ? "active" : ""}"
                type="button"
                data-category="${escapeHTML(category)}"
                aria-pressed="${category === activeCategory}">
          ${escapeHTML(category)}
        </button>
      `).join("");
    }

    function renderProducts() {
      const grid = document.getElementById("productGrid");
      const matching = products.filter(product => {
        const categoryMatch = activeCategory === "الكل" || product.category === activeCategory;
        const searchText = `${product.name || ""} ${product.category || ""} ${product.description || ""}`.toLowerCase();
        return categoryMatch && searchText.includes(searchTerm.toLowerCase());
      });

      document.getElementById("productCount").textContent = `عدد المنتجات: ${matching.length}`;

      if (!matching.length) {
        grid.innerHTML = `<div class="empty-state">لم نجد منتجات مطابقة. جرّبي كلمة بحث أو تصنيفًا آخر.</div>`;
        return;
      }

      grid.innerHTML = matching.map((product, index) => {
        const outOfStock = Number(product.stock) <= 0;
        return `
          <article class="product-card">
            <div class="product-art art-${index % 4}">
              <span class="product-category-tag">${escapeHTML(product.category)}</span>
              <span class="product-emoji">${escapeHTML(product.emoji || "🧁")}</span>
            </div>
            <div class="product-info">
              <h3>${escapeHTML(product.name)}</h3>
              <p>${escapeHTML(product.description || "منتج مميز لمستلزمات الحلويات والتغليف.")}</p>
              <div class="stock-text ${outOfStock ? "out" : ""}">
                ${outOfStock ? "نفد المخزون" : `متوفر: ${Number(product.stock)} قطعة`}
              </div>
              <div class="product-bottom">
                <span class="product-price">${formatPrice(product.price)}</span>
                <button class="add-button" type="button" data-add-id="${escapeHTML(product.id)}" ${outOfStock ? "disabled" : ""}>
                  أضف للسلة
                </button>
              </div>
            </div>
          </article>
        `;
      }).join("");
    }

    function renderStore() {
      renderCategories();
      renderProducts();
      renderCart();
    }

    function getCartItems() {
      return Object.entries(cart).map(([id, rawQty]) => {
        const product = products.find(item => String(item.id) === String(id));
        const qty = Math.max(0, parseInt(rawQty, 10) || 0);
        return product && qty ? { product, qty } : null;
      }).filter(Boolean);
    }

    function renderCart() {
      const itemsContainer = document.getElementById("cartItems");
      const emptyCart = document.getElementById("emptyCart");
      const cartSummary = document.getElementById("cartSummary");
      const items = getCartItems();
      const count = items.reduce((sum, item) => sum + item.qty, 0);
      const total = items.reduce((sum, item) => sum + Number(item.product.price) * item.qty, 0);

      document.getElementById("cartCount").textContent = count;
      emptyCart.classList.toggle("hidden", items.length > 0);
      cartSummary.classList.toggle("hidden", items.length === 0);
      document.getElementById("cartTotal").textContent = formatPrice(total);

      itemsContainer.innerHTML = items.map(({ product, qty }) => `
        <div class="cart-line">
          <div class="cart-line-art">${escapeHTML(product.emoji || "🧁")}</div>
          <div>
            <h3>${escapeHTML(product.name)}</h3>
            <small>${formatPrice(product.price)}</small>
            <div class="qty-controls">
              <button type="button" data-cart-action="minus" data-id="${escapeHTML(product.id)}" aria-label="تقليل الكمية">−</button>
              <span>${qty}</span>
              <button type="button" data-cart-action="plus" data-id="${escapeHTML(product.id)}" aria-label="زيادة الكمية">+</button>
            </div>
          </div>
          <button class="remove-item" type="button" data-cart-action="remove" data-id="${escapeHTML(product.id)}">حذف</button>
        </div>
      `).join("");
    }

    function addToCart(id) {
      const product = products.find(item => String(item.id) === String(id));
      if (!product) return;

      const currentQty = Number(cart[id]) || 0;
      if (currentQty >= Number(product.stock)) {
        showToast("لا توجد كمية إضافية متاحة من هذا المنتج.");
        return;
      }

      cart[id] = currentQty + 1;
      saveState();
      renderCart();
      showToast("أُضيف المنتج إلى السلة.");
    }

    function openCart() {
      document.getElementById("cartDrawer").classList.add("open");
      document.getElementById("drawerOverlay").classList.add("active");
      document.getElementById("cartDrawer").setAttribute("aria-hidden", "false");
      document.body.classList.add("no-scroll");
    }

    function closeCart() {
      document.getElementById("cartDrawer").classList.remove("open");
      document.getElementById("drawerOverlay").classList.remove("active");
      document.getElementById("cartDrawer").setAttribute("aria-hidden", "true");
      document.body.classList.remove("no-scroll");
    }

    function setAdminMode(enabled) {
      document.getElementById("storeView").classList.toggle("hidden", enabled);
      document.getElementById("adminView").classList.toggle("hidden", !enabled);
      document.body.classList.toggle("admin-mode", enabled);
      document.getElementById("adminToggle").textContent = enabled ? "← العودة للمتجر" : "⚙️ لوحة التحكم";
      closeCart();
      if (enabled) {
        renderAdmin();
        window.scrollTo({ top: 0, behavior: "smooth" });
      }
    }

    function updateCategoryList() {
      const list = document.getElementById("categoriesList");
      const defaults = ["أدوات الخَبز", "تزيين الكيك", "التغليف", "مكونات وتزيين", "مستلزمات المناسبات"];
      const categories = [...new Set([...defaults, ...products.map(p => p.category).filter(Boolean)])];
      list.innerHTML = categories.map(category => `<option value="${escapeHTML(category)}"></option>`).join("");
    }

    function displayDate(value) {
      const date = new Date(value);
      return Number.isNaN(date.getTime()) ? "—" : date.toLocaleDateString("ar-DZ");
    }

    function renderAdmin() {
      const totalValue = orders
        .filter(order => order.status !== "cancelled")
        .reduce((sum, order) => sum + (Number(order.total) || 0), 0);
      const newOrders = orders.filter(order => order.status === "new").length;

      document.getElementById("adminStats").innerHTML = `
        <div class="stat-card"><span>عدد المنتجات</span><strong>${products.length}</strong></div>
        <div class="stat-card"><span>كل الطلبات</span><strong>${orders.length}</strong></div>
        <div class="stat-card"><span>طلبات جديدة</span><strong>${newOrders}</strong></div>
        <div class="stat-card"><span>قيمة الطلبات غير الملغاة</span><strong>${formatPrice(totalValue)}</strong></div>
      `;

      updateCategoryList();

      const productsBody = document.getElementById("adminProductsBody");
      if (!products.length) {
        productsBody.innerHTML = `<tr><td colspan="5">لا توجد منتجات بعد.</td></tr>`;
      } else {
        productsBody.innerHTML = products.map(product => `
          <tr>
            <td><strong>${escapeHTML(product.emoji || "🧁")} ${escapeHTML(product.name)}</strong></td>
            <td>${escapeHTML(product.category)}</td>
            <td>${formatPrice(product.price)}</td>
            <td>${Number(product.stock) || 0}</td>
            <td>
              <div class="table-actions">
                <button class="table-action" type="button" data-product-action="edit" data-id="${escapeHTML(product.id)}">تعديل</button>
                <button class="table-action delete" type="button" data-product-action="delete" data-id="${escapeHTML(product.id)}">حذف</button>
              </div>
            </td>
          </tr>
        `).join("");
      }

      const ordersBody = document.getElementById("adminOrdersBody");
      if (!orders.length) {
        ordersBody.innerHTML = `<tr><td colspan="5">لا توجد طلبات حتى الآن. ستظهر الطلبات الجديدة هنا.</td></tr>`;
      } else {
        ordersBody.innerHTML = orders.map(order => {
          const customer = order.customer || {};
          const orderItems = Array.isArray(order.items) ? order.items : [];
          const itemSummary = orderItems.map(item =>
            `${escapeHTML(item.name)} × ${Number(item.qty) || 0}`
          ).join("، ") || "—";
          const currentStatus = statusLabels[order.status] ? order.status : "new";
          const options = Object.entries(statusLabels).map(([value, label]) =>
            `<option value="${value}" ${currentStatus === value ? "selected" : ""}>${label}</option>`
          ).join("");

          return `
            <tr>
              <td><strong>${escapeHTML(order.id || "—")}</strong><small>${displayDate(order.createdAt)}</small></td>
              <td>
                <strong>${escapeHTML(customer.name || "—")}</strong>
                <small>${escapeHTML(customer.phone || "")}</small>
                <small>${escapeHTML(customer.address || "")}</small>
              </td>
              <td>${itemSummary}</td>
              <td>${formatPrice(order.total)}</td>
              <td>
                <select class="status-select" data-order-id="${escapeHTML(order.id)}" aria-label="تغيير حالة الطلب">
                  ${options}
                </select>
              </td>
            </tr>
          `;
        }).join("");
      }
    }

    function resetProductForm() {
      const form = document.getElementById("productForm");
      form.reset();
      document.getElementById("editProductId").value = "";
      document.getElementById("productEmoji").value = "🧁";
      document.getElementById("saveProductButton").textContent = "إضافة المنتج";
      document.getElementById("cancelEdit").classList.add("hidden");
    }

    function startProductEdit(id) {
      const product = products.find(item => String(item.id) === String(id));
      if (!product) return;

      document.getElementById("editProductId").value = product.id;
      document.getElementById("productName").value = product.name || "";
      document.getElementById("productCategory").value = product.category || "";
      document.getElementById("productPrice").value = Number(product.price) || 0;
      document.getElementById("productStock").value = Number(product.stock) || 0;
      document.getElementById("productEmoji").value = product.emoji || "🧁";
      document.getElementById("productDescription").value = product.description || "";
      document.getElementById("saveProductButton").textContent = "حفظ التعديلات";
      document.getElementById("cancelEdit").classList.remove("hidden");
      document.getElementById("productForm").scrollIntoView({ behavior: "smooth", block: "center" });
    }

    function changeOrderStatus(orderId, nextStatus) {
      const order = orders.find(item => String(item.id) === String(orderId));
      if (!order || !statusLabels[nextStatus]) return;

      const previousStatus = order.status || "new";
      const items = Array.isArray(order.items) ? order.items : [];

      if (nextStatus === "cancelled" && previousStatus !== "cancelled" && order.stockReserved !== false) {
        items.forEach(item => {
          const productId = item.productId || item.id;
          const product = products.find(p => String(p.id) === String(productId));
          if (product) product.stock = (Number(product.stock) || 0) + (Number(item.qty) || 0);
        });
        order.stockReserved = false;
      }

      if (previousStatus === "cancelled" && nextStatus !== "cancelled" && order.stockReserved === false) {
        const canReserve = items.every(item => {
          const productId = item.productId || item.id;
          const product = products.find(p => String(p.id) === String(productId));
          return !product || Number(product.stock) >= (Number(item.qty) || 0);
        });

        if (!canReserve) {
          showToast("المخزون الحالي لا يكفي لإعادة تفعيل هذا الطلب.");
          renderAdmin();
          return;
        }

        items.forEach(item => {
          const productId = item.productId || item.id;
          const product = products.find(p => String(p.id) === String(productId));
          if (product) product.stock = Number(product.stock) - (Number(item.qty) || 0);
        });
        order.stockReserved = true;
      }

      order.status = nextStatus;
      saveState();
      renderStore();
      renderAdmin();
      showToast("تم تحديث حالة الطلب.");
    }

    document.getElementById("categoryFilters").addEventListener("click", event => {
      const button = event.target.closest("[data-category]");
      if (!button) return;
      activeCategory = button.dataset.category;
      renderCategories();
      renderProducts();
    });

    document.getElementById("productSearch").addEventListener("input", event => {
      searchTerm = event.target.value.trim();
      renderProducts();
    });

    document.getElementById("productGrid").addEventListener("click", event => {
      const button = event.target.closest("[data-add-id]");
      if (button) addToCart(button.dataset.addId);
    });

    document.getElementById("cartToggle").addEventListener("click", openCart);
    document.getElementById("closeCart").addEventListener("click", closeCart);
    document.getElementById("drawerOverlay").addEventListener("click", closeCart);

    document.addEventListener("keydown", event => {
      if (event.key === "Escape") closeCart();
    });

    document.getElementById("cartItems").addEventListener("click", event => {
      const button = event.target.closest("[data-cart-action]");
      if (!button) return;

      const id = button.dataset.id;
      const action = button.dataset.cartAction;
      const product = products.find(item => String(item.id) === String(id));
      const currentQty = Number(cart[id]) || 0;

      if (action === "remove") {
        delete cart[id];
      } else if (action === "plus" && product) {
        if (currentQty >= Number(product.stock)) {
          showToast("وصلتِ إلى الحد المتوفر من هذا المنتج.");
          return;
        }
        cart[id] = currentQty + 1;
      } else if (action === "minus") {
        if (currentQty <= 1) delete cart[id];
        else cart[id] = currentQty - 1;
      }

      saveState();
      renderCart();
    });

    document.getElementById("checkoutForm").addEventListener("submit", event => {
      event.preventDefault();

      const customer = {
        name: document.getElementById("customerName").value.trim(),
        phone: document.getElementById("customerPhone").value.trim(),
        address: document.getElementById("customerAddress").value.trim()
      };

      const items = getCartItems();
      if (!items.length) return;

      const unavailable = items.find(({ product, qty }) => Number(product.stock) < qty);
      if (unavailable) {
        showToast(`الكمية المتاحة من ${unavailable.product.name} غير كافية.`);
        renderStore();
        return;
      }

      const orderItems = items.map(({ product, qty }) => ({
        productId: product.id,
        name: product.name,
        emoji: product.emoji,
        price: Number(product.price),
        qty
      }));

      const total = orderItems.reduce((sum, item) => sum + item.price * item.qty, 0);
      const order = {
        id: `SW-${Date.now().toString().slice(-6)}`,
        customer,
        items: orderItems,
        total,
        status: "new",
        stockReserved: true,
        createdAt: new Date().toISOString()
      };

      orderItems.forEach(item => {
        const product = products.find(p => String(p.id) === String(item.productId));
        if (product) product.stock = Number(product.stock) - item.qty;
      });

      orders.unshift(order);
      cart = {};
      saveState();
      document.getElementById("checkoutForm").reset();
      renderStore();
      renderAdmin();
      closeCart();
      showToast(`تم تسجيل الطلب ${order.id} بنجاح.`);
    });

    document.getElementById("adminToggle").addEventListener("click", () => {
      const isAdminVisible = !document.getElementById("adminView").classList.contains("hidden");
      setAdminMode(!isAdminVisible);
    });

    document.getElementById("backToStore").addEventListener("click", () => setAdminMode(false));

    document.getElementById("productForm").addEventListener("submit", event => {
      event.preventDefault();

      const editId = document.getElementById("editProductId").value;
      const productData = {
        name: document.getElementById("productName").value.trim(),
        category: document.getElementById("productCategory").value.trim(),
        price: Number(document.getElementById("productPrice").value),
        stock: Number(document.getElementById("productStock").value),
        emoji: document.getElementById("productEmoji").value.trim() || "🧁",
        description: document.getElementById("productDescription").value.trim()
      };

      if (!productData.name || !productData.category || !Number.isFinite(productData.price) || !Number.isFinite(productData.stock)) {
        showToast("يرجى التأكد من إدخال بيانات المنتج والسعر والمخزون.");
        return;
      }

      if (editId) {
        products = products.map(product =>
          String(product.id) === String(editId) ? { ...product, ...productData } : product
        );
        showToast("تم تحديث المنتج.");
      } else {
        products.unshift({
          id: `p-${Date.now()}-${Math.random().toString(16).slice(2, 7)}`,
          ...productData
        });
        showToast("تمت إضافة المنتج.");
      }

      saveState();
      resetProductForm();
      renderStore();
      renderAdmin();
    });

    document.getElementById("cancelEdit").addEventListener("click", resetProductForm);

    document.getElementById("adminProductsBody").addEventListener("click", event => {
      const button = event.target.closest("[data-product-action]");
      if (!button) return;

      const id = button.dataset.id;
      if (button.dataset.productAction === "edit") {
        startProductEdit(id);
      } else if (button.dataset.productAction === "delete") {
        const product = products.find(item => String(item.id) === String(id));
        if (!product || !confirm(`هل تريدين حذف المنتج «${product.name}»؟`)) return;

        products = products.filter(item => String(item.id) !== String(id));
        delete cart[id];
        saveState();
        renderStore();
        renderAdmin();
        showToast("تم حذف المنتج.");
      }
    });

    document.getElementById("adminOrdersBody").addEventListener("change", event => {
      const select = event.target.closest("[data-order-id]");
      if (select) changeOrderStatus(select.dataset.orderId, select.value);
    });

    document.getElementById("year").textContent = new Date().getFullYear();

    renderStore();
    renderAdmin();
  </script>
</body>
</html>
