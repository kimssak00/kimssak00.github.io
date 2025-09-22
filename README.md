
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Neon Genesis — A3 Landscape · Biological Sample (Left) + Process Panels (Right)</title>
  <style>
    :root{
      --bg:#0a0a0a; --fg:#fff; --dim:rgba(255,255,255,0.64);
      --card:#050505; --border:rgba(255,255,255,0.16);
      --gap:18px; --pad:16px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:var(--bg);color:var(--fg);font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial}

    .a3{aspect-ratio:1189/841; width:100vw; height:100vh; max-height:100dvh; margin:0 auto; display:grid; grid-template-columns:1fr 1fr; gap:var(--gap); padding:var(--gap)}

    .left{position:relative; border:1px solid var(--border); border-radius:14px; overflow:hidden; background:#000}
    .right{display:grid; grid-template-columns:1fr 1fr; grid-template-rows:1fr 1fr; gap:var(--gap)}

    .panel{position:relative; background:var(--card); border:1px solid var(--border); border-radius:14px; overflow:hidden; display:flex; flex-direction:column}
    .head{padding:10px var(--pad) 8px; display:flex; flex-direction:column; gap:4px}
    .title{font-size:12px; font-weight:800; letter-spacing:.1em; text-transform:uppercase}
    .cap{font-size:11px; color:var(--dim)}
    .frame{position:relative; flex:1; background:#000}
    iframe, canvas{position:absolute; inset:0; width:100%; height:100%; border:0; display:block}
    .badge{position:absolute; left:10px; bottom:8px; font-size:10px; color:var(--dim)}
  </style>
</head>
<body>
  <main class="a3">
    <!-- Left: Biological Sample (큰 화면) -->
    <aside class="left">
      <iframe src="neon_genesis_biological_sample copy.html" title="Biological Sample"></iframe>
    </aside>

    <!-- Right: Process Panels (Generation, Cohesion, Branching, Reconfiguration) -->
    <section class="right">
      <!-- 0. Generation (생성) -->
      <article class="panel" id="panel-generation">
        <div class="head">
          <div class="title">Step 0 · Generation (생성)</div>
          <div class="cap">탄생·출현 단계 — 샘플이 태어나고 장에 들어선다</div>
        </div>
        <div class="frame">
          <iframe src="생성.html" title="Generation"></iframe>
          <div class="badge">Mode: spawn cadence & lifetime</div>
        </div>
      </article>

      <!-- 1. Cohesion (응집) -->
      <article class="panel" id="panel-cohesion">
        <div class="head">
          <div class="title">Step 1 · Cohesion (응집)</div>
          <div class="cap">모이는 동작을 강조 — 중앙 응집, 분산 최소화</div>
        </div>
        <div class="frame">
          <iframe src="응집.html" title="Cohesion"></iframe>
          <div class="badge">Rule: cohesion≫alignment, separation↓</div>
        </div>
      </article>

      <!-- 2. Branching (분기) -->
      <article class="panel" id="panel-branching">
        <div class="head">
          <div class="title">Step 2 · Branching (분기)</div>
          <div class="cap">모였다가 다중 군체로 퍼짐 — 빠른 리듬의 분기/합류</div>
        </div>
        <div class="frame">
          <iframe src="분기.html" title="Branching"></iframe>
          <div class="badge">Mode: gather ↔ disperse</div>
        </div>
      </article>

      <!-- 3. Reconfiguration (재구성) -->
      <article class="panel" id="panel-reconfig">
        <div class="head">
          <div class="title">Step 3 · Reconfiguration (재구성)</div>
          <div class="cap">거리 유지 상태에서 네트워크가 연속 변환</div>
        </div>
        <div class="frame">
          <iframe src="재구성.html" title="Reconfiguration"></iframe>
          <div class="badge">Graph: topology morphing</div>
        </div>
      </article>
    </section>
  </main>
</body>
</html>
