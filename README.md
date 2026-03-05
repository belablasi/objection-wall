<!DOCTYPE html>
<!-- saved from url=(0055)file:///Users/belablasi/Downloads/objection-wall-2.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Objection Wall — Indicium AI SKO</title>
<link href="./Objection Wall — Indicium AI SKO_files/css2" rel="stylesheet">
<style>
:root {
  --dark-blue: #1C1D2F;
  --vibrant-blue: #3A58EE;
  --light-blue: #699BFB;
  --lavender: #DEDAF4;
  --atlantic: #AAE2E5;
  --white: #ffffff;
  --card-bg: #23253a;
  --card-border: rgba(58,88,238,0.2);
  --cust-primary: #3A58EE;
  --cust-accent: #699BFB;
  --part-primary: #0fa8b0;
  --part-accent: #AAE2E5;
}
*{margin:0;padding:0;box-sizing:border-box}
body{background:var(--dark-blue);font-family:'Inter',Arial,sans-serif;color:var(--white);min-height:100vh;overflow-x:hidden}
body::before{content:'';position:fixed;inset:0;background-image:linear-gradient(rgba(58,88,238,0.05) 1px,transparent 1px),linear-gradient(90deg,rgba(58,88,238,0.05) 1px,transparent 1px);background-size:40px 40px;pointer-events:none;z-index:0}
body::after{content:'';position:fixed;top:-200px;right:-200px;width:600px;height:600px;background:radial-gradient(circle,rgba(58,88,238,0.15) 0%,transparent 70%);pointer-events:none;z-index:0}
.container{position:relative;z-index:1;max-width:1280px;margin:0 auto;padding:36px 24px 80px}

/* HEADER */
header{display:flex;align-items:center;justify-content:space-between;margin-bottom:40px;padding-bottom:20px;border-bottom:1px solid rgba(105,155,251,0.18)}
.logo-area{display:flex;align-items:center;gap:12px}
.logo-icon{width:36px;height:36px;background:linear-gradient(135deg,var(--vibrant-blue),var(--light-blue));border-radius:8px;display:flex;align-items:center;justify-content:center;font-weight:900;font-size:15px;color:white;flex-shrink:0}
.logo-text{font-size:14px;font-weight:700;letter-spacing:.04em;text-transform:uppercase}
.logo-sub{font-size:10px;color:var(--light-blue);font-family:'Roboto Mono',monospace;letter-spacing:.08em;margin-top:1px}
.header-badge{font-family:'Roboto Mono',monospace;font-size:11px;color:var(--atlantic);background:rgba(170,226,229,0.1);border:1px solid rgba(170,226,229,0.28);padding:5px 12px;border-radius:20px;letter-spacing:.06em;text-transform:uppercase}

/* HERO */
.hero{text-align:center;margin-bottom:36px}
.hero-eyebrow{font-family:'Roboto Mono',monospace;font-size:11px;font-weight:500;color:var(--vibrant-blue);letter-spacing:.15em;text-transform:uppercase;margin-bottom:12px}
.hero h1{font-size:clamp(32px,5vw,58px);font-weight:900;line-height:1;letter-spacing:-.03em;margin-bottom:12px}
.hero h1 span{background:linear-gradient(90deg,var(--vibrant-blue),var(--light-blue),var(--atlantic));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.hero-sub{font-size:15px;color:rgba(222,218,244,.65);max-width:540px;margin:0 auto;line-height:1.6}

/* TIMER */
.timer-wrap{display:flex;flex-direction:column;align-items:center;margin-bottom:40px;gap:12px}
.timer-row{display:flex;align-items:center;gap:20px}
.timer-display{font-family:'Roboto Mono',monospace;font-size:50px;font-weight:700;letter-spacing:.04em;min-width:130px;text-align:center;line-height:1;transition:color .3s}
.timer-display.urgent{color:#ff6b6b}
.timer-display.halfway{color:var(--atlantic)}
.timer-label{font-family:'Roboto Mono',monospace;font-size:10px;color:rgba(222,218,244,.45);text-transform:uppercase;letter-spacing:.12em;text-align:center;margin-top:3px}
.timer-btns{display:flex;flex-direction:column;gap:7px}
.tbtn{font-family:'Roboto Mono',monospace;font-size:11px;font-weight:500;letter-spacing:.07em;text-transform:uppercase;padding:9px 18px;border-radius:6px;border:none;cursor:pointer;transition:all .2s}
.tbtn-start{background:var(--vibrant-blue);color:white}.tbtn-start:hover{background:#2e47d4;transform:translateY(-1px)}
.tbtn-reset{background:transparent;color:var(--lavender);border:1px solid rgba(222,218,244,.25)}.tbtn-reset:hover{border-color:var(--lavender)}
.progress-track{width:100%;max-width:380px;height:3px;background:rgba(255,255,255,.08);border-radius:2px;overflow:hidden}
.progress-fill{height:100%;background:linear-gradient(90deg,var(--vibrant-blue),var(--atlantic));border-radius:2px;transition:width 1s linear;width:100%}

/* TWO LANE INPUT */
.lanes-input{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:32px}
@media(max-width:700px){.lanes-input{grid-template-columns:1fr}}
.lane-input-box{border-radius:14px;padding:22px 24px;position:relative;overflow:hidden}
.lane-input-box::before{content:'';position:absolute;top:0;left:0;right:0;height:3px}
.lane-input-box.customer{background:rgba(58,88,238,0.1);border:1px solid rgba(58,88,238,0.3)}
.lane-input-box.customer::before{background:linear-gradient(90deg,var(--cust-primary),var(--cust-accent))}
.lane-input-box.partner{background:rgba(15,168,176,0.08);border:1px solid rgba(170,226,229,0.3)}
.lane-input-box.partner::before{background:linear-gradient(90deg,var(--part-primary),var(--part-accent))}
.lane-label{display:flex;align-items:center;gap:8px;margin-bottom:14px}
.lane-emoji{font-size:18px}
.lane-title{font-size:13px;font-weight:700;letter-spacing:.06em;text-transform:uppercase}
.lane-input-box.customer .lane-title{color:var(--light-blue)}
.lane-input-box.partner .lane-title{color:var(--atlantic)}
.lane-desc{font-size:11px;font-family:'Roboto Mono',monospace;opacity:.45;margin-left:auto}
.input-row{display:flex;gap:10px}
.table-select{font-family:'Roboto Mono',monospace;font-size:11px;font-weight:500;border:1px solid rgba(255,255,255,.15);color:rgba(255,255,255,.7);padding:10px 10px;border-radius:7px;outline:none;cursor:pointer;letter-spacing:.04em;width:100px;flex-shrink:0;transition:border-color .2s;background:rgba(255,255,255,.05)}
.table-select:focus{border-color:rgba(255,255,255,.4)}
.table-select option{background:var(--dark-blue);color:white}
.obj-input{flex:1;font-family:'Inter',sans-serif;font-size:13px;background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.1);color:var(--white);padding:10px 13px;border-radius:7px;outline:none;transition:border-color .2s}
.obj-input::placeholder{color:rgba(255,255,255,.25)}
.lane-input-box.customer .obj-input:focus{border-color:var(--cust-primary)}
.lane-input-box.partner .obj-input:focus{border-color:var(--part-primary)}
.post-btn{font-family:'Inter',sans-serif;font-size:12px;font-weight:600;border:none;padding:10px 16px;border-radius:7px;cursor:pointer;white-space:nowrap;transition:all .2s;flex-shrink:0}
.lane-input-box.customer .post-btn{background:var(--cust-primary);color:white}.lane-input-box.customer .post-btn:hover{background:#2e47d4}
.lane-input-box.partner .post-btn{background:var(--part-primary);color:white}.lane-input-box.partner .post-btn:hover{background:#0b8a91}

/* STATS */
.stats-row{display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-bottom:28px}
.stat-chip{font-family:'Roboto Mono',monospace;font-size:11px;font-weight:500;padding:6px 13px;border-radius:20px;letter-spacing:.04em}
.stat-chip.total-cust{background:rgba(58,88,238,.18);border:1px solid rgba(58,88,238,.4);color:var(--light-blue)}
.stat-chip.total-part{background:rgba(15,168,176,.15);border:1px solid rgba(170,226,229,.35);color:var(--atlantic)}
.stat-chip.table-tag{background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.12);color:rgba(255,255,255,.55)}

/* WALL */
.wall-section-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:14px;flex-wrap:wrap;gap:8px}
.wall-section-title{display:flex;align-items:center;gap:8px}
.wall-section-label{font-size:11px;font-weight:700;letter-spacing:.12em;text-transform:uppercase;font-family:'Roboto Mono',monospace}
.customer-label{color:var(--light-blue)}.partner-label{color:var(--atlantic)}
.wall-count{font-family:'Roboto Mono',monospace;font-size:11px;font-weight:500;padding:3px 9px;border-radius:12px}
.wall-count.c{background:rgba(58,88,238,.2);color:var(--light-blue);border:1px solid rgba(58,88,238,.35)}
.wall-count.p{background:rgba(15,168,176,.15);color:var(--atlantic);border:1px solid rgba(170,226,229,.3)}
.filter-row{display:flex;gap:5px;flex-wrap:wrap}
.filter-btn{font-family:'Roboto Mono',monospace;font-size:10px;font-weight:500;padding:4px 9px;border-radius:20px;border:1px solid rgba(255,255,255,.13);background:transparent;color:rgba(255,255,255,.4);cursor:pointer;transition:all .2s;letter-spacing:.04em}
.filter-btn.active-c,.fc:hover{background:rgba(58,88,238,.2)!important;border-color:var(--vibrant-blue)!important;color:var(--light-blue)!important}
.filter-btn.active-p,.fp:hover{background:rgba(15,168,176,.15)!important;border-color:var(--part-primary)!important;color:var(--atlantic)!important}

.dual-wall{display:grid;grid-template-columns:1fr 1fr;gap:24px;align-items:start;margin-bottom:40px}
@media(max-width:700px){.dual-wall{grid-template-columns:1fr}}
.cards-wall{display:flex;flex-direction:column;gap:12px}

/* CARD */
.card{background:var(--card-bg);border-radius:11px;padding:16px 18px;position:relative;overflow:hidden;animation:cardIn .3s cubic-bezier(.34,1.56,.64,1) both;transition:transform .2s,box-shadow .2s;border:1px solid var(--card-border);padding-left:22px}
.card:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(0,0,0,.25)}
@keyframes cardIn{from{opacity:0;transform:scale(.85) translateY(8px)}to{opacity:1;transform:scale(1) translateY(0)}}
.card-accent{position:absolute;top:0;left:0;right:0;height:3px}
.card-accent.c{background:linear-gradient(90deg,var(--cust-primary),var(--cust-accent))}
.card-accent.p{background:linear-gradient(90deg,var(--part-primary),var(--part-accent))}
.card::after{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;border-radius:0}
.card.t1::after{background:#3A58EE}.card.t2::after{background:#8b9ff8}.card.t3::after{background:#AAE2E5}
.card.t4::after{background:#699BFB}.card.t5::after{background:#DEDAF4}.card.t6::after{background:#b8aaee}
.card-text{font-size:13px;font-weight:500;line-height:1.55;color:var(--white);margin-bottom:12px}
.card-footer{display:flex;align-items:center;justify-content:space-between}
.card-table-tag{font-family:'Roboto Mono',monospace;font-size:10px;font-weight:500;letter-spacing:.05em;text-transform:uppercase;padding:2px 8px;border-radius:4px;background:rgba(255,255,255,.07);color:rgba(255,255,255,.5)}
.card-actions{display:flex;align-items:center;gap:7px}
.card-vote-btn{background:none;border:1px solid rgba(255,255,255,.13);border-radius:20px;color:rgba(255,255,255,.45);font-size:11px;padding:3px 9px;cursor:pointer;font-family:'Inter',sans-serif;transition:all .2s;display:flex;align-items:center;gap:4px}
.card-vote-btn.voted,.card-vote-btn:hover{border-color:var(--vibrant-blue);color:var(--light-blue);background:rgba(58,88,238,.2)}
.card-delete{background:none;border:none;color:rgba(255,255,255,.18);cursor:pointer;font-size:13px;padding:0 3px;transition:color .2s;line-height:1}
.card-delete:hover{color:#ff6b6b}

.empty-state{text-align:center;padding:48px 16px;color:rgba(222,218,244,.3)}
.empty-icon{font-size:36px;margin-bottom:10px;opacity:.4}
.empty-state p{font-size:13px}

.wall-divider{border:none;border-top:1px solid rgba(105,155,251,.1);margin:8px 0 28px}

/* TOP PANELS */
.top-panels{display:grid;grid-template-columns:1fr 1fr;gap:24px}
@media(max-width:700px){.top-panels{grid-template-columns:1fr}}
.top-panel{padding:22px 24px;border-radius:14px}
.top-panel.cust{background:rgba(58,88,238,.08);border:1px solid rgba(58,88,238,.25)}
.top-panel.part{background:rgba(15,168,176,.07);border:1px solid rgba(170,226,229,.2)}
.top-panel h3{font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:.12em;font-family:'Roboto Mono',monospace;margin-bottom:16px}
.top-panel.cust h3{color:var(--light-blue)}.top-panel.part h3{color:var(--atlantic)}
.top-list{list-style:none;display:flex;flex-direction:column;gap:9px}
.top-item{display:flex;align-items:center;gap:10px;font-size:12px;color:var(--lavender)}
.top-rank{font-family:'Roboto Mono',monospace;font-size:10px;font-weight:700;width:20px;text-align:right;flex-shrink:0}
.top-panel.cust .top-rank{color:var(--cust-primary)}.top-panel.part .top-rank{color:var(--part-primary)}
.top-bar{height:3px;border-radius:2px;flex-shrink:0;transition:width .4s ease}
.top-panel.cust .top-bar{background:linear-gradient(90deg,var(--cust-primary),var(--cust-accent))}
.top-panel.part .top-bar{background:linear-gradient(90deg,var(--part-primary),var(--part-accent))}
.top-votes{font-family:'Roboto Mono',monospace;font-size:10px;flex-shrink:0;margin-left:auto}
.top-panel.cust .top-votes{color:var(--light-blue)}.top-panel.part .top-votes{color:var(--atlantic)}
.top-empty{font-size:12px;color:rgba(255,255,255,.25);font-family:'Roboto Mono',monospace}

@media(max-width:600px){.timer-display{font-size:38px}.input-row{flex-wrap:wrap}.post-btn,.obj-input,.table-select{width:100%}}
</style>
</head>
<body>
<div class="container">

  <header>
    <div class="logo-area">
      <div class="logo-icon">I</div>
      <div>
        <div class="logo-text">Indicium AI</div>
        <div class="logo-sub">Sales Kickoff · FY2026</div>
      </div>
    </div>
    <div class="header-badge">🔥 Live SKO Activity</div>
  </header>

  <div class="hero">
    <div class="hero-eyebrow">☠ Group Exercise</div>
    <h1>The <span>Objection</span> Wall</h1>
    <p class="hero-sub">Brainstorm with your table. Post the hardest objections you hear — from <strong style="color:var(--light-blue)">customers</strong> during the sales cycle and from <strong style="color:var(--atlantic)">partners</strong> during co-sell motions.</p>
  </div>

  <div class="timer-wrap">
    <div class="timer-row">
      <div>
        <div class="timer-display" id="timerDisplay">5:00</div>
        <div class="timer-label">minutes remaining</div>
      </div>
      <div class="timer-btns">
        <button class="tbtn tbtn-start" id="timerBtn" onclick="toggleTimer()">▶ Start</button>
        <button class="tbtn tbtn-reset" onclick="resetTimer()">↺ Reset</button>
      </div>
    </div>
    <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
  </div>

  <!-- DUAL INPUT -->
  <div class="lanes-input">
    <div class="lane-input-box customer">
      <div class="lane-label">
        <span class="lane-emoji">🧑‍💼</span>
        <span class="lane-title">Customer Objection</span>
        <span class="lane-desc">prospects push back on…</span>
      </div>
      <div class="input-row">
        <select class="table-select" id="custTable">
          <option value="1">Table 1</option><option value="2">Table 2</option>
          <option value="3">Table 3</option><option value="4">Table 4</option>
          <option value="5">Table 5</option><option value="6">Table 6</option>
        </select>
        <input class="obj-input" id="custInput" type="text" placeholder="e.g. We already have an internal team…" maxlength="200" onkeydown="if(event.key===&#39;Enter&#39;)addCard(&#39;customer&#39;)">
        <button class="post-btn" onclick="addCard(&#39;customer&#39;)">Post →</button>
      </div>
    </div>
    <div class="lane-input-box partner">
      <div class="lane-label">
        <span class="lane-emoji">🤝</span>
        <span class="lane-title">Partner Objection</span>
        <span class="lane-desc">partners / sellers resist…</span>
      </div>
      <div class="input-row">
        <select class="table-select" id="partTable">
          <option value="1">Table 1</option><option value="2">Table 2</option>
          <option value="3">Table 3</option><option value="4">Table 4</option>
          <option value="5">Table 5</option><option value="6">Table 6</option>
        </select>
        <input class="obj-input" id="partInput" type="text" placeholder="e.g. Databricks has preferred vendors already…" maxlength="200" onkeydown="if(event.key===&#39;Enter&#39;)addCard(&#39;partner&#39;)">
        <button class="post-btn" onclick="addCard(&#39;partner&#39;)">Post →</button>
      </div>
    </div>
  </div>

  <div class="stats-row" id="statsRow"><div class="stat-chip total-cust">2 customer objections</div><div class="stat-chip total-part">2 partner objections</div><div class="stat-chip table-tag">T1: 2</div><div class="stat-chip table-tag">T2: 1</div><div class="stat-chip table-tag">T3: 1</div></div>

  <!-- DUAL WALL -->
  <div class="dual-wall">
    <div>
      <div class="wall-section-header">
        <div class="wall-section-title">
          <span>🧑‍💼</span>
          <span class="wall-section-label customer-label">Customer Objections</span>
          <span class="wall-count c" id="custCount">2</span>
        </div>
        <div class="filter-row" id="custFilterRow">
          <button class="filter-btn fc active-c" onclick="setFilter(&#39;customer&#39;,&#39;all&#39;,this)">All</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;1&#39;,this)">T1</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;2&#39;,this)">T2</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;3&#39;,this)">T3</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;4&#39;,this)">T4</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;5&#39;,this)">T5</button>
          <button class="filter-btn fc" onclick="setFilter(&#39;customer&#39;,&#39;6&#39;,this)">T6</button>
        </div>
      </div>
      <div class="cards-wall" id="custWall"><div class="card t1"><div class="card-accent c"></div><div class="card-text">We already have an internal data team — why do we need you?</div><div class="card-footer"><span class="card-table-tag">Table 1</span><div class="card-actions"><button class="card-vote-btn " onclick="vote(&#39;customer&#39;,1772741686416.9053)">▲ 0</button><button class="card-delete" onclick="deleteCard(&#39;customer&#39;,1772741686416.9053)" title="Remove">✕</button></div></div></div><div class="card t2"><div class="card-accent c"></div><div class="card-text">Your pricing is too high compared to other vendors.</div><div class="card-footer"><span class="card-table-tag">Table 2</span><div class="card-actions"><button class="card-vote-btn " onclick="vote(&#39;customer&#39;,1772741686416.4507)">▲ 0</button><button class="card-delete" onclick="deleteCard(&#39;customer&#39;,1772741686416.4507)" title="Remove">✕</button></div></div></div></div>
    </div>
    <div>
      <div class="wall-section-header">
        <div class="wall-section-title">
          <span>🤝</span>
          <span class="wall-section-label partner-label">Partner Objections</span>
          <span class="wall-count p" id="partCount">2</span>
        </div>
        <div class="filter-row" id="partFilterRow">
          <button class="filter-btn fp active-p" onclick="setFilter(&#39;partner&#39;,&#39;all&#39;,this)">All</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;1&#39;,this)">T1</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;2&#39;,this)">T2</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;3&#39;,this)">T3</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;4&#39;,this)">T4</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;5&#39;,this)">T5</button>
          <button class="filter-btn fp" onclick="setFilter(&#39;partner&#39;,&#39;6&#39;,this)">T6</button>
        </div>
      </div>
      <div class="cards-wall" id="partWall"><div class="card t1"><div class="card-accent p"></div><div class="card-text">Databricks already has preferred partners they push.</div><div class="card-footer"><span class="card-table-tag">Table 1</span><div class="card-actions"><button class="card-vote-btn " onclick="vote(&#39;partner&#39;,1772741686416.8596)">▲ 0</button><button class="card-delete" onclick="deleteCard(&#39;partner&#39;,1772741686416.8596)" title="Remove">✕</button></div></div></div><div class="card t3"><div class="card-accent p"></div><div class="card-text">Why bring in Indicium when we can handle implementation ourselves?</div><div class="card-footer"><span class="card-table-tag">Table 3</span><div class="card-actions"><button class="card-vote-btn " onclick="vote(&#39;partner&#39;,1772741686416.9602)">▲ 0</button><button class="card-delete" onclick="deleteCard(&#39;partner&#39;,1772741686416.9602)" title="Remove">✕</button></div></div></div></div>
    </div>
  </div>

  <hr class="wall-divider">

  <div class="top-panels">
    <div class="top-panel cust">
      <h3>🏆 Top Customer Objections</h3>
      <ul class="top-list" id="custTopList"><li class="top-empty">Vote on cards to surface the biggest ones</li></ul>
    </div>
    <div class="top-panel part">
      <h3>🏆 Top Partner Objections</h3>
      <ul class="top-list" id="partTopList"><li class="top-empty">Vote on cards to surface the biggest ones</li></ul>
    </div>
  </div>

</div>
<script>
let cards={customer:[],partner:[]};
let filters={customer:'all',partner:'all'};
let timerInterval=null,secondsLeft=300,timerRunning=false;
const TOTAL=300;

// Seeds
[
  {lane:'customer',table:'1',text:"We already have an internal data team — why do we need you?"},
  {lane:'customer',table:'2',text:"Your pricing is too high compared to other vendors."},
  {lane:'partner',table:'1',text:"Databricks already has preferred partners they push."},
  {lane:'partner',table:'3',text:"Why bring in Indicium when we can handle implementation ourselves?"},
].forEach(s=>cards[s.lane].push({id:uid(),table:s.table,text:s.text,votes:0,voted:false}));

renderAll();

function uid(){return Date.now()+Math.random()}

function addCard(lane){
  const inp=document.getElementById(lane==='customer'?'custInput':'partInput');
  const tbl=document.getElementById(lane==='customer'?'custTable':'partTable').value;
  const txt=inp.value.trim();
  if(!txt){inp.focus();return;}
  cards[lane].unshift({id:uid(),table:tbl,text:txt,votes:0,voted:false});
  inp.value='';
  renderAll();
}

function deleteCard(lane,id){
  cards[lane]=cards[lane].filter(c=>c.id!==id);
  renderAll();
}

function vote(lane,id){
  const c=cards[lane].find(c=>c.id===id);
  if(!c)return;
  c.voted=!c.voted;
  c.votes+=c.voted?1:-1;
  renderAll();
}

function setFilter(lane,val,btn){
  filters[lane]=val;
  const rowId=lane==='customer'?'custFilterRow':'partFilterRow';
  document.querySelectorAll('#'+rowId+' .filter-btn').forEach(b=>b.classList.remove('active-c','active-p'));
  btn.classList.add(lane==='customer'?'active-c':'active-p');
  renderAll();
}

function renderAll(){
  renderLane('customer');
  renderLane('partner');
  renderStats();
  renderTop();
}

function renderLane(lane){
  const wallId=lane==='customer'?'custWall':'partWall';
  const countId=lane==='customer'?'custCount':'partCount';
  const wall=document.getElementById(wallId);
  const f=filters[lane];
  const filtered=f==='all'?cards[lane]:cards[lane].filter(c=>c.table===f);
  document.getElementById(countId).textContent=cards[lane].length;
  if(!filtered.length){
    wall.innerHTML='<div class="empty-state"><div class="empty-icon">'+(lane==='customer'?'🧑‍💼':'🤝')+'</div><p>No '+lane+' objections posted yet</p></div>';
    return;
  }
  wall.innerHTML=filtered.map(c=>'<div class="card t'+c.table+'"><div class="card-accent '+(lane==='customer'?'c':'p')+'"></div><div class="card-text">'+esc(c.text)+'</div><div class="card-footer"><span class="card-table-tag">Table '+c.table+'</span><div class="card-actions"><button class="card-vote-btn '+(c.voted?'voted':'')+'" onclick="vote(\''+lane+'\','+c.id+')">▲ '+c.votes+'</button><button class="card-delete" onclick="deleteCard(\''+lane+'\','+c.id+')" title="Remove">✕</button></div></div></div>').join('');
}

function renderStats(){
  const row=document.getElementById('statsRow');
  const per={};
  [...cards.customer,...cards.partner].forEach(c=>{per[c.table]=(per[c.table]||0)+1;});
  let h='<div class="stat-chip total-cust">'+cards.customer.length+' customer objection'+(cards.customer.length!==1?'s':'')+'</div>';
  h+='<div class="stat-chip total-part">'+cards.partner.length+' partner objection'+(cards.partner.length!==1?'s':'')+'</div>';
  [1,2,3,4,5,6].forEach(t=>{if(per[t])h+='<div class="stat-chip table-tag">T'+t+': '+per[t]+'</div>';});
  row.innerHTML=h;
}

function renderTop(){
  ['customer','partner'].forEach(lane=>{
    const listId=lane==='customer'?'custTopList':'partTopList';
    const list=document.getElementById(listId);
    const top=[...cards[lane]].filter(c=>c.votes>0).sort((a,b)=>b.votes-a.votes).slice(0,5);
    if(!top.length){list.innerHTML='<li class="top-empty">Vote on cards to surface the biggest ones</li>';return;}
    const maxV=top[0].votes;
    list.innerHTML=top.map((c,i)=>'<li class="top-item"><span class="top-rank">#'+(i+1)+'</span><div class="top-bar" style="width:'+Math.max(20,(c.votes/maxV)*110)+'px"></div><span style="flex:1">'+esc(c.text.length>60?c.text.slice(0,60)+'…':c.text)+'</span><span class="top-votes">▲'+c.votes+'</span></li>').join('');
  });
}

function esc(s){return s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;')}

function toggleTimer(){
  if(timerRunning){clearInterval(timerInterval);timerRunning=false;document.getElementById('timerBtn').textContent='▶ Resume';}
  else{if(secondsLeft<=0){resetTimer();return;}timerRunning=true;document.getElementById('timerBtn').textContent='⏸ Pause';timerInterval=setInterval(()=>{secondsLeft--;updateTimerUI();if(secondsLeft<=0){clearInterval(timerInterval);timerRunning=false;document.getElementById('timerBtn').textContent="⏱ Time's Up!";}},1000);}
}
function resetTimer(){clearInterval(timerInterval);timerRunning=false;secondsLeft=TOTAL;document.getElementById('timerBtn').textContent='▶ Start';updateTimerUI();}
function updateTimerUI(){
  const m=Math.floor(secondsLeft/60),s=secondsLeft%60;
  const d=document.getElementById('timerDisplay');
  d.textContent=m+':'+(String(s).padStart(2,'0'));
  d.className='timer-display'+(secondsLeft<=60?' urgent':secondsLeft<=150?' halfway':'');
  document.getElementById('progressFill').style.width=((secondsLeft/TOTAL)*100)+'%';
}
</script>


</body></html>
