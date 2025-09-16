<!--
DaryanDesign - Netlify Starter
Single-file HTML/CSS project ready to upload to Netlify.

How to deploy:
1) Option A - Drag & Drop: Save this file as index.html inside a folder (with an "assets" folder if you add images). Zip or open the folder and drag the folder (or the build folder containing index.html) into Netlify Sites > "Drag & drop your site output folder here".
2) Option B - Git: Create a GitHub repository, add this file as index.html at repo root, connect repository in Netlify (New site from Git) and choose main branch. Netlify will auto-deploy.

To change site name: Netlify Settings -> Domain Management -> Change site name.

If you want a multi-file project (separate CSS/JS/assets) or a GitHub repo created for you, tell me and I'll prepare it.
--><!doctype html>

<html lang="ku">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>DaryanDesign — Portfolio</title>
  <meta name="description" content="DaryanDesign - simple portfolio template ready for Netlify" />
  <link rel="icon" href="data:;base64,iVBORw0KGgo=" />
  <style>
    /* Simple, clean responsive styling */
    :root{--bg:#0f1724;--card:#0b1220;--accent:#21c7a8;--muted:#94a3b8;--glass:rgba(255,255,255,0.04)}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial; background:linear-gradient(180deg,var(--bg),#071028);color:#e6eef6;-webkit-font-smoothing:antialiased}
    .container{max-width:1100px;margin:36px auto;padding:0 20px}header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
.brand{display:flex;align-items:center;gap:12px}
.logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#7ef0d6);display:flex;align-items:center;justify-content:center;font-weight:700;color:#022;box-shadow:0 6px 18px rgba(2,6,23,0.6)}
nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}
nav a.cta{background:var(--accent);color:#022;padding:8px 12px;border-radius:10px}

.hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center}
.hero h1{font-size:32px;margin:0 0 12px}
.hero p{color:var(--muted);line-height:1.6}
.card{background:var(--card);padding:20px;border-radius:14px;box-shadow:0 6px 24px rgba(2,6,23,0.6)}

.skills{display:flex;gap:10px;flex-wrap:wrap;margin-top:12px}
.tag{background:var(--glass);padding:8px 10px;border-radius:999px;font-size:13px;color:var(--muted)}

.profile-pic{width:100%;height:100%;min-height:220px;border-radius:12px;background:linear-gradient(135deg,#083047,#07203a);display:flex;align-items:center;justify-content:center;color:#7de6d3;font-weight:700}

.projects{display:grid;grid-template-columns:repeat(auto-fill,minmax(240px,1fr));gap:18px;margin-top:28px}
.project{padding:14px;border-radius:12px;background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);border:1px solid rgba(255,255,255,0.03)}
.project h3{margin:0 0 8px;font-size:16px}
.project p{margin:0;color:var(--muted);font-size:13px}

footer{margin:48px 0 12px;color:var(--muted);text-align:center;font-size:14px}

/* responsive */
@media (max-width:880px){
  .hero{grid-template-columns:1fr}
  nav{display:none}
}

/* small helper styles */
.row{display:flex;gap:12px;align-items:center}
.btn{display:inline-block;padding:10px 14px;border-radius:10px;font-weight:700}

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">DD</div>
        <div>
          <div style="font-weight:800;font-size:18px">DaryanDesign</div>
          <div style="font-size:12px;color:var(--muted)">Creative web & UI design</div>
        </div>
      </div><nav>
    <a href="#projects">پڕۆژەکان</a>
    <a href="#contact">پەیوەندیم پێو بکە</a>
    <a class="cta" href="#contact">هێنان</a>
  </nav>
</header>

<section class="hero">
  <div>
    <h1>سڵاو! من DaryanDesign — وێبسایت و یۆ آی دیزاین</h1>
    <p>ئەمە نموونەیەکی سادەی پۆرتفۆلیۆیە بۆ نمایشکردنی پڕۆژەکانت و پەیوەندیکردن بە میوانان. ئەم فایلە هەمووی لە یەک فایل HTML ـە و ئاسانە لەسەر Netlify دیپلۆی بکەی.</p>

    <div class="card" style="margin-top:18px">
      <div style="font-weight:700;margin-bottom:8px">تواناکان</div>
      <div class="skills">
        <div class="tag">HTML</div>
        <div class="tag">CSS</div>
        <div class="tag">Responsive</div>
        <div class="tag">Netlify</div>
        <div class="tag">Portfolio</div>
      </div>
    </div>

    <div style="margin-top:18px">
      <a class="btn" href="#projects" style="background:transparent;border:1px solid rgba(255,255,255,0.06)">بینینی پڕۆژەکان</a>
    </div>
  </div>

  <aside class="card">
    <div class="profile-pic">عکس/لوگو</div>
    <div style="margin-top:12px">
      <div style="font-weight:800">DaryanDesign</div>
      <div style="color:var(--muted);font-size:13px;margin-top:6px">دیزاینەر و دولەوەر لە دروستکردنی وێبسایت و یۆ آی</div>
      <div style="margin-top:12px" class="row">
        <div class="tag">Erbil</div>
        <div class="tag">Freelance</div>
      </div>
    </div>
  </aside>
</section>

<section id="projects">
  <h2 style="margin-top:36px">پڕۆژەکان</h2>
  <div class="projects">
    <div class="project">
      <h3>Parwana Shop</h3>
      <p>وێبسایتی فڕۆشتن؛ قالبی سادە بۆ storefront و checkout.</p>
    </div>
    <div class="project">
      <h3>Sport App UI</h3>
      <p>پڕۆتوتایپی موبایل بۆ تێکنیکی وازی و هەواڵەکانی یاری.</p>
    </div>
    <div class="project">
      <h3>Restaurant Landing</h3>
      <p>لێندینگ پیچ بۆ مەکۆی خواردن و نیشاندانی مینو.</p>
    </div>
    <div class="project">
      <h3>Personal Blog</h3>
      <p>بلاگ و سیستم پەیامەکان، SEO friendly.</p>
    </div>
  </div>
</section>

<section id="contact" style="margin-top:36px">
  <h2>پەیوەندیم پێو بکە</h2>
  <div class="card" style="margin-top:12px;display:grid;grid-template-columns:1fr 1fr;gap:12px">
    <div>
      <label style="display:block;font-weight:700;margin-bottom:6px">ناوت</label>
      <input placeholder="ناوت لێرە بنوسە" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" />
      <label style="display:block;font-weight:700;margin:12px 0 6px">ئیمەیڵ</label>
      <input placeholder="email@example.com" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" />
    </div>
    <div>
      <label style="display:block;font-weight:700;margin-bottom:6px">پەیام</label>
      <textarea placeholder="پەیامەکەت بنووسە" style="width:100%;height:140px;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit"></textarea>
      <div style="margin-top:10px">
        <button class="btn" style="background:var(--accent);color:#022">ناردن</button>
      </div>
    </div>
  </div>
  <div style="margin-top:12px;color:var(--muted)">ئیمەیڵ: <strong>hello@daryandesign.local</strong> — بەرواری نیشان: 2025</div>
</section>

<footer>
  © DaryanDesign — ئەم پڕۆژەیە ساده و بۆ دیسپلەیە. دەتوانی ناوەکانی پڕۆژە هەموو گۆڕانکاری بکەیت.
</footer>

  </div>  <script>
    // small interaction: smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        e.preventDefault();
        const id = a.getAttribute('href');
        const el = document.querySelector(id);
        if(el) el.scrollIntoView({behavior:'smooth', block:'start'});
      })
    });
  </script></body>
</html>
