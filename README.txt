:root{
  --bg:#ffffff; --bg-soft:#f6f7fb; --ink:#0e1116; --muted:#6b7280;
  --line:#e7e9f0; --brand:#3b5bdb; --brand-dark:#2f49b0; --brand-soft:#eef1fe;
  --accent:#ff5d8f; --green:#16a34a; --amber:#f59e0b; --radius:16px;
  --shadow:0 1px 2px rgba(16,17,22,.04),0 8px 24px rgba(16,17,22,.06);
  --maxw:1180px; --font:'Inter',-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,Helvetica,Arial,sans-serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:var(--font);color:var(--ink);background:var(--bg);line-height:1.5;-webkit-font-smoothing:antialiased}
a{color:inherit;text-decoration:none}
img{max-width:100%;display:block}
.container{max-width:var(--maxw);margin:0 auto;padding:0 20px}
.btn{display:inline-flex;align-items:center;gap:8px;border:0;cursor:pointer;font-weight:600;font-size:14px;padding:11px 18px;border-radius:12px;transition:.18s;font-family:inherit}
.btn-primary{background:var(--brand);color:#fff}
.btn-primary:hover{background:var(--brand-dark);transform:translateY(-1px)}
.btn-ghost{background:var(--brand-soft);color:var(--brand)}
.btn-ghost:hover{background:#e2e7fe}
.btn-block{width:100%;justify-content:center}
.pill{display:inline-flex;align-items:center;gap:6px;font-size:12px;font-weight:600;padding:5px 11px;border-radius:999px}
.pill-sale{background:#ffe4ec;color:#d6336c}
.pill-new{background:#dcfce7;color:#15803d}
.pill-hot{background:#fff0db;color:#b45309}

/* Header */
header.site{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.85);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;gap:20px;height:68px}
.logo{display:flex;align-items:center;gap:10px;font-weight:800;font-size:20px;letter-spacing:-.4px}
.logo .mark{width:34px;height:34px}
.nav-links{display:flex;gap:22px;margin-left:8px}
.nav-links a{font-size:14px;font-weight:500;color:var(--muted)}
.nav-links a:hover{color:var(--ink)}
.search{flex:1;max-width:420px;display:flex;align-items:center;gap:8px;background:var(--bg-soft);border:1px solid var(--line);border-radius:12px;padding:9px 14px}
.search input{border:0;background:transparent;outline:0;width:100%;font-size:14px;font-family:inherit}
.nav-actions{display:flex;align-items:center;gap:10px}
.icon-btn{position:relative;width:42px;height:42px;border-radius:12px;border:1px solid var(--line);background:#fff;display:flex;align-items:center;justify-content:center;cursor:pointer;font-size:18px}
.icon-btn:hover{background:var(--bg-soft)}
.cart-count{position:absolute;top:-6px;right:-6px;background:var(--accent);color:#fff;font-size:11px;font-weight:700;min-width:18px;height:18px;border-radius:999px;display:flex;align-items:center;justify-content:center;padding:0 4px}
.lang{position:relative}
.lang-btn{display:flex;align-items:center;gap:6px;font-size:14px;font-weight:600;padding:9px 12px;border:1px solid var(--line);border-radius:12px;background:#fff;cursor:pointer;font-family:inherit}
.lang-menu{position:absolute;right:0;top:50px;background:#fff;border:1px solid var(--line);border-radius:14px;box-shadow:var(--shadow);padding:8px;display:none;grid-template-columns:1fr 1fr;gap:2px;width:280px;max-height:300px;overflow:auto}
.lang-menu.open{display:grid}
.lang-menu button{text-align:left;border:0;background:transparent;padding:8px 10px;border-radius:8px;font-size:13px;cursor:pointer;font-family:inherit}
.lang-menu button:hover{background:var(--brand-soft);color:var(--brand)}

/* Hero */
.hero{background:linear-gradient(135deg,#eef1fe 0%,#f6f7fb 60%,#ffeef4 100%);border-radius:0}
.hero-grid{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center;padding:64px 0}
.hero h1{font-size:50px;line-height:1.05;letter-spacing:-1.5px;font-weight:800;margin-bottom:18px}
.hero h1 .grad{background:linear-gradient(90deg,var(--brand),var(--accent));-webkit-background-clip:text;background-clip:text;color:transparent}
.hero p{font-size:18px;color:var(--muted);max-width:480px;margin-bottom:26px}
.hero-cta{display:flex;gap:12px;flex-wrap:wrap}
.hero-trust{display:flex;gap:26px;margin-top:30px}
.hero-trust div b{display:block;font-size:22px;font-weight:800}
.hero-trust div span{font-size:13px;color:var(--muted)}
.hero-art{position:relative}

/* Section */
section.block{padding:54px 0}
.sec-head{display:flex;align-items:flex-end;justify-content:space-between;margin-bottom:24px}
.sec-head h2{font-size:26px;font-weight:800;letter-spacing:-.6px}
.sec-head p{color:var(--muted);font-size:14px;margin-top:4px}
.sec-head a{font-size:14px;font-weight:600;color:var(--brand)}

/* Categories */
.cats{display:flex;gap:12px;overflow-x:auto;padding-bottom:6px}
.cat{flex:0 0 auto;display:flex;flex-direction:column;align-items:center;gap:8px;width:96px;padding:16px 8px;background:var(--bg-soft);border:1px solid var(--line);border-radius:var(--radius);cursor:pointer;transition:.18s}
.cat:hover{border-color:var(--brand);background:var(--brand-soft);transform:translateY(-2px)}
.cat .emoji{font-size:26px}
.cat span{font-size:12px;font-weight:600;color:var(--muted)}

/* Flash banner */
.flash{background:linear-gradient(90deg,#1f2447,#3b5bdb);color:#fff;border-radius:var(--radius);padding:22px 26px;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:16px}
.flash .ft{display:flex;align-items:center;gap:14px}
.flash h3{font-size:20px;font-weight:800}
.flash .timer{display:flex;gap:8px}
.flash .timer .t{background:rgba(255,255,255,.16);border-radius:10px;padding:8px 12px;font-weight:800;font-variant-numeric:tabular-nums;min-width:48px;text-align:center}
.flash .timer .t span{display:block;font-size:10px;font-weight:500;opacity:.8}

/* Product grid */
.grid{display:grid;grid-template-columns:repeat(4,1fr);gap:20px}
.card{background:#fff;border:1px solid var(--line);border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);transition:.2s;cursor:pointer}
.card:hover{transform:translateY(-4px);box-shadow:0 14px 34px rgba(16,17,22,.1);border-color:#d7dbeb}
.card .thumb{position:relative;aspect-ratio:1/1;background:var(--bg-soft)}
.card .thumb .tags{position:absolute;top:10px;left:10px;display:flex;gap:6px}
.card .save{position:absolute;top:10px;right:10px;width:34px;height:34px;border-radius:999px;background:rgba(255,255,255,.9);border:0;cursor:pointer;font-size:15px}
.card .body{padding:14px}
.card .body .name{font-size:14px;font-weight:600;line-height:1.35;height:38px;overflow:hidden}
.card .rate{font-size:12px;color:var(--muted);margin:6px 0}
.card .price{display:flex;align-items:baseline;gap:8px}
.card .price .now{font-size:18px;font-weight:800}
.card .price .was{font-size:13px;color:var(--muted);text-decoration:line-through}
.card .add{margin-top:10px}

/* Steps */
.steps{display:grid;grid-template-columns:repeat(4,1fr);gap:20px}
.step{background:#fff;border:1px solid var(--line);border-radius:var(--radius);padding:22px}
.step .n{width:40px;height:40px;border-radius:12px;background:var(--brand-soft);color:var(--brand);font-weight:800;display:flex;align-items:center;justify-content:center;margin-bottom:14px}
.step h4{font-size:16px;margin-bottom:6px}
.step p{font-size:13px;color:var(--muted)}

/* Shipping */
.ship{display:grid;grid-template-columns:repeat(4,1fr);gap:16px}
.ship .opt{border:1px solid var(--line);border-radius:var(--radius);padding:20px;text-align:center}
.ship .opt .ic{font-size:30px}
.ship .opt h4{margin:8px 0 4px;font-size:16px}
.ship .opt .eta{font-size:13px;color:var(--muted)}
.ship .opt .cost{margin-top:8px;font-weight:800;color:var(--brand)}

/* CTA */
.cta{background:linear-gradient(135deg,var(--brand),#6b46e5);color:#fff;border-radius:24px;padding:54px;text-align:center}
.cta h2{font-size:32px;font-weight:800;letter-spacing:-.6px;margin-bottom:10px}
.cta p{opacity:.9;margin-bottom:24px}
.cta .btn-primary{background:#fff;color:var(--brand)}

/* Footer */
footer.site{background:#0e1116;color:#aeb4c2;padding:54px 0 30px;margin-top:40px}
.foot-grid{display:grid;grid-template-columns:1.4fr 1fr 1fr 1fr;gap:30px;margin-bottom:34px}
footer .logo{color:#fff}
footer h5{color:#fff;font-size:14px;margin-bottom:14px;letter-spacing:.3px}
footer ul{list-style:none}
footer li{margin-bottom:9px;font-size:14px}
footer a:hover{color:#fff}
.foot-bottom{border-top:1px solid #232633;padding-top:22px;display:flex;justify-content:space-between;font-size:13px;flex-wrap:wrap;gap:12px}

/* Catalog (album) */
.catalog{display:grid;grid-template-columns:240px 1fr;gap:30px;align-items:start}
.filters{position:sticky;top:90px;background:#fff;border:1px solid var(--line);border-radius:var(--radius);padding:20px}
.filters h4{font-size:13px;text-transform:uppercase;letter-spacing:.5px;color:var(--muted);margin:16px 0 10px}
.filters h4:first-child{margin-top:0}
.filters label{display:flex;align-items:center;gap:8px;font-size:14px;padding:5px 0;cursor:pointer}
.chips{display:flex;flex-wrap:wrap;gap:8px}
.chip{font-size:12px;padding:6px 12px;border:1px solid var(--line);border-radius:999px;cursor:pointer}
.chip:hover,.chip.active{background:var(--brand-soft);border-color:var(--brand);color:var(--brand)}
.catalog .grid{grid-template-columns:repeat(3,1fr)}
.page-head{padding:40px 0 10px}
.page-head h1{font-size:34px;font-weight:800;letter-spacing:-1px}
.page-head .crumb{font-size:13px;color:var(--muted);margin-bottom:8px}
.toolbar{display:flex;justify-content:space-between;align-items:center;margin-bottom:20px}
.toolbar .count{font-size:14px;color:var(--muted)}
.toolbar select{font-family:inherit;font-size:14px;padding:9px 12px;border:1px solid var(--line);border-radius:10px;background:#fff}

@media(max-width:980px){
  .hero-grid{grid-template-columns:1fr;padding:40px 0}
  .hero h1{font-size:38px}
  .grid{grid-template-columns:repeat(2,1fr)}
  .steps,.ship{grid-template-columns:repeat(2,1fr)}
  .foot-grid{grid-template-columns:1fr 1fr}
  .nav-links,.search{display:none}
  .catalog{grid-template-columns:1fr}
  .filters{position:static}
  .catalog .grid{grid-template-columns:repeat(2,1fr)}
}
@media(max-width:560px){
  .grid,.catalog .grid{grid-template-columns:repeat(2,1fr);gap:12px}
  .hero h1{font-size:32px}
}
