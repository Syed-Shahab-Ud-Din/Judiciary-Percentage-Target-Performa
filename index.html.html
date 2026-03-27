<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pendency, Percentage Target & Printing System</title>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
  <style>
    :root {
      --navy: #082a74;
      --yellow: #ffef00;
      --cyan: #20dbe5;
      --light: #efefef;
      --white: #ffffff;
      --black: #000000;
      --border: #1c1c1c;
      --danger: #c40000;
      --shadow: none;
    }

    * { box-sizing: border-box; }
    .start-screen {
  position: fixed;
  top:0; left:0;
  width:100%;
  height:100%;
  background:#041f5c;
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  z-index:9999;
}

/* ===== PROFESSIONAL JUDICIARY WATERMARK ===== */
.start-screen::before {
  content: "⚖";
  position: absolute;
  font-size: 320px;
  color: rgba(255,255,255,0.08);
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.start-screen::after {
  content: "JUDICIARY";
  position: absolute;
  top: 60%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 60px;
  font-weight: 900;
  letter-spacing: 8px;
  color: rgba(255,255,255,0.06);
}

.start-content {
  color:#f5e6a8;
  font-weight:900;
  font-size:30px;
  line-height:1.8;
}

.start-btn {
  position:absolute;
  bottom:30px;
  right:30px;
  padding:14px 26px;
  font-weight:800;
  background:#f5e6a8;
  border:none;
  border-radius:10px;
  cursor:pointer;
}

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: #ffffff;
      color: #111;
    }

    .app-wrap {
      max-width: 1500px;
      margin: 0 auto;
      padding: 18px;
    }

    .toolbar {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
      margin-bottom: 18px;
      align-items: center;
    }

    .btn {
      border: none;
      border-radius: 10px;
      padding: 12px 18px;
      font-size: 15px;
      font-weight: 700;
      cursor: pointer;
      box-shadow: var(--shadow);
    }

    .btn-primary { background: var(--navy); color: white; }
    .btn-secondary { background: white; color: var(--navy); border: 2px solid var(--navy); }
    .btn-danger { background: #8d1111; color: white; }

    .hint {
      display: none;
      font-size: 14px;
      color: #344054;
      margin-left: auto;
    }

    .page {
      display: none;
      background: white;
      border-radius: 0;
      box-shadow: var(--shadow);
      overflow: hidden;
    }

    .page.active { display: block; }

    .editing-wrap { padding: 0; }

    .edit-title {
      background: var(--navy);
      color: white;
      text-align: center;
      padding: 20px 12px;
      font-size: 24px;
      font-weight: 800;
      letter-spacing: .3px;
    }

    table { width: 100%; border-collapse: collapse; }

    .edit-table th,
    .edit-table td {
      border: 2px solid rgba(0,0,0,0.45);
      text-align: center;
      vertical-align: middle;
      padding: 10px 8px;
    }

    .edit-table thead th {
      background: var(--navy);
      color: white;
      font-size: 54px;
      font-style: italic;
      font-weight: 900;
      line-height: 1;
      padding: 14px 8px;
    }

    .type-col {
      width: 35%;
      font-size: 34px;
      font-style: italic;
      font-weight: 900;
      line-height: 1.15;
    }

    .num-cell {
      width: 25%;
      background: white;
    }

    .total-col {
      width: 15%;
      background: var(--navy) !important;
      color: white;
      font-weight: 900;
    }

    .row-grey td { background: #e7e4dd; }
    .row-grey .type-col { background: #e2dfd7; }
    .row-yellow td { background: var(--yellow); }
    .row-cyan td { background: var(--cyan); }
    .row-navy td { background: var(--navy); color: white; }

    .label-big {
      display: block;
      font-size: 34px;
      font-weight: 900;
      font-style: italic;
      line-height: 1.1;
    }

    .label-note {
      display: block;
      margin-top: 10px;
      color: red;
      font-size: 16px;
      font-weight: 700;
    }

    input.data-input {
      width: 100%;
      max-width: 220px;
      border: none;
      background: transparent;
      text-align: center;
      font-weight: 900;
      font-size: 86px;
      line-height: 1;
      outline: none;
      color: #000;
      font-family: Arial, Helvetica, sans-serif;
    }

    .readonly-number {
      font-size: 54px;
      font-weight: 900;
      line-height: 1;
      display: block;
      padding: 16px 6px;
    }

    .small-total {
      font-size: 18px;
      color: white;
    }

    .print-page {
      background: #ffffff;
      color: black;
      font-family: "Times New Roman", Times, serif;
      padding-bottom: 24px;
    }

    .print-shell {
      width: 100%;
      max-width: 794px;
      margin: 0 auto;
      background: #ffffff;
    }

    .print-table,
    .print-table th,
    .print-table td,
    .print-target,
    .header-block,
    .section-title,
    .signature-box {
      border: 1.7px solid #777;
    }

    .header-block {
      text-align: center;
      background: #ffffff;
      border-bottom: none;
    }

    .court-line {
      font-size: 34px;
      font-style: italic;
      line-height: 1.15;
      padding: 10px 8px 6px;
    }

    .sub-line {
      font-size: 18px;
      font-style: italic;
      line-height: 1.15;
      padding: 5px 8px 0;
    }

    .date-line {
      font-size: 18px;
      font-style: italic;
      font-weight: 700;
      padding: 5px 8px 8px;
    }

    .print-table th,
    .print-table td {
      text-align: center;
      padding: 8px 6px;
      background: #ffffff;
    }

    .print-table th {
      font-size: 18px;
      font-style: italic;
      font-family: Arial, Helvetica, sans-serif;
      font-weight: 800;
    }

    .row-head {
      font-size: 22px;
      font-family: Arial, Helvetica, sans-serif;
      font-style: italic;
      font-weight: 800;
    }

    .print-value {
      font-size: 18px;
      font-weight: 500;
      line-height: 1;
    }

    .print-percentage {
      font-size: 26px;
      font-style: italic;
      font-weight: 800;
    }

    .print-target {
      display: grid;
      grid-template-columns: 1fr 170px;
      margin-top: 14px;
      background: #ffffff;
    }

    .target-text {
      padding: 14px 12px;
      text-align: center;
      font-size: 14px;
      font-family: Arial, Helvetica, sans-serif;
      font-style: italic;
      font-weight: 800;
      line-height: 1.35;
      border-right: 1.7px solid #777;
    }

    .target-number {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 34px;
      font-weight: 800;
      font-family: Arial, Helvetica, sans-serif;
    }

    .section-title {
      text-align: center;
      font-size: 24px;
      font-style: italic;
      padding: 10px 8px 6px;
      border-bottom: none;
      margin-top: 14px;
      background: #ffffff;
    }

    .signature-box {
      height: 100px;
      border-top: none;
      position: relative;
      background: #ffffff;
    }

    .signature-text {
      position: absolute;
      right: 26px;
      bottom: 24px;
      text-align: center;
      font-family: Arial, Helvetica, sans-serif;
    }

    .signature-text .sign-main {
      font-size: 18px;
      font-weight: 900;
      margin-bottom: 6px;
    }

    .signature-text .sign-sub {
      font-size: 24px;
    }

    .pdf-footer {
      display: none;
      text-align: center;
      font-family: "Times New Roman", Times, serif;
      font-size: 12pt;
      font-style: italic;
      font-weight: 700;
      margin-top: 12px;
    }

    .status-box {
      display: none;
      padding: 14px 18px;
      background: #eef4ff;
      border: 1px solid #c7d7ff;
      color: #15367b;
      font-size: 14px;
      border-radius: 12px;
      margin-bottom: 14px;
    }

    @media (max-width: 1100px) {
      .edit-table thead th { font-size: 36px; }
      .type-col, .label-big { font-size: 24px; }
      input.data-input { font-size: 54px; max-width: 150px; }
      .readonly-number { font-size: 36px; }
      .small-total { font-size: 32px; }
      .court-line { font-size: 38px; }
      .sub-line { font-size: 30px; }
      .date-line { font-size: 18px; }
      .print-value, .print-percentage { font-size: 30px; }
      .section-title { font-size: 18px; }
      .target-text { font-size: 20px; }
      .target-number { font-size: 24px; }
    }

    @media (max-width: 780px) {
      .app-wrap { padding: 10px; }
      .toolbar { flex-direction: column; align-items: stretch; }
      .hint { margin-left: 0; }
      .edit-table thead th { font-size: 22px; }
      .type-col, .label-big { font-size: 18px; }
      .label-note { font-size: 12px; }
      input.data-input { font-size: 34px; max-width: 95px; }
      .readonly-number { font-size: 18px; }
      .small-total { font-size: 22px; }
      .print-target { grid-template-columns: 1fr 120px; }
      .target-number { font-size: 18px; }
      .target-text { font-size: 13px; padding: 16px 10px; }
      .print-table th { font-size: 16px; }
      .row-head { font-size: 14px; }
      .print-value, .print-percentage { font-size: 22px; }
      .court-line { font-size: 22px; }
      .sub-line { font-size: 18px; }
      .date-line { font-size: 13px; }
      .section-title { font-size: 20px; }
      .signature-box { height: 120px; }
      .signature-text .sign-main { font-size: 18px; }
      .signature-text .sign-sub { font-size: 16px; }
    }


    body.pdf-export,
    body.pdf-export .print-page,
    body.pdf-export .print-shell,
    body.pdf-export .header-block,
    body.pdf-export .print-table th,
    body.pdf-export .print-table td,
    body.pdf-export .print-target,
    body.pdf-export .section-title,
    body.pdf-export .signature-box {
      background: #ffffff !important;
      box-shadow: none !important;
    }


    #printingPage,
    #printingPage * {
      box-shadow: none !important;
    }

    #printingPage {
      background: #ffffff !important;
      padding: 0 !important;
      margin: 0 !important;
    }

    .print-shell {
      background: #ffffff !important;
      margin: 0 auto !important;
      padding: 8mm 8mm 6mm 8mm !important;
      min-height: auto !important;
    }

    @page {
      size: A4 portrait;
      margin: 10mm;
    }

    @media print {
      html, body { width: 210mm; height: 297mm; background: #ffffff !important; }
      body { margin: 0; padding: 0; background: white; }
      .no-print { display: none !important; }
      .page:not(#printingPage) { display: none !important; }
      #printingPage {
        display: block !important;
        box-shadow: none !important;
        border-radius: 0 !important;
        width: 100% !important;
        background: #ffffff !important;
      }
      .print-shell {
        width: 100% !important;
        max-width: none !important;
        box-shadow: none !important;
        background: #ffffff !important;
      }
      .pdf-footer { display: block !important; }
    }
  </style>
</head>
<body>
<div class="start-screen" id="startScreen">
  <div class="start-content"
        (باسمہ تعالیٰ) 
        <br>
    PERCENTAGE  TARGET  PERFORMA<br>
    Prepared by <br>
    Syed Shahab Ud Din <br>
    Junior Clerk <br>
    Sessions Court, 
    Battagram
  </div>

  <button class="start-btn" onclick="startApp()">Start</button>
</div>
  <div class="app-wrap no-print" id="mainApp" style="display:none;">
    <div class="toolbar">
      <button class="btn btn-primary" id="showEditingBtn">Open Editing Page</button>
      <button class="btn btn-secondary" id="showPrintingBtn">Open Printing Page</button>
      <button class="btn btn-primary" id="downloadPdfBtn">Download PDF</button>
      <button class="btn btn-danger" id="resetBtn">Reset All Data</button>
      <div class="hint">Editing page and printing page are fully linked. All entries are saved automatically.</div>
    </div>
    <div class="status-box" id="statusBox">System ready. Enter values on the Editing Page.</div>
  </div>

  <section class="page active editing-wrap" id="editingPage">
    <div class="edit-title">Fill in Entries here</div>
    
    <div style="padding:16px 18px 10px; background:#ffffff; border-bottom:2px solid rgba(0,0,0,0.12);">
      <div style="font-size:18px; font-weight:700; margin-bottom:8px; color:#082a74;">Court Name</div>
      <input id="court_name_input" type="text" value="In the Court of DSJ, Battagram"
             style="width:100%; max-width:700px; padding:10px 12px; font-size:20px; font-weight:700; border:2px solid #082a74; border-radius:8px; outline:none;" />
    </div>

    <table class="edit-table">
      <thead>
        <tr>
          <th>Types</th>
          <th>Criminal</th>
          <th>Civil</th>
          <th>Total</th>
        </tr>
      </thead>
      <tbody>
        <tr class="row-grey">
          <td class="type-col">Previous Month (<span id="editingMonthName">Current</span>) Pendency</td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="prev_criminal" value="0" /></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="prev_civil" value="0" /></td>
          <td class="total-col"><span class="readonly-number small-total" id="prev_total">0</span></td>
        </tr>
        <tr class="row-yellow">
          <td class="type-col">
            <span class="label-big">INSTITUTION CASES</span>
            <span class="label-note">Add Remanded and Restore Cases Here Also</span>
          </td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="inst_criminal" value="0" /></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="inst_civil" value="0" /></td>
          <td class="total-col"><span class="readonly-number small-total" id="inst_total">0</span></td>
        </tr>
        <tr class="row-yellow">
          <td class="type-col"><span class="label-big">DISPOSED CASES</span></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="disp_criminal" value="0" /></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="disp_civil" value="0" /></td>
          <td class="total-col"><span class="readonly-number small-total" id="disp_total">0</span></td>
        </tr>
        <tr class="row-cyan">
          <td class="type-col"><span class="label-big">Transfer In Cases</span></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="transfer_in_criminal" value="0" /></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="transfer_in_civil" value="0" /></td>
          <td class="total-col"><span class="readonly-number small-total" id="transfer_in_total">0</span></td>
        </tr>
        <tr class="row-cyan">
          <td class="type-col"><span class="label-big">Transfer Out Cases</span></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="transfer_out_criminal" value="0" /></td>
          <td class="num-cell"><input class="data-input" type="number" min="0" id="transfer_out_civil" value="0" /></td>
          <td class="total-col"><span class="readonly-number small-total" id="transfer_out_total">0</span></td>
        </tr>
        <tr class="row-navy">
          <td class="type-col"><span class="label-big">Total Current Pendency</span></td>
          <td class="num-cell"><span class="readonly-number" id="current_pendency_criminal">0</span></td>
          <td class="num-cell"><span class="readonly-number" id="current_pendency_civil">0</span></td>
          <td class="total-col"><span class="readonly-number" id="current_pendency_total">0</span></td>
        </tr>
      </tbody>
    </table>
  </section>

  <section class="page print-page" id="printingPage">
    <div id="printArea" class="print-shell">
      <div class="header-block">
        <div class="court-line" id="print_court_name">In the Court of DSJ, Battagram</div>
      </div>
      <div class="header-block">
        <div class="sub-line">Percentage Target &amp; Pendency</div>
      </div>
      <div class="header-block">
        <div class="date-line" id="liveDateTime">--</div>
      </div>

      <table class="print-table">
        <thead>
          <tr>
            <th>Type</th>
            <th>Institution Cases</th>
            <th>Disposed Cases</th>
            <th>Percentage</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="row-head">Criminal Cases</td>
            <td class="print-value" id="print_inst_criminal">0</td>
            <td class="print-value" id="print_disp_criminal">0</td>
            <td class="print-percentage" id="print_pct_criminal">0.00%</td>
          </tr>
          <tr>
            <td class="row-head">Civil Cases</td>
            <td class="print-value" id="print_inst_civil">0</td>
            <td class="print-value" id="print_disp_civil">0</td>
            <td class="print-percentage" id="print_pct_civil">0.00%</td>
          </tr>
          <tr>
            <td class="row-head">Total Cases</td>
            <td class="print-value" id="print_inst_total">0</td>
            <td class="print-value" id="print_disp_total">0</td>
            <td class="print-percentage" id="print_pct_total">0.00%</td>
          </tr>
        </tbody>
      </table>

      <div class="print-target">
        <div class="target-text">
          At this stage, if the given number of pending cases are disposed of,<br>
          this Court will achieve 110% of its disposal target.
        </div>
        <div class="target-number" id="targetRequired">0</div>
      </div>

      <div class="section-title">Current total Pendency till now</div>
      <table class="print-table">
        <thead>
          <tr>
            <th>Type</th>
            <th>Criminal</th>
            <th>Civil</th>
            <th>Total</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="row-head">Current Month Pendency</td>
            <td class="print-value" id="print_current_criminal">0</td>
            <td class="print-value" id="print_current_civil">0</td>
            <td class="print-value" id="print_current_total">0</td>
          </tr>
          <tr>
            <td class="row-head">Transfer In Cases</td>
            <td class="print-value" id="print_transfer_in_criminal">0</td>
            <td class="print-value" id="print_transfer_in_civil">0</td>
            <td class="print-value" id="print_transfer_in_total">0</td>
          </tr>
          <tr>
            <td class="row-head">Transfer Out Cases</td>
            <td class="print-value" id="print_transfer_out_criminal">0</td>
            <td class="print-value" id="print_transfer_out_civil">0</td>
            <td class="print-value" id="print_transfer_out_total">0</td>
          </tr>
          <tr>
            <td class="row-head" style="font-size:26px;">Total</td>
            <td class="print-percentage" id="print_total_criminal">0</td>
            <td class="print-percentage" id="print_total_civil">0</td>
            <td class="print-percentage" id="print_total_total">0</td>
          </tr>
        </tbody>
      </table>

      <div class="signature-box">
        <div class="signature-text">
          <div class="sign-main">SIGNATURE</div>
          <div class="sign-sub">Reader/Muharrir</div>
        </div>
      </div>
      <div class="pdf-footer">This Performa is based on CFMIS (PQS)</div>
    </div>
  </section>

  <script>
  function startApp() {
  document.getElementById("startScreen").style.display = "none";
  document.getElementById("mainApp").style.display = "block";
}
    const STORAGE_KEY = 'pendency_percentage_printing_system_v1';

    const COURT_NAME_KEY = 'pendency_percentage_printing_system_court_name';

    const fieldIds = [
      'prev_criminal', 'prev_civil',
      'inst_criminal', 'inst_civil',
      'disp_criminal', 'disp_civil',
      'transfer_in_criminal', 'transfer_in_civil',
      'transfer_out_criminal', 'transfer_out_civil'
    ];

    const inputs = Object.fromEntries(fieldIds.map(id => [id, document.getElementById(id)]));
    const courtNameInput = document.getElementById('court_name_input');
    const statusBox = document.getElementById('statusBox');

    function safeNumber(value) {
      const num = parseInt(value, 10);
      return Number.isFinite(num) && num >= 0 ? num : 0;
    }

    function setMonthName() {
      const now = new Date();
      const previousMonth = new Date(now.getFullYear(), now.getMonth() - 1, 1);
      const monthName = previousMonth.toLocaleString('en-US', { month: 'long' });
      document.getElementById('editingMonthName').textContent = monthName;
    }

    function formatDateTime() {
      const now = new Date();
      const weekday = now.toLocaleDateString('en-US', { weekday: 'long' });
      const day = now.toLocaleDateString('en-US', { day: '2-digit' });
      const month = now.toLocaleDateString('en-US', { month: 'long' });
      const year = now.toLocaleDateString('en-US', { year: 'numeric' });
      const time = now.toLocaleTimeString('en-US', {
        hour: 'numeric', minute: '2-digit', second: '2-digit', hour12: true
      });
      return `${weekday}, ${day} ${month} ${year}  ${time}`;
    }

    function updateDateTime() {
      document.getElementById('liveDateTime').textContent = formatDateTime();
    }

    function percentage(disposed, institution) {
      if (institution <= 0) return 0;
      return (disposed / institution) * 100;
    }

    function formatPercentage(value) {
      return `${value.toFixed(2)}%`;
    }

    function targetRequired(totalInstitution, totalDisposed) {
      const raw = (totalInstitution * 1.10) - totalDisposed;
      const need = Math.ceil(raw);
      return need <= 0 ? 'Achieved' : String(need);
    }

    function saveData() {
      const data = {};
      fieldIds.forEach(id => {
        data[id] = safeNumber(inputs[id].value);
      });
      localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
    }


    function saveCourtName() {
      const value = (courtNameInput?.value || 'In the Court of DSJ, Battagram').trim() || 'In the Court of DSJ, Battagram';
      localStorage.setItem(COURT_NAME_KEY, value);
      const printEl = document.getElementById('print_court_name');
      if (printEl) printEl.textContent = value;
    }

    function loadCourtName() {
      const saved = localStorage.getItem(COURT_NAME_KEY);
      const value = (saved && saved.trim()) ? saved.trim() : 'In the Court of DSJ, Battagram';
      if (courtNameInput) courtNameInput.value = value;
      const printEl = document.getElementById('print_court_name');
      if (printEl) printEl.textContent = value;
    }

    function loadData() {
      try {
        const raw = localStorage.getItem(STORAGE_KEY);
        if (!raw) return;
        const data = JSON.parse(raw);
        fieldIds.forEach(id => {
          if (data[id] !== undefined) inputs[id].value = safeNumber(data[id]);
        });
      } catch (e) {
        console.error('Load error:', e);
      }
    }

    function updateTotalsAndPrint() {
      const prevCr = safeNumber(inputs.prev_criminal.value);
      const prevCv = safeNumber(inputs.prev_civil.value);
      const instCr = safeNumber(inputs.inst_criminal.value);
      const instCv = safeNumber(inputs.inst_civil.value);
      const dispCr = safeNumber(inputs.disp_criminal.value);
      const dispCv = safeNumber(inputs.disp_civil.value);
      const tinCr = safeNumber(inputs.transfer_in_criminal.value);
      const tinCv = safeNumber(inputs.transfer_in_civil.value);
      const toutCr = safeNumber(inputs.transfer_out_criminal.value);
      const toutCv = safeNumber(inputs.transfer_out_civil.value);

      const prevTotal = prevCr + prevCv;
      const instTotal = instCr + instCv;
      const dispTotal = dispCr + dispCv;
      const tinTotal = tinCr + tinCv;
      const toutTotal = toutCr + toutCv;

      const currentCr = prevCr + instCr + tinCr - dispCr - toutCr;
      const currentCv = prevCv + instCv + tinCv - dispCv - toutCv;
      const currentTotal = currentCr + currentCv;

      document.getElementById('prev_total').textContent = prevTotal;
      document.getElementById('inst_total').textContent = instTotal;
      document.getElementById('disp_total').textContent = dispTotal;
      document.getElementById('transfer_in_total').textContent = tinTotal;
      document.getElementById('transfer_out_total').textContent = toutTotal;
      document.getElementById('current_pendency_criminal').textContent = currentCr;
      document.getElementById('current_pendency_civil').textContent = currentCv;
      document.getElementById('current_pendency_total').textContent = currentTotal;

      const printInstCr = Math.max(0, instCr - tinCr);
      const printInstCv = Math.max(0, instCv - tinCv);
      const printDispCr = Math.max(0, dispCr - toutCr);
      const printDispCv = Math.max(0, dispCv - toutCv);
      const printInstTotal = printInstCr + printInstCv;
      const printDispTotal = printDispCr + printDispCv;

      const pctCr = percentage(printDispCr, printInstCr);
      const pctCv = percentage(printDispCv, printInstCv);
      const pctTotal = percentage(printDispTotal, printInstTotal);

      document.getElementById('print_inst_criminal').textContent = printInstCr;
      document.getElementById('print_inst_civil').textContent = printInstCv;
      document.getElementById('print_inst_total').textContent = printInstTotal;
      document.getElementById('print_disp_criminal').textContent = printDispCr;
      document.getElementById('print_disp_civil').textContent = printDispCv;
      document.getElementById('print_disp_total').textContent = printDispTotal;
      document.getElementById('print_pct_criminal').textContent = formatPercentage(pctCr);
      document.getElementById('print_pct_civil').textContent = formatPercentage(pctCv);
      document.getElementById('print_pct_total').textContent = formatPercentage(pctTotal);

      document.getElementById('targetRequired').textContent = targetRequired(printInstTotal, printDispTotal);

      document.getElementById('print_current_criminal').textContent = currentCr;
      document.getElementById('print_current_civil').textContent = currentCv;
      document.getElementById('print_current_total').textContent = currentTotal;
      document.getElementById('print_transfer_in_criminal').textContent = tinCr;
      document.getElementById('print_transfer_in_civil').textContent = tinCv;
      document.getElementById('print_transfer_in_total').textContent = tinTotal;
      document.getElementById('print_transfer_out_criminal').textContent = toutCr;
      document.getElementById('print_transfer_out_civil').textContent = toutCv;
      document.getElementById('print_transfer_out_total').textContent = toutTotal;
      document.getElementById('print_total_criminal').textContent = currentCr;
      document.getElementById('print_total_civil').textContent = currentCv;
      document.getElementById('print_total_total').textContent = currentTotal;

      saveData();
      if (statusBox) {
        statusBox.textContent = '';
      }
    }

    function bindInputs() {
      if (courtNameInput) {
        courtNameInput.addEventListener('input', () => {
          saveCourtName();
        });
        courtNameInput.addEventListener('change', () => {
          saveCourtName();
        });
      }
      fieldIds.forEach(id => {
        inputs[id].addEventListener('input', (e) => {
          if (e.target.value !== '' && safeNumber(e.target.value) < 0) {
            e.target.value = 0;
          }
          updateTotalsAndPrint();
        });
        inputs[id].addEventListener('change', (e) => {
          if (e.target.value === '') e.target.value = 0;
          updateTotalsAndPrint();
        });
      });
    }

    function showPage(pageId) {
      document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
      document.getElementById(pageId).classList.add('active');
      if (statusBox) {
        statusBox.textContent = '';
      }
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    async function downloadPDF() {
      updateDateTime();
      const element = document.getElementById('printArea');
      const footer = document.querySelector('.pdf-footer');
      footer.style.display = 'block';

      const opt = {
        margin: [0.4, 0.4, 0.4, 0.4],
        filename: 'Pendency_Percentage_Printing_System.pdf',
        image: { type: 'jpeg', quality: 0.98 },
        html2canvas: { scale: 1.0, useCORS: true, scrollY: 0, backgroundColor: '#ffffff' },
        jsPDF: { unit: 'in', format: 'a4', orientation: 'portrait' },
        pagebreak: { mode: ['avoid-all'] }
      };

      try {
        document.body.classList.add('pdf-export');
        if (statusBox) statusBox.textContent = '';
        await html2pdf().set(opt).from(element).save();
        if (statusBox) statusBox.textContent = '';
      } catch (error) {
        console.error(error);
        if (statusBox) statusBox.textContent = '';
      } finally {
        document.body.classList.remove('pdf-export');
        footer.style.display = 'none';
      }
    }

    function resetAll() {
      if (!confirm('Are you sure you want to clear all data?')) return;
      fieldIds.forEach(id => { inputs[id].value = 0; });
      localStorage.removeItem(STORAGE_KEY);
      updateTotalsAndPrint();
      if (statusBox) statusBox.textContent = '';
    }

    document.getElementById('showEditingBtn').addEventListener('click', () => showPage('editingPage'));
    document.getElementById('showPrintingBtn').addEventListener('click', () => { saveCourtName(); updateDateTime(); showPage('printingPage'); });
    document.getElementById('downloadPdfBtn').addEventListener('click', downloadPDF);
    document.getElementById('resetBtn').addEventListener('click', resetAll);

    setMonthName();
    loadCourtName();
    loadData();
    bindInputs();
    updateDateTime();
    updateTotalsAndPrint();
    setInterval(updateDateTime, 1000);
  </script>
</body>
</html>
