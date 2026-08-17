<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hashim Ali | Safety Inspector & HSE Professional</title>

<!-- FontAwesome Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
:root {
  --bg-main: #030712;
  --bg-card: #0b0f19;
  --bg-card-hover: #111827;
  --accent-cyan: #00f2fe;
  --accent-purple: #a855f7;
  --accent-blue: #3b82f6;
  --accent-glow: rgba(0, 242, 254, 0.4);
  --text-main: #f8fafc;
  --text-muted: #94a3b8;
  --border-color: rgba(255, 255, 255, 0.08);
  --border-hover: rgba(0, 242, 254, 0.5);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Inter', 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
  -webkit-tap-highlight-color: transparent;
}

::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: var(--bg-main);
}

::-webkit-scrollbar-thumb {
  background: #1e293b;
  border-radius: 4px;
}

::-webkit-scrollbar-thumb:hover {
  background: var(--accent-cyan);
}

body {
  background-color: var(--bg-main);
  color: var(--text-main);
  line-height: 1.6;
  overflow-x: hidden;
  background-image:
    radial-gradient(circle at 10% 20%, rgba(0, 242, 254, 0.08) 0%, transparent 40%),
    radial-gradient(circle at 90% 80%, rgba(168, 85, 247, 0.08) 0%, transparent 40%);
}

header {
  background: linear-gradient(135deg, rgba(11, 15, 25, 0.95), rgba(3, 7, 18, 0.98)),
              url('https://images.unsplash.com/photo-1504917595217-d4dc5ebe6122?auto=format&fit=crop&w=1200&q=80');
  background-size: cover;
  background-position: center;
  padding: 80px 20px 60px;
  text-align: center;
  border-bottom: 1px solid var(--border-color);
  position: relative;
}

header::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 80%;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--accent-cyan), var(--accent-purple), transparent);
}

.profile-img-container {
  display: inline-block;
  cursor: pointer;
  position: relative;
  margin-bottom: 25px;
  z-index: 100;
  user-select: none;
}

.profile-img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid var(--accent-cyan);
  box-shadow: 0 0 35px var(--accent-glow);
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  pointer-events: none;
}

.profile-img-container.zoomed .profile-img {
  transform: scale(2.1);
  box-shadow: 0 0 80px rgba(0, 242, 254, 0.9), 0 0 120px rgba(168, 85, 247, 0.6);
  border-color: #ffffff;
}

.profile-social-bar {
  display: flex;
  justify-content: center;
  gap: 12px;
  flex-wrap: wrap;
  margin-bottom: 28px;
}

.social-pill {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 10px 18px;
  background: rgba(255, 255, 255, 0.04);
  border: 1px solid var(--border-color);
  border-radius: 30px;
  color: var(--text-main);
  text-decoration: none;
  font-size: 13px;
  font-weight: 500;
  backdrop-filter: blur(10px);
  transition: all 0.3s ease;
  cursor: pointer;
}

.social-pill i {
  color: var(--accent-cyan);
  font-size: 15px;
  pointer-events: none;
}

.social-pill.selected {
  background: rgba(0, 242, 254, 0.2);
  border-color: var(--accent-cyan);
  color: #fff;
  transform: translateY(-3px) scale(1.05);
  box-shadow: 0 0 25px rgba(0, 242, 254, 0.5);
}

header h1 {
  font-size: 46px;
  font-weight: 800;
  letter-spacing: -0.5px;
  background: linear-gradient(90deg, #ffffff 30%, var(--accent-cyan), var(--accent-purple));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 8px;
  text-shadow: 0 0 40px rgba(0, 242, 254, 0.2);
}

header p {
  font-size: 17px;
  color: var(--accent-cyan);
  margin-bottom: 28px;
  font-weight: 600;
  letter-spacing: 0.5px;
}

.header-btns {
  display: flex;
  justify-content: center;
  gap: 16px;
  flex-wrap: wrap;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 12px 26px;
  background: rgba(255, 255, 255, 0.03);
  color: var(--text-main);
  text-decoration: none;
  border-radius: 14px;
  font-weight: 600;
  font-size: 14px;
  border: 1px solid var(--border-color);
  backdrop-filter: blur(12px);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
}

.btn.selected {
  background: rgba(0, 242, 254, 0.2);
  border-color: var(--accent-cyan);
  color: #fff;
  transform: translateY(-4px) scale(1.03);
  box-shadow: 0 0 30px rgba(0, 242, 254, 0.5);
}

.btn-primary {
  background: linear-gradient(135deg, #00f2fe, #3b82f6);
  color: #030712;
  border: none;
  font-weight: 700;
  box-shadow: 0 4px 25px rgba(0, 242, 254, 0.4);
}

.btn-primary.selected {
  background: linear-gradient(135deg, #3b82f6, #00f2fe);
  color: #fff;
  box-shadow: 0 6px 35px rgba(0, 242, 254, 0.8);
}

section {
  max-width: 1050px;
  margin: auto;
  padding: 55px 20px;
}

h2 {
  font-size: 28px;
  margin-bottom: 30px;
  color: #fff;
  display: flex;
  align-items: center;
  gap: 14px;
  font-weight: 700;
}

h2 i {
  color: var(--accent-cyan);
  text-shadow: 0 0 15px var(--accent-glow);
}

h2::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(90deg, var(--border-hover), transparent);
  margin-left: 15px;
}

.about-glowing-wrapper {
  position: relative;
  border-radius: 22px;
  padding: 2px;
  overflow: hidden;
  cursor: pointer;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.4);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  max-width: 800px;
  margin: 0 auto;
}

.about-glowing-wrapper:hover {
  transform: translateY(-4px);
  box-shadow: 0 15px 45px rgba(0, 242, 254, 0.25);
}

.about-glowing-wrapper::before {
  content: '';
  position: absolute;
  inset: -50%;
  background: conic-gradient(from 0deg at 50% 50%, transparent 0deg, var(--accent-cyan) 90deg, var(--accent-purple) 180deg, transparent 270deg, transparent 360deg);
  animation: rotateLight 4s linear infinite;
}

@keyframes rotateLight {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.about {
  position: relative;
  background: var(--bg-card);
  padding: 35px;
  border-radius: 20px;
  font-size: 16px;
  color: var(--text-muted);
  text-align: center !important;
  z-index: 1;
}

.about p {
  text-align: center !important;
  margin: 0 auto;
}

.skills {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
}

.skill {
  background: var(--bg-card);
  padding: 24px;
  border-radius: 16px;
  text-align: left;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  border: 1px solid var(--border-color);
  display: flex;
  align-items: center;
  gap: 16px;
  cursor: pointer;
}

.skill i {
  font-size: 26px;
  color: var(--accent-cyan);
  transition: transform 0.3s ease;
}

.skill h3 {
  font-size: 15px;
  color: var(--text-main);
  font-weight: 600;
}

.skill:hover {
  transform: translateY(-6px);
  border-color: var(--accent-cyan);
  background: var(--bg-card-hover);
  box-shadow: 0 12px 35px rgba(0, 242, 254, 0.15);
}

.skill:hover i {
  transform: scale(1.25) rotate(5deg);
  color: var(--accent-purple);
}

.projects {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}

.card {
  background: var(--bg-card);
  padding: 30px;
  border-radius: 20px;
  border: 1px solid var(--border-color);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: relative;
  overflow: hidden;
  cursor: pointer;
}

.card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, var(--accent-cyan), var(--accent-purple));
  opacity: 0;
  transition: opacity 0.3s ease;
}

.card:hover {
  border-color: var(--border-hover);
  transform: translateY(-8px);
  box-shadow: 0 20px 45px rgba(0, 0, 0, 0.6), 0 0 25px rgba(0, 242, 254, 0.2);
}

.card:hover::before {
  opacity: 1;
}

.card h3 {
  color: var(--accent-cyan);
  margin-bottom: 14px;
  font-size: 20px;
  font-weight: 700;
}

.card p {
  color: var(--text-muted);
  font-size: 14px;
  margin-bottom: 20px;
}

.tags {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
}

.tag {
  background: rgba(0, 242, 254, 0.06);
  color: var(--accent-cyan);
  padding: 6px 14px;
  border-radius: 10px;
  font-size: 12px;
  font-weight: 600;
  border: 1px solid rgba(0, 242, 254, 0.15);
}

.education-container {
  display: flex;
  justify-content: center;
}

.contact-container {
  display: flex;
  justify-content: center;
}

.thm-badge-card {
  background: var(--bg-card);
  padding: 30px;
  border-radius: 20px;
  border: 1px solid var(--border-color);
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.4);
  width: 100%;
  max-width: 800px;
  text-align: center;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.thm-badge-card:hover {
  border-color: var(--border-hover);
  transform: translateY(-8px);
  box-shadow: 0 20px 45px rgba(0, 0, 0, 0.6), 0 0 25px rgba(0, 242, 254, 0.2);
}

footer {
  text-align: center;
  padding: 40px;
  background: var(--bg-card);
  margin-top: 70px;
  border-top: 1px solid var(--border-color);
  color: var(--text-muted);
  font-size: 14px;
}

@media (max-width: 600px) {
  header h1 { font-size: 32px; }
  header p { font-size: 15px; }
  .header-btns { flex-direction: column; }
  .profile-social-bar { gap: 8px; }
  .social-pill { padding: 8px 14px; font-size: 12px; }
}
</style>
</head>

<body>

<header>

  <div class="profile-img-container" id="profileImgContainer" title="Click to zoom profile photo">
    <img class="profile-img"
         id="profileImg"
         src="https://github.com/hashimsafetyinspector.png"
         alt="Hashim Ali">
  </div>

  <div class="profile-social-bar">

    <a class="social-pill two-click-link"
       data-href="https://github.com/hashimsafetyinspector">
      <i class="fab fa-github"></i> GitHub
    </a>

    <a class="social-pill two-click-link"
       data-href="https://www.linkedin.com/"
       target="_blank">
      <i class="fab fa-linkedin"></i> LinkedIn
    </a>

  </div>

  <h1>Hashim Ali</h1>
  <p>Safety Inspector | HSE Professional | Professional Safety Adviser</p>

  <div class="header-btns">

    <a class="btn btn-primary two-click-link"
       data-href="https://www.linkedin.com/"
       target="_blank">
      <i class="fab fa-linkedin"></i> Connect on LinkedIn
    </a>

    <a class="btn two-click-link"
       data-href="https://github.com/hashimsafetyinspector"
       target="_blank">
      <i class="fab fa-github"></i> Visit GitHub
    </a>

  </div>

</header>


<section>

  <h2>
    <i class="fas fa-user-shield"></i>
    About Me
  </h2>

  <div class="about-glowing-wrapper" id="aboutWrapper">

    <div class="about">

      <p>
        I am a dedicated Safety Inspector and HSE professional with a strong focus on workplace safety,
        hazard identification, risk awareness and safe working practices. I have completed professional
        safety training including NEBOSH IGC, IOSH and OSHA, along with HSE training. I am committed
        to promoting a safe working environment and supporting organizations in maintaining effective
        health and safety standards.
      </p>

    </div>

  </div>

</section>


<section>

  <h2>
    <i class="fas fa-hard-hat"></i>
    Core Skills
  </h2>

  <div class="skills">

    <div class="skill">
      <i class="fas fa-shield-halved"></i>
      <h3>Workplace Safety</h3>
    </div>

    <div class="skill">
      <i class="fas fa-triangle-exclamation"></i>
      <h3>Hazard Identification</h3>
    </div>

    <div class="skill">
      <i class="fas fa-clipboard-check"></i>
      <h3>Safety Inspection</h3>
    </div>

    <div class="skill">
      <i class="fas fa-person-falling-burst"></i>
      <h3>Risk Awareness</h3>
    </div>

    <div class="skill">
      <i class="fas fa-file-word"></i>
      <h3>MS Word</h3>
    </div>

    <div class="skill">
      <i class="fas fa-file-excel"></i>
      <h3>MS Excel</h3>
    </div>

    <div class="skill">
      <i class="fas fa-file-powerpoint"></i>
      <h3>MS PowerPoint</h3>
    </div>

    <div class="skill">
      <i class="fas fa-computer"></i>
      <h3>Computer Skills</h3>
    </div>

  </div>

</section>


<section>

  <h2>
    <i class="fas fa-briefcase"></i>
    Professional Experience
  </h2>

  <div class="projects">

    <div class="card">

      <div>

        <h3>Safety Inspector</h3>

        <p>
          Responsible for supporting workplace safety practices, identifying potential hazards,
          observing safe working procedures and promoting a safe working environment.
        </p>

      </div>

      <div class="tags">
        <span class="tag">Safety</span>
        <span class="tag">HSE</span>
        <span class="tag">Inspection</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>MS Office — 1 Year Experience</h3>

        <p>
          One year of practical experience using Microsoft Word, Excel, PowerPoint and InPage
          for documentation, data management and office-related tasks.
        </p>

      </div>

      <div class="tags">
        <span class="tag">MS Word</span>
        <span class="tag">Excel</span>
        <span class="tag">PowerPoint</span>
        <span class="tag">InPage</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>Embroidery Machine Operator</h3>

        <p>
          One year of experience working as an Embroidery Machine Operator with practical
          experience in machine operation and production-related work.
        </p>

      </div>

      <div class="tags">
        <span class="tag">Machine Operation</span>
        <span class="tag">Production</span>
        <span class="tag">Quality</span>
      </div>

    </div>

  </div>

</section>


<section>

  <h2>
    <i class="fas fa-certificate"></i>
    Certifications & Training
  </h2>

  <div class="projects">

    <div class="card">

      <div>

        <h3>NEBOSH IGC</h3>

        <p>
          NEBOSH International General Certificate focused on occupational health and safety
          principles and workplace risk management.
        </p>

      </div>

      <div class="tags">
        <span class="tag">NEBOSH</span>
        <span class="tag">IGC</span>
        <span class="tag">Safety</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>IOSH — 30 Hours</h3>

        <p>
          Completed 30 hours of IOSH safety training with focus on workplace health and safety.
        </p>

      </div>

      <div class="tags">
        <span class="tag">IOSH</span>
        <span class="tag">30 Hours</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>OSHA — 48 Hours</h3>

        <p>
          Completed 48 hours of OSHA-related safety training covering workplace safety
          awareness and hazard prevention.
        </p>

      </div>

      <div class="tags">
        <span class="tag">OSHA</span>
        <span class="tag">48 Hours</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>HSE Training</h3>

        <p>
          Completed a 3-month HSE training program focused on health, safety and environmental
          workplace practices.
        </p>

      </div>

      <div class="tags">
        <span class="tag">HSE</span>
        <span class="tag">3 Months</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>Professional Safety Adviser</h3>

        <p>
          Professional safety training focused on supporting organizations in maintaining
          effective workplace health and safety practices.
        </p>

      </div>

      <div class="tags">
        <span class="tag">Safety Adviser</span>
        <span class="tag">HSE</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>Computer Basic Course</h3>

        <p>
          Basic computer training covering essential computer operations and office productivity.
        </p>

      </div>

      <div class="tags">
        <span class="tag">Computer</span>
        <span class="tag">Basic IT</span>
      </div>

    </div>


    <div class="card">

      <div>

        <h3>Master in MS Office</h3>

        <p>
          Training in Microsoft Word, Microsoft Excel, Microsoft PowerPoint and InPage.
        </p>

      </div>

      <div class="tags">
        <span class="tag">Word</span>
        <span class="tag">Excel</span>
        <span class="tag">PowerPoint</span>
        <span class="tag">InPage</span>
      </div>

    </div>

  </div>

</section>


<section>

  <h2>
    <i class="fas fa-graduation-cap"></i>
    Education
  </h2>

  <div class="education-container">

    <div class="card" style="width: 100%; max-width: 800px;">

      <div>

        <h3>FSc — 70%</h3>

        <p>
          Intermediate / FSc education completed with 70% marks.
        </p>

        <div class="tags">
          <span class="tag">FSc</span>
          <span class="tag">70%</span>
        </div>

        <br>

        <h3>Matric — 80%</h3>

        <p>
          Matriculation completed with 80% marks.
        </p>

        <div class="tags">
          <span class="tag">Matric</span>
          <span class="tag">80%</span>
        </div>

      </div>

    </div>

  </div>

</section>


<section>

  <h2>
    <i class="fas fa-user-tie"></i>
    Professional Profile
  </h2>

  <div class="contact-container">

    <div class="thm-badge-card">

      <h3 style="color:#fff; font-size:20px; margin-bottom:15px;">
        <i class="fas fa-hard-hat" style="color:var(--accent-cyan);"></i>
        Safety Inspector & HSE Professional
      </h3>

      <p style="color:var(--text-muted);">
        Dedicated to workplace safety, hazard identification, risk awareness,
        HSE practices and maintaining a safe working environment.
      </p>

    </div>

  </div>

</section>


<footer>

  <p>
    © 2026 Hashim Ali | Safety Inspector & HSE Professional
  </p>

</footer>


<script>

function vibrate(pattern = [80]) {
  if ('vibrate' in navigator) {
    try {
      navigator.vibrate(pattern);
    } catch (e) {}
  }
}


document.querySelectorAll(
  '.skill, .card, .thm-badge-card, .about-glowing-wrapper'
).forEach(elem => {

  elem.addEventListener('click', () => vibrate([60]));

});


const profileBox = document.getElementById('profileImgContainer');

if (profileBox) {

  profileBox.addEventListener('click', (e) => {

    e.stopPropagation();

    profileBox.classList.toggle('zoomed');

    vibrate([120, 50, 120]);

  });


  document.addEventListener('click', (e) => {

    if (!profileBox.contains(e.target)) {

      profileBox.classList.remove('zoomed');

    }

  });

}


const twoClickLinks = document.querySelectorAll('.two-click-link');

twoClickLinks.forEach(link => {

  link.addEventListener('click', function(e) {

    e.preventDefault();
    e.stopPropagation();

    if (this.classList.contains('selected')) {

      const targetUrl = this.getAttribute('data-href');
      const isBlank = this.getAttribute('target') === '_blank';

      vibrate([50, 50, 100]);

      if (isBlank) {

        window.open(targetUrl, '_blank');

      } else {

        window.location.href = targetUrl;

      }

      this.classList.remove('selected');

    } else {

      document.querySelectorAll('.two-click-link')
        .forEach(item => item.classList.remove('selected'));

      this.classList.add('selected');

      vibrate([60]);

    }

  });

});

</script>

</body>
</html>
