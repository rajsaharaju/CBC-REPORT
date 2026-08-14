<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CBC — Verification Report Generator</title>
<style>
  :root{
    --brand-blue:#1F5FA8;
    --brand-blue-dark:#123A66;
    --brand-blue-deep:#0E2E52;
    --brand-green:#6FBE44;
    --bg:#F4F7FB;
    --surface:#FFFFFF;
    --ink:#1B2430;
    --muted:#5B6B7F;
    --border:#DCE3EC;
    --border-strong:#B9C6D6;
    --danger:#C0392B;
    --radius:10px;
    --font-head:Georgia,'Times New Roman',serif;
    --font-body:'Segoe UI',Arial,Helvetica,sans-serif;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    font-family:var(--font-body);
    background:var(--bg);
    color:var(--ink);
    -webkit-font-smoothing:antialiased;
  }
  a{color:inherit;}

  /* ===== Top bar ===== */
  .topbar{
    background:linear-gradient(180deg,var(--brand-blue) 0%, var(--brand-blue-dark) 100%);
    color:#fff;
    padding:14px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:10px;
    position:sticky;
    top:0;
    z-index:50;
    box-shadow:0 2px 10px rgba(14,46,82,0.25);
  }
  .brand{display:flex;align-items:center;gap:12px;}
  .brand-mark{
    width:42px;height:42px;border-radius:50%;
    background:#fff;
    display:flex;align-items:center;justify-content:center;
    font-family:var(--font-head);
    font-weight:700;
    font-size:16px;
    color:var(--brand-blue);
    border:2px solid var(--brand-green);
    flex-shrink:0;
  }
  .brand-text .name{font-family:var(--font-head);font-size:18px;font-weight:700;letter-spacing:.2px;line-height:1.15;}
  .brand-text .tag{font-size:11px;letter-spacing:1.5px;opacity:.85;text-transform:uppercase;}
  .tabs{display:flex;gap:6px;background:rgba(255,255,255,0.12);padding:4px;border-radius:8px;}
  .tab-btn{
    border:none;background:transparent;color:#fff;
    padding:8px 16px;border-radius:6px;font-size:13.5px;font-weight:600;
    cursor:pointer;opacity:.8;transition:.15s;
  }
  .tab-btn.active{background:#fff;color:var(--brand-blue-dark);opacity:1;}
  .tab-btn:hover{opacity:1;}

  .app{max-width:980px;margin:0 auto;padding:22px 16px 80px;}

  /* ===== Section cards ===== */
  .section-card{
    background:var(--surface);
    border:1px solid var(--border);
    border-radius:var(--radius);
    margin-bottom:16px;
    overflow:hidden;
  }
  .section-head{
    padding:13px 18px;
    background:#F0F5FB;
    border-bottom:1px solid var(--border);
    display:flex;
    align-items:center;
    gap:10px;
  }
  .section-num{
    width:24px;height:24px;border-radius:50%;
    background:var(--brand-blue);color:#fff;
    display:flex;align-items:center;justify-content:center;
    font-size:12px;font-weight:700;flex-shrink:0;
  }
  .section-title{font-family:var(--font-head);font-size:15.5px;font-weight:700;color:var(--brand-blue-dark);}
  .section-body{padding:16px 18px 6px;}

  .field-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px 16px;}
  .field-grid.cols-3{grid-template-columns:1fr 1fr 1fr;}
  .field{margin-bottom:12px;}
  .field.full{grid-column:1/-1;}
  .field label{
    display:block;font-size:12px;font-weight:600;color:var(--muted);
    margin-bottom:5px;text-transform:uppercase;letter-spacing:.3px;
  }
  .field input[type=text],
  .field input[type=date],
  .field input[type=time],
  .field input[type=number],
  .field textarea,
  .field select{
    width:100%;padding:9px 11px;border:1px solid var(--border-strong);
    border-radius:6px;font-size:14px;font-family:inherit;color:var(--ink);
    background:#fff;
  }
  .field input:focus,.field textarea:focus,.field select:focus{
    outline:2px solid var(--brand-blue);outline-offset:1px;border-color:var(--brand-blue);
  }
  .field textarea{resize:vertical;min-height:54px;}
  .hint{font-size:11px;color:var(--muted);margin-top:4px;}

  .choice-group{display:flex;flex-wrap:wrap;gap:8px;}
  .choice-group label{
    display:flex;align-items:center;gap:6px;
    font-size:13px;font-weight:500;color:var(--ink);
    text-transform:none;letter-spacing:0;
    background:#F4F7FB;border:1px solid var(--border);
    padding:7px 12px;border-radius:20px;cursor:pointer;
    transition:.12s;margin-bottom:0;
  }
  .choice-group input{accent-color:var(--brand-blue);margin:0;}
  .choice-group label:has(input:checked){
    background:var(--brand-blue);border-color:var(--brand-blue);color:#fff;
  }

  .row-inline{display:flex;gap:12px;flex-wrap:wrap;}
  .row-inline > .field{flex:1;min-width:140px;}

  /* ===== Action bar ===== */
  .action-bar{
    position:sticky;bottom:0;background:var(--surface);
    border-top:1px solid var(--border);
    padding:12px 16px;margin:0 -16px -80px;
    display:flex;gap:10px;flex-wrap:wrap;justify-content:flex-end;
    box-shadow:0 -4px 14px rgba(20,40,70,0.06);
  }
  .btn{
    border:none;border-radius:7px;padding:10px 18px;font-size:13.5px;font-weight:600;
    cursor:pointer;transition:.15s;font-family:inherit;
  }
  .btn-primary{background:var(--brand-blue);color:#fff;}
  .btn-primary:hover{background:var(--brand-blue-dark);}
  .btn-ghost{background:#fff;color:var(--brand-blue);border:1px solid var(--brand-blue);}
  .btn-ghost:hover{background:#EEF4FB;}
  .btn-danger{background:#fff;color:var(--danger);border:1px solid var(--danger);}
  .btn-danger:hover{background:#FBEBEA;}
  .btn-sm{padding:6px 12px;font-size:12.5px;}

  /* ===== History ===== */
  .history-toolbar{display:flex;justify-content:space-between;align-items:center;gap:10px;margin-bottom:14px;flex-wrap:wrap;}
  .history-list{display:flex;flex-direction:column;gap:10px;}
  .history-item{
    background:var(--surface);border:1px solid var(--border);border-radius:var(--radius);
    padding:14px 16px;display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap;
  }
  .history-main .h-name{font-weight:700;font-size:14.5px;color:var(--ink);}
  .history-main .h-meta{font-size:12px;color:var(--muted);margin-top:3px;}
  .history-actions{display:flex;gap:8px;flex-wrap:wrap;}
  .empty-state{
    text-align:center;padding:60px 20px;color:var(--muted);
    background:var(--surface);border:1px dashed var(--border-strong);border-radius:var(--radius);
  }
  .empty-state .big{font-size:32px;margin-bottom:8px;}

  /* ===== Toast ===== */
  .toast{
    position:fixed;bottom:24px;left:50%;transform:translateX(-50%) translateY(20px);
    background:var(--brand-blue-deep);color:#fff;padding:10px 20px;border-radius:8px;
    font-size:13.5px;font-weight:600;opacity:0;pointer-events:none;transition:.25s;z-index:200;
    box-shadow:0 6px 20px rgba(0,0,0,.25);
  }
  .toast.show{opacity:1;transform:translateX(-50%) translateY(0);}

  /* ===== Print view (screen preview of the letterhead report) ===== */
  #printSheet{display:none;}
  .sheet{
    background:#fff;
    max-width:820px;margin:0 auto;
    box-shadow:0 4px 24px rgba(20,40,70,0.12);
    border:1px solid var(--border);
  }
  .letterhead{
    padding:26px 34px 14px;
    display:flex;align-items:center;gap:16px;
    border-bottom:3px solid var(--brand-green);
  }
  .lh-mark{
    width:54px;height:54px;border-radius:50%;
    border:2.5px solid var(--brand-green);
    display:flex;align-items:center;justify-content:center;
    font-family:var(--font-head);font-weight:700;font-size:19px;color:var(--brand-blue);
    flex-shrink:0;
  }
  .lh-text .lh-name{font-family:var(--font-head);font-size:22px;font-weight:700;color:var(--brand-blue);}
  .lh-text .lh-sub{font-size:11px;color:var(--muted);letter-spacing:.5px;text-transform:uppercase;margin-top:2px;}
  .sheet-body{padding:22px 34px 10px;}
  .doc-title{text-align:center;font-family:var(--font-head);font-size:16px;font-weight:700;color:var(--ink);margin-bottom:2px;}
  .doc-sub{text-align:center;font-size:12px;color:var(--muted);margin-bottom:18px;}
  .doc-meta-row{display:flex;justify-content:space-between;font-size:12.5px;margin-bottom:16px;padding:0 4px;}
  .doc-meta-row div span{display:block;font-weight:700;color:var(--ink);}
  .doc-meta-row div small{color:var(--muted);text-transform:uppercase;font-size:10px;letter-spacing:.4px;}

  table.rep-table{width:100%;border-collapse:collapse;margin-bottom:16px;font-size:12.5px;}
  table.rep-table caption{
    text-align:left;font-family:var(--font-head);font-weight:700;font-size:13px;
    color:#fff;background:var(--brand-blue);padding:6px 10px;caption-side:top;
  }
  table.rep-table th, table.rep-table td{
    border:1px solid var(--border-strong);padding:6px 9px;text-align:left;vertical-align:top;
  }
  table.rep-table th{background:#EFF4FA;width:34%;font-weight:600;color:var(--brand-blue-dark);}
  table.rep-table td.ans{font-weight:600;}
  table.rep-table td.chk{width:70px;text-align:center;font-weight:700;color:var(--brand-blue-dark);}

  .stamp{
    display:inline-flex;align-items:center;gap:6px;
    border:2px dashed var(--brand-green);color:var(--brand-blue-dark);
    padding:6px 12px;border-radius:6px;font-weight:700;font-size:11px;
    letter-spacing:1px;text-transform:uppercase;transform:rotate(-3deg);
  }

  .sig-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px;margin:26px 0 10px;font-size:12px;}
  .sig-box{border-top:1px solid var(--ink);padding-top:6px;min-height:44px;}
  .sig-box .sig-label{font-weight:700;}
  .sig-box .sig-sub{color:var(--muted);margin-top:2px;}

  .lh-footer{
    background:var(--brand-blue);color:#fff;font-size:10.5px;
    padding:9px 34px;text-align:center;letter-spacing:.3px;
  }

  .preview-toolbar{max-width:820px;margin:0 auto 14px;display:flex;justify-content:space-between;flex-wrap:wrap;gap:10px;}

  @media (max-width:680px){
    .field-grid, .field-grid.cols-3{grid-template-columns:1fr;}
    .row-inline{flex-direction:column;}
    .sig-grid{grid-template-columns:1fr;}
    .doc-meta-row{flex-direction:column;gap:8px;}
    .sheet-body,.letterhead{padding-left:18px;padding-right:18px;}
  }

  /* ===== Print media ===== */
  @media print{
    body *{visibility:hidden;}
    #printSheet, #printSheet *{visibility:visible;}
    #printSheet{display:block;position:absolute;top:0;left:0;width:100%;}
    .sheet{box-shadow:none;border:none;max-width:100%;}
    .preview-toolbar{display:none;}
    @page{margin:12mm;}
  }
</style>
</head>
<body>

<div class="topbar">
  <div class="brand">
    <div class="brand-mark">CBC</div>
    <div class="brand-text">
      <div class="name">Credit Benevolence Consultancy</div>
      <div class="tag">Verification Report Generator</div>
    </div>
  </div>
  <div class="tabs">
    <button class="tab-btn active" data-tab="form" onclick="switchTab('form')">New Report</button>
    <button class="tab-btn" data-tab="history" onclick="switchTab('history')">History</button>
  </div>
</div>

<div class="app">

  <!-- ============ FORM TAB ============ -->
  <div id="tab-form">

    <div class="section-card">
      <div class="section-head"><div class="section-num">1</div><div class="section-title">Report Reference</div></div>
      <div class="section-body">
        <div class="field-grid cols-3">
          <div class="field">
            <label>Reference / File No.</label>
            <input type="text" id="f_refno" placeholder="CC-72553">
          </div>
          <div class="field">
            <label>Receiving Date</label>
            <input type="date" id="f_recdate">
          </div>
          <div class="field">
            <label>Submission Date</label>
            <input type="date" id="f_subdate">
          </div>
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-head"><div class="section-num">2</div><div class="section-title">Personal Details</div></div>
      <div class="section-body">
        <div class="field-grid">
          <div class="field"><label>Applicant's Name</label><input type="text" id="f_appname"></div>
          <div class="field"><label>Mobile / Land Phone</label><input type="text" id="f_mobile"></div>
          <div class="field full"><label>Current Residence (Address)</label><input type="text" id="f_address"></div>
          <div class="field"><label>Spouse's Name</label><input type="text" id="f_spouse"></div>
          <div class="field"><label>Work Address of Spouse (if any)</label><input type="text" id="f_spousework" placeholder="N/A"></div>
        </div>

        <div class="field full">
          <label>Residential Status</label>
          <div class="choice-group" data-group="f_resstatus">
            <label><input type="radio" name="f_resstatus" value="Family Owned">Family Owned</label>
            <label><input type="radio" name="f_resstatus" value="Owned">Owned</label>
            <label><input type="radio" name="f_resstatus" value="Rented">Rented</label>
            <label><input type="radio" name="f_resstatus" value="Others">Others</label>
          </div>
        </div>

        <div class="field full">
          <label>Residence Size</label>
          <div class="choice-group" data-group="f_ressize">
            <label><input type="radio" name="f_ressize" value="Very Small">Very Small</label>
            <label><input type="radio" name="f_ressize" value="Small">Small</label>
            <label><input type="radio" name="f_ressize" value="Medium">Medium</label>
            <label><input type="radio" name="f_ressize" value="Large">Large</label>
          </div>
        </div>

        <div class="row-inline">
          <div class="field"><label>Years in Current Location</label><input type="number" min="0" id="f_resyears"></div>
          <div class="field"><label>Months</label><input type="number" min="0" max="11" id="f_resmonths"></div>
          <div class="field" style="flex:2"><label>Nearest Landmark</label><input type="text" id="f_landmark" placeholder="N/A"></div>
        </div>

        <div class="field full">
          <label>Behaviour of the Person</label>
          <div class="choice-group" data-group="f_behaviour">
            <label><input type="radio" name="f_behaviour" value="Excellent">Excellent</label>
            <label><input type="radio" name="f_behaviour" value="Good">Good</label>
            <label><input type="radio" name="f_behaviour" value="Suspicious">Suspicious</label>
            <label><input type="radio" name="f_behaviour" value="Bad">Bad</label>
          </div>
        </div>

        <div class="row-inline">
          <div class="field"><label>Person Contacted (Name)</label><input type="text" id="f_contactname" placeholder="Self"></div>
          <div class="field"><label>Contact Date</label><input type="date" id="f_contactdate"></div>
          <div class="field"><label>Contact Time</label><input type="time" id="f_contacttime"></div>
        </div>

        <div class="field full">
          <label>Residence Remarks</label>
          <textarea id="f_resremarks" placeholder="Physically verified &amp; found authentic"></textarea>
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-head"><div class="section-num">3</div><div class="section-title">Employment / Business Details</div></div>
      <div class="section-body">
        <div class="field full">
          <label>Type of Profession</label>
          <div class="choice-group" data-group="f_profession">
            <label><input type="radio" name="f_profession" value="Service">Service</label>
            <label><input type="radio" name="f_profession" value="Business">Business</label>
            <label><input type="radio" name="f_profession" value="Business/Service">Business/Service</label>
            <label><input type="radio" name="f_profession" value="Others">Others (Land Lord, Doctor)</label>
          </div>
        </div>

        <div class="field-grid">
          <div class="field"><label>Company Name</label><input type="text" id="f_company"></div>
          <div class="field"><label>Designation</label><input type="text" id="f_designation"></div>
          <div class="field full"><label>Office Address</label><input type="text" id="f_officeaddr"></div>
          <div class="field"><label>Office Phone (Land)</label><input type="text" id="f_officephone_land"></div>
          <div class="field"><label>Office Phone (Mobile)</label><input type="text" id="f_officephone_mob"></div>
        </div>

        <div class="row-inline">
          <div class="field"><label>Business/Service Length — Years</label><input type="number" min="0" id="f_biz_years"></div>
          <div class="field"><label>Months</label><input type="number" min="0" max="11" id="f_biz_months"></div>
          <div class="field"><label>No. of Employees</label><input type="number" min="0" id="f_employees"></div>
        </div>

        <div class="row-inline">
          <div class="field"><label>LOI Verified By (Name)</label><input type="text" id="f_loiname" list="dl_loiname"></div>
          <div class="field"><label>Designation</label><input type="text" id="f_loidesig" list="dl_loidesig"></div>
        </div>

        <div class="field-grid">
          <div class="field"><label>Nature of Business</label><input type="text" id="f_natureofbiz"></div>
          <div class="field">
            <label>Service Status</label>
            <div class="choice-group" data-group="f_servicestatus">
              <label><input type="radio" name="f_servicestatus" value="Permanent">Permanent</label>
              <label><input type="radio" name="f_servicestatus" value="Contractual">Contractual</label>
            </div>
          </div>
        </div>

        <div class="field full"><label>Salary Remark (for serviceman)</label><input type="text" id="f_salaryremark" placeholder="OK"></div>

        <div class="field full">
          <label>Business Place Status</label>
          <div class="choice-group" data-group="f_bizstatus">
            <label><input type="radio" name="f_bizstatus" value="Rented">Rented</label>
            <label><input type="radio" name="f_bizstatus" value="Owned">Owned</label>
            <label><input type="radio" name="f_bizstatus" value="Company Owned">Company Owned</label>
          </div>
        </div>

        <div class="field full">
          <label>Business Place Size</label>
          <div class="choice-group" data-group="f_bizsize">
            <label><input type="radio" name="f_bizsize" value="Very Small">Very Small</label>
            <label><input type="radio" name="f_bizsize" value="Small">Small</label>
            <label><input type="radio" name="f_bizsize" value="Medium">Medium</label>
            <label><input type="radio" name="f_bizsize" value="Large">Large</label>
          </div>
        </div>

        <div class="field full">
          <label>Business / Office Signboard</label>
          <div class="choice-group" data-group="f_signboard">
            <label><input type="radio" name="f_signboard" value="Small">Small</label>
            <label><input type="radio" name="f_signboard" value="Medium">Medium</label>
            <label><input type="radio" name="f_signboard" value="Large">Large</label>
            <label><input type="radio" name="f_signboard" value="No Signboard">No Signboard</label>
          </div>
        </div>

        <div class="field full">
          <label>Location Convenience</label>
          <div class="choice-group" data-group="f_convenience">
            <label><input type="radio" name="f_convenience" value="Easy">Easy</label>
            <label><input type="radio" name="f_convenience" value="Little Difficult">Little Difficult</label>
            <label><input type="radio" name="f_convenience" value="Difficult">Difficult</label>
            <label><input type="radio" name="f_convenience" value="Unable to locate">Unable to locate</label>
          </div>
        </div>

        <div class="field full">
          <label>General Remarks</label>
          <textarea id="f_generalremarks" placeholder="CPV-OK   LOI-OK   B/S-N/A"></textarea>
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-head"><div class="section-num">4</div><div class="section-title">References</div></div>
      <div class="section-body">
        <div class="field-grid cols-3">
          <div class="field"><label>1st Reference — Name</label><input type="text" id="f_ref1name"></div>
          <div class="field"><label>Relationship</label><input type="text" id="f_ref1rel"></div>
          <div class="field"><label>Mobile No.</label><input type="text" id="f_ref1mobile"></div>
        </div>
        <div class="field-grid cols-3">
          <div class="field"><label>2nd Reference — Name</label><input type="text" id="f_ref2name"></div>
          <div class="field"><label>Relationship</label><input type="text" id="f_ref2rel"></div>
          <div class="field"><label>Mobile No.</label><input type="text" id="f_ref2mobile"></div>
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-head"><div class="section-num">5</div><div class="section-title">Field Agent</div></div>
      <div class="section-body">
        <div class="field-grid cols-3">
          <div class="field"><label>Field Agent's Name</label><input type="text" id="f_agentname" list="dl_agentname"></div>
          <div class="field"><label>Agent Sign Date</label><input type="date" id="f_agentdate"></div>
        </div>
      </div>
    </div>

    <datalist id="dl_loiname"></datalist>
    <datalist id="dl_loidesig"></datalist>
    <datalist id="dl_agentname"></datalist>

  </div>

  <!-- ============ HISTORY TAB ============ -->
  <div id="tab-history" style="display:none;">
    <div class="history-toolbar">
      <div style="font-size:13px;color:var(--muted);">Saved reports are stored in this browser only.</div>
      <div style="display:flex;gap:8px;">
        <button class="btn btn-ghost btn-sm" onclick="exportHistory()">Export JSON</button>
        <label class="btn btn-ghost btn-sm" style="cursor:pointer;margin:0;">
          Import JSON
          <input type="file" accept=".json" onchange="importHistory(event)" style="display:none;">
        </label>
      </div>
    </div>
    <div class="history-list" id="historyList"></div>
  </div>

</div>

<!-- ============ ACTION BAR (form tab only) ============ -->
<div class="action-bar" id="actionBar">
  <button class="btn btn-ghost" onclick="clearForm(true)">New / Clear</button>
  <button class="btn btn-ghost" onclick="saveReport()">Save to History</button>
  <button class="btn btn-primary" onclick="openPreview()">Preview &amp; Print</button>
</div>

<!-- ============ PRINT / PREVIEW SHEET ============ -->
<div id="previewView" style="display:none;">
  <div class="app" style="padding-top:22px;">
    <div class="preview-toolbar">
      <button class="btn btn-ghost" onclick="closePreview()">&larr; Back to Edit</button>
      <button class="btn btn-primary" onclick="window.print()">Print / Save as PDF</button>
    </div>
  </div>

  <div id="printSheet" style="display:block;">
    <div class="sheet">
      <div class="letterhead">
        <div class="lh-mark">CBC</div>
        <div class="lh-text">
          <div class="lh-name">Credit Benevolence Consultancy</div>
          <div class="lh-sub">Field Verification &amp; Advisory Services</div>
        </div>
      </div>

      <div class="sheet-body">
        <div class="doc-title">Verification Report</div>
        <div class="doc-sub">Meghna Bank PLC. — Retail Banking Division — Credit Card Solution</div>

        <div class="doc-meta-row">
          <div><small>Reference No.</small><span id="p_refno">—</span></div>
          <div><small>Receiving Date</small><span id="p_recdate">—</span></div>
          <div><small>Submission Date</small><span id="p_subdate">—</span></div>
        </div>

        <table class="rep-table">
          <caption>Personal Details — Verified &amp; Found Authentic</caption>
          <tbody id="p_personal"></tbody>
        </table>

        <table class="rep-table">
          <caption>Employment / Business Details — Verified &amp; Found Authentic</caption>
          <tbody id="p_employment"></tbody>
        </table>

        <table class="rep-table">
          <caption>Reference Details</caption>
          <tbody id="p_references"></tbody>
        </table>

        <div style="text-align:right;margin:14px 0 6px;"><span class="stamp">✓ Field Verified</span></div>

        <div class="sig-grid">
          <div class="sig-box"><div class="sig-label">Team Leader</div><div class="sig-sub">Seal &amp; Sign — Date: ____________</div></div>
          <div class="sig-box"><div class="sig-label">Manager</div><div class="sig-sub">Seal &amp; Sign — Date: ____________</div></div>
          <div class="sig-box"><div class="sig-label" id="p_agentname">Field Agent</div><div class="sig-sub">Sign — Date: <span id="p_agentdate">____________</span></div></div>
        </div>
      </div>

      <div class="lh-footer">
        18/15, Azam Road, (Ground Floor) Block-D, Mohammadpur, Dhaka-1207, Mob: 01911572579, 01747823232, 01832265816, E-mail: intcbc30@gmail.com
      </div>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
const FIELD_IDS = [
  'f_refno','f_recdate','f_subdate',
  'f_appname','f_mobile','f_address','f_spouse','f_spousework',
  'f_resyears','f_resmonths','f_landmark',
  'f_contactname','f_contactdate','f_contacttime','f_resremarks',
  'f_company','f_designation','f_officeaddr','f_officephone_land','f_officephone_mob',
  'f_biz_years','f_biz_months','f_employees','f_loiname','f_loidesig',
  'f_natureofbiz','f_salaryremark','f_generalremarks',
  'f_ref1name','f_ref1rel','f_ref1mobile','f_ref2name','f_ref2rel','f_ref2mobile',
  'f_agentname','f_agentdate'
];
const RADIO_GROUPS = [
  'f_resstatus','f_ressize','f_behaviour','f_profession','f_servicestatus',
  'f_bizstatus','f_bizsize','f_signboard','f_convenience'
];
const REMEMBER_KEYS = ['f_loiname','f_loidesig','f_agentname']; // fields whose last value auto-fills next time
const STORAGE_KEY = 'cbc_reports_v1';
const LASTVALS_KEY = 'cbc_lastvalues_v1';
const REFNO_KEY = 'cbc_lastrefno_v1';

let editingId = null; // if set, "Save" updates this history entry instead of creating new

function todayISO(){
  const d = new Date();
  return d.toISOString().slice(0,10);
}
function nowTimeStr(){
  const d = new Date();
  return d.toTimeString().slice(0,5);
}
function fmtDateHuman(iso){
  if(!iso) return '—';
  const [y,m,d] = iso.split('-');
  if(!y) return iso;
  return `${d}.${m}.${y.slice(2)}`;
}

function switchTab(tab){
  document.getElementById('tab-form').style.display = tab==='form' ? 'block' : 'none';
  document.getElementById('actionBar').style.display = tab==='form' ? 'flex' : 'none';
  document.getElementById('tab-history').style.display = tab==='history' ? 'block' : 'none';
  document.querySelectorAll('.tab-btn').forEach(b=>b.classList.toggle('active', b.dataset.tab===tab));
  if(tab==='history') renderHistory();
}

function showToast(msg){
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  clearTimeout(showToast._tm);
  showToast._tm = setTimeout(()=>t.classList.remove('show'), 2200);
}

function getRadioValue(name){
  const el = document.querySelector(`input[name="${name}"]:checked`);
  return el ? el.value : '';
}
function setRadioValue(name, value){
  document.querySelectorAll(`input[name="${name}"]`).forEach(el=>{
    el.checked = (el.value === value);
  });
}

function collectForm(){
  const data = {};
  FIELD_IDS.forEach(id=>{
    const el = document.getElementById(id);
    data[id] = el ? el.value : '';
  });
  RADIO_GROUPS.forEach(name=>{ data[name] = getRadioValue(name); });
  return data;
}
function fillForm(data){
  FIELD_IDS.forEach(id=>{
    const el = document.getElementById(id);
    if(el) el.value = data[id] || '';
  });
  RADIO_GROUPS.forEach(name=>{ setRadioValue(name, data[name] || ''); });
}

function nextRefNo(){
  const last = localStorage.getItem(REFNO_KEY);
  if(!last) return '';
  const m = last.match(/^(.*?)(\d+)$/);
  if(!m) return '';
  const prefix = m[1];
  const num = (parseInt(m[2],10) + 1).toString().padStart(m[2].length,'0');
  return prefix + num;
}

function clearForm(isNew){
  document.querySelectorAll('#tab-form input[type=text], #tab-form textarea').forEach(el=>el.value='');
  document.querySelectorAll('#tab-form input[type=radio]').forEach(el=>el.checked=false);
  document.querySelectorAll('#tab-form input[type=number]').forEach(el=>el.value='');
  editingId = null;

  if(isNew){
    document.getElementById('f_recdate').value = todayISO();
    document.getElementById('f_subdate').value = todayISO();
    document.getElementById('f_contactdate').value = todayISO();
    document.getElementById('f_contacttime').value = nowTimeStr();
    document.getElementById('f_agentdate').value = todayISO();

    const lastvals = JSON.parse(localStorage.getItem(LASTVALS_KEY) || '{}');
    REMEMBER_KEYS.forEach(id=>{
      const el = document.getElementById(id);
      if(el && lastvals[id]) el.value = lastvals[id];
    });

    const suggestedRef = nextRefNo();
    if(suggestedRef) document.getElementById('f_refno').value = suggestedRef;

    showToast('New report ready — dates auto-filled');
  } else {
    document.getElementById('f_recdate').value = '';
    document.getElementById('f_subdate').value = '';
  }
}

function refreshDatalists(){
  const lastvals = JSON.parse(localStorage.getItem(LASTVALS_KEY) || '{}');
  const history = getHistory();
  const pool = { f_loiname:new Set(), f_loidesig:new Set(), f_agentname:new Set() };
  history.forEach(r=>{
    if(r.data.f_loiname) pool.f_loiname.add(r.data.f_loiname);
    if(r.data.f_loidesig) pool.f_loidesig.add(r.data.f_loidesig);
    if(r.data.f_agentname) pool.f_agentname.add(r.data.f_agentname);
  });
  Object.keys(pool).forEach(id=>{
    const dl = document.getElementById('dl_' + id.replace('f_',''));
    if(dl) dl.innerHTML = [...pool[id]].map(v=>`<option value="${escapeHtml(v)}">`).join('');
  });
}

function escapeHtml(str){
  return String(str).replace(/[&<>"']/g, c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
}

function getHistory(){
  return JSON.parse(localStorage.getItem(STORAGE_KEY) || '[]');
}
function setHistory(list){
  localStorage.setItem(STORAGE_KEY, JSON.stringify(list));
}

function saveReport(){
  const data = collectForm();
  if(!data.f_appname){
    showToast('Applicant\'s Name is needed before saving');
    return;
  }
  const history = getHistory();

  // remember last-used values for auto-fill next time
  const lastvals = JSON.parse(localStorage.getItem(LASTVALS_KEY) || '{}');
  REMEMBER_KEYS.forEach(id=>{ if(data[id]) lastvals[id] = data[id]; });
  localStorage.setItem(LASTVALS_KEY, JSON.stringify(lastvals));
  if(data.f_refno) localStorage.setItem(REFNO_KEY, data.f_refno);

  if(editingId){
    const idx = history.findIndex(r=>r.id===editingId);
    if(idx>-1){
      history[idx].data = data;
      history[idx].savedAt = new Date().toISOString();
    }
  } else {
    editingId = 'r' + Date.now();
    history.unshift({ id: editingId, data, savedAt: new Date().toISOString() });
  }
  setHistory(history);
  refreshDatalists();
  showToast('Report saved to history');
}

function renderHistory(){
  const list = getHistory();
  const container = document.getElementById('historyList');
  if(list.length===0){
    container.innerHTML = `<div class="empty-state"><div class="big">🗂️</div>No saved reports yet.<br>Fill the form and hit "Save to History".</div>`;
    return;
  }
  container.innerHTML = list.map(r=>{
    const d = r.data;
    const saved = new Date(r.savedAt);
    return `
      <div class="history-item">
        <div class="history-main">
          <div class="h-name">${escapeHtml(d.f_appname || '(No name)')}</div>
          <div class="h-meta">Ref: ${escapeHtml(d.f_refno || '—')} &nbsp;·&nbsp; Submitted: ${fmtDateHuman(d.f_subdate)} &nbsp;·&nbsp; Saved ${saved.toLocaleDateString()}</div>
        </div>
        <div class="history-actions">
          <button class="btn btn-ghost btn-sm" onclick="loadReport('${r.id}')">Open / Edit</button>
          <button class="btn btn-ghost btn-sm" onclick="duplicateReport('${r.id}')">Duplicate</button>
          <button class="btn btn-danger btn-sm" onclick="deleteReport('${r.id}')">Delete</button>
        </div>
      </div>`;
  }).join('');
}

function loadReport(id){
  const history = getHistory();
  const r = history.find(x=>x.id===id);
  if(!r) return;
  fillForm(r.data);
  editingId = id;
  switchTab('form');
  showToast('Report loaded — edits will update this entry');
}

function duplicateReport(id){
  const history = getHistory();
  const r = history.find(x=>x.id===id);
  if(!r) return;
  fillForm(r.data);
  editingId = null;
  document.getElementById('f_recdate').value = todayISO();
  document.getElementById('f_subdate').value = todayISO();
  const suggestedRef = nextRefNo();
  if(suggestedRef) document.getElementById('f_refno').value = suggestedRef;
  switchTab('form');
  showToast('Duplicated as a new report — update the details and save');
}

function deleteReport(id){
  if(!confirm('Delete this report from history? This cannot be undone.')) return;
  let history = getHistory();
  history = history.filter(x=>x.id!==id);
  setHistory(history);
  renderHistory();
  showToast('Report deleted');
}

function exportHistory(){
  const data = localStorage.getItem(STORAGE_KEY) || '[]';
  const blob = new Blob([data], {type:'application/json'});
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url;
  a.download = 'cbc-reports-backup.json';
  a.click();
  URL.revokeObjectURL(url);
}
function importHistory(event){
  const file = event.target.files[0];
  if(!file) return;
  const reader = new FileReader();
  reader.onload = e=>{
    try{
      const imported = JSON.parse(e.target.result);
      if(!Array.isArray(imported)) throw new Error('bad format');
      const existing = getHistory();
      const existingIds = new Set(existing.map(r=>r.id));
      const merged = existing.concat(imported.filter(r=>!existingIds.has(r.id)));
      setHistory(merged);
      renderHistory();
      refreshDatalists();
      showToast('Import complete');
    }catch(err){
      showToast('Could not read that file');
    }
  };
  reader.readAsText(file);
  event.target.value = '';
}

/* ===== Preview / Print ===== */
function rowHtml(label, value, verified){
  const chk = verified===false ? '' : (value ? '<td class="chk">✓ Yes</td>' : '<td class="chk">—</td>');
  return `<tr><th>${escapeHtml(label)}</th><td class="ans">${escapeHtml(value || '—')}</td>${chk}</tr>`;
}

function buildPreview(){
  const d = collectForm();

  document.getElementById('p_refno').textContent = d.f_refno || '—';
  document.getElementById('p_recdate').textContent = fmtDateHuman(d.f_recdate);
  document.getElementById('p_subdate').textContent = fmtDateHuman(d.f_subdate);

  const resYearsMonths = [
    d.f_resyears ? `${d.f_resyears} yr` : '', d.f_resmonths ? `${d.f_resmonths} mo` : ''
  ].filter(Boolean).join(' ');
  const contact = [d.f_contactname, fmtDateHuman(d.f_contactdate), d.f_contacttime].filter(Boolean).join(' · ');

  document.getElementById('p_personal').innerHTML = [
    rowHtml("Applicant's Name", d.f_appname),
    rowHtml("Current Residence", d.f_address),
    rowHtml("Mobile / Land Phone", d.f_mobile),
    rowHtml("Spouse's Name", d.f_spouse),
    rowHtml("Work Address of Spouse", d.f_spousework),
    rowHtml("Residential Status", d.f_resstatus),
    rowHtml("Residence Size", d.f_ressize),
    rowHtml("Years in Current Location", resYearsMonths),
    rowHtml("Nearest Landmark", d.f_landmark),
    rowHtml("Behaviour of the Person", d.f_behaviour),
    rowHtml("Person Contacted", contact),
    rowHtml("Residence Remarks", d.f_resremarks),
  ].join('');

  const bizYearsMonths = [
    d.f_biz_years ? `${d.f_biz_years} yr` : '', d.f_biz_months ? `${d.f_biz_months} mo` : '',
    d.f_employees ? `${d.f_employees} employees` : ''
  ].filter(Boolean).join(' · ');
  const officePhone = [d.f_officephone_land, d.f_officephone_mob].filter(Boolean).join(' / ');
  const loi = [d.f_loiname, d.f_loidesig].filter(Boolean).join(' — ');

  document.getElementById('p_employment').innerHTML = [
    rowHtml("Type of Profession", d.f_profession),
    rowHtml("Company Name", d.f_company),
    rowHtml("Office Address", d.f_officeaddr),
    rowHtml("Office Phone", officePhone),
    rowHtml("Business/Service Length", bizYearsMonths),
    rowHtml("LOI Verified By", loi),
    rowHtml("Nature of Business", d.f_natureofbiz),
    rowHtml("Designation", d.f_designation),
    rowHtml("Service Status", d.f_servicestatus),
    rowHtml("Salary Remark", d.f_salaryremark),
    rowHtml("Business Place Status", d.f_bizstatus),
    rowHtml("Business Place Size", d.f_bizsize),
    rowHtml("Business/Office Signboard", d.f_signboard),
    rowHtml("Location Convenience", d.f_convenience),
    rowHtml("General Remarks", d.f_generalremarks, false),
  ].join('');

  document.getElementById('p_references').innerHTML = [
    rowHtml("1st Reference — Name", d.f_ref1name),
    rowHtml("Relationship / Mobile", [d.f_ref1rel, d.f_ref1mobile].filter(Boolean).join(' · '), false),
    rowHtml("2nd Reference — Name", d.f_ref2name),
    rowHtml("Relationship / Mobile", [d.f_ref2rel, d.f_ref2mobile].filter(Boolean).join(' · '), false),
  ].join('');

  document.getElementById('p_agentname').textContent = d.f_agentname ? `Field Agent — ${d.f_agentname}` : 'Field Agent';
  document.getElementById('p_agentdate').textContent = fmtDateHuman(d.f_agentdate);
}

function openPreview(){
  buildPreview();
  document.querySelector('.app').style.display = 'none';
  document.getElementById('actionBar').style.display = 'none';
  document.querySelector('.topbar').style.display = 'none';
  document.getElementById('previewView').style.display = 'block';
}
function closePreview(){
  document.querySelector('.app').style.display = 'block';
  document.getElementById('actionBar').style.display = 'flex';
  document.querySelector('.topbar').style.display = 'flex';
  document.getElementById('previewView').style.display = 'none';
}

/* ===== Init ===== */
window.addEventListener('DOMContentLoaded', ()=>{
  refreshDatalists();
  clearForm(true);
});
</script>

</body>
</html>
