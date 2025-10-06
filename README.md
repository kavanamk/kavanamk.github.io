<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kavana Manvi — Portfolio / Resume</title>

  <style>
    /* ---------- Global ---------- */
    :root{
      --accent: #2a7ae2;
      --muted-bg: #f3f3f3;
      --nav-bg: #e9f0fc;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      line-height: 1.45;
      color: #222;
      background: #fff;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }

    img {
      max-width: 100%;
      height: auto;
      display: block;
    }

    h2, h3 {
      color: var(--accent);
      margin: 0.6rem 0;
    }

    /* ---------- Tabs navigation - responsive ---------- */
    .tabs-wrap { /* container to allow drop-shadow separation */
      position: sticky;
      top: 0;
      z-index: 1000;
      background: var(--nav-bg);
      border-bottom: 1px solid #ccc;
    }

    .tabs-nav {
      display: flex;
      gap: 1rem;
      padding: 0.6rem;
      align-items: center;
      justify-content: center;

      /* Important for mobile: allow horizontal scroll when needed */
      overflow-x: auto;
      -webkit-overflow-scrolling: touch; /* smooth kinetic scrolling on iOS */
      white-space: nowrap; /* keep link items on a single scrollable row */
      box-sizing: border-box;
    }

    /* make each tab behave like an inline pill and stay tappable */
    .tab-link {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      flex: 0 0 auto;             /* don't shrink, don't stretch */
      font-size: 1rem;
      font-weight: 600;
      color: var(--accent);
      text-decoration: none;
      padding: 0.45rem 0.9rem;
      border-radius: 6px;
      transition: background-color 0.18s ease, transform 0.18s ease;
      margin: 0 0.15rem;
      box-sizing: border-box;
    }

    /* hover / focus states */
    .tab-link:hover,
    .tab-link:focus {
      background-color: #dce6f9;
      outline: none;
      transform: translateY(-2px);
    }

    /* active state */
    .tab-link.active {
      background-color: var(--accent);
      color: #fff;
    }

    /* focus visible for keyboard users */
    .tab-link:focus-visible {
      box-shadow: 0 0 0 3px rgba(42,122,226,0.18);
    }

    /* ---------- Main container ---------- */
    .container {
      max-width: 1100px;
      margin: 1.25rem auto;
      padding: 0 1rem;
    }

    .hero-image {
      display: block;
      margin: 1rem auto;
      max-width: 900px;
      border-radius: 8px;
      object-fit: cover;
    }

    .center {
      text-align: center;
    }

    /* ---------- Link boxes (roles/projects shortcuts) ---------- */
    .link-boxes {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin: 2rem auto;
      max-width: 1200px;
      flex-wrap: wrap; /* Allow wrapping on smaller screens */
    }

    .link-box {
      flex: 1 1 220px; /* base width ~220px, will wrap as needed */
      min-width: 180px;
      max-width: 300px;
      background-color: var(--muted-bg);
      border: 1px solid #ccc;
      border-radius: 8px;
      padding: 1.5rem;
      text-align: center;
      font-family: 'Helvetica Neue', sans-serif;
      font-size: 1.05rem;
      color: var(--accent);
      text-decoration: none;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .link-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 10px rgba(0, 0, 0, 0.08);
    }

    /* ---------- Content blocks ---------- */
    .section {
      padding: 1rem 0 2rem 0;
      border-bottom: 0px solid #eee;
    }

    .edu-list, .skills-list {
      margin: 0.5rem 0 1rem 0;
      padding-left: 1rem;
    }

    .skill-tag {
      background-color: #dce6f9;
      color: var(--accent);
      font-size: 0.85rem;
      padding: 0.3rem 0.6rem;
      border-radius: 999px;
      margin: 0.2rem;
      display: inline-block;
      font-weight: 500;
    }

    /* ---------- Project grid ---------- */
    .project-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1.25rem;
      max-width: 900px;
      margin: 1.25rem auto;
    }

    .project-box {
      background-color: var(--muted-bg);
      border: 1px solid #ccc;
      border-radius: 12px;
      padding: 1.25rem;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-decoration: none;
      color: inherit;
      display: block;
    }

    .project-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 10px rgba(0,0,0,0.06);
    }

    .project-title { font-size: 1.12rem; font-weight: 600; color: var(--accent); margin-bottom: 0.25rem; }
    .project-description { font-size: 0.98rem; margin-bottom: 0.8rem; color: #333; }

    /* ---------- Certificate cards ---------- */
    .course-card {
      border: 1px solid #ddd;
      padding: 1rem;
      border-radius: 8px;
      max-width: 900px;
      margin: 1rem auto;
      box-shadow: 0 2px 8px rgba(0,0,0,0.03);
    }

    /* ---------- Responsive tweaks ---------- */
    @media (max-width: 880px) {
      .container { padding: 0 0.8rem; }
      .project-grid { gap: 1rem; }
    }

    @media (max-width: 640px) {
      .tabs-nav { gap: 0.5rem; padding: 0.4rem; }
      .tab-link { font-size: 0.92rem; padding: 0.4rem 0.75rem; border-radius: 6px; }
      .hero-image { margin: 0.6rem 0; border-radius: 6px; }
      .link-box { padding: 1rem; font-size: 0.98rem; min-width: 140px; }
    }

    /* Optional small-screen layout: stack project boxes more tightly */
    @media (max-width: 480px) {
      .project-grid { gap: 0.8rem; }
      .link-boxes { gap: 0.9rem; }
    }

    /* small visual helpers */
    .muted { color: #666; font-size: 0.95rem; }
    .bullet { margin-left: 1rem; margin-bottom: 0.35rem; }

  </style>
</head>
<body>

  <!-- Sticky tab nav -->
  <div class="tabs-wrap" aria-label="Primary navigation">
    <nav class="tabs-nav" role="navigation">
      <a href="#work-experience" class="tab-link" id="link-work">Work</a>
      <a href="#skills" class="tab-link" id="link-skills">Skills</a>
      <a href="#projects" class="tab-link" id="link-projects">Projects</a>
      <a href="#certificates" class="tab-link" id="link-certificates">Certificates</a>
    </nav>
  </div>

  <main class="container" role="main">
    <!-- Hero image -->
    <img src="images/LLM-13.jpg" alt="LLM hero" class="hero-image" />

    <h3 class="center" style="color: var(--accent);">I'd be a great fit for these roles</h3>

    <!-- Short link boxes -->
    <div class="link-boxes" role="list">
      <a class="link-box" href="https://github.com/kavanamk/Educative-DSA" target="_blank" rel="noopener noreferrer" role="listitem">DSA</a>
      <a class="link-box" href="https://github.com/kavanamk/Educative-System-Design" target="_blank" rel="noopener noreferrer" role="listitem">System Design</a>
      <a class="link-box" href="#projects" role="listitem">Projects</a>
      <a class="link-box" href="#work-experience" role="listitem">Work Experience</a>
    </div>

    <!-- EDUCATION -->
    <section class="section" id="education">
      <h2>EDUCATION</h2>

      <h3>Master of Science, Computer Science</h3>
      <p class="muted"><img src="images/depaul.jpg" width="26" alt="DePaul logo" style="vertical-align:middle; margin-right:6px;" /> DePaul University, Chicago (GPA - 3.86)</p>
      <ul class="edu-list">
        <li><strong>Foundational CS courses:</strong> Object oriented programming, Distributed System, Database management system, Computer Programming, Algorithms and Data structures</li>
        <li><strong>Foundational Data Science courses:</strong> Fundamentals of Data Science in R, Data Visualization, Data Regression and analysis, Image Processing</li>
        <li><strong>Advanced Data Science courses:</strong> Programming Machine Learning Algorithms, Advanced Machine Learning, Computer Vision</li>
      </ul>

      <h3>Bachelor of Science, Computer Science</h3>
      <p class="muted"><img src="images/nieit.jpg" width="26" alt="NIE logo" style="vertical-align:middle; margin-right:6px;" /> NIE, India</p>
      <p class="muted">Courses: Mathematics, Physics, Chemistry Statistics, Data Structure, Algorithms, Compiler Design, Cybersecurity, Internet of things, UI Design, Microprocessor and Assembly language, Java, J2EE, Database, Computer Architecture, OpenGL, Computer Graphics, Big Data, Data mining, Artificial Intelligence, Software Engineering, Unix</p>
    </section>

    <!-- WORK EXPERIENCE -->
    <section class="section" id="work-experience" tabindex="-1">
      <h2>WORK EXPERIENCE</h2>

      <article style="margin-top:0.6rem;">
        <h3><img src="images/oracle.jpg" width="28" alt="Oracle logo" style="vertical-align:middle; margin-right:6px;" /> Software Engineer at Oracle</h3>
        <ul class="edu-list">
          <li class="bullet">Performed Defect correction and management of ETL scripts and reports produced using SQL, OCI and Tableau.</li>
          <li class="bullet">Led full-stack development for 75+ Jira tickets, handling issue analysis, design, implementation, and testing.</li>
          <li class="bullet">Improved code runtime from 6–7 hours to 40 seconds, earning 2022 “Innovate and Simplify” Quarterly Award.</li>
          <li class="bullet">Recognised twice as “Star of the Sprint” for exceeding expectations with additional testing alongside sprint deliverables, removing roadblocks.</li>
          <li class="bullet">Conducted 35+ client issue investigations over 6 months to identify root causes.</li>
        </ul>
      </article>

      <article style="margin-top:1rem;">
        <h3><img src="images/oracle.jpg" width="28" alt="Oracle logo" style="vertical-align:middle; margin-right:6px;" /> Software Intern at Oracle</h3>
        <ul class="edu-list">
          <li class="bullet">Developed full-stack web features for internal business performance application (eBoard) using ReactJS, Spring Boot, PHP, SQL, HTML, CSS, JavaScript, jQuery, and AJAX.</li>
          <li class="bullet">Delivered 6+ data visualization dashboards displaying Jenkins job execution status, improving visibility for 30+ revenue cycle teams.</li>
          <li class="bullet">Created summary and drill-down analytics reports used by directors and senior managers for performance oversight.</li>
        </ul>
      </article>
    </section>

    <!-- SKILLS -->
    <section class="section" id="skills" tabindex="-1">
      <h2>SKILLS</h2>
      <p class="muted"><strong>Programming Languages:</strong> C, C++, Java, T-SQL, PL/SQL, Python, Scala, Apache Spark, R, MySQL</p>
      <p class="muted"><strong>Web Technology:</strong> HTML, CSS, JavaScript, PHP, jQuery, AJAX, ReactJS, JSON, XML</p>
      <p class="muted"><strong>Machine Learning:</strong> TensorFlow, Octave, MATLAB, Tableau, PyTorch, deep learning</p>
      <p class="muted"><strong>Others:</strong> Git, SVM, Excel, MS Office, SDLC – Agile and Jira, Jenkins, CI/CD</p>
      <p class="muted"><strong>Soft skills:</strong> effective communication, problem-solving, critical thinking, growth mindset, curiosity</p>

      <div style="margin-top:0.8rem;">
        <strong>I'm also an Expert in Data Structures, Algorithms and System design</strong>
      </div>

      <div class="link-boxes" style="max-width:600px; margin-top:1rem;">
        <a class="link-box" href="https://github.com/kavanamk/Educative-DSA" target="_blank" rel="noopener noreferrer">DSA</a>
        <a class="link-box" href="https://github.com/kavanamk/Educative-System-Design" target="_blank" rel="noopener noreferrer">System Design</a>
      </div>
    </section>

    <!-- PROJECTS -->
    <section class="section" id="projects" tabindex="-1">
      <h2>PROJECTS</h2>

      <div class="project-grid">
        <div>
          <h3>Data Analysis and Visualization</h3>
          <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank" rel="noopener noreferrer">
            <div class="project-title">Predicting Birth Weight</div>
            <div class="project-description">Built a Regression model for dataset with 36 explanatory variables and 108,082 observations. Achieved 12% adjusted R-squared despite forward/backward selection, interaction terms, polynomials, and transformations — much variability remained unexplained.</div>
            <div class="skills">
              <span class="skill-tag">R</span>
              <span class="skill-tag">Regression</span>
              <span class="skill-tag">Data Analysis</span>
              <span class="skill-tag">Hypothesis testing</span>
            </div>
          </a>
        </div>

        <a class="project-box" href="https://github.com/kavanamk/Data-Visualization/blob/main/DV/Final%20Report%20Data%20Vizards.pdf" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Police Killing Dashboard</div>
          <div class="project-description">Visualizations including Sankey, Bar Graph, Star Plot and Interactive Choropleth for exploring police killings by age, race, armed status, gender, and income.</div>
          <div class="skills">
            <span class="skill-tag">R</span>
            <span class="skill-tag">Tableau</span>
            <span class="skill-tag">Data Visualization</span>
          </div>
        </a>

        <h3>Machine Learning</h3>

        <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Credit Risk</div>
          <div class="project-description">Engineered features and consolidated 30K+ loan purposes using TF-IDF + OpenAI API, enabling a 94% accurate credit risk model. Trained Logistic Regression, Random Forest, and XGBoost; evaluated with AUC, F1, and profit curves.</div>
          <div class="skills">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">scikit-learn</span>
            <span class="skill-tag">OpenAI API</span>
            <span class="skill-tag">NLP</span>
            <span class="skill-tag">TF-IDF</span>
          </div>
        </a>

        <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Autism Screening</div>
          <div class="project-description">Used Mutual Information and Recursive Feature Elimination for feature selection. Evaluated XGBoost, SVM-RBF, Logistic Regression, Random Forest, and MLP. Achieved 97.2% CV accuracy and 1.0 sensitivity with SVM-RBF.</div>
          <div class="skills">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">scikit-learn</span>
            <span class="skill-tag">XGBoost</span>
            <span class="skill-tag">SVM</span>
            <span class="skill-tag">MLP</span>
          </div>
        </a>

        <a class="project-box" href="https://github.com/kavanamk/Generative-AI" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Generative AI</div>
          <div class="project-description">Hands-on with RBMs, VAEs, GANs, and Transformers using TensorFlow 2. Built projects like image generation, deepfakes, music composition, and game agent training with GAIL.</div>
          <div class="skills">
            <span class="skill-tag">TensorFlow 2</span>
            <span class="skill-tag">GAN</span>
            <span class="skill-tag">VAE</span>
            <span class="skill-tag">Transformers</span>
            <span class="skill-tag">GAIL</span>
          </div>
        </a>

        <a class="project-box" href="https://github.com/kavanamk/Obesity-Level-Classification" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Obesity Level Classification</div>
          <div class="project-description">Collected, cleaned, and pre-processed data. Applied PCA and K-Means clustering. Achieved 92.95% accuracy using Decision Trees with pruning and tuned KNN.</div>
          <div class="skills">
            <span class="skill-tag">R</span>
            <span class="skill-tag">PCA</span>
            <span class="skill-tag">K-Means</span>
            <span class="skill-tag">Decision Trees</span>
            <span class="skill-tag">KNN</span>
          </div>
        </a>

        <a class="project-box" href="https://github.com/kavanamk/Natural-Language-Processing-using-Python" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Text Classification</div>
          <div class="project-description">Built a sentiment analysis pipeline using Bag of Words and TF-IDF with a Logistic Regression classifier. Trained on 2,000 samples and achieved 84.37% accuracy.</div>
          <div class="skills">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">NLP</span>
            <span class="skill-tag">TF-IDF</span>
            <span class="skill-tag">Logistic Regression</span>
          </div>
        </a>

        <a class="project-box" href="https://github.com/kavanamk/Programming-ML-Applications/blob/main/Final%20Project/Final_Project.ipynb" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Heart Failure Prediction</div>
          <div class="project-description">Implemented SVM, Decision Trees, and ensemble methods. Developed a weighted voting model using Random Forest, Bagging, and Boosting, reaching 88% accuracy.</div>
          <div class="skills">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">scikit-learn</span>
            <span class="skill-tag">SVM</span>
            <span class="skill-tag">Ensemble Learning</span>
          </div>
        </a>

        <h3>Software Development</h3>

        <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank" rel="noopener noreferrer">
          <div class="project-title">Distributed File Retrieval Engine</div>
          <div class="project-description">Built a distributed client-server file retrieval system with Java and ZeroMQ. Implemented multithreaded dispatcher/worker server with TF-based ranked search on Chameleon Cloud.</div>
          <div class="skills">
            <span class="skill-tag">Java</span>
            <span class="skill-tag">ZeroMQ</span>
            <span class="skill-tag">Multithreading</span>
            <span class="skill-tag">Distributed System</span>
          </div>
        </a>

      </div>
    </section>

    <!-- CERTIFICATES -->
    <section class="section" id="certificates" tabindex="-1">
      <h2>CERTIFICATES</h2>

      <div class="course-card">
        <h3>Machine Learning</h3>
        <p class="muted">The course includes supervised learning (linear regression, logistic regression, neural networks), unsupervised learning (clustering, dimensionality reduction), and key concepts like model evaluation, bias-variance tradeoff, and regularization. It emphasizes intuition behind algorithms and uses Octave/MATLAB for hands-on practice.</p>
        <div style="width:100%; height:220px; overflow:hidden; border-radius:6px; margin-top:1rem;">
          <img src="images/ml.jpg" alt="Machine Learning Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
        </div>
      </div>

      <div class="course-card">
        <h3>Developing Large Language Models (LLMs)</h3>
        <p class="muted">Completed a Skill Path in PyTorch and Deep Learning, covering tensors, neural networks, autograd, and optimization. Gained hands-on experience with GANs, transformers, and attention mechanisms, leading up to training and fine-tuning LLMs for real-world NLP tasks.</p>
        <div style="width:100%; height:220px; overflow:hidden; border-radius:6px; margin-top:1rem;">
          <img src="images/Educative_DevelopingLLM.jpg" alt="LLM Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
        </div>
      </div>

      <div class="course-card">
        <h3>System Design</h3>
        <p class="muted">Abstractions, consistency models, distributed computing building blocks (CDN, DNS, Load Balancers, Key-value store, NoSQL, Cache, BLOBs, Monitoring systems, Search, Message Queues, Pub-sub, etc.). Extensive design of popular systems like YouTube, Instagram, Quora, Maps, TikTok, Uber.</p>
        <div style="width:100%; height:220px; overflow:hidden; border-radius:6px; margin-top:1rem;">
          <img src="images/Educative_SysytemDesign.jpg" alt="System Design Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
        </div>
      </div>
    </section>

  </main>

  <!-- Small script to toggle .active on tab links and focus target section for accessibility -->
  <script>
    (function() {
      const links = document.querySelectorAll('.tab-link');

      function setActiveByHash() {
        const hash = window.location.hash || '#work-experience';
        links.forEach(l => l.classList.remove('active'));
        const active = document.querySelector('.tabs-nav a[href="' + hash + '"]');
        if (active) active.classList.add('active');

        // Move focus to the section for better keyboard/screen reader experience
        try {
          const target = document.querySelector(hash);
          if (target) {
            // slightly delay to allow browser scroll to finish
            setTimeout(() => target.focus({preventScroll:true}), 200);
          }
        } catch(e) {
          // ignore invalid selectors
        }
      }

      // initial
      setActiveByHash();

      // update when hash changes (user clicks or navigates)
      window.addEventListener('hashchange', setActiveByHash);

      // click handler: make sure small-screen tapped link becomes active immediately
      links.forEach(l => l.addEventListener('click', function() {
        links.forEach(x => x.classList.remove('active'));
        this.classList.add('active');
      }));

      // ensure keyboard visible focus for accessibility
      document.addEventListener('keydown', function(e) {
        if (e.key === 'Tab') document.body.classList.add('user-is-tabbing');
      });
    })();
  </script>

</body>
</html>
