from pathlib import Path

html = r'''<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Md. Hasib Islam — Cybersecurity, Penetration Testing, Bug Bounty, Security Engineering and AI Security Research.">
<meta name="author" content="Md. Hasib Islam">
<title>Md. Hasib Islam | Cybersecurity Profile</title>
<style>
:root{
  --bg:#03050a; --panel:#081019; --panel2:#0d1722; --text:#e6edf3;
  --muted:#94a3b8; --green:#00e5a8; --blue:#38bdf8; --purple:#a855f7;
  --red:#ff5555; --border:rgba(148,163,184,.18);
}
*{box-sizing:border-box;scroll-behavior:smooth}
body{margin:0;background:radial-gradient(circle at top,#0b1b25 0,#03050a 42%);color:var(--text);font-family:Inter,Segoe UI,Arial,sans-serif;line-height:1.65}
a{color:var(--blue);text-decoration:none}
a:hover{color:var(--green)}
.container{max-width:1180px;margin:auto;padding:0 22px}
.hero{min-height:90vh;display:grid;place-items:center;text-align:center;padding:70px 20px;position:relative;overflow:hidden}
.hero:before{content:"";position:absolute;inset:0;background:linear-gradient(120deg,transparent 35%,rgba(0,229,168,.07),transparent 65%);animation:pulse 7s infinite}
@keyframes pulse{50%{transform:translateX(8%);opacity:.6}}
.badge{display:inline-block;border:1px solid var(--green);color:var(--green);padding:7px 14px;border-radius:999px;font:700 12px monospace;letter-spacing:2px}
h1{font-size:clamp(42px,8vw,86px);margin:18px 0 8px;line-height:1.05;letter-spacing:-3px}
.gradient{background:linear-gradient(90deg,var(--green),var(--blue),var(--purple));-webkit-background-clip:text;background-clip:text;color:transparent}
.typing{font:700 clamp(15px,2vw,22px) monospace;color:var(--green);min-height:34px}
.hero p{max-width:820px;margin:22px auto;color:var(--muted);font-size:18px}
.buttons{display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin:28px 0}
.btn{padding:11px 18px;border:1px solid var(--border);border-radius:10px;background:rgba(8,16,25,.8);font-weight:700}
.btn.primary{border-color:var(--green);color:var(--green)}
section{padding:70px 0;border-top:1px solid var(--border)}
.section-title{font-size:30px;margin:0 0 10px}.section-sub{color:var(--muted);margin-bottom:28px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:18px}
.card{background:linear-gradient(145deg,var(--panel),var(--panel2));border:1px solid var(--border);border-radius:16px;padding:24px;box-shadow:0 15px 50px rgba(0,0,0,.18)}
.card h3{margin-top:0}.card p,.card li{color:#b8c4d3}
.tags{display:flex;flex-wrap:wrap;gap:8px}.tag{padding:7px 10px;border-radius:8px;background:#101d29;border:1px solid var(--border);font:600 12px monospace;color:#cbd5e1}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:14px}
.stat{padding:20px;text-align:center;border:1px solid var(--border);border-radius:14px;background:#071018}.stat strong{display:block;font-size:28px;color:var(--green)}.stat span{color:var(--muted);font-size:13px}
.bar{height:8px;background:#172330;border-radius:99px;overflow:hidden;margin:8px 0 18px}.bar i{display:block;height:100%;background:linear-gradient(90deg,var(--green),var(--blue));border-radius:99px}
table{width:100%;border-collapse:collapse;background:var(--panel);border-radius:12px;overflow:hidden}th,td{text-align:left;padding:13px;border-bottom:1px solid var(--border)}th{color:var(--green);font-size:13px}td{color:#cbd5e1}
.timeline{border-left:2px solid var(--green);padding-left:22px}.timeline article{margin-bottom:28px}.timeline h3{margin-bottom:3px}.timeline small{color:var(--green)}
pre{white-space:pre-wrap;background:#02070c;border:1px solid var(--border);padding:20px;border-radius:14px;color:#9fe9d0;overflow:auto}
footer{text-align:center;padding:50px 20px;color:var(--muted)}
.notice{border-left:4px solid #f59e0b;background:rgba(245,158,11,.07);padding:16px;border-radius:8px;color:#dbe4ed}
@media(max-width:650px){h1{letter-spacing:-1px}.hero{min-height:auto;padding-top:90px}.container{padding:0 16px}th,td{font-size:13px;padding:9px}}
</style>
</head>
<body>

<header class="hero" id="top">
  <div>
    <span class="badge">CYBERSECURITY • SECURITY ENGINEERING • RESEARCH</span>
    <h1>MD. <span class="gradient">HASIB ISLAM</span></h1>
    <div class="typing" id="typing"></div>
    <p>Cybersecurity-focused Computer Science graduate working across web and API security, network security, penetration testing, bug bounty research, security automation, tool development and AI-assisted security research.</p>
    <div class="buttons">
      <a class="btn primary" href="https://hasib.live" target="_blank">🌐 Portfolio</a>
      <a class="btn" href="https://github.com/khuttes" target="_blank">💻 GitHub</a>
      <a class="btn" href="mailto:ihasib199@gmail.com">📧 Email</a>
    </div>
    <div class="tags" style="justify-content:center">
      <span class="tag">🇧🇩 Bangladesh</span><span class="tag">Web Security</span><span class="tag">API Security</span>
      <span class="tag">Pentesting</span><span class="tag">Bug Bounty</span><span class="tag">AI × Security</span>
    </div>
  </div>
</header>

<main class="container">

<section id="about">
<h2 class="section-title">🧭 Security Profile</h2>
<p class="section-sub">A single-page professional security portfolio and technical profile.</p>
<div class="grid">
<div class="card">
<h3>👨‍💻 About</h3>
<p>I focus on identifying weaknesses, understanding security risk, automating repetitive security work and engineering systems that are harder to compromise.</p>
<ul>
<li>Web & API penetration testing</li><li>Network reconnaissance and security</li><li>Bug bounty methodology</li><li>Authentication & authorization security</li>
<li>Security automation and tooling</li><li>AI-assisted security research</li><li>Defensive engineering</li>
</ul>
</div>
<div class="card">
<h3>🎯 Security Mission</h3>
<p><strong>Discover → Validate → Understand → Report → Remediate → Retest</strong></p>
<p>The objective is actionable security intelligence and measurable risk reduction — not merely finding vulnerabilities.</p>
<div>Recon <div class="bar"><i style="width:90%"></i></div></div>
<div>Web Security <div class="bar"><i style="width:90%"></i></div></div>
<div>Network Security <div class="bar"><i style="width:80%"></i></div></div>
<div>Automation <div class="bar"><i style="width:80%"></i></div></div>
<div>Python <div class="bar"><i style="width:90%"></i></div></div>
<div>AI Security <div class="bar"><i style="width:70%"></i></div></div>
</div>
</div>
</section>

<section id="domains">
<h2 class="section-title">🧩 Security Domains</h2>
<div class="grid">
<div class="card"><h3>🌐 Application Security</h3><div class="tags"><span class="tag">OWASP Top 10</span><span class="tag">XSS</span><span class="tag">CSRF</span><span class="tag">XXE</span><span class="tag">IDOR/BOLA</span><span class="tag">Injection</span></div></div>
<div class="card"><h3>🔌 API Security</h3><div class="tags"><span class="tag">Endpoint Discovery</span><span class="tag">Access Control</span><span class="tag">Input Validation</span><span class="tag">Business Logic</span></div></div>
<div class="card"><h3>🌍 Network Security</h3><div class="tags"><span class="tag">Enumeration</span><span class="tag">Service Analysis</span><span class="tag">Traffic Inspection</span><span class="tag">Attack Surface</span></div></div>
<div class="card"><h3>🤖 AI × Cybersecurity</h3><div class="tags"><span class="tag">RAG</span><span class="tag">Local AI</span><span class="tag">Phishing Detection</span><span class="tag">Security Automation</span></div></div>
</div>
</section>

<section id="arsenal">
<h2 class="section-title">⚔️ Security Arsenal</h2>
<div class="grid">
<div class="card"><h3>🔎 Reconnaissance</h3><ul><li>Nmap</li><li>Subfinder</li><li>HTTPX</li><li>Katana</li><li>Wayback / GAU</li><li>Nuclei</li><li>DNS & subdomain enumeration</li><li>Attack-surface mapping</li></ul></div>
<div class="card"><h3>🧪 Application Testing</h3><ul><li>Burp Suite</li><li>OWASP methodology</li><li>IDOR / BOLA</li><li>XSS</li><li>Injection testing</li><li>CSRF / XXE</li><li>Authentication & authorization testing</li><li>API security</li></ul></div>
<div class="card"><h3>🛠️ Security Operations</h3><ul><li>Wireshark</li><li>Metasploit</li><li>Hashcat</li><li>Bettercap</li><li>BeEF</li><li>Kismet</li><li>Linux security tooling</li><li>Log analysis & automation</li></ul></div>
</div>
<p class="notice">⚠️ <strong>Ethical Security:</strong> Security research and testing should be performed only on owned systems, authorized environments, labs, CTFs, or programs that explicitly permit testing.</p>
</section>

<section id="stack">
<h2 class="section-title">💻 Technology Stack</h2>
<div class="grid">
<div class="card"><h3>Programming & Scripting</h3><div class="tags"><span class="tag">Python</span><span class="tag">JavaScript</span><span class="tag">Bash</span><span class="tag">PowerShell</span><span class="tag">C</span><span class="tag">C++</span><span class="tag">HTML5</span><span class="tag">CSS3</span></div></div>
<div class="card"><h3>Frameworks & Databases</h3><div class="tags"><span class="tag">Django</span><span class="tag">Flask</span><span class="tag">MySQL</span><span class="tag">PostgreSQL</span><span class="tag">MongoDB</span></div></div>
<div class="card"><h3>Platforms & Infrastructure</h3><div class="tags"><span class="tag">Kali Linux</span><span class="tag">Ubuntu</span><span class="tag">Windows</span><span class="tag">Docker</span><span class="tag">Git</span><span class="tag">GitHub</span></div></div>
</div>
</section>

<section id="projects">
<h2 class="section-title">🚀 Featured Security Projects</h2>
<div class="grid">
<div class="card"><h3>🤖 AI SOC Analyst Copilot</h3><p>Local-first security operations concept for ingesting, normalizing, retrieving and analyzing security telemetry through RAG-style workflows.</p><div class="tags"><span class="tag">Local AI</span><span class="tag">RAG</span><span class="tag">Log Analysis</span><span class="tag">Automation</span></div></div>
<div class="card"><h3>🎣 AI Phishing Detection System</h3><p>Security research concept combining URL, header, content-intent and attachment indicators into a phishing classification and alerting workflow.</p><div class="tags"><span class="tag">Detection</span><span class="tag">Classification</span><span class="tag">Threat Analysis</span></div></div>
<div class="card"><h3>🔐 CS-GPAS — Graphical Authentication</h3><p>Browser-based graphical authentication concept using sequential image selection instead of conventional text passwords.</p><div class="tags"><span class="tag">Authentication</span><span class="tag">Web</span><span class="tag">UX</span></div></div>
<div class="card"><h3>💥 Brute-Force Attack Simulator</h3><p>Educational browser simulator demonstrating repeated password-guessing mechanics in a controlled environment with real-time progress visualization.</p><div class="tags"><span class="tag">JavaScript</span><span class="tag">Simulation</span><span class="tag">Security Awareness</span></div></div>
<div class="card"><h3>🕵️ Mini Nmap Port Scanner</h3><p>Security-learning project focused on understanding network service discovery and port-scanning concepts.</p></div>
<div class="card"><h3>🧪 Malware Behavior Analysis Tool</h3><p>Research-oriented concept for observing suspicious behavior, extracting indicators and supporting controlled analysis workflows.</p></div>
<div class="card"><h3>🛡️ API Attack Detection System</h3><p>Concept for monitoring API activity and identifying anomalous or suspicious request patterns.</p></div>
<div class="card"><h3>🎙️ Deepfake Voice Scam Detection</h3><p>Research direction focused on identifying synthetic or manipulated voice signals associated with scam scenarios.</p></div>
</div>
</section>

<section id="workflow">
<h2 class="section-title">🏗️ Security Research Workflow</h2>
<pre>
RECON → ENUMERATION → TESTING → VALIDATION & EVIDENCE
                                      ↓
                                RISK / IMPACT
                                      ↓
                         REPORT → REMEDIATE → RETEST
</pre>
<p><strong>Engineering principle:</strong> A vulnerability is only valuable when it can be reproduced, explained, prioritized and ultimately remediated.</p>
</section>

<section id="matrix">
<h2 class="section-title">📈 Capability Matrix</h2>
<table>
<thead><tr><th>Domain</th><th>Focus Areas</th></tr></thead>
<tbody>
<tr><td>🌐 Web Security</td><td>OWASP Top 10, authentication, authorization, session security, injection, XSS</td></tr>
<tr><td>🔌 API Security</td><td>Endpoint discovery, access control, validation, business-logic testing</td></tr>
<tr><td>🌍 Network Security</td><td>Enumeration, service analysis, traffic inspection, attack-surface assessment</td></tr>
<tr><td>🔐 Authentication</td><td>Graphical authentication, password security, access-control analysis</td></tr>
<tr><td>🐞 Bug Bounty</td><td>Reconnaissance, manual validation, vulnerability research, responsible reporting</td></tr>
<tr><td>🤖 AI Security</td><td>AI-assisted analysis, RAG workflows, phishing detection, security automation</td></tr>
<tr><td>🧰 Tool Development</td><td>Python, JavaScript, Bash, automation and security utilities</td></tr>
<tr><td>🛡️ Defensive Security</td><td>Logging, detection concepts, remediation guidance and hardening</td></tr>
</tbody>
</table>
</section>

<section id="education">
<h2 class="section-title">🎓 Education</h2>
<div class="timeline">
<article><small>2024</small><h3>B.Sc. in Computer Science & Engineering</h3><p>Varendra University, Rajshahi</p></article>
<article><small>2019</small><h3>Higher Secondary Certificate — Science</h3><p>Naogaon Government College</p></article>
<article><small>2017</small><h3>Secondary School Certificate — Science</h3><p>Naogaon KD Government High School</p></article>
</div>
</section>

<section id="certifications">
<h2 class="section-title">📜 Certifications & Training</h2>
<div class="grid">
<div class="card"><h3>SkillUp by Simplilearn</h3><p>CISSP Fundamentals / Cybersecurity / Ethical Hacking / Kali Linux</p></div>
<div class="card"><h3>Great Learning</h3><p>Network Security, Mobile Platforms & Network Architecture, Advanced Cyber Security</p></div>
<div class="card"><h3>IBM</h3><p>Cybersecurity Careers</p></div>
<div class="card"><h3>HP Foundation</h3><p>Professional Networking & Cybersecurity Awareness</p></div>
</div>
</section>

<section id="research">
<h2 class="section-title">🔭 Current Research Direction</h2>
<div class="stats">
<div class="stat"><strong>✓</strong><span>Web Application Security</span></div>
<div class="stat"><strong>✓</strong><span>Network Security</span></div>
<div class="stat"><strong>✓</strong><span>Bug Bounty Methodology</span></div>
<div class="stat"><strong>✓</strong><span>Security Automation</span></div>
<div class="stat"><strong>→</strong><span>AI Security Operations</span></div>
<div class="stat"><strong>→</strong><span>Detection Engineering</span></div>
<div class="stat"><strong>→</strong><span>Advanced API Security</span></div>
<div class="stat"><strong>→</strong><span>Security Research & Publication</span></div>
<div class="stat"><strong>→</strong><span>Privacy-Preserving Local AI</span></div>
</div>
</section>

<section id="philosophy">
<h2 class="section-title">📂 Repository Philosophy</h2>
<div class="grid">
<div class="card"><h3>01 — Practical</h3><p>Security research should solve real problems, not exist only as a proof of concept.</p></div>
<div class="card"><h3>02 — Reproducible</h3><p>Projects should be documented clearly enough for authorized researchers and developers to understand the methodology.</p></div>
<div class="card"><h3>03 — Responsible</h3><p>Offensive security knowledge should support authorized testing, defense, education and responsible vulnerability disclosure.</p></div>
</div>
</section>

<section id="collaboration">
<h2 class="section-title">🤝 Collaboration</h2>
<div class="tags">
<span class="tag">Cybersecurity Research</span><span class="tag">Bug Bounty Tooling</span><span class="tag">Web/API Security</span>
<span class="tag">AI × Cybersecurity</span><span class="tag">SOC & Detection Engineering</span><span class="tag">Security Automation</span>
<span class="tag">CTF / Security Labs</span><span class="tag">Technical Research</span><span class="tag">Open Source Security</span>
</div>
</section>

<section id="contact">
<h2 class="section-title">📫 Connect</h2>
<div class="grid">
<div class="card"><h3>🌐 Portfolio</h3><p><a href="https://hasib.live" target="_blank">hasib.live</a></p></div>
<div class="card"><h3>💻 GitHub</h3><p><a href="https://github.com/khuttes" target="_blank">github.com/khuttes</a></p></div>
<div class="card"><h3>📧 Email</h3><p><a href="mailto:ihasib199@gmail.com">ihasib199@gmail.com</a></p></div>
</div>
</section>

</main>

<footer>
<p><strong>⚡ Secure by Design • Curious by Nature • Relentless in Research</strong></p>
<p>© Md. Hasib Islam • Cybersecurity Research & Engineering</p>
<p><a href="#top">↑ Back to top</a></p>
</footer>

<script>
const lines=[
"CYBERSECURITY SPECIALIST",
"WEB & NETWORK PENETRATION TESTING",
"BUG BOUNTY & APPLICATION SECURITY",
"SECURITY TOOL DEVELOPMENT",
"AI + CYBERSECURITY RESEARCH",
"BUILDING AND SECURING DIGITAL SYSTEMS"
];
let li=0,ci=0,del=false;
const el=document.getElementById("typing");
function type(){
 const text=lines[li];
 el.textContent=del?text.slice(0,ci--):text.slice(0,ci++);
 if(!del && ci>text.length){del=true;setTimeout(type,1300);return}
 if(del && ci<0){del=false;li=(li+1)%lines.length;ci=0}
 setTimeout(type,del?35:65);
}
type();
</script>
</body>
</html>'''

path = Path("/mnt/data/Md_Hasib_Islam_Cybersecurity_Profile.html")
path.write_text(html, encoding="utf-8")
print(path)
