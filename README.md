# medical-ai
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Hub 主站</title>

<style>
* {margin:0;padding:0;box-sizing:border-box;}
body {
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto;
    background:#0f172a;
    color:#fff;
    scroll-behavior:smooth;
}

/* ========== 动态背景 ========== */
.bg-svg {
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    z-index:-1;
}

/* ========== 顶部导航 ========== */
nav {
    position:fixed;
    top:0;
    width:100%;
    background:rgba(15,23,42,0.8);
    backdrop-filter:blur(8px);
    display:flex;
    justify-content:center;
    gap:30px;
    padding:15px;
    z-index:1000;
}

nav a {
    color:#94a3b8;
    text-decoration:none;
    font-weight:600;
    transition:0.3s;
}

nav a.active,
nav a:hover {
    color:#38bdf8;
}

/* ========== 页面结构 ========== */
section {
    padding:120px 20px 80px;
    min-height:100vh;
    max-width:1100px;
    margin:auto;
}

h2 {
    font-size:2rem;
    margin-bottom:30px;
    border-left:5px solid #38bdf8;
    padding-left:15px;
}

/* ========== 卡片样式 ========== */
.grid {
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:25px;
}

.card {
    background:rgba(30,41,59,0.8);
    padding:25px;
    border-radius:16px;
    text-align:center;
    transition:0.3s;
    backdrop-filter:blur(6px);
}

.card:hover {
    transform:translateY(-8px);
    box-shadow:0 10px 25px rgba(56,189,248,0.4);
}

.card svg {
    width:60px;
    height:60px;
    margin-bottom:15px;
}

.card a {
    display:block;
    color:#38bdf8;
    text-decoration:none;
    font-weight:600;
    margin-top:8px;
}

footer {
    text-align:center;
    padding:40px;
    background:#020617;
}
</style>
</head>
<body>

<!-- 动态 SVG 背景 -->
<svg class="bg-svg" viewBox="0 0 800 600" preserveAspectRatio="none">
  <defs>
    <linearGradient id="grad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0ea5e9">
        <animate attributeName="stop-color"
          values="#0ea5e9;#6366f1;#0ea5e9"
          dur="8s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#6366f1"/>
    </linearGradient>
  </defs>
  <rect width="800" height="600" fill="url(#grad)" opacity="0.15"/>
</svg>

<!-- 顶部导航 -->
<nav>
  <a href="#models">大模型</a>
  <a href="#art">AI 作画</a>
  <a href="#video">AI 视频</a>
  <a href="#write">AI 写作</a>
  <a href="#audio">音乐语音</a>
</nav>

<!-- ========== 大模型 ========== -->
<section id="models">
<h2>🔥 大模型</h2>
<div class="grid">

<div class="card">
<svg viewBox="0 0 24 24" fill="#38bdf8">
<circle cx="12" cy="12" r="10"/>
</svg>
ChatGPT
<a href="https://chat.openai.com">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#6366f1">
<rect x="4" y="4" width="16" height="16" rx="4"/>
</svg>
Claude
<a href="https://www.anthropic.com">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#22d3ee">
<polygon points="12,2 22,22 2,22"/>
</svg>
Gemini
<a href="https://gemini.google.com">访问官网</a>
</div>

</div>
</section>

<!-- ========== 作画 ========== -->
<section id="art">
<h2>🎨 AI 作画</h2>
<div class="grid">

<div class="card">
<svg viewBox="0 0 24 24" fill="#f59e0b">
<path d="M12 2a10 10 0 1 0 0 20z"/>
</svg>
Midjourney
<a href="https://www.midjourney.com">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#10b981">
<circle cx="12" cy="12" r="8"/>
</svg>
Stable Diffusion
<a href="https://stability.ai">访问官网</a>
</div>

</div>
</section>

<!-- ========== 视频 ========== -->
<section id="video">
<h2>🎬 AI 视频</h2>
<div class="grid">

<div class="card">
<svg viewBox="0 0 24 24" fill="#ec4899">
<polygon points="5,3 19,12 5,21"/>
</svg>
Runway
<a href="https://runwayml.com">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#f43f5e">
<rect x="3" y="5" width="18" height="14" rx="2"/>
</svg>
Pika
<a href="https://pika.art">访问官网</a>
</div>

</div>
</section>

<!-- ========== 写作 ========== -->
<section id="write">
<h2>✍ AI 写作</h2>
<div class="grid">

<div class="card">
<svg viewBox="0 0 24 24" fill="#3b82f6">
<path d="M3 21l3-3 12-12-3-3L3 15z"/>
</svg>
Jasper
<a href="https://www.jasper.ai">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#14b8a6">
<circle cx="12" cy="12" r="6"/>
</svg>
Copy.ai
<a href="https://www.copy.ai">访问官网</a>
</div>

</div>
</section>

<!-- ========== 音乐 ========== -->
<section id="audio">
<h2>🎵 音乐 & 语音</h2>
<div class="grid">

<div class="card">
<svg viewBox="0 0 24 24" fill="#a855f7">
<path d="M9 3v12a4 4 0 1 0 2 3V7h6V3z"/>
</svg>
Suno
<a href="https://suno.ai">访问官网</a>
</div>

<div class="card">
<svg viewBox="0 0 24 24" fill="#06b6d4">
<rect x="9" y="2" width="6" height="20" rx="3"/>
</svg>
ElevenLabs
<a href="https://elevenlabs.io">访问官网</a>
</div>

</div>
</section>

<footer>
© 2026 AI Hub 主站 | 可自由扩展
</footer>

<!-- ========== 滚动高亮脚本 ========== -->
<script>
const sections = document.querySelectorAll("section");
const navLinks = document.querySelectorAll("nav a");

window.addEventListener("scroll", () => {
  let current = "";
  sections.forEach(section => {
    const sectionTop = section.offsetTop - 150;
    if (pageYOffset >= sectionTop) {
      current = section.getAttribute("id");
    }
  });

  navLinks.forEach(a => {
    a.classList.remove("active");
    if (a.getAttribute("href") === "#" + current) {
      a.classList.add("active");
    }
  });
});
</script>

</body>
</html>
