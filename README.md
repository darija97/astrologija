[index.html](https://github.com/user-attachments/files/31123486/index.html)
<!DOCTYPE html>
<html lang="me">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Danica | Tvoja zvijezda vodilja</title>
<meta name="description" content="Tarot i gledanje u šolju. Pisano lično za tebe, s pažnjom i povjerenjem.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Marcellus&family=Playfair+Display:wght@500&family=Source+Sans+3:wght@400;600&display=swap&subset=latin-ext" rel="stylesheet">
<style>
:root{
  --night:#0b1120; --night2:#101a2e; --night3:#16233c;
  --text:#ded2c4; --head:#f2e9db; --muted:#8b95a8;
  --gold:#b99a4a; --gold2:#d4b96a; --plumline:rgba(185,154,74,.22);
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{font-family:'Source Sans 3',sans-serif;font-weight:400;background:var(--night);color:var(--text);line-height:1.7;font-size:16.5px}
h1,h2,h3{font-family:'Marcellus',serif;color:var(--head);font-weight:400;line-height:1.22;letter-spacing:.015em}
.wrap{max-width:1060px;margin:0 auto;padding:0 24px}
.kicker{font-size:12px;letter-spacing:.35em;text-transform:uppercase;color:var(--gold);font-weight:600}
.btn{display:inline-block;padding:14px 34px;border:1px solid var(--gold);background:transparent;color:var(--gold2);border-radius:999px;
  font-family:'Source Sans 3',sans-serif;font-weight:600;font-size:14px;letter-spacing:.12em;text-transform:uppercase;
  cursor:pointer;text-decoration:none;transition:.25s}
.btn:hover{background:var(--gold);color:var(--night)}
.btn.solid{background:var(--gold);color:var(--night)}
.btn.solid:hover{background:var(--gold2);border-color:var(--gold2)}

nav{position:sticky;top:0;background:rgba(11,17,32,.92);backdrop-filter:blur(8px);border-bottom:1px solid var(--plumline);z-index:50}
nav .wrap{display:flex;align-items:center;justify-content:space-between;height:68px}
.logo{font-family:'Marcellus',serif;font-size:27px;color:var(--head);text-decoration:none;letter-spacing:.04em}
.logo span{color:var(--gold)}
nav ul{display:flex;gap:26px;list-style:none}
nav ul a{color:var(--text);text-decoration:none;font-size:13px;letter-spacing:.14em;text-transform:uppercase}
nav ul a:hover{color:var(--gold2)}
@media(max-width:900px){nav ul{display:none}}

.hero{position:relative;padding:130px 0 120px;text-align:center;overflow:hidden;
  background:radial-gradient(ellipse 90% 70% at 50% -10%, #1c2c4d 0%, var(--night) 65%)}
.dial{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:min(880px,150vw);aspect-ratio:1;pointer-events:none}
.hero .wrap{position:relative}
.stars{position:absolute;inset:0;pointer-events:none;background-image:
  radial-gradient(1px 1px at 12% 28%, rgba(222,210,196,.8) 50%, transparent 51%),
  radial-gradient(1px 1px at 78% 18%, rgba(222,210,196,.6) 50%, transparent 51%),
  radial-gradient(1.5px 1.5px at 32% 62%, rgba(212,185,106,.7) 50%, transparent 51%),
  radial-gradient(1px 1px at 64% 44%, rgba(222,210,196,.5) 50%, transparent 51%),
  radial-gradient(1px 1px at 88% 66%, rgba(212,185,106,.5) 50%, transparent 51%),
  radial-gradient(1.5px 1.5px at 45% 12%, rgba(222,210,196,.7) 50%, transparent 51%),
  radial-gradient(1px 1px at 22% 82%, rgba(222,210,196,.4) 50%, transparent 51%),
  radial-gradient(1px 1px at 55% 78%, rgba(212,185,106,.45) 50%, transparent 51%)}
.hero h1{font-family:'Playfair Display',serif;font-weight:500;font-size:clamp(74px,13vw,150px);line-height:1.02;margin:14px auto 20px;letter-spacing:.01em}
.hero p.sub{font-size:18px;color:var(--muted);max-width:540px;margin:0 auto}
.cta-row{display:flex;gap:16px;justify-content:center;flex-wrap:wrap}
.hero .cta-row .btn{border-radius:999px;padding:15px 38px;min-width:272px;text-align:center}
@media(max-width:640px){.hero .cta-row .btn{min-width:0;width:100%}}
.moons{display:flex;align-items:center;justify-content:center;gap:14px;margin:36px auto 42px}
.moons::before,.moons::after{content:'';height:1px;width:64px;background:var(--plumline)}
.moon{width:19px;height:19px;border-radius:50%;border:1px solid rgba(212,185,106,.75);flex:none}
.moon.m2{background:linear-gradient(90deg,transparent 50%,var(--head) 50%)}
.moon.m3{background:linear-gradient(90deg,transparent 28%,var(--head) 28%)}
.moon.m4{background:var(--head)}
.moon.m5{background:linear-gradient(90deg,var(--head) 72%,transparent 72%)}
.moon.m6{background:linear-gradient(90deg,var(--head) 50%,transparent 50%)}

.strip{border-top:1px solid var(--plumline);border-bottom:1px solid var(--plumline);background:var(--night2);padding:20px 0}
.strip .wrap{display:flex;justify-content:center;gap:10px 46px;flex-wrap:wrap;font-size:13px;letter-spacing:.1em;text-transform:uppercase;color:var(--muted)}
.strip b{color:var(--gold2);font-weight:600}

section{padding:96px 0}
section h2{font-size:clamp(28px,3.4vw,40px);margin:14px 0 12px}
.lead{color:var(--muted);font-size:17px;max-width:600px;margin-bottom:52px}
.center{text-align:center}.center .lead{margin-left:auto;margin-right:auto}
.rule{width:56px;height:1px;background:var(--gold);opacity:.7;margin:22px 0}
.center .rule{margin-left:auto;margin-right:auto}

/* SERVICES AS MENU */
.cards{display:grid;grid-template-columns:repeat(2,1fr);gap:24px}
@media(max-width:600px){.cards{grid-template-columns:1fr}}
.card{background:var(--night2);border:1px solid var(--plumline);border-radius:20px;padding:38px 32px;display:flex;flex-direction:column;transition:background .3s}
.card:hover{background:var(--night3)}
.card svg{width:32px;height:32px;stroke:var(--gold);fill:none;stroke-width:1.3;margin-bottom:18px}
.card h3{font-size:23px;margin-bottom:16px}
.menu{list-style:none;margin-bottom:22px;flex:1}
.menu li{display:flex;justify-content:space-between;align-items:baseline;gap:12px;
  padding:9px 0;border-bottom:1px dotted rgba(185,154,74,.3);font-size:14px}
.menu li span:first-child{color:var(--text)}
.menu li span:last-child{font-family:'Marcellus',serif;color:var(--gold2);white-space:nowrap}
.card .btn{align-self:flex-start;padding:10px 24px;font-size:12px}

#kako{background:var(--night2);border-top:1px solid var(--plumline);border-bottom:1px solid var(--plumline)}
.steps{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:40px}
.step .n{font-family:'Marcellus',serif;font-size:54px;color:var(--gold);opacity:.85;line-height:1}
.step h3{font-size:20px;margin:12px 0 8px}
.step p{font-size:15px;color:var(--muted)}

.upload-box{border:1px solid var(--plumline);border-radius:20px;background:var(--night2);padding:48px 38px;text-align:center;max-width:560px;margin:0 auto}
.cup-grid{display:grid;grid-template-columns:1fr 1fr;gap:24px;align-items:stretch;max-width:920px;margin:0 auto}
@media(max-width:760px){.cup-grid{grid-template-columns:1fr}}
.cup-grid .upload-box{max-width:none;margin:0;display:flex;flex-direction:column;justify-content:center}
.cup-art{border:1px solid var(--plumline);border-radius:20px;background:var(--night2);padding:34px 32px;display:flex;flex-direction:column;align-items:center}
.cup-art svg{width:150px;margin-bottom:14px}
.symlist{list-style:none;width:100%;text-align:left}
.symlist li{display:flex;justify-content:space-between;gap:14px;padding:9px 0;border-bottom:1px dotted rgba(185,154,74,.3);font-size:14px}
.symlist li span:first-child{font-family:'Marcellus',serif;color:var(--gold2)}
.symlist li span:last-child{color:var(--muted);text-align:right}
.upload-box img{max-width:200px;margin:20px auto;display:block;border:1px solid var(--plumline)}
.note{font-size:13px;color:var(--muted);margin-top:16px}

/* TAROT */
#tarot{background:radial-gradient(ellipse 70% 80% at 50% 120%, #1c2c4d 0%, var(--night) 70%)}
.tarot-row{display:flex;gap:26px;justify-content:center;flex-wrap:wrap;margin:10px 0 30px}
.tslot{display:flex;flex-direction:column;align-items:center;gap:14px}
.tslot .pos-top{font-size:12px;letter-spacing:.26em;text-transform:uppercase;color:var(--gold2)}
.tcard{width:210px;height:355px;perspective:1000px;cursor:pointer}
@media(max-width:720px){.tcard{width:150px;height:254px}}
.tcard .inner{position:relative;width:100%;height:100%;transition:transform .7s;transform-style:preserve-3d}
.tcard.flipped .inner{transform:rotateY(180deg)}
.tface{position:absolute;inset:0;backface-visibility:hidden;border:1px solid var(--gold);border-radius:16px;display:flex;
  flex-direction:column;align-items:center;justify-content:center;padding:14px;text-align:center}
.tback{background:linear-gradient(160deg,#14213a,#0d1526);justify-content:space-around}
.tback::before{content:'';position:absolute;inset:9px;border:1px solid rgba(185,154,74,.4);border-radius:11px}
.tback .mini{color:var(--gold);opacity:.8;letter-spacing:20px;font-size:13px;text-indent:20px}
.tback .big{color:var(--gold2);font-size:46px;text-shadow:0 0 22px rgba(212,185,106,.9),0 0 64px rgba(212,185,106,.45)}
.fan{display:flex;justify-content:center;margin:6px 0 34px;min-height:140px}
.fcard{width:76px;height:124px;border:1px solid var(--gold);border-radius:9px;margin-left:-40px;cursor:pointer;
  background:linear-gradient(160deg,#14213a,#0d1526);position:relative;transition:transform .25s, box-shadow .25s}
.fcard:first-child{margin-left:0}
.fcard::after{content:'\2726';position:absolute;inset:0;display:flex;align-items:center;justify-content:center;
  color:var(--gold2);font-size:20px;text-shadow:0 0 12px rgba(212,185,106,.8)}
.fcard:hover{transform:translateY(-16px);box-shadow:0 14px 28px rgba(0,0,0,.5);z-index:5}
.fcard.gone{visibility:hidden;pointer-events:none}
.slot-empty{width:100%;height:100%;border:1px dashed rgba(185,154,74,.4);border-radius:16px;display:flex;
  align-items:center;justify-content:center;color:var(--muted);font-size:13px;letter-spacing:.1em}
.tcta{display:none;margin:34px auto 0;max-width:640px;border:1px solid var(--plumline);border-radius:24px;
  padding:40px 36px;background:var(--night2)}
.tcta h3{font-size:26px;margin-bottom:10px}
.tcta p{color:var(--muted);font-size:15.5px;margin-bottom:24px}
.tcta-row{display:flex;gap:14px;justify-content:center;flex-wrap:wrap}
.pillbtn{padding:15px 32px;border-radius:999px;border:none;background:var(--gold);color:var(--night);
  font-family:'Source Sans 3',sans-serif;font-weight:600;font-size:13px;letter-spacing:.14em;text-transform:uppercase;cursor:pointer}
.pillbtn:hover{background:var(--gold2)}
.pillghost{padding:15px 32px;border-radius:999px;border:1px solid var(--plumline);color:var(--muted);
  font-size:13px;letter-spacing:.14em;text-transform:uppercase}
.tfront{background:var(--night2);transform:rotateY(180deg);padding:0;overflow:hidden}
.tfront img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
.tfront .tlabel{position:absolute;left:0;right:0;bottom:0;padding:34px 10px 10px;background:linear-gradient(transparent,rgba(7,11,20,.95) 65%);z-index:2}
.tfront .rn{font-family:'Marcellus',serif;color:var(--gold);font-size:15px;letter-spacing:.2em}
.tfront .tname{font-family:'Marcellus',serif;color:var(--head);font-size:21px;margin:8px 0}
.tfront .pos{font-size:11px;letter-spacing:.22em;text-transform:uppercase;color:var(--muted)}
.tmeanings{max-width:640px;margin:0 auto;text-align:left}
.tmeanings p{border-left:1px solid var(--gold);padding:2px 0 2px 18px;margin-bottom:14px;font-size:15.5px;color:var(--text)}
.tmeanings p b{font-family:'Marcellus',serif;color:var(--gold2);font-weight:400}
.tsummary{max-width:640px;margin:30px auto 0;border:1px solid var(--gold);border-radius:20px;background:var(--night2);padding:32px 34px;text-align:center}
.tsummary p{margin-top:12px;font-size:16px;color:var(--text);line-height:1.75}


#odanici .wrap{display:grid;grid-template-columns:.75fr 1.25fr;gap:56px;align-items:center}
@media(max-width:860px){#odanici .wrap{grid-template-columns:1fr}}
.sigil{aspect-ratio:1;border:1px solid var(--plumline);border-radius:50%;display:flex;align-items:center;justify-content:center;position:relative}
.sigil::before{content:'';position:absolute;inset:14px;border:1px solid var(--plumline);border-radius:50%}
.story{font-size:16.5px;color:var(--text)}
.story em{font-family:'Marcellus',serif;font-style:normal;font-size:21px;color:var(--gold2)}
.story .sig{font-family:'Marcellus',serif;font-size:22px;color:var(--head);letter-spacing:.03em}

#iskustva{border-bottom:1px solid var(--plumline)}
.quotes{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:22px}
.q{border:1px solid var(--plumline);border-radius:20px;padding:32px 28px;background:var(--night2)}
.q p{font-family:'Marcellus',serif;font-size:17.5px;color:var(--text);line-height:1.55}
.q .who{margin-top:18px;font-size:12px;letter-spacing:.16em;text-transform:uppercase;color:var(--gold)}

details{border-bottom:1px solid var(--plumline);padding:20px 4px;max-width:720px;margin:0 auto}
summary{font-family:'Marcellus',serif;font-size:20px;color:var(--head);cursor:pointer;list-style:none}
summary::-webkit-details-marker{display:none}
summary::after{content:'+';float:right;color:var(--gold);font-size:22px}
details[open] summary::after{content:'\2013'}
details p{margin-top:12px;font-size:15px;color:var(--muted)}

footer{padding:56px 0 36px;font-size:13.5px;color:var(--muted)}
footer .disclaimer{border-top:1px solid var(--plumline);margin-top:26px;padding-top:22px;font-size:12.5px;line-height:1.8}

/* ORDER FORM MODAL */
.modal-bg{position:fixed;inset:0;background:rgba(5,9,18,.85);display:none;align-items:center;justify-content:center;z-index:100;padding:20px;overflow-y:auto}
.modal-bg.open{display:flex}
.modal{background:var(--night2);border:1px solid var(--plumline);border-radius:20px;padding:40px 38px;max-width:520px;width:100%}
.modal h3{font-size:25px;margin:10px 0 6px}
.mclose{position:absolute;top:10px;right:18px;color:var(--muted);font-size:28px;cursor:pointer;line-height:1}
.mclose:hover{color:var(--gold2)}
.modal .sub2{font-size:14px;color:var(--muted);margin-bottom:24px}
.field{margin-bottom:16px;text-align:left}
.field label{display:block;font-size:12px;letter-spacing:.14em;text-transform:uppercase;color:var(--gold);margin-bottom:6px}
.field input,.field select,.field textarea{width:100%;padding:12px 14px;border:1px solid var(--plumline);
  background:var(--night);color:var(--text);font-size:15px;font-family:inherit;color-scheme:dark}
.field textarea{min-height:96px;resize:vertical}
.themes{display:flex;gap:10px;flex-wrap:wrap}
.themes label{display:inline-flex;align-items:center;gap:7px;font-size:14px;color:var(--text);
  border:1px solid var(--plumline);padding:8px 14px;cursor:pointer;letter-spacing:0;text-transform:none}
.themes input{width:auto}
.modal .close{position:absolute;margin-top:-26px;margin-left:calc(100% - 18px);color:var(--muted);cursor:pointer;font-size:20px}
#formOk{display:none;text-align:center;padding:20px 0}
#formOk .star{color:var(--gold);font-size:30px}
</style>
</head>
<body>

<nav>
  <div class="wrap">
    <a class="logo" href="#">Danica<span>&#10022;</span></a>
    <ul>
      <li><a href="#usluge">Ponuda</a></li>
      <li><a href="#kako">Kako do usluge?</a></li>
      <li><a href="#tarot">Tarot</a></li>
      <li><a href="#odanici">O Danici</a></li>
      <li><a href="#iskustva">Iskustva</a></li>
    </ul>
    <a class="btn" style="padding:9px 20px;font-size:11px" href="#usluge">Zatraži čitanje</a>
  </div>
</nav>

<header class="hero">
  <div class="stars"></div>
  <svg class="dial" viewBox="0 0 800 800" aria-hidden="true">
    <circle cx="400" cy="400" r="296" fill="none" stroke="#b99a4a" stroke-opacity=".18" stroke-width="1"/>
    <g id="dialTicks" stroke="#b99a4a" stroke-opacity=".5" stroke-width="1.6"></g>
  </svg>
  <div class="wrap">
    <div class="kicker">Tarot &middot; Gledanje u šolju</div>
    <h1>Danica</h1>
    <p class="sub">Karte i šolja odavno znaju ono što ti se plete oko srca. Mi to samo pročitamo za tebe, kao nekada, s pažnjom i povjerenjem.</p>
    <div class="moons" aria-hidden="true">
      <span class="moon m1"></span><span class="moon m2"></span><span class="moon m3"></span><span class="moon m4"></span><span class="moon m5"></span><span class="moon m6"></span><span class="moon m7"></span>
    </div>
    <div class="cta-row">
      <a class="btn solid" href="#usluge">Zatraži svoje čitanje</a>
      <a class="btn" href="#tarot">Otvori karte besplatno</a>
    </div>
  </div>
</header>

<div class="strip">
  <div class="wrap">
    <div>Odgovor u roku od <b>24 do 72 sata</b></div>
    <div>Diskrecija <b>bez izuzetka</b></div>
    <div>Iza svakog čitanja <b>stručni tim</b></div>
    <div>Pisano <b>samo za tebe</b></div>
  </div>
</div>

<section id="usluge">
  <div class="wrap">
    <div class="kicker">Ponuda</div>
    <h2>Izaberi svoje čitanje</h2>
    <div class="rule"></div>
    <p class="lead">Svako čitanje nastaje za jedno srce i jedno pitanje. Bez šablona.</p>
    <div class="cards">
      <div class="card">
        <svg viewBox="0 0 24 24"><path d="M4 9h13v5a6 6 0 0 1-6.5 6A6 6 0 0 1 4 14V9z"/><path d="M17 10c3-.5 5 1 4.5 3.5S18 17 16.5 16.5"/><path d="M8 6c-1-1.2.6-1.8.2-3M11.5 5.5c-1-1.2.6-1.8.2-3"/></svg>
        <h3>Gledanje u šolju</h3>
        <ul class="menu">
          <li><span>Pisano tumačenje sa simbolima</span><span>9 &euro;</span></li>
          <li><span>Uz Daničinu glasovnu poruku</span><span>15 &euro;</span></li>
        </ul>
        <button class="btn" onclick="openOrder('Gledanje u šolju')">Naruči</button>
      </div>
      <div class="card">
        <svg viewBox="0 0 24 24"><rect x="7" y="3" width="10" height="16" rx="1"/><path d="M12 8l1.2 2.4L16 11l-2.4 1.2L12 15l-1.2-2.8L8 11l2.8-.6L12 8z" stroke-width="1"/><path d="M4 6l1.5 14"/><path d="M20 6l-1.5 14"/></svg>
        <h3>Tarot</h3>
        <ul class="menu">
          <li><span>Karte za tvoj dan &middot; tri karte</span><span>besplatno</span></li>
          <li><span>Detaljno otvaranje s tumačenjem</span><span>15 &euro;</span></li>
        </ul>
        <a class="btn" href="#tarot">Otvori karte</a>
      </div>
    </div>
  </div>
</section>

<section id="kako">
  <div class="wrap center">
    <div class="kicker">Postupak</div>
    <h2>Kako funkcioniše</h2>
    <div class="rule"></div>
    <p class="lead">Tri koraka, ni jedan više. Sve završiš s telefona dok ti se kafa hladi.</p>
    <div class="steps">
      <div class="step">
        <div class="n">I</div>
        <h3>Izaberi čitanje</h3>
        <p>Šolja ili karte. Ono što ti sada treba.</p>
      </div>
      <div class="step">
        <div class="n">II</div>
        <h3>Podijeli s nama</h3>
        <p>Datum rođenja, tvoje pitanje ili slika šolje. I par riječi o tome šta želiš da protumačimo.</p>
      </div>
      <div class="step">
        <div class="n">III</div>
        <h3>Primi svoje čitanje</h3>
        <p>U roku od 24 do 72 sata stiže ti čitanje pisano samo za tebe. Na mejl, samo tebi.</p>
      </div>
    </div>
  </div>
</section>

<section id="solja">
  <div class="wrap center">
    <div class="kicker">Proba</div>
    <h2>Slikaj svoju šolju</h2>
    <div class="rule"></div>
    <p class="lead">Skuvaj kafu bez filtera, popij je polako, pa okreni šolju na tacnu. Kad se talog slije, slikaj iznutra uz dobro svjetlo.</p>
    <div class="cup-grid">
      <div class="cup-art">
        <svg viewBox="0 0 140 120" fill="none" stroke="#b99a4a" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M56 10c-4 6 4 9 0 16" opacity=".7"/>
          <path d="M74 8c-4 7 4 10 0 17" opacity=".7"/>
          <path d="M36 38h58v16c0 18-13 30-29 30S36 72 36 54V38z"/>
          <path d="M94 44c11-3 18 3 16 11s-11 10-17 8"/>
          <path d="M46 50c4 4 10 3 13-1M62 62c5 3 11 1 13-3" opacity=".8"/>
          <path d="M72 48l2 4 4 1-4 1-2 4-2-4-4-1 4-1 2-4z" fill="#b99a4a" stroke="none" opacity=".9"/>
          <ellipse cx="65" cy="96" rx="42" ry="5"/>
          <ellipse cx="65" cy="104" rx="28" ry="3.5" opacity=".6"/>
        </svg>
        <ul class="symlist">
          <li><span>Ptica</span><span>vijest koja stiže izdaleka</span></li>
          <li><span>Srce</span><span>ljubav, nova ili probuđena</span></li>
          <li><span>Put</span><span>promjena koja se već sprema</span></li>
          <li><span>Riba</span><span>dobitak i napredak</span></li>
        </ul>
        <p class="note">Ovo je tek zrno iz Daničinog rječnika simbola. Svaka šolja priča svoju priču.</p>
      </div>
      <div class="upload-box">
        <input type="file" id="cupPhoto" accept="image/*" style="display:none" onchange="previewCup(event)">
        <button class="btn" onclick="document.getElementById('cupPhoto').click()">Izaberi fotografiju</button>
        <div id="cupPreview"></div>
        <p class="note">Prototip: fotografija ostaje u tvom pretraživaču i nigdje se ne šalje. U pravoj verziji stiže direktno kod Danice i briše se nakon 30 dana.</p>
      </div>
    </div>
  </div>
</section>

<section id="tarot">
  <div class="wrap center">
    <div class="kicker">Besplatno</div>
    <h2>Tvoje karte za danas</h2>
    <div class="rule"></div>
    <p class="lead">Karte su promiješane za današnji dan. Izvuci tri iz lepeze i okreni ih jednu po jednu kad budeš spremna. Kad okreneš sve tri, ispod te čeka i kratak opis tvog dana.</p>
    <div class="fan" id="fanRow"></div>
    <div class="tarot-row" id="tarotRow"></div>
    <div class="tmeanings" id="tarotMeanings"></div>
    <div id="tarotSummary" class="tsummary" style="display:none">
      <div class="kicker">Tvoj dan, ukratko</div>
      <p id="tarotSummaryText"></p>
    </div>
    <div id="tarotCta" class="tcta">
      <h3>Karte su ti nešto poručile.</h3>
      <p>Ako želiš da ti Danica pročita dan do kraja, uz tvoje pitanje i lični osvrt, naruči detaljno čitanje.</p>
      <div class="tcta-row">
        <button class="pillbtn" onclick="openOrder('Tarot: detaljno otvaranje')">Naruči detaljno čitanje &middot; 15 &euro;</button>
        <span class="pillghost">Nove karte te čekaju sjutra &#10022;</span>
      </div>
    </div>
  </div>
</section>

<section id="odanici">
  <div class="wrap">
    <div class="sigil">
      <svg width="120" height="120" viewBox="0 0 100 100">
        <path d="M50 6l6 32 32 6-32 6-6 32-6-32-32-6 32-6 6-32z" fill="none" stroke="#b99a4a" stroke-width="1.2"/>
        <circle cx="50" cy="50" r="10" fill="none" stroke="#b99a4a" stroke-width="1" opacity=".7"/>
      </svg>
    </div>
    <div class="story">
      <div class="kicker">O Danici</div>
      <h2>Ime koje se pamti prije interneta</h2>
      <div class="rule"></div>
      <p><em>Prije nego što su postojale razne aplikacije, postojala je zvijezda Danica. Posljednja koja se gasi pred zoru, ona koja je vodila putnike kući.</em></p>
      <br>
      <p>I postojala je uvijek jedna Danica u komšiluku. Žena kojoj si nosila šolju i srce, i od koje si odlazila lakša. Naša Danica je ta ista zvijezda i ta ista žena, samo što je sada uvijek tu, gdje god da si.</p>
      <br>
      <p>Iza imena Danica danas stoji mali, posvećen tim. Žene koje ovaj zanat nose iz kuće i uče ga godinama. Nijedno čitanje ne kreće ka tebi bez naše potpune posvećenosti. Bez straha, bez prijetnji, bez "skidanja uroka". Ozbiljno, pošteno i tebi u korist.</p>
      <br>
      <p class="sig">Danica. Tvoja zvijezda vodilja.</p>
    </div>
  </div>
</section>

<section id="iskustva">
  <div class="wrap center">
    <div class="kicker">Iskustva</div>
    <h2>Šta kažu žene koje su probale</h2>
    <div class="rule"></div>
    <p class="lead">Prava imena, pravi gradovi.</p>
    <div class="quotes">
      <div class="q">
        <p>„Iskreno, naručila sam iz zezanja. A onda sam čitala tumačenje tri puta i plakala kod trećeg. Kao da me neko konačno vidio."</p>
        <div class="who">Milena &middot; 46 &middot; Nikšić</div>
      </div>
      <div class="q">
        <p>„Pitala sam za posao, dobila odgovor za dva dana. Nije mi obećala kule i gradove, i baš zato joj vjerujem. Ono što je rekla, desilo se."</p>
        <div class="who">Ivana &middot; 29 &middot; Split</div>
      </div>
      <div class="q">
        <p>„Moja rahmetli nana je gledala u fildžan cijelom komšiluku. Kad sam otvorila Daničino tumačenje, osjetila sam isti onaj mir. Hvala ti."</p>
        <div class="who">Amra &middot; 38 &middot; Sarajevo</div>
      </div>
    </div>
  </div>
</section>

<section id="faq">
  <div class="wrap center">
    <div class="kicker">Pitanja</div>
    <h2>Česta pitanja</h2>
    <div class="rule"></div>
    <br>
    <div style="text-align:left">
      <details>
        <summary>Da li je moje čitanje zaista privatno?</summary>
        <p>Jeste, i to bez izuzetka. Tvoja pitanja, podaci i fotografije se ne dijele ni sa kim, ne objavljuju se i ne koriste se za reklame. Fotografije šolje brišemo nakon 30 dana.</p>
      </details>
      <details>
        <summary>Šta ako se ne prepoznam u čitanju?</summary>
        <p>Javi nam se u roku od 7 dana i vraćamo ti novac, bez ispitivanja. Ovaj posao ima smisla samo ako ti nešto znači.</p>
      </details>
      <details>
        <summary>Kako da pripremim šolju za slikanje?</summary>
        <p>Popij domaću kafu bez filtera, okreni šolju naopako na tacnu i sačekaj nekoliko minuta da se talog slije. Onda slikaj unutrašnjost iz dva ugla, uz dobro svjetlo. Sve ostalo je naš posao.</p>
      </details>
    </div>
  </div>
</section>

<footer>
  <div class="wrap">
    <a class="logo" href="#">Danica<span>&#10022;</span></a>
    <p style="margin-top:10px">Karte i šolja, na jednom mjestu i pisano samo za tebe. Da sebe čuješ jasnije.</p>
    <div class="disclaimer">
      Čitanja su vodič, podrška i razgovor sa sobom, a ne zamjena za medicinski, pravni ili finansijski savjet. Namijenjeno punoljetnim osobama.
      Ako se u čitanju ne prepoznaš, u roku od 7 dana vraćamo novac.
      &copy; Danica 2026. Sva prava zadržana.
    </div>
  </div>
</footer>

<div class="modal-bg" id="modalBg" onclick="if(event.target===this)closeOrder()">
  <div class="modal" style="position:relative">
    <span class="mclose" onclick="closeOrder()" title="Zatvori">&times;</span>
    <div style="color:var(--gold);font-size:26px;text-align:center">&#10022;</div>
    <form id="orderForm" onsubmit="return submitOrder(event)">
      <h3 style="text-align:center">Tvoja narudžba</h3>
      <p class="sub2" style="text-align:center">Reci nam za koga pišemo. Što više podijeliš, čitanje je tačnije.</p>
      <div class="field"><label>Čitanje</label>
        <select id="fUsluga">
          <option>Gledanje u šolju &middot; 9 &euro;</option>
          <option>Gledanje u šolju uz glasovnu poruku &middot; 15 &euro;</option>
          <option>Tarot: detaljno otvaranje &middot; 15 &euro;</option>
        </select>
      </div>
      <div class="field"><label>Ime</label><input type="text" id="fIme" required placeholder="Kako da ti se obratimo"></div>
      <div class="field"><label>Mejl</label><input type="email" required placeholder="Na koji stiže čitanje"></div>
      <div class="field"><label>Datum rođenja</label><input type="text" inputmode="numeric" placeholder="dd/mm/gggg"></div>
      <div class="field"><label>Teme koje te zanimaju</label>
        <div class="themes">
          <label><input type="checkbox"> Ljubav</label>
          <label><input type="checkbox"> Posao i novac</label>
          <label><input type="checkbox"> Porodica</label>
          <label><input type="checkbox"> Ja i moj mir</label>
        </div>
      </div>
      <div class="field"><label>Napiši nam nešto o sebi</label>
        <textarea placeholder="Šta te muči, šta čekaš, šta bi pitala da sjedimo uz kafu..."></textarea>
      </div>
      <div style="text-align:center;margin-top:22px">
        <button class="btn solid" type="submit">Pošalji narudžbu</button>
      </div>
      <p class="note" style="text-align:center">Prototip: podaci se ne šalju i ne čuvaju nigdje. U pravoj verziji ovdje ide sigurno plaćanje.</p>
    </form>
    <div id="formOk">
      <div class="star">&#10022;</div>
      <h3>Hvala ti na povjerenju</h3>
      <p class="sub2">Ovo je rani prototip pa narudžbe još nijesu aktivne. Vrata otvaramo uskoro, i prve čitateljke čeka posebna cijena.</p>
      <button class="btn" onclick="closeOrder()">Važi, čekam vas</button>
    </div>
  </div>
</div>

<script>
/* ---------- DIAL TICKS ---------- */
(function(){
  const g = document.getElementById('dialTicks');
  if(!g) return;
  for (let i = 0; i < 48; i++){
    const l = document.createElementNS('http://www.w3.org/2000/svg','line');
    l.setAttribute('x1','400'); l.setAttribute('y1','4');
    l.setAttribute('x2','400'); l.setAttribute('y2','20');
    l.setAttribute('transform','rotate(' + (i * 7.5) + ' 400 400)');
    g.appendChild(l);
  }
})();

/* ---------- ORDER FORM ---------- */
function openOrder(usluga){
  const sel = document.getElementById('fUsluga');
  for (const o of sel.options){ if(o.text.toLowerCase().startsWith(usluga.split(':')[0].toLowerCase()) && o.text.toLowerCase().includes(usluga.split(':').pop().trim().split(' ')[0].toLowerCase())){ sel.value = o.text; break; } }
  document.getElementById('orderForm').style.display='block';
  document.getElementById('formOk').style.display='none';
  document.getElementById('modalBg').classList.add('open');
}
function closeOrder(){ document.getElementById('modalBg').classList.remove('open'); }
function submitOrder(e){
  e.preventDefault();
  document.getElementById('orderForm').style.display='none';
  document.getElementById('formOk').style.display='block';
  return false;
}

/* ---------- CUP PREVIEW ---------- */
function previewCup(e){
  const f = e.target.files[0];
  if(!f) return;
  const box = document.getElementById('cupPreview');
  box.innerHTML = '';
  const img = document.createElement('img');
  img.src = URL.createObjectURL(f);
  box.appendChild(img);
  const p = document.createElement('p');
  p.style.cssText = 'color:#d4b96a;margin-top:4px;font-size:14px';
  p.textContent = 'Slika je poslata Danici.';
  box.appendChild(p);
}

/* ---------- TAROT ---------- */
const TAROT = [
 ['0','Luda','Dan je kao stvoren za nešto novo. Ne oklijevaj previše, kreni pa će se put sam otvoriti.','RWS_Tarot_00_Fool.jpg','želju za novim početkom',1],
 ['I','Čarobnica','Danas u svojim rukama imaš sve što ti treba. Samo se sjeti da to i upotrijebiš.','RWS_Tarot_01_Magician.jpg','osjećaj da možeš sve kad hoćeš',1],
 ['II','Sveštenica','Danas vjeruj intuiciji više nego riječima. Vodi se osjećajem.','RWS_Tarot_02_High_Priestess.jpg','intuiciju koja ne griješi',0],
 ['III','Carica','Dan da se brineš o sebi. Nešto lijepo se sprema, ne požuruj ništa.','RWS_Tarot_03_Empress.jpg','potrebu za nježnošću',1],
 ['IV','Car','Danas si u potpunoj kontroli. Reci jasno šta hoćeš i ostani čvrsto pri tome.','RWS_Tarot_04_Emperor.jpg','potrebu za redom i čvrstom riječju',0],
 ['V','Učitelj','Poslušaj danas nekog starijeg ili iskusnijeg. Jedan savjet će ti vrijediti zlata.','RWS_Tarot_05_Hierophant.jpg','tuđi savjet koji vrijedi poslušati',0],
 ['VI','Ljubavnici','Danas te čeka izbor. Biraj srcem, ali neka i razum nešto kaže.','RWS_Tarot_06_Lovers.jpg','izbor koji se više ne da odlagati',0],
 ['VII','Kočija','Danas se ide naprijed. Uzmi stvar u svoje ruke i ne osvrći se.','RWS_Tarot_07_Chariot.jpg','snagu da guraš naprijed',1],
 ['VIII','Snaga','Danas pobjeđuješ mirnoćom. Ne troši se na rasprave, tvoja tišina je jača.','RWS_Tarot_08_Strength.jpg','tihu snagu koja se ne dokazuje',1],
 ['IX','Pustinjakinja','Odvoji danas malo vremena samo za sebe. To nije bježanje, to je neophodna obnova tvoje energije.','RWS_Tarot_09_Hermit.jpg','potrebu za mirom i samoćom',0],
 ['X','Točak sreće','Danas se nešto okreće u tvoju korist. Budi spremna da uhvatiš priliku.','RWS_Tarot_10_Wheel_of_Fortune.jpg','sreću koja se okreće na tvoju stranu',1],
 ['XI','Pravda','Danas će se ukazati istina. Budi poštena prema sebi i traži isto od drugih.','RWS_Tarot_11_Justice.jpg','istinu koja izlazi na vidjelo',0],
 ['XII','Obješeni','Danas ništa ne radi na silu. Sačekaj i pogledaj stvar iz drugog ugla.','RWS_Tarot_12_Hanged_Man.jpg','poziv da zastaneš i sačekaš',-1],
 ['XIII','Smrt','Danas nešto pusti. Kad se jedna vrata zatvore, otvore se druga.','RWS_Tarot_13_Death.jpg','kraj nečega što je odavno dotrajalo',-1],
 ['XIV','Umjerenost','Polako danas. Ni previše, ni premalo, sve s mjerom.','RWS_Tarot_14_Temperance.jpg','potrebu za mjerom i mirom',0],
 ['XV','Đavo','Pripazi danas na stare navike. Ono što te vuče nazad nije jače od tebe.','RWS_Tarot_15_Devil.jpg','stare navike koje se ne predaju lako',-1],
 ['XVI','Kula','Ako se danas nešto izjalovi, pusti neka se izjalovi. Nije bilo za tebe, čisti se teren.','RWS_Tarot_16_Tower.jpg','rušenje nečega što ionako nije bilo tvoje',-1],
 ['XVII','Zvijezda','Danas ti se vraća nada. Najgore je prošlo.','RWS_Tarot_17_Star.jpg','nadu koja se vraća',1],
 ['XVIII','Mjesec','Danas nije sve kako izgleda. Važne odluke ostavi dok se ne razbistri.','RWS_Tarot_18_Moon.jpg','maglu u kojoj ne treba žuriti',-1],
 ['XIX','Sunce','Vedar dan pred tobom. Iskoristi ga za ono što voliš i ljude koji te vole.','RWS_Tarot_19_Sun.jpg','vedrinu koja se ne da pokvariti',1],
 ['XX','Sud','Danas ti dolazi jasnoća. Ono što odavno znaš, danas smiješ i priznati.','RWS_Tarot_20_Judgement.jpg','jasnoću koja konačno dolazi',1],
 ['XXI','Svijet','Danas se jedan krug lijepo zatvara. Osvrni se na to koliko si prešla.','RWS_Tarot_21_World.jpg','krug koji se lijepo zatvara',1]
];
let drawn = [], flippedCount = 0, picked = 0;

function seededRandom(seed){ return function(){ seed |= 0; seed = seed + 0x6D2B79F5 | 0;
  let t = Math.imul(seed ^ seed >>> 15, 1 | seed); t = t + Math.imul(t ^ t >>> 7, 61 | t) ^ t;
  return ((t ^ t >>> 14) >>> 0) / 4294967296; }; }

function buildTarot(){
  drawn = [null,null,null]; flippedCount = 0; picked = 0;
  const d = new Date();
  const rnd = seededRandom(d.getFullYear()*10000 + (d.getMonth()+1)*100 + d.getDate());
  const deck = TAROT.map((c,i)=>i);
  for (let i = deck.length-1; i > 0; i--){ const j = Math.floor(rnd()*(i+1)); [deck[i],deck[j]] = [deck[j],deck[i]]; }
  const fanIdx = deck.slice(0, 9);

  const fan = document.getElementById('fanRow');
  fan.innerHTML = '';
  fanIdx.forEach((cardIdx, i) => {
    const f = document.createElement('div');
    f.className = 'fcard';
    f.style.transform = 'rotate(' + ((i - 4) * 4) + 'deg) translateY(' + (Math.abs(i - 4) * 5) + 'px)';
    f.onclick = () => pickCard(f, cardIdx);
    fan.appendChild(f);
  });

  const row = document.getElementById('tarotRow');
  row.innerHTML = '';
  document.getElementById('tarotMeanings').innerHTML = '';
  document.getElementById('tarotCta').style.display = 'none';
  for (let i = 0; i < 3; i++){
    const slot = document.createElement('div');
    slot.className = 'tslot'; slot.id = 'slot' + i;
    const holder = document.createElement('div');
    holder.className = 'tcard'; holder.style.cursor = 'default';
    holder.innerHTML = '<div class="slot-empty">izvuci kartu</div>';
    slot.appendChild(holder);
    row.appendChild(slot);
  }
  const s = document.getElementById('tarotSummary');
  if (s) s.style.display = 'none';
}

function pickCard(fanEl, cardIdx){
  if (picked >= 3 || fanEl.classList.contains('gone')) return;
  fanEl.classList.add('gone');
  const i = picked++;
  drawn[i] = TAROT[cardIdx];
  const c = drawn[i];
  const holder = document.querySelectorAll('#tarotRow .tcard')[i];
  holder.style.cursor = 'pointer';
  const front = document.createElement('div');
  front.className = 'tface tfront';
  const img = document.createElement('img');
  img.src = 'https://commons.wikimedia.org/wiki/Special:FilePath/' + c[3] + '?width=440';
  img.alt = c[1]; img.loading = 'lazy';
  img.onerror = () => { img.style.display = 'none'; };
  const lab = document.createElement('div');
  lab.className = 'tlabel';
  lab.innerHTML = '<div class="tname">' + c[0] + ' &middot; ' + c[1] + '</div>';
  front.appendChild(img); front.appendChild(lab);
  const inner = document.createElement('div');
  inner.className = 'inner';
  inner.innerHTML = '<div class="tface tback"><span class="mini">&#10022; &#10022; &#10022;</span><span class="big">&#10022;</span><span class="mini">&#10022; &#10022; &#10022;</span></div>';
  inner.appendChild(front);
  holder.innerHTML = '';
  holder.appendChild(inner);
  holder.onclick = () => flipCard(holder, i);
}

function flipCard(el, i){
  if (el.classList.contains('flipped') || !drawn[i]) return;
  el.classList.add('flipped');
  const m = document.getElementById('tarotMeanings');
  const p = document.createElement('p');
  p.innerHTML = '<b>' + drawn[i][1] + '.</b> ' + drawn[i][2];
  m.appendChild(p);
  if (++flippedCount === 3){
    showSummary();
    document.getElementById('tarotCta').style.display = 'block';
  }
}

function showSummary(){
  const cards = drawn.filter(Boolean);
  if (cards.length < 3) return;
  const t1 = cards[0][4], t2 = cards[1][4], t3 = cards[2][4];
  const tone = cards[0][5] + cards[1][5] + cards[2][5];
  let closing;
  if (tone >= 2) closing = 'Sve u svemu, dan ti ide naruku. Nemoj ga potraćiti na brige koje nisu tvoje.';
  else if (tone <= -1) closing = 'Dan traži da budeš nježna prema sebi. Ne moraš danas ništa riješiti, dovoljno je da sebe staviš u prioritet.';
  else closing = 'Dan neće biti spokojan i jednolik, ali ako svemu pristupiš polako, završićeš dan mirnija nego što si počela.';
  document.getElementById('tarotSummaryText').textContent =
    'Tvoje tri karte danas spajaju ' + t1 + ', ' + t2 + ' i ' + t3 + '. ' + closing;
  document.getElementById('tarotSummary').style.display = 'block';
}
document.addEventListener('DOMContentLoaded', buildTarot);

</script>
</body>
</html>
