* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

html {
  background: #070b14;
}

body {
  background: #070b14;
  color: #f5f7ff;
  font-family: Arial, Helvetica, sans-serif;
}

a {
  color: inherit;
  text-decoration: none;
}

.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
  background: rgba(7, 11, 20, 0.85);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.08);
}

.nav-container {
  max-width: 1150px;
  margin: auto;
  height: 75px;
  padding: 0 25px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 28px;
  font-weight: 800;
}

.logo span {
  color: #7c5cff;
}

.nav-links {
  display: flex;
  gap: 30px;
}

.nav-links a {
  color: #b8c0d4;
  font-size: 15px;
  transition: 0.3s;
}

.nav-links a:hover {
  color: #ffffff;
}

.menu-btn {
  display: none;
  border: 0;
  background: none;
  color: white;
  font-size: 26px;
  cursor: pointer;
}

.hero {
  min-height: 100vh;
  max-width: 1150px;
  margin: auto;
  padding: 150px 25px 80px;

  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 70px;
  align-items: center;
}

.hello {
  color: #8d75ff;
  font-weight: 600;
  margin-bottom: 15px;
}

.hero h1 {
  font-size: clamp(48px, 7vw, 82px);
  line-height: 1;
  margin-bottom: 20px;
}

.hero h1 span {
  color: #8d75ff;
}

.hero h2 {
  font-size: 24px;
  line-height: 1.4;
  color: #c5ccdd;
  max-width: 650px;
}

.hero-text {
  margin-top: 25px;
  color: #8992a7;
  line-height: 1.8;
  max-width: 650px;
  font-size: 17px;
}

.hero-buttons {
  display: flex;
  gap: 15px;
  margin-top: 35px;
}

.btn {
  padding: 14px 24px;
  border-radius: 10px;
  font-weight: 600;
  display: inline-block;
  transition: 0.3s;
}

.btn.primary {
  background: #7c5cff;
  color: white;
}

.btn.primary:hover {
  transform: translateY(-3px);
  background: #6b4bea;
}

.btn.secondary {
  border: 1px solid #30384c;
  color: white;
}

.btn.secondary:hover {
  background: #151b29;
  transform: translateY(-3px);
}

.socials {
  display: flex;
  gap: 25px;
  margin-top: 30px;
}

.socials a {
  color: #aeb6c8;
}

.socials a:hover {
  color: #8d75ff;
}

.code-window {
  background: #0d1321;
  border: 1px solid #222b3d;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 25px 70px rgba(0, 0, 0, 0.4);
}

.window-top {
  height: 45px;
  padding: 0 18px;
  display: flex;
  align-items: center;
  gap: 8px;
  background: #111827;
}

.window-top span {
  width: 11px;
  height: 11px;
  border-radius: 50%;
  background: #384255;
}

.code-window pre {
  padding: 30px;
  overflow-x: auto;
  color: #cbd5e1;
  line-height: 1.7;
  font-size: 14px;
}

.section {
  max-width: 1150px;
  margin: auto;
  padding: 110px 25px;
}

.section-heading {
  text-align: center;
  margin-bottom: 55px;
}

.section-heading p {
  color: #8d75ff;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 2px;
  margin-bottom: 12px;
}

.section-heading h2 {
  font-size: 42px;
}

.about-grid {
  display: grid;
  grid-template-columns: 1.3fr 0.7fr;
  gap: 70px;
  align-items: center;
}

.about-grid h3 {
  font-size: 28px;
  margin-bottom: 20px;
}

.about-grid p {
  color: #929bad;
  line-height: 1.8;
  margin-bottom: 18px;
}

.info-card {
  background: #0d1321;
  border: 1px solid #20293b;
  border-radius: 16px;
  padding: 25px;
}

.info-item {
  display: flex;
  align-items: center;
  gap: 15px;
  padding: 18px 0;
  border-bottom: 1px solid #20293b;
}

.info-item:last-child {
  border-bottom: 0;
}

.info-item span {
  font-size: 25px;
}

.info-item div {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.info-item small {
  color: #778096;
}

.info-item strong {
  color: #e9edf5;
}

.skills-section {
  background: #0a0f1b;
  max-width: none;
}

.skills-section > * {
  max-width: 1100px;
  margin-left: auto;
  margin-right: auto;
}

.skills-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
}

.skill-card {
  padding: 16px 24px;
  border: 1px solid #252f43;
  border-radius: 10px;
  background: #0e1524;
  color: #cbd3e3;
  transition: 0.3s;
}

.skill-card:hover {
  border-color: #7c5cff;
  transform: translateY(-4px);
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

.project-card {
  background: #0d1321;
  border: 1px solid #20293b;
  border-radius: 16px;
  padding: 30px;
  transition: 0.3s;
}

.project-card:hover {
  transform: translateY(-7px);
  border-color: #7c5cff;
}

.project-icon {
  font-size: 30px;
  margin-bottom: 20px;
}

.project-card h3 {
  font-size: 22px;
  margin-bottom: 15px;
}

.project-card p {
  color: #8d96aa;
  line-height: 1.7;
  margin-bottom: 25px;
}

.project-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.project-tech span {
  padding: 7px 11px;
  background: #171f31;
  border-radius: 6px;
  font-size: 12px;
  color: #b5bdd0;
}

.timeline {
  max-width: 800px;
  margin: auto;
}

.timeline-item {
  position: relative;
  padding-left: 45px;
  padding-bottom: 45px;
  border-left: 1px solid #30394c;
}

.timeline-dot {
  position: absolute;
  left: -6px;
  top: 0;
  width: 11px;
  height: 11px;
  background: #7c5cff;
  border-radius: 50%;
}

.timeline-content span {
  color: #8d75ff;
  font-size: 13px;
  font-weight: bold;
}

.timeline-content h3 {
  font-size: 24px;
  margin: 10px 0 5px;
}

.timeline-content h4 {
  color: #aeb6c8;
  margin-bottom: 15px;
}

.timeline-content p {
  color: #858ea2;
  line-height: 1.7;
}

.contact-section {
  padding-bottom: 130px;
}

.contact-box {
  text-align: center;
  background: #0d1321;
  border: 1px solid #20293b;
  border-radius: 20px;
  padding: 70px 30px;
}

.contact-box > p:first-child {
  color: #8d75ff;
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
}

.contact-box h2 {
  font-size: 45px;
  margin: 15px 0;
}

.contact-box p {
  color: #8d96aa;
  max-width: 600px;
  margin: auto;
  line-height: 1.7;
}

.contact-buttons {
  margin-top: 30px;
  display: flex;
  justify-content: center;
  gap: 15px;
}

footer {
  border-top: 1px solid #1b2435;
  padding: 30px;
  text-align: center;
  color: #6e778b;
  font-size: 14px;
}

@media (max-width: 850px) {
  .hero {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .hero-card {
    order: -1;
  }

  .about-grid {
    grid-template-columns: 1fr;
  }

  .projects-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 650px) {
  .menu-btn {
    display: block;
  }

  .nav-links {
    display: none;
    position: absolute;
    top: 75px;
    left: 0;
    right: 0;
    padding: 25px;
    flex-direction: column;
    background: #0b101c;
    border-bottom: 1px solid #20293b;
  }

  .nav-links.open {
    display: flex;
  }

  .hero {
    padding-top: 125px;
  }

  .hero h1 {
    font-size: 52px;
  }

  .hero h2 {
    font-size: 20px;
  }

  .hero-buttons {
    flex-direction: column;
  }

  .btn {
    text-align: center;
  }

  .section-heading h2 {
    font-size: 34px;
  }

  .contact-box h2 {
    font-size: 34px;
  }

  .code-window pre {
    font-size: 12px;
  }
}
