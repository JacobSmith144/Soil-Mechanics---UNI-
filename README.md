[engm2010_soil_mechanics_portal.html](https://github.com/user-attachments/files/28667360/engm2010_soil_mechanics_portal.html)
# engm2010-soil-mechanics.
Exam practice portal with interactive question versions, answer checking, working-method buttons, solutions and examiner tips.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ENGM 2010 Soil Mechanics — Exam Practice Portal</title>
<style>
*{
  box-sizing:border-box;
}

body{
  margin:0;
  font-family:Arial, sans-serif;
  background:#e9eef5;
  color:#111827;
}

.site-header{
  position:sticky;
  top:0;
  z-index:1000;
  background:#115e59;
  color:white;
  box-shadow:0 3px 12px rgba(0,0,0,.18);
}

.navbar{
  max-width:1200px;
  margin:0 auto;
  display:flex;
  align-items:center;
  justify-content:space-between;
  padding:14px 24px;
}

.logo{
  font-size:22px;
  font-weight:900;
  letter-spacing:.2px;
}

.nav-links{
  display:flex;
  gap:10px;
  align-items:center;
  flex-wrap:wrap;
}

.nav-links button{
  border:none;
  background:transparent;
  color:white;
  font-weight:800;
  padding:10px 14px;
  border-radius:8px;
  cursor:pointer;
  font-size:15px;
}

.nav-links button:hover{
  background:rgba(255,255,255,.14);
}

.nav-links button.active{
  background:white;
  color:#115e59;
}

.main-shell{
  max-width:1200px;
  margin:28px auto;
  padding:0 20px 30px;
}

.home-panel{
  background:white;
  border-radius:14px;
  padding:34px;
  box-shadow:0 8px 24px rgba(0,0,0,.10);
}

.hero{
  text-align:center;
  margin-bottom:28px;
}

.hero h1{
  margin:0 0 10px;
  font-size:34px;
}

.hero p{
  margin:0 auto;
  max-width:760px;
  font-size:17px;
  line-height:1.6;
  color:#374151;
}

.cards{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:18px;
  margin-top:28px;
}

.card{
  background:#f9fafb;
  border:1px solid #cbd5e1;
  border-radius:14px;
  padding:22px;
}

.card h2{
  margin:0 0 8px;
  font-size:22px;
}

.card p{
  margin:0 0 16px;
  line-height:1.5;
}

.card button{
  background:#115e59;
  color:white;
  border:none;
  padding:11px 16px;
  border-radius:9px;
  font-weight:900;
  cursor:pointer;
}

.card button:hover{
  background:#0f766e;
}

.question-section{
  display:none;
}

.question-frame{
  width:100%;
  min-height:1850px;
  border:none;
  border-radius:14px;
  background:white;
  box-shadow:0 8px 24px rgba(0,0,0,.10);
}

#q1Frame{
  min-height:3450px;
}

#q2Frame{
  min-height:1750px;
}

#q3Frame{
  min-height:2200px;
}

#q4Frame{
  min-height:1900px;
}

.footer-note{
  text-align:center;
  color:#64748b;
  font-size:13px;
  margin-top:18px;
}

@media(max-width:800px){
  .navbar{
    align-items:flex-start;
    gap:12px;
    flex-direction:column;
  }

  .cards{
    grid-template-columns:1fr;
  }

  .hero h1{
    font-size:28px;
  }

  .question-frame{
    min-height:2400px;
  }

  #q1Frame{
    min-height:4300px;
  }
}
</style>
</head>

<body>
<header class="site-header">
  <div class="navbar">
    <div class="logo">ENGM 2010 Soil Mechanics</div>

    <nav class="nav-links">
      <button id="homeBtn" class="active" onclick="showPage('home')">Home</button>
      <button id="q1Btn" onclick="showPage('q1')">Q1</button>
      <button id="q2Btn" onclick="showPage('q2')">Q2</button>
      <button id="q3Btn" onclick="showPage('q3')">Q3</button>
      <button id="q4Btn" onclick="showPage('q4')">Q4</button>
    </nav>
  </div>
</header>

<main class="main-shell">

  <section id="home" class="home-panel">
    <div class="hero">
      <h1>ENGM 2010 Soil Mechanics</h1>
      <p>
        Exam practice portal with interactive question versions, answer checking,
        working-method buttons, solutions and examiner tips.
      </p>
    </div>

    <div class="cards">
      <div class="card">
        <h2>Question 1</h2>
        <p>Soil classification and phase relationships. Question 1(a) and 1(b) are linked with one version selector.</p>
        <button onclick="showPage('q1')">Start Question 1</button>
      </div>

      <div class="card">
        <h2>Question 2</h2>
        <p>Compaction test practice with dry unit weight graph and multiple practice versions.</p>
        <button onclick="showPage('q2')">Start Question 2</button>
      </div>

      <div class="card">
        <h2>Question 3</h2>
        <p>Constant head permeability test with SVG diagram, head values, effective stress and permeability.</p>
        <button onclick="showPage('q3')">Start Question 3</button>
      </div>

      <div class="card">
        <h2>Question 4</h2>
        <p>Preconsolidation pressure and OCR with recreated figures and practice versions.</p>
        <button onclick="showPage('q4')">Start Question 4</button>
      </div>
    </div>
  </section>

  <section id="q1" class="question-section">
    <iframe id="q1Frame" class="question-frame" src="geo_question_1_final_same_layout_ab.html"></iframe>
  </section>

  <section id="q2" class="question-section">
    <iframe id="q2Frame" class="question-frame" src="geo_question_2a_5_versions.html"></iframe>
  </section>

  <section id="q3" class="question-section">
    <iframe id="q3Frame" class="question-frame" src="geo_question_3_svg_versions.html"></iframe>
  </section>

  <section id="q4" class="question-section">
    <iframe id="q4Frame" class="question-frame" src="geo_question_4_ab_5_versions.html"></iframe>
  </section>

  <div class="footer-note">
    Use the navbar to move between questions without opening separate files.
  </div>
</main>

<script>
function showPage(pageId){
  const pages = ["home","q1","q2","q3","q4"];
  pages.forEach(id => {
    const section = document.getElementById(id);
    if(section){
      section.style.display = id === pageId ? (id === "home" ? "block" : "block") : "none";
    }

    const btn = document.getElementById(id + "Btn");
    if(btn){
      btn.classList.toggle("active", id === pageId);
    }
  });

  window.scrollTo({top:0, behavior:"smooth"});
}
</script>
</body>
</html>
