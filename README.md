"use client";

import { useState } from "react";

export default function Home() {
  const [menuOpen, setMenuOpen] = useState(false);

  const skills = [
    "Python",
    "SQL",
    "Java",
    "Pandas",
    "NumPy",
    "Git",
    "GitHub",
    "AWS",
    "Google Cloud",
    "Data Analytics",
    "Data Engineering",
    "Automation",
  ];

  const projects = [
    {
      title: "Python Data Analysis",
      description:
        "Data analysis projects using Python, Pandas, NumPy and Jupyter Notebook.",
      tech: ["Python", "Pandas", "NumPy"],
    },
    {
      title: "Cloud Data Engineering",
      description:
        "Learning and building data engineering workflows with cloud technologies, Python and SQL.",
      tech: ["Python", "SQL", "Cloud"],
    },
    {
      title: "Web Scraping Project",
      description:
        "A data collection project focused on web scraping, cleaning datasets and preparing data for databases.",
      tech: ["Python", "Web Scraping", "SQL"],
    },
  ];

  return (
    <main>
      {/* Navigation */}
      <nav className="navbar">
        <div className="nav-container">
          <a href="#" className="logo">
            MB<span>.</span>
          </a>

          <button
            className="menu-btn"
            onClick={() => setMenuOpen(!menuOpen)}
          >
            ☰
          </button>

          <div className={`nav-links ${menuOpen ? "open" : ""}`}>
            <a href="#home" onClick={() => setMenuOpen(false)}>
              Home
            </a>
            <a href="#about" onClick={() => setMenuOpen(false)}>
              About
            </a>
            <a href="#skills" onClick={() => setMenuOpen(false)}>
              Skills
            </a>
            <a href="#projects" onClick={() => setMenuOpen(false)}>
              Projects
            </a>
            <a href="#contact" onClick={() => setMenuOpen(false)}>
              Contact
            </a>
          </div>
        </div>
      </nav>

      {/* Hero */}
      <section id="home" className="hero">
        <div className="hero-content">
          <p className="hello">Hello, I'm</p>

          <h1>
            Muhammad <span>Bilal</span>
          </h1>

          <h2>BS Computer Science Student & Data Professional in Training</h2>

          <p className="hero-text">
            I'm passionate about Python, Data Analytics, Data Engineering and
            Cloud Technologies. I enjoy turning raw data into useful insights
            and building practical solutions with code.
          </p>

          <div className="hero-buttons">
            <a href="#projects" className="btn primary">
              View My Projects
            </a>

            <a href="#contact" className="btn secondary">
              Contact Me
            </a>
          </div>

          <div className="socials">
            <a
              href="https://github.com/M-Bilal-CDE"
              target="_blank"
              rel="noopener noreferrer"
            >
              GitHub
            </a>

            <a
              href="https://www.linkedin.com/in/muhammad-bilal-82348a37a"
              target="_blank"
              rel="noopener noreferrer"
            >
              LinkedIn
            </a>
          </div>
        </div>

        <div className="hero-card">
          <div className="code-window">
            <div className="window-top">
              <span></span>
              <span></span>
              <span></span>
            </div>

            <pre>
{`const bilal = {
  education: "BS Computer Science",
  focus: [
    "Python",
    "Data Analytics",
    "Data Engineering",
    "Cloud"
  ],
  goal: "Build useful solutions",
  status: "Always Learning 🚀"
};`}
            </pre>
          </div>
        </div>
      </section>

      {/* About */}
      <section id="about" className="section">
        <div className="section-heading">
          <p>GET TO KNOW ME</p>
          <h2>About Me</h2>
        </div>

        <div className="about-grid">
          <div>
            <h3>Who am I?</h3>

            <p>
              I'm Muhammad Bilal, a BS Computer Science student at Iqra
              University with a strong interest in Data Analytics, Data
              Engineering and Cloud Technologies.
            </p>

            <p>
              I'm currently developing my technical skills through practical
              projects and continuous learning. My main focus is Python, SQL,
              data processing and cloud technologies.
            </p>

            <p>
              I believe in learning by building. My goal is to create
              practical projects that solve real-world problems and continue
              growing as a technology professional.
            </p>
          </div>

          <div className="info-card">
            <div className="info-item">
              <span>🎓</span>
              <div>
                <small>Education</small>
                <strong>BS Computer Science</strong>
              </div>
            </div>

            <div className="info-item">
              <span>🐍</span>
              <div>
                <small>Main Language</small>
                <strong>Python</strong>
              </div>
            </div>

            <div className="info-item">
              <span>☁️</span>
              <div>
                <small>Current Focus</small>
                <strong>Cloud Data Engineering</strong>
              </div>
            </div>

            <div className="info-item">
              <span>📊</span>
              <div>
                <small>Interest</small>
                <strong>Data Analytics</strong>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Skills */}
      <section id="skills" className="section skills-section">
        <div className="section-heading">
          <p>MY TOOLKIT</p>
          <h2>Skills & Technologies</h2>
        </div>

        <div className="skills-container">
          {skills.map((skill) => (
            <div className="skill-card" key={skill}>
              {skill}
            </div>
          ))}
        </div>
      </section>

      {/* Projects */}
      <section id="projects" className="section">
        <div className="section-heading">
          <p>MY WORK</p>
          <h2>Featured Projects</h2>
        </div>

        <div className="projects-grid">
          {projects.map((project) => (
            <div className="project-card" key={project.title}>
              <div className="project-icon">🚀</div>

              <h3>{project.title}</h3>

              <p>{project.description}</p>

              <div className="project-tech">
                {project.tech.map((tech) => (
                  <span key={tech}>{tech}</span>
                ))}
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* Education */}
      <section className="section education-section">
        <div className="section-heading">
          <p>MY JOURNEY</p>
          <h2>Education & Learning</h2>
        </div>

        <div className="timeline">
          <div className="timeline-item">
            <div className="timeline-dot"></div>

            <div className="timeline-content">
              <span>Current</span>
              <h3>BS Computer Science</h3>
              <h4>Iqra University</h4>
              <p>
                Studying computer science with a focus on programming,
                software development and computing fundamentals.
              </p>
            </div>
          </div>

          <div className="timeline-item">
            <div className="timeline-dot"></div>

            <div className="timeline-content">
              <span>Professional Training</span>
              <h3>Cloud Data Engineering</h3>
              <h4>Saylani Mass IT Training</h4>
              <p>
                Developing practical skills in Python, data engineering,
                databases, cloud technologies and automation.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="section contact-section">
        <div className="contact-box">
          <p>LET'S CONNECT</p>

          <h2>Have a project in mind?</h2>

          <p>
            I'm always interested in learning, collaborating and working on
            interesting technology projects.
          </p>

          <div className="contact-buttons">
            <a
              href="https://github.com/M-Bilal-CDE"
              target="_blank"
              rel="noopener noreferrer"
              className="btn primary"
            >
              GitHub
            </a>

            <a
              href="https://www.linkedin.com/in/muhammad-bilal-82348a37a"
              target="_blank"
              rel="noopener noreferrer"
              className="btn secondary"
            >
              LinkedIn
            </a>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer>
        <p>
          © {new Date().getFullYear()} Muhammad Bilal. Built with Next.js.
        </p>
      </footer>
    </main>
  );
}
