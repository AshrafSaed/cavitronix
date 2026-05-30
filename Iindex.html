<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>CAVITRONIX · Cavitation Tool</title>
<!-- fonts use system stacks only — no external dependency, works fully offline -->
<style>
  :root{
    --bg:#070c16; --panel1:#0e1729; --panel2:#0a111e; --card:#0b1220;
    --line:#16263f; --line2:#1e3a5f; --txt:#e5edff; --mut:#7c8aa3; --mut2:#64748b;
    --teal:#38bdf8; --teal2:#0ea5e9; --violet:#a78bfa;
    --green:#22c55e; --yellow:#eab308; --amber:#f59e0b; --red:#ef4444; --dred:#991b1b;
    --mono:ui-monospace,'SF Mono',Menlo,Consolas,'Liberation Mono',monospace;
  }
  *{box-sizing:border-box}
  body{
    margin:0; min-height:100vh; color:var(--txt);
    font-family:system-ui,-apple-system,'Segoe UI',Roboto,sans-serif;
    background:radial-gradient(1200px 600px at 80% -10%, #11203a 0%, var(--bg) 55%);
    padding:22px 20px 44px;
  }
  input[type=number]::-webkit-outer-spin-button,input[type=number]::-webkit-inner-spin-button{opacity:.4}
  .mono{font-family:var(--mono)}
  .card{background:linear-gradient(180deg,var(--panel1),var(--panel2));border:1px solid var(--line);border-radius:14px;padding:16px 14px 10px}
  /* header */
  header{display:flex;align-items:center;gap:16px;flex-wrap:wrap;margin-bottom:16px;border-bottom:1px solid var(--line);padding-bottom:16px}
  .logo{display:flex;align-items:center;gap:10px;padding:8px 14px;border-radius:12px;border:1px solid var(--line2);
    background:linear-gradient(135deg,var(--panel1),var(--card));box-shadow:0 0 0 1px rgba(56,189,248,.08),0 8px 24px rgba(2,132,199,.18)}
  .logo .m{width:30px;height:30px;border-radius:8px;flex:0 0 auto;background:linear-gradient(135deg,var(--teal),var(--teal2));
    display:grid;place-items:center;color:#06121f;font-weight:900;font-size:18px;font-family:var(--mono);box-shadow:0 4px 12px rgba(2,132,199,.45)}
  .logo .wm{font-size:18px;font-weight:700;letter-spacing:.14em;line-height:1}
  .logo .wm b{color:var(--teal);font-weight:700}
  .logo .sub{font-size:8.5px;font-weight:700;letter-spacing:.34em;color:#5b6b86;margin-top:3px;display:block}
  .title{font-size:22px;font-weight:700;letter-spacing:.04em}
  .title span{color:var(--teal)}
  .subtitle{font-size:12px;color:var(--mut)}
  .owner{font-size:11px;text-align:right;color:#5b6b86;font-family:var(--mono);line-height:1.5}
  /* tabs */
  .tabs{display:flex;gap:8px;margin-bottom:20px;flex-wrap:wrap}
  .tab{cursor:pointer;padding:10px 18px;border-radius:10px;font-size:13.5px;font-weight:700;letter-spacing:.03em;
    border:1px solid var(--line2);background:var(--card);color:var(--mut);transition:all .15s;font-family:inherit}
  .tab.active{border-color:var(--teal);background:linear-gradient(135deg,#0c2236,var(--card));color:var(--teal);
    box-shadow:0 0 0 1px rgba(56,189,248,.3),0 6px 18px rgba(2,132,199,.22)}
  /* analysis layout */
  .analysis{display:grid;grid-template-columns:minmax(280px,340px) 1fr;gap:20px;align-items:start}
  .sectlabel{font-size:12px;letter-spacing:.1em;text-transform:uppercase;color:var(--teal);font-weight:700;margin-bottom:10px}
  .devrow{display:flex;gap:10px;margin-bottom:16px}
  .devbtn{flex:1;cursor:pointer;text-align:left;padding:12px 14px;border-radius:10px;border:1px solid var(--line2);
    background:var(--card);color:var(--txt);transition:all .15s;font-family:inherit}
  .devbtn.active{border-color:var(--teal);background:linear-gradient(135deg,#0c2236,var(--card));
    box-shadow:0 0 0 1px rgba(56,189,248,.3),0 6px 18px rgba(2,132,199,.25)}
  .devbtn .t{font-size:13px;font-weight:700;color:#cdd9ee}
  .devbtn.active .t{color:var(--teal)}
  .devbtn .s{font-size:10px;color:var(--mut2);margin-top:2px}
  .ingrid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
  .fld{display:flex;flex-direction:column;gap:4px}
  .fld.dis{opacity:.4}
  .fld label{font-size:11px;letter-spacing:.08em;text-transform:uppercase;color:#7dd3fc;font-weight:700}
  .fld input{background:var(--card);color:var(--txt);border:1px solid var(--line2);border-radius:8px;padding:9px 11px;
    font-size:15px;font-family:var(--mono);outline:none;width:100%}
  .fld .hint{font-size:10px;color:var(--mut2)}
  .hintbox{margin-top:16px;font-size:11px;color:#5b6b86;line-height:1.7;font-family:var(--mono)}
  .results{display:flex;flex-direction:column;gap:18px}
  .twocol{display:grid;grid-template-columns:1fr 1fr;gap:14px}
  .bigcard{padding:16px}
  .bigcard .lab{font-size:11px;color:var(--mut2);letter-spacing:.08em;text-transform:uppercase;font-weight:700}
  .bigcard .val{font-size:34px;font-weight:700;font-family:var(--mono)}
  .bigcard .st{font-size:14px;font-weight:700}
  .metrics{display:grid;grid-template-columns:repeat(auto-fit,minmax(118px,1fr));gap:10px}
  .metric{background:linear-gradient(180deg,var(--panel1),var(--card));border:1px solid var(--line);border-radius:10px;padding:10px 12px}
  .metric .lab{font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:var(--mut2);font-weight:700}
  .metric .val{font-size:18px;font-weight:700;font-family:var(--mono);margin-top:2px}
  .metric .val u{font-size:11px;color:var(--mut2);font-weight:600;font-style:normal}
  .chartcard .ct{font-size:13px;font-weight:700;margin-bottom:4px}
  .chartcard .ct em{color:var(--teal);font-style:normal}
  .legend{display:flex;flex-wrap:wrap;gap:10px;padding:6px 4px 4px}
  .legend .it{display:flex;align-items:center;gap:6px;font-size:10.5px;color:#9fb0cc}
  .legend .sw{width:12px;height:12px;border-radius:3px;opacity:.7}
  .pvnote{font-size:11px;color:var(--mut);padding:4px 4px 8px;font-family:var(--mono)}
  svg{width:100%;height:auto;display:block}
  /* formulas + converter */
  .twogrid{display:grid;grid-template-columns:1fr 1fr;gap:18px;align-items:start}
  .sect{padding:18px}
  .sect .head{display:flex;align-items:baseline;justify-content:space-between;margin-bottom:12px;flex-wrap:wrap;gap:6px}
  .sect .head .t{font-size:15px;font-weight:700;color:var(--teal);letter-spacing:.04em}
  .sect .head .std{font-size:10px;color:#5b6b86;font-family:var(--mono)}
  .formula{padding:10px 12px;border-radius:10px;background:var(--card);border:1px solid var(--line);margin-bottom:8px}
  .formula .ex{font-family:var(--mono);font-size:15px;color:var(--txt);font-weight:700}
  .formula .de{font-size:11px;color:var(--mut);margin-top:4px}
  table.units{border-collapse:collapse;width:100%;font-size:12.5px}
  table.units th{text-align:left;padding:4px 10px;color:#5b6b86;font-size:10px;text-transform:uppercase}
  table.units td{padding:6px 10px;border-bottom:1px solid var(--line)}
  table.units td.sy{font-family:var(--mono);color:#7dd3fc;font-weight:700}
  table.units td.nm{color:#cdd9ee}
  table.units td.un{font-family:var(--mono);color:var(--txt)}
  .convrow{display:flex;gap:10px;margin-bottom:14px;flex-wrap:wrap}
  .convrow input{flex:1;min-width:120px;background:var(--card);color:var(--txt);border:1px solid var(--line2);border-radius:8px;
    padding:10px 12px;font-size:16px;font-family:var(--mono)}
  .convrow select{background:var(--card);color:#7dd3fc;border:1px solid var(--line2);border-radius:8px;padding:10px 12px;
    font-size:15px;font-family:var(--mono);font-weight:700}
  .convout{display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:8px}
  .convout .c{background:var(--card);border:1px solid var(--line);border-radius:9px;padding:8px 10px}
  .convout .c.on{background:linear-gradient(135deg,#0c2236,var(--card));border-color:var(--teal)}
  .convout .c .u{font-size:10px;color:var(--mut2);text-transform:uppercase;font-weight:700}
  .convout .c .v{font-size:15px;font-weight:700;font-family:var(--mono)}
  .convout .c.on .v{color:var(--teal)}
  .hidden{display:none}
  .printbtn{cursor:pointer;font-family:inherit;font-weight:700;font-size:12.5px;letter-spacing:.03em;
    padding:9px 14px;border-radius:10px;border:1px solid var(--line2);background:var(--card);color:var(--teal)}
  .printbtn:hover{border-color:var(--teal);box-shadow:0 0 0 1px rgba(56,189,248,.3)}
  @media(max-width:880px){.analysis{grid-template-columns:1fr}.twogrid,.twocol{grid-template-columns:1fr}}
  @media print{
    @page{size:A4;margin:10mm}
    html,body{background:#070c16 !important;-webkit-print-color-adjust:exact;print-color-adjust:exact}
    .tabs,.printbtn{display:none !important}
    .card,.chartcard,.metric,.bigcard,.sect{break-inside:avoid;page-break-inside:avoid}
    .analysis{grid-template-columns:300px 1fr}
    body{padding:0}
  }
</style>
</head>
<body>
  <header>
    <div class="logo">
      <span class="m">M</span>
      <span>
        <span class="wm">MIGA<b>TRONIX</b></span>
        <span class="sub">FLOW ENGINEERING</span>
      </span>
    </div>
    <div style="flex:1;min-width:220px">
      <div class="title">CAVITRONIX <span>· Cavitation Tool</span></div>
      <div class="subtitle">Control-valve &amp; orifice cavitation · σ indices · Antoine Pv · unit conversion</div>
    </div>
    <div class="owner">ASHRAF SAED<br>CAVITRONIX AI OWNER</div>
    <button id="printBtn" class="printbtn" title="Print or Save as PDF">⎙ Print / PDF</button>
  </header>
 
  <div class="tabs">
    <button class="tab active" data-tab="analysis">Analysis</button>
    <button class="tab" data-tab="formulas">Formulas &amp; Units</button>
    <button class="tab" data-tab="converter">Unit Converter</button>
  </div>
 
  <!-- ============ ANALYSIS ============ -->
  <div id="tab-analysis" class="analysis">
    <!-- input panel -->
    <div class="card" style="padding:16px">
      <div class="sectlabel">Device Type</div>
      <div class="devrow">
        <button class="devbtn active" data-device="valve">
          <div class="t">◣ Control Valve</div><div class="s">ISA RP75.23 / IEC 60534</div>
        </button>
        <button class="devbtn" data-device="orifice">
          <div class="t">◎ Orifice Plate</div><div class="s">ISO 5167 / Tullis</div>
        </button>
      </div>
 
      <div class="sectlabel">Inputs</div>
      <div class="ingrid">
        <div class="fld"><label>P1 gauge</label><input id="in-P1g" type="number" step="0.1" value="6.0"><span class="hint">upstream · bar(g)</span></div>
        <div class="fld"><label>P2 gauge</label><input id="in-P2g" type="number" step="0.1" value="1.5"><span class="hint">downstream · bar(g)</span></div>
        <div class="fld"><label>Flow Q</label><input id="in-Q" type="number" step="1" min="0" value="40"><span class="hint">flow rate · m³/h</span></div>
        <div class="fld"><label>Temperature</label><input id="in-T" type="number" step="1" value="20"><span class="hint">temperature · °C</span></div>
        <div class="fld"><label>Density ρ</label><input id="in-rho" type="number" step="1" value="998"><span class="hint">density · kg/m³</span></div>
        <div class="fld"><label>Pipe D</label><input id="in-D" type="number" step="1" value="80"><span class="hint">pipe diameter · mm</span></div>
        <div class="fld" id="fld-Kvmax"><label>Kv,max</label><input id="in-Kvmax" type="number" step="1" value="63"><span class="hint">valve · m³/h·bar⁻⁰·⁵</span></div>
        <div class="fld" id="fld-FL"><label>FL</label><input id="in-FL" type="number" step="0.01" value="0.9"><span class="hint">valve · recovery factor</span></div>
        <div class="fld" id="fld-Cd"><label>Cd</label><input id="in-Cd" type="number" step="0.01" value="0.62"><span class="hint">orifice · discharge coeff.</span></div>
        <div class="fld" id="fld-dbore"><label>Bore d</label><input id="in-dbore" type="number" step="1" value="40"><span class="hint">orifice · bore Ø · mm</span></div>
      </div>
      <div class="hintbox" id="hintbox"></div>
    </div>
 
    <!-- results -->
    <div class="results">
      <div class="twocol" id="bigcards"></div>
      <div class="metrics" id="metrics"></div>
 
      <div class="card chartcard">
        <div class="ct" id="ct1"></div>
        <div id="chart1"></div>
        <div class="legend" id="leg1"></div>
      </div>
      <div class="card chartcard">
        <div class="ct" id="ct2"></div>
        <div id="chart2"></div>
        <div class="legend" id="leg2"></div>
      </div>
      <div class="card chartcard">
        <div class="ct">Pv vs Temperature · Antoine (water) — professional curve</div>
        <div id="chart3"></div>
        <div class="pvnote" id="pvnote"></div>
      </div>
    </div>
  </div>
 
  <!-- ============ FORMULAS ============ -->
  <div id="tab-formulas" class="twogrid hidden"></div>
 
  <!-- ============ CONVERTER ============ -->
  <div id="tab-converter" class="twogrid hidden"></div>
 
<script>
/* ===================== constants ===================== */
const ATM_BAR=1.01325, BAR_TO_PA=1e5, G=9.81, PC_WATER_BAR=220.64;
const PSI_PER_BAR=14.5037738, M_H2O_PER_BAR=10.19716213, KV_TO_CV=1.156;
const isNum=x=>typeof x==="number"&&isFinite(x);
const safeDiv=(a,b)=>Math.abs(b)>1e-12?a/b:NaN;
const fmt=(x,d=3)=>isNum(x)?x.toLocaleString("en-US",{minimumFractionDigits:d,maximumFractionDigits:d}):"—";
 
function vaporPressureBarAbs(tC){
  const A=8.07131,B=1730.63,C=233.426;
  const mmHg=Math.pow(10,A-B/(C+tC));
  return mmHg*133.322/BAR_TO_PA;
}
function sigma1Status(s){
  if(!isNum(s))return{label:"Invalid",color:"#9ca3af"};
  if(s>2.0)return{label:"No Cavitation",color:"#22c55e"};
  if(s>1.7)return{label:"Incipient Cavitation",color:"#eab308"};
  if(s>1.3)return{label:"Moderate Cavitation",color:"#f59e0b"};
  if(s>1.0)return{label:"Severe Cavitation",color:"#ef4444"};
  return{label:"Flashing / Evaporation",color:"#991b1b"};
}
function sigma2Status(s){
  if(!isNum(s))return{label:"Invalid",color:"#9ca3af"};
  if(s>4.0)return{label:"No Cavitation",color:"#22c55e"};
  if(s>3.5)return{label:"Incipient Cavitation",color:"#eab308"};
  if(s>2.65)return{label:"Moderate Cavitation",color:"#f59e0b"};
  if(s>2.0)return{label:"Severe Cavitation",color:"#ef4444"};
  return{label:"Flashing / Choked Flow",color:"#991b1b"};
}
const S1_BANDS=[
  {y1:2.0,y2:3.0,color:"#22c55e",label:"No Cavitation  (σ > 2.0)"},
  {y1:1.7,y2:2.0,color:"#eab308",label:"Incipient  (1.7–2.0)"},
  {y1:1.3,y2:1.7,color:"#f59e0b",label:"Moderate  (1.3–1.7)"},
  {y1:1.0,y2:1.3,color:"#ef4444",label:"Severe  (1.0–1.3)"},
  {y1:0.0,y2:1.0,color:"#991b1b",label:"Flashing  (σ ≤ 1.0)"},
];
const S2_BANDS=[
  {y1:4.0,y2:5.5,color:"#22c55e",label:"No Cavitation  (σ > 4.0)"},
  {y1:3.5,y2:4.0,color:"#eab308",label:"Incipient  (3.5–4.0)"},
  {y1:2.65,y2:3.5,color:"#f59e0b",label:"Moderate  (2.65–3.5)"},
  {y1:2.0,y2:2.65,color:"#ef4444",label:"Severe  (2.0–2.65)"},
  {y1:0.0,y2:2.0,color:"#991b1b",label:"Flashing / Choked  (σ ≤ 2.0)"},
];
 
/* ===================== core calc ===================== */
function calcAll(inp){
  const{device,P1g,P2g,Qm3h,tC,rho,Cd,KvMax,Dmm,FL,dBoreMm}=inp;
  const P1abs=P1g+ATM_BAR, P2abs=P2g+ATM_BAR;
  const Pv=vaporPressureBarAbs(tC);
  const dP=P1abs-P2abs, Qm3s=Qm3h/3600;
  const Dm=Dmm>0?Dmm/1000:NaN;
  const Apipe=isNum(Dm)?Math.PI*Dm*Dm/4:NaN;
  const Vpipe=isNum(Apipe)&&Apipe>0?Qm3s/Apipe:NaN;
  const head=rho>0?dP*BAR_TO_PA/(rho*G):NaN;
  // valve
  const Kv=dP>0?Qm3h/Math.sqrt(dP/(rho/1000)):NaN;
  const Cv=isNum(Kv)?Kv*KV_TO_CV:NaN;
  const openingPct=KvMax>0&&isNum(Kv)?Kv/KvMax*100:NaN;
  const FF=0.96-0.28*Math.sqrt(Pv/PC_WATER_BAR);
  const dPchoked=FL>0?FL*FL*(P1abs-FF*Pv):NaN;
  const valveChoked=isNum(dPchoked)?dP>=dPchoked:false;
  const sigmaValve=safeDiv(P1abs-Pv,dP);
  // orifice
  const dBoreM=dBoreMm>0?dBoreMm/1000:NaN;
  const Athroat=isNum(dBoreM)?Math.PI*dBoreM*dBoreM/4:NaN;
  const beta=isNum(Dm)&&isNum(dBoreM)&&Dm>0?dBoreM/Dm:NaN;
  const Vthroat=isNum(Athroat)&&Athroat>0?Qm3s/Athroat:NaN;
  const Aeff=dP>0&&Cd>0&&rho>0?Qm3s/(Cd*Math.sqrt(2*dP*BAR_TO_PA/rho)):NaN;
  const Veff=isNum(Aeff)&&Aeff>0?Qm3s/Aeff:NaN;
  const sigmaOri=isNum(Veff)&&Veff>0?safeDiv((P1abs-Pv)*BAR_TO_PA,0.5*rho*Veff*Veff):NaN;
  const sigmaTullis=safeDiv(P2abs-Pv,dP);
  const s1=sigma1Status(sigmaValve), s2=sigma2Status(sigmaOri);
  const primary=device==="valve"
    ?{sigma:sigmaValve,status:s1,name:"σ — Valve cavitation index (ISA)"}
    :{sigma:sigmaOri,status:s2,name:"σ — Orifice dynamic-pressure index"};
  return{P1abs,P2abs,Pv,dP,Qm3s,Apipe,Vpipe,head,Kv,Cv,openingPct,FF,dPchoked,valveChoked,
    sigmaValve,s1,Athroat,AthroatMm2:isNum(Athroat)?Athroat*1e6:NaN,beta,Vthroat,Aeff,
    AeffMm2:isNum(Aeff)?Aeff*1e6:NaN,Veff,sigmaOri,sigmaTullis,s2,primary};
}
 
/* ===================== SVG chart ===================== */
function chartSVG(o){
  const W=600,H=260,ml=52,mr=18,mt=14,mb=36;
  const pw=W-ml-mr, ph=H-mt-mb;
  const[x0,x1]=o.xDomain,[y0,y1]=o.yDomain;
  const sx=v=>ml+(v-x0)/(x1-x0)*pw;
  const sy=v=>mt+ph-(v-y0)/(y1-y0)*ph;
  let s=`<svg viewBox="0 0 ${W} ${H}" preserveAspectRatio="xMidYMid meet">`;
  // bands
  if(o.bands)for(const b of o.bands){
    const yt=Math.min(b.y2,y1), yb=Math.max(b.y1,y0);
    if(yt<=yb)continue;
    s+=`<rect x="${ml}" y="${sy(yt)}" width="${pw}" height="${sy(yb)-sy(yt)}" fill="${b.color}" opacity="0.13"/>`;
  }
  // grid + ticks
  const xt=o.xTicks||5, ytk=o.yTicks||5;
  for(let i=0;i<=xt;i++){const xv=x0+(x1-x0)*i/xt;const px=sx(xv);
    s+=`<line x1="${px}" y1="${mt}" x2="${px}" y2="${mt+ph}" stroke="#1b2a44" stroke-dasharray="3 3"/>`;
    s+=`<text x="${px}" y="${mt+ph+16}" fill="#5b6b86" font-size="11" text-anchor="middle" font-family="var(--mono)">${(+xv.toFixed(2)).toLocaleString()}</text>`;}
  for(let i=0;i<=ytk;i++){const yv=y0+(y1-y0)*i/ytk;const py=sy(yv);
    s+=`<line x1="${ml}" y1="${py}" x2="${ml+pw}" y2="${py}" stroke="#1b2a44" stroke-dasharray="3 3"/>`;
    s+=`<text x="${ml-8}" y="${py+4}" fill="#5b6b86" font-size="11" text-anchor="end" font-family="var(--mono)">${(+yv.toFixed(2)).toLocaleString()}</text>`;}
  // axis labels
  s+=`<text x="${ml+pw/2}" y="${H-4}" fill="#5b6b86" font-size="11" text-anchor="middle">${o.xLabel||""}</text>`;
  s+=`<text x="14" y="${mt+ph/2}" fill="#5b6b86" font-size="12" text-anchor="middle" transform="rotate(-90 14 ${mt+ph/2})">${o.yLabel||""}</text>`;
  // ref vertical line
  if(isNum(o.refLineX)){const px=sx(o.refLineX);
    s+=`<line x1="${px}" y1="${mt}" x2="${px}" y2="${mt+ph}" stroke="#7dd3fc" stroke-dasharray="5 4"/>`;
    if(o.refLabel)s+=`<text x="${px}" y="${mt-2}" fill="#7dd3fc" font-size="11" text-anchor="middle">${o.refLabel}</text>`;}
  // series polyline (clip to plot)
  const pts=o.data.filter(p=>isNum(p.x)&&isNum(p.y)).map(p=>{
    const cy=Math.max(y0,Math.min(y1,p.y));
    return `${sx(p.x).toFixed(1)},${sy(cy).toFixed(1)}`;}).join(" ");
  s+=`<polyline points="${pts}" fill="none" stroke="${o.color||'#38bdf8'}" stroke-width="2.5" stroke-linejoin="round"/>`;
  // op point
  if(o.op&&isNum(o.op.x)&&isNum(o.op.y)&&o.op.y>=y0&&o.op.y<=y1&&o.op.x>=x0&&o.op.x<=x1){
    s+=`<circle cx="${sx(o.op.x)}" cy="${sy(o.op.y)}" r="6" fill="${o.op.color||'#fff'}" stroke="#fff" stroke-width="1.5"/>`;}
  s+=`</svg>`;
  return s;
}
function legendHTML(bands){
  return bands.map(b=>`<div class="it"><span class="sw" style="background:${b.color}"></span>${b.label}</div>`).join("");
}
 
/* ===================== state + read ===================== */
let device="valve";
const $=id=>document.getElementById(id);
function readInputs(){
  const num=id=>parseFloat($(id).value);
  return{device,
    P1g:num("in-P1g"),P2g:num("in-P2g"),Qm3h:num("in-Q"),tC:num("in-T"),
    rho:num("in-rho"),Cd:num("in-Cd"),KvMax:num("in-Kvmax"),Dmm:num("in-D"),
    FL:num("in-FL"),dBoreMm:num("in-dbore")};
}
 
/* ===================== render analysis ===================== */
function renderAnalysis(){
  const isValve=device==="valve";
  // toggle device buttons + disabled fields
  document.querySelectorAll(".devbtn").forEach(b=>b.classList.toggle("active",b.dataset.device===device));
  $("fld-Kvmax").classList.toggle("dis",!isValve); $("in-Kvmax").disabled=!isValve;
  $("fld-FL").classList.toggle("dis",!isValve);    $("in-FL").disabled=!isValve;
  $("fld-Cd").classList.toggle("dis",isValve);     $("in-Cd").disabled=isValve;
  $("fld-dbore").classList.toggle("dis",isValve);  $("in-dbore").disabled=isValve;
 
  const r=calcAll(readInputs());
 
  // hint box — BOTH formula sets always shown
  const tagV=`<span style="color:${isValve?'#38bdf8':'#5b6b86'};font-weight:700">VALVE${isValve?' · active':''}</span>`;
  const tagO=`<span style="color:${!isValve?'#38bdf8':'#5b6b86'};font-weight:700">ORIFICE${!isValve?' · active':''}</span>`;
  $("hintbox").innerHTML=
    `${tagV} (ISA / IEC 60534)<br>`+
    `σ = (P1abs − Pv) / ΔP<br>Kv = Q·√((ρ/1000)/ΔP) ; Cv = 1.156·Kv<br>`+
    `FF = 0.96 − 0.28·√(Pv/Pc)<br>ΔP_choked = FL²·(P1abs − FF·Pv)<br><br>`+
    `${tagO} (ISO 5167 / Tullis)<br>`+
    `A = π·d²/4 ; β = d/D<br>Aeff = Q/(Cd·√(2ΔP·10⁵/ρ)) ; V = Q/Aeff<br>`+
    `σ = (P1abs − Pv)·10⁵/(0.5·ρ·V²)<br>σ_Tullis = (P2abs − Pv)/ΔP`;
 
  // big cards — BOTH σ indices always shown; active device highlighted
  const pill=on=>on?`<span style="font-size:9px;font-weight:800;letter-spacing:.1em;color:#06121f;background:#38bdf8;border-radius:5px;padding:2px 6px;margin-left:8px;vertical-align:middle">ACTIVE</span>`:"";
  const big=
    `<div class="card bigcard" style="border:1px solid ${isValve?'#38bdf8':'var(--line)'};border-left:4px solid ${r.s1.color};${isValve?'box-shadow:0 0 0 1px rgba(56,189,248,.25)':''}">
       <div class="lab">σ — Valve index (ISA)${pill(isValve)}</div>
       <div class="val" style="color:${r.s1.color}">${fmt(r.sigmaValve,3)}</div>
       <div class="st" style="color:${r.s1.color}">${r.s1.label}</div>
       <div class="mono" style="font-size:11px;color:#9fb0cc;margin-top:6px">σ=(P1−Pv)/ΔP &nbsp;·&nbsp; ΔP_choked=${fmt(r.dPchoked)} bar &nbsp;·&nbsp; <b style="color:${r.valveChoked?'#ef4444':'#22c55e'}">${r.valveChoked?'CHOKED':'not choked'}</b></div>
     </div>`+
    `<div class="card bigcard" style="border:1px solid ${!isValve?'#38bdf8':'var(--line)'};border-left:4px solid ${r.s2.color};${!isValve?'box-shadow:0 0 0 1px rgba(56,189,248,.25)':''}">
       <div class="lab">σ — Orifice index (dynamic)${pill(!isValve)}</div>
       <div class="val" style="color:${r.s2.color}">${fmt(r.sigmaOri,3)}</div>
       <div class="st" style="color:${r.s2.color}">${r.s2.label}</div>
       <div class="mono" style="font-size:11px;color:#9fb0cc;margin-top:6px">σ=(P1−Pv)/(½ρV²) &nbsp;·&nbsp; σ_Tullis=<b style="color:#a78bfa">${fmt(r.sigmaTullis,3)}</b></div>
     </div>`;
  $("bigcards").innerHTML=big;
 
  // metric grid
  const M=(lab,val,unit,color)=>`<div class="metric"><div class="lab">${lab}</div>
    <div class="val" style="${color?`color:${color}`:''}">${val} <u>${unit}</u></div></div>`;
  let mt=
    M("P1 abs",fmt(r.P1abs),"bar a")+M("P2 abs",fmt(r.P2abs),"bar a")+
    M("Pv abs",fmt(r.Pv,4),"bar a","#7dd3fc")+M("ΔP",fmt(r.dP),"bar")+
    M("P2 − Pv",fmt(r.P2abs-r.Pv,3),"bar",(r.P2abs-r.Pv)<=0?'#ef4444':'#22c55e')+
    M("V pipe",fmt(r.Vpipe,2),"m/s")+M("Head loss",fmt(r.head,2),"m");
  if(isValve){
    mt+=M("Kv",fmt(r.Kv,2),"m³/h","#7dd3fc")+M("Cv",fmt(r.Cv,2),"US")+
        M("Opening",fmt(r.openingPct,1),"%")+M("FF",fmt(r.FF,4),"—");
  }else{
    mt+=M("A bore",fmt(r.AthroatMm2,2),"mm²")+M("A eff (Cd)",fmt(r.AeffMm2,2),"mm²")+
        M("V eff",fmt(r.Veff,2),"m/s","#7dd3fc")+M("V throat",fmt(r.Vthroat,2),"m/s")+
        M("β = d/D",fmt(r.beta,3),"—");
  }
  $("metrics").innerHTML=mt;
 
  // chart 1: sigma valve vs dP
  const top1=Math.max(r.dP*2,0.5);
  const d1=[];for(let i=1;i<=120;i++){const dp=top1*i/120;d1.push({x:+dp.toFixed(3),y:(r.P1abs-r.Pv)/dp});}
  $("ct1").innerHTML=`Valve index σ vs ΔP ${isValve?'<em>· active device</em>':''}`;
  $("chart1").innerHTML=chartSVG({data:d1,xDomain:[0,top1],yDomain:[0,3],xLabel:"ΔP [bar]",yLabel:"σ",
    bands:S1_BANDS,op:{x:r.dP,y:r.sigmaValve,color:r.s1.color}});
  $("leg1").innerHTML=legendHTML(S1_BANDS);
 
  // chart 2: sigma orifice vs V
  const vTop=Math.max(isNum(r.Veff)?r.Veff*2:10,2);
  const d2=[];for(let i=1;i<=120;i++){const v=vTop*i/120;d2.push({x:+v.toFixed(3),y:((r.P1abs-r.Pv)*BAR_TO_PA)/(0.5*readInputs().rho*v*v)});}
  $("ct2").innerHTML=`Orifice index σ vs effective velocity ${!isValve?'<em>· active device</em>':''}`;
  $("chart2").innerHTML=chartSVG({data:d2,xDomain:[0,vTop],yDomain:[0,5.5],xLabel:"V eff [m/s]",yLabel:"σ",
    bands:S2_BANDS,op:{x:r.Veff,y:r.sigmaOri,color:r.s2.color}});
  $("leg2").innerHTML=legendHTML(S2_BANDS);
 
  // chart 3: Pv vs T
  const d3=[];for(let t=0;t<=120;t+=2)d3.push({x:t,y:+vaporPressureBarAbs(t).toFixed(5)});
  const tC=readInputs().tC;
  $("chart3").innerHTML=chartSVG({data:d3,xDomain:[0,120],yDomain:[0,2.1],xLabel:"T [°C]",yLabel:"Pv [bar abs]",
    color:"#a78bfa",refLineX:tC,refLabel:`T=${tC}°C`,op:{x:tC,y:r.Pv,color:"#a78bfa"}});
  $("pvnote").innerHTML=`Pv(T=${tC}°C) = ${fmt(r.Pv,5)} bar abs`;
}
 
/* ===================== formulas page ===================== */
function fblock(ex,de){return`<div class="formula"><div class="ex">${ex}</div><div class="de">${de}</div></div>`;}
function sect(t,std,body){return`<div class="card sect"><div class="head"><div class="t">${t}</div><div class="std">${std||''}</div></div>${body}</div>`;}
function renderFormulas(){
  let h="";
  h+=sect("Pressure &amp; Vapor Pressure","—",
    fblock("P_abs = P_gauge + 1.01325","gauge → absolute pressure [bar]")+
    fblock("ΔP = P1_abs − P2_abs","net pressure drop across the device [bar]")+
    fblock("Pv = 10^(A − B/(C+T)) · 133.322 / 10⁵","Antoine, water: A=8.07131, B=1730.63, C=233.426; T in °C → Pv [bar abs]")+
    fblock("h = ΔP·10⁵ / (ρ·g)","head loss [m], g = 9.81 m/s²"));
  h+=sect("Control Valve","ISA RP75.23 · IEC 60534-2-1",
    fblock("σ = (P1_abs − Pv) / ΔP","service cavitation index (dimensionless)")+
    fblock("Kv = Q · √( (ρ/1000) / ΔP )","flow coefficient [m³/h·bar⁻⁰·⁵], Q in m³/h")+
    fblock("Cv = 1.156 · Kv","US flow coefficient [gpm·psi⁻⁰·⁵]")+
    fblock("Opening % = (Kv / Kv,max) · 100","relative valve travel / capacity")+
    fblock("FF = 0.96 − 0.28·√(Pv/Pc)","critical-pressure-ratio factor; Pc(water)=220.64 bar")+
    fblock("ΔP_choked = FL²·(P1_abs − FF·Pv)","choked/flashing when ΔP ≥ ΔP_choked; FL (globe≈0.9, butterfly≈0.6)"));
  h+=sect("Orifice Plate","ISO 5167 · Tullis",
    fblock("A = π·d² / 4 ;  β = d / D","bore area [m²] and diameter ratio (d=bore, D=pipe)")+
    fblock("Q = Cd · A · √(2·ΔP·10⁵ / ρ)","discharge equation; Cd≈0.61 sharp-edged")+
    fblock("A_eff = Q / ( Cd · √(2·ΔP·10⁵/ρ) )","effective (vena-contracta) area [m²]")+
    fblock("V = Q / A_eff","effective throat velocity [m/s]")+
    fblock("σ = (P1_abs − Pv)·10⁵ / (0.5·ρ·V²)","dynamic-pressure cavitation index (dimensionless)")+
    fblock("σ_Tullis = (P2_abs − Pv) / ΔP","downstream-referenced orifice cavitation index"));
  h+=sect("Pipe &amp; Continuity","—",
    fblock("A_pipe = π·D² / 4","pipe cross-section [m²]")+
    fblock("V_pipe = Q / A_pipe","mean pipe velocity [m/s]")+
    fblock("Q[m³/s] = Q[m³/h] / 3600","flow unit base conversion"));
  const u=(sy,nm,un)=>`<tr><td class="sy">${sy}</td><td class="nm">${nm}</td><td class="un">${un}</td></tr>`;
  h+=sect("Symbols &amp; Units","SI / engineering",
    `<table class="units"><thead><tr><th>Symbol</th><th>Quantity</th><th>Unit</th></tr></thead><tbody>`+
    u("P1, P2","Absolute pressures","bar abs")+u("ΔP","Pressure drop","bar")+
    u("Pv","Vapor pressure","bar abs")+u("Q","Volumetric flow","m³/h (m³/s)")+
    u("ρ","Density","kg/m³")+u("T","Temperature","°C")+
    u("D, d","Pipe / bore diameter","mm (m)")+u("A","Area","m² (mm²)")+
    u("V","Velocity","m/s")+u("Kv / Cv","Flow coefficient","m³/h·bar⁻⁰·⁵ / gpm·psi⁻⁰·⁵")+
    u("Cd","Discharge coefficient","—")+u("FL","Pressure-recovery factor","—")+
    u("σ","Cavitation index","—")+u("h","Head loss","m")+u("g","Gravity","9.81 m/s²")+
    `</tbody></table>`);
  $("tab-formulas").innerHTML=h;
}
 
/* ===================== converter page ===================== */
const PRESSURE={
  toBar:{bar:v=>v,kPa:v=>v/100,Pa:v=>v/BAR_TO_PA,MPa:v=>v*10,psi:v=>v/PSI_PER_BAR,mH2O:v=>v/M_H2O_PER_BAR},
  fromBar:{bar:b=>b,kPa:b=>b*100,Pa:b=>b*BAR_TO_PA,MPa:b=>b/10,psi:b=>b*PSI_PER_BAR,mH2O:b=>b*M_H2O_PER_BAR}};
const FLOW={
  toBase:{"m³/h":v=>v,"m³/s":v=>v*3600,"L/s":v=>v*3.6,"L/min":v=>v*0.06,"GPM":v=>v*0.227124707},
  fromBase:{"m³/h":b=>b,"m³/s":b=>b/3600,"L/s":b=>b/3.6,"L/min":b=>b/0.06,"GPM":b=>b/0.227124707}};
const DIAM={toBase:{mm:v=>v,inch:v=>v*25.4},fromBase:{mm:b=>b,inch:b=>b/25.4}};
 
const convState={};
function convBlock(key,title,units,std){
  const opts=units.map(u=>`<option value="${u}">${u}</option>`).join("");
  return sect(title,std,
    `<div class="convrow">
       <input type="number" step="0.1" id="cv-${key}-val" value="1">
       <select id="cv-${key}-unit">${opts}</select>
     </div>
     <div class="convout" id="cv-${key}-out"></div>`);
}
function renderConverter(){
  $("tab-converter").innerHTML=
    convBlock("p","Pressure",["bar","kPa","Pa","MPa","psi","mH2O"],"1 bar = 14.5038 psi = 10.197 mH2O")+
    convBlock("f","Flow rate",["m³/h","m³/s","L/s","L/min","GPM"],"base m³/h · GPM = US gallon/min")+
    convBlock("d","Diameter",["mm","inch"],"1 inch = 25.4 mm")+
    convBlock("t","Temperature",["°C","°F","K"],"°C · °F · K");
  convState.p={units:["bar","kPa","Pa","MPa","psi","mH2O"],map:PRESSURE,dec:4};
  convState.f={units:["m³/h","m³/s","L/s","L/min","GPM"],map:FLOW,dec:4};
  convState.d={units:["mm","inch"],map:DIAM,dec:3};
  convState.t={units:["°C","°F","K"],temp:true,dec:2};
  ["p","f","d","t"].forEach(k=>{
    $(`cv-${k}-val`).addEventListener("input",()=>updateConv(k));
    $(`cv-${k}-unit`).addEventListener("change",()=>updateConv(k));
    updateConv(k);
  });
}
function updateConv(k){
  const cs=convState[k];
  const val=parseFloat($(`cv-${k}-val`).value);
  const unit=$(`cv-${k}-unit`).value;
  let out={};
  if(cs.temp){
    const c=unit==="°C"?val:unit==="°F"?(val-32)*5/9:val-273.15;
    out={"°C":c,"°F":c*9/5+32,"K":c+273.15};
  }else{
    const base=isNum(val)?cs.map.toBase?cs.map.toBase[unit](val):cs.map.toBar[unit](val):NaN;
    const fromFn=cs.map.fromBase||cs.map.fromBar;
    cs.units.forEach(u=>out[u]=fromFn[u](base));
  }
  $(`cv-${k}-out`).innerHTML=cs.units.map(u=>
    `<div class="c ${u===unit?'on':''}"><div class="u">${u}</div><div class="v">${fmt(out[u],cs.dec)}</div></div>`).join("");
}
 
/* ===================== wiring ===================== */
function switchTab(name){
  document.querySelectorAll(".tab").forEach(t=>t.classList.toggle("active",t.dataset.tab===name));
  $("tab-analysis").classList.toggle("hidden",name!=="analysis");
  $("tab-formulas").classList.toggle("hidden",name!=="formulas");
  $("tab-converter").classList.toggle("hidden",name!=="converter");
}
document.querySelectorAll(".tab").forEach(t=>t.addEventListener("click",()=>switchTab(t.dataset.tab)));
document.querySelectorAll(".devbtn").forEach(b=>b.addEventListener("click",()=>{device=b.dataset.device;renderAnalysis();}));
["in-P1g","in-P2g","in-Q","in-T","in-rho","in-Cd","in-Kvmax","in-D","in-FL","in-dbore"]
  .forEach(id=>$(id).addEventListener("input",renderAnalysis));
 
renderAnalysis();
renderFormulas();
renderConverter();
document.getElementById("printBtn").addEventListener("click",()=>window.print());
</script>
</body>
</html>
