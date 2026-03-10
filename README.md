
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kavana Manvi Krishnamurthy</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet" />
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-padding-top: 80px; }

    body {
      background-color: #0a0a0a;
      color: #f0f0f0;
      font-family: 'Poppins', sans-serif;
    }

    h1, h2, h3 { color: #ff2d78; }
    a { color: #ff2d78; }

    /* ── NAVBAR ── */
    .navbar {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 1rem 2rem;
      background-color: #0a0a0a;
      padding: 1rem 1.5rem;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 12px rgba(255, 45, 120, 0.15);
      border-bottom: 1px solid #1f1f1f;
    }
    .navbar a {
      text-decoration: none;
      color: #ff2d78;
      font-weight: 600;
      font-size: 0.95rem;
      transition: color 0.3s ease;
    }
    .navbar a:hover { color: #ffffff; }

    /* ── HERO ── */
    .hero {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 1.5rem 2rem;
    }

    .hero h1 {
      font-size: clamp(2rem, 6vw, 3rem);
      font-weight: 700;
      color: #ff2d78;
      margin-bottom: 2rem;
      letter-spacing: -0.01em;
    }

    .hero-body {
      display: flex;
      align-items: flex-start;
      gap: 2rem;
      flex-wrap: wrap;
    }

    .hero-photo {
      flex-shrink: 0;
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #ff2d78;
      box-shadow: 0 0 20px rgba(255, 45, 120, 0.3);
    }

    .hero-text {
      flex: 1;
      min-width: 220px;
    }

    .hero-text p {
      color: #cccccc;
      font-size: 0.97rem;
      line-height: 1.8;
      margin-bottom: 1.4rem;
    }

    .social-links {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
    }

    .social-btn {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      background-color: #111111;
      border: 1px solid #ff2d7855;
      color: #ff2d78;
      text-decoration: none;
      padding: 0.45rem 1rem;
      border-radius: 20px;
      font-size: 0.82rem;
      font-weight: 500;
      transition: background 0.2s ease, transform 0.2s ease;
    }
    .social-btn:hover {
      background-color: #ff2d7822;
      transform: translateY(-2px);
    }

    /* ── SHARED SECTION WRAPPER ── */
    .section-wrap {
      max-width: 900px;
      margin: 0 auto;
      padding: 1rem 1.5rem;
    }

    /* ── DATA ROLES ── */
    .data-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin: 1.5rem 0 2.5rem;
    }

    .data-box {
      background-color: #111111;
      color: white;
      border-radius: 16px;
      padding: 20px 25px;
      box-shadow: 0 4px 10px rgba(255, 45, 120, 0.1);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
      width: 100%;
      max-width: 820px;
      border-top: 3px solid #ff2d78;
    }
    .data-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 20px rgba(255, 45, 120, 0.25);
    }
    .data-title {
      font-size: 1.2rem;
      font-weight: 600;
      margin-bottom: 4px;
      color: #ff2d78;
    }
    .data-subtitle {
      font-size: 0.88rem;
      color: #aaaaaa;
      margin-bottom: 12px;
    }
    .data-bubbles {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }

    /* ── SKILL TAG (shared) ── */
    .skill-tag {
      background-color: #1e1e1e;
      color: #ff2d78;
      border: 1px solid #ff2d7855;
      padding: 5px 11px;
      border-radius: 20px;
      font-size: 0.82em;
      font-weight: 500;
      white-space: nowrap;
      transition: background-color 0.2s ease, transform 0.2s ease;
      text-decoration: none;
      display: inline-block;
    }
    .skill-tag:hover {
      background-color: #ff2d7822;
      transform: scale(1.04);
    }

    /* ── LINK BOXES ── */
    .link-boxes {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1rem auto 2rem;
      max-width: 500px;
    }
    .link-box {
      flex: 1 1 120px;
      background-color: #111111;
      border: 1px solid #ff2d7844;
      border-radius: 8px;
      padding: 1rem;
      text-align: center;
      font-size: 1rem;
      color: #ff2d78;
      text-decoration: none;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .link-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 16px rgba(255, 45, 120, 0.2);
    }

    /* ── EDU BLOCKS ── */
    .edu-block {
      background: #111111;
      border: 1px solid #1f1f1f;
      border-left: 3px solid #ff2d78;
      border-radius: 10px;
      padding: 1.5rem 2rem;
      margin-bottom: 1.5rem;
    }
    .edu-block h3 { color: #ff2d78; margin: 0 0 0.3rem 0; font-size: 1rem; }
    .edu-block h4 { color: #cccccc; font-weight: 500; margin: 0 0 0.8rem 0; font-size: 0.9rem; }
    .edu-block p { color: #999999; font-size: 0.88rem; line-height: 1.7; margin: 0.3rem 0; }
    .edu-block strong { color: #dddddd; }

    /* ── EXP BLOCKS ── */
    .exp-block {
      background: #111111;
      border: 1px solid #1f1f1f;
      border-left: 3px solid #ff2d78;
      border-radius: 10px;
      padding: 1.5rem 2rem;
      margin-bottom: 1.5rem;
    }
    .exp-block h3 { color: #ff2d78; margin: 0 0 1rem 0; font-size: 1rem; }
    .exp-block ul { margin: 0; padding-left: 1.2rem; }
    .exp-block li { color: #cccccc; font-size: 0.9rem; line-height: 1.7; margin-bottom: 0.5rem; }
    .exp-block li strong { color: #ffffff; }

    /* ── SKILLS BLOCK ── */
    .skills-block {
      background: #111111;
      border: 1px solid #1f1f1f;
      border-radius: 10px;
      padding: 1.5rem 2rem;
      margin-bottom: 2rem;
    }
    .skills-block ul { margin: 0; padding-left: 1.2rem; }
    .skills-block li { color: #cccccc; font-size: 0.9rem; line-height: 1.9; }
    .skills-block li strong { color: #ff2d78; }

    /* ── PROJECT BOX ── */
    .project-box {
      background-color: #111111;
      border: 1px solid #1f1f1f;
      border-radius: 12px;
      padding: 1.5rem;
      color: #cccccc;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-decoration: none;
      display: block;
    }
    .project-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 20px rgba(255, 45, 120, 0.15);
    }
    .project-title {
      font-size: 1.1rem;
      font-weight: 600;
      color: #ff2d78;
      margin-bottom: 0.5rem;
    }
    .project-description {
      font-size: 0.88rem;
      margin-bottom: 1rem;
      color: #aaaaaa;
      line-height: 1.7;
    }
    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    /* ── PROJECT GRID ── */
    .project-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1.2rem;
      margin: 1.5rem 0;
    }
    .project-grid h3 {
      color: #ff2d78;
      margin: 1.2rem 0 0.3rem 0;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      border-bottom: 1px solid #1f1f1f;
      padding-bottom: 0.5rem;
    }

    /* ── COURSE CARDS ── */
    .course-card {
      border: 1px solid #1f1f1f;
      background: #111111;
      padding: 1.5rem;
      border-radius: 10px;
      max-width: 700px;
      margin: 1.5rem auto;
      box-shadow: 0 2px 12px rgba(255, 45, 120, 0.08);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }
    .course-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(255, 45, 120, 0.15);
    }
    .course-card h2 { color: #ff2d78; margin-bottom: 0.5rem; font-size: 1.1rem; }
    .course-card p { color: #999999; font-size: 0.88rem; line-height: 1.6; }

    /* ── SECTION HEADINGS ── */
    .section-heading {
      color: #ff2d78;
      padding-top: 2.5rem;
      margin-bottom: 1rem;
      font-size: clamp(1.2rem, 3vw, 1.6rem);
    }

    /* ── FOOTER ── */
    .footer {
      text-align: center;
      padding: 2rem 1rem 3rem;
      color: #444444;
      font-size: 0.8rem;
      border-top: 1px solid #1a1a1a;
      margin-top: 4rem;
    }
    .footer span { color: #ff2d78; }

    /* ── RESPONSIVE ── */
    @media (max-width: 600px) {
      .hero-body {
        flex-direction: column;
        align-items: center;
        text-align: center;
      }
      .social-links { justify-content: center; }
      .hero h1 { text-align: center; }
      .exp-block, .edu-block, .skills-block { padding: 1.2rem 1rem; }
    }
  </style>
</head>
<body>

  <!-- ── HERO ── -->
  <div class="hero">
    <h1>Kavana Manvi Krishnamurthy</h1>
    <div class="hero-body">
      <img src="images/dp5.jpg" alt="Kavana Manvi Krishnamurthy" class="hero-photo" />
      <div class="hero-text">
        <p>
          The secret ingredient behind my great coding skills is love — and a lot of discipline!
          I bring a solid foundation in software engineering from my time at Oracle and a Master's in Computer Science.
          I'm passionate about Machine Learning, Data Analytics, and solving tough problems (300+ on LeetCode!).
        </p>
        <div class="social-links">
          <a class="social-btn" href="https://linkedin.com/in/kavanamk" target="_blank">
            <svg width="14" height="14" viewBox="0 0 24 24" fill="#ff2d78"><path d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"/><circle cx="4" cy="4" r="2"/></svg>
            LinkedIn
          </a>
          <a class="social-btn" href="https://github.com/kavanamk" target="_blank">
            <svg width="14" height="14" viewBox="0 0 24 24" fill="#ff2d78"><path d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.166 6.839 9.489.5.092.682-.217.682-.482 0-.237-.009-.868-.013-1.703-2.782.604-3.369-1.342-3.369-1.342-.454-1.154-1.11-1.462-1.11-1.462-.908-.62.069-.608.069-.608 1.003.07 1.531 1.03 1.531 1.03.892 1.529 2.341 1.087 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.11-4.555-4.943 0-1.091.39-1.984 1.029-2.683-.103-.253-.446-1.27.098-2.647 0 0 .84-.269 2.75 1.025A9.578 9.578 0 0112 6.836a9.59 9.59 0 012.504.337c1.909-1.294 2.747-1.025 2.747-1.025.546 1.377.202 2.394.1 2.647.64.699 1.028 1.592 1.028 2.683 0 3.842-2.339 4.687-4.566 4.935.359.309.678.919.678 1.852 0 1.336-.012 2.415-.012 2.743 0 .267.18.578.688.48C19.138 20.163 22 16.418 22 12c0-5.523-4.477-10-10-10z"/></svg>
            GitHub
          </a>
          <a class="social-btn" href="https://kavanamlstuff.blogspot.com/" target="_blank">
            <svg width="14" height="14" viewBox="0 0 24 24" fill="#ff2d78"><path d="M19 3H5a2 2 0 00-2 2v14a2 2 0 002 2h14a2 2 0 002-2V5a2 2 0 00-2-2zm-5 14H7v-2h7v2zm3-4H7v-2h10v2zm0-4H7V7h10v2z"/></svg>
            ML Blog
          </a>
          <a class="social-btn" href="https://x.com/kavmlstuff" target="_blank">
            <svg width="14" height="14" viewBox="0 0 24 24" fill="#ff2d78"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
            X / Twitter
          </a>
        </div>
      </div>
    </div>
  </div>

  <!-- ── NAVBAR ── -->
  <nav class="navbar">
    <a href="#work-experience">Work</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#certificates">Certificates</a>
  </nav>

  <!-- ── ROLES ── -->
  <div class="section-wrap">
    <h3 style="text-align:center; color:#ff2d78; margin: 2rem 0 0.5rem;">I'd be a great fit for these roles</h3>
    <div class="data-container">
      <div class="data-box">
        <div class="data-title">Data Analyst</div>
        <div class="data-subtitle">Transform data into insights</div>
        <div class="data-bubbles">
          <span class="skill-tag">SQL (3+ years)</span>
          <span class="skill-tag">R</span>
          <span class="skill-tag">Python (NumPy, Pandas)</span>
          <span class="skill-tag">Excel</span>
          <span class="skill-tag">Tableau</span>
        </div>
      </div>
      <div class="data-box">
        <div class="data-title">Data Engineer</div>
        <div class="data-subtitle">Build data pipelines & Data Lakehouses</div>
        <div class="data-bubbles">
          <span class="skill-tag">ETL Pipelines</span>
          <span class="skill-tag">SQL (3+ years)</span>
          <span class="skill-tag">Spark / PySpark</span>
          <span class="skill-tag">AWS S3</span>
          <span class="skill-tag">GCP</span>
          <span class="skill-tag">Snowflake</span>
        </div>
      </div>
      <div class="data-box">
        <div class="data-title">AI / ML Data Scientist</div>
        <div class="data-subtitle">Develop predictive & AI models</div>
        <div class="data-bubbles">
          <span class="skill-tag">SQL</span>
          <span class="skill-tag">R</span>
          <span class="skill-tag">Python (scikit-learn, TensorFlow/Keras, PyTorch)</span>
          <span class="skill-tag">Predictive Modeling</span>
          <span class="skill-tag">Statistical Analysis</span>
          <span class="skill-tag">Generative AI</span>
          <span class="skill-tag">LLMs</span>
          <span class="skill-tag">Multi-Agents</span>
          <span class="skill-tag">RAG</span>
          <span class="skill-tag">Vector Databases</span>
        </div>
      </div>
    </div>

    <!-- ── EDUCATION ── -->
    <h2 id="education" class="section-heading">EDUCATION</h2>

    <div class="edu-block">
      <h3>Master of Science, Computer Science</h3>
      <h4><img src="images/depaul.jpg" width="18" style="vertical-align:middle; margin-right:6px;"/>DePaul University, Chicago &nbsp;·&nbsp; GPA: 3.86</h4>
      <p><strong>Foundational CS:</strong> Object Oriented Programming, Distributed Systems, Database Management, Algorithms & Data Structures</p>
      <p><strong>Foundational Data Science:</strong> Fundamentals of Data Science in R, Data Visualization, Data Regression & Analysis, Image Processing</p>
      <p><strong>Advanced Data Science:</strong> Programming ML Algorithms, Advanced Machine Learning, Computer Vision</p>
    </div>

    <div class="edu-block">
      <h3>Bachelor of Science, Computer Science</h3>
      <h4><img src="images/nieit.jpg" width="18" style="vertical-align:middle; margin-right:6px;"/>NIE, India</h4>
      <p><strong>Courses:</strong> Mathematics, Statistics, Data Structures, Algorithms, Compiler Design, Cybersecurity, IoT, Microprocessor & Assembly, Java, J2EE, Database, Computer Architecture, OpenGL, Big Data, Data Mining, AI, Software Engineering, Unix</p>
    </div>

    <!-- ── WORK EXPERIENCE ── -->
    <h2 id="work-experience" class="section-heading">WORK EXPERIENCE</h2>

    <div class="exp-block">
      <h3><img src="images/oracle.jpg" width="20" style="vertical-align:middle; margin-right:8px;"/>Software Engineer — Oracle</h3>
      <ul>
        <li>Performed defect correction and management of ETL scripts and reports using SQL, OCI and Tableau.</li>
        <li>Led full-stack development for <strong>75+ Jira tickets</strong>, handling issue analysis, design, implementation, and testing.</li>
        <li><strong>Improved code runtime from 6–7 hours to 40 seconds</strong>, earning 2022 "Innovate and Simplify" Quarterly Award.</li>
        <li>Recognised twice as <strong>"Star of the Sprint"</strong> for exceeding expectations with additional testing alongside sprint deliverables, removing roadblocks.</li>
        <li>Conducted <strong>35+ client issue investigations</strong> over 6 months to identify root causes.</li>
      </ul>
    </div>

    <div class="exp-block">
      <h3><img src="images/oracle.jpg" width="20" style="vertical-align:middle; margin-right:8px;"/>Software Intern — Oracle</h3>
      <ul>
        <li>Developed full-stack web features for internal business performance application (eBoard) using ReactJS, Spring Boot, PHP, SQL, HTML, CSS, JavaScript, jQuery, and AJAX.</li>
        <li>Delivered <strong>6+ data visualization dashboards</strong> displaying Jenkins job execution status, improving visibility for 30+ revenue cycle teams. Recognized by senior leadership for impact and design quality.</li>
        <li>Created summary and drill-down analytics reports used by directors and senior managers for performance oversight.</li>
      </ul>
    </div>

    <!-- ── SKILLS ── -->
    <h2 id="skills" class="section-heading">SKILLS</h2>

    <div class="skills-block">
      <ul>
        <li><strong>Programming Language:</strong> Python, R, C, Java, Scala, C++</li>
        <li><strong>Big Data:</strong> HDFS, Spark, Hadoop, GCP — Cloud Storage, BigQuery, Pub/Sub, Dataflow</li>
        <li><strong>Machine Learning:</strong> TensorFlow, PyTorch, Keras, Octave, MATLAB, Generative AI, NLP, CV</li>
        <li><strong>Web Technology:</strong> HTML, CSS, JavaScript, PHP, jQuery, AJAX, ReactJS, JSON, XML</li>
        <li><strong>Others:</strong> Git, SVM, Subversion, Excel, MS Office, SDLC – Agile & Jira, Jenkins, CI/CD</li>
        <li><strong>Soft Skills:</strong> Effective communication, problem-solving, critical thinking, growth mindset, curiosity</li>
      </ul>
    </div>

    <h2 style="color:#ff2d78; font-size:1.1rem; margin-bottom:0.5rem;">I'm also an Expert in Data Structures, Algorithms and System Design</h2>
    <div class="link-boxes">
      <a class="link-box" href="https://github.com/kavanamk/Educative-DSA" target="_blank">DSA</a>
      <a class="link-box" href="https://github.com/kavanamk/Educative-System-Design" target="_blank">System Design</a>
    </div>

    <!-- ── ML BLOG ── -->
    <h2 id="ml-blog" class="section-heading">MACHINE LEARNING BLOG</h2>

    <div class="project-box" style="margin-bottom: 2rem;">
      <div style="width:100%; height:260px; overflow:hidden; border-radius:10px; margin-bottom:1rem;">
        <img src="images/MLblog.jpg" alt="ML Blog" style="width:100%; height:100%; object-fit:cover; display:block;" />
      </div>
      <div class="project-description">
        As a Machine Learning practitioner, I translate complex data into actionable, intelligent solutions. My expertise spans the entire ML lifecycle — from rigorous data preparation and statistical modeling to implementing cutting-edge Deep Learning and Generative AI architectures. I focus on building and deploying scalable models, including Supervised, Unsupervised, and Reinforcement Learning systems, consistently driving innovation by turning theoretical concepts into robust, real-world predictive and creative applications.
      </div>
      <a href="https://kavanamlstuff.blogspot.com/" target="_blank" class="skill-tag">Read Full Blog →</a>
    </div>

    <!-- ── PROJECTS ── -->
    <h2 id="projects" class="section-heading">PROJECTS</h2>

    <div class="project-grid">

      <h3>Data Analysis & Visualization</h3>

      <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank">
        <div class="project-title">Predicting Birth Weight</div>
        <div class="project-description">Built a Regression model for dataset with 36 explanatory variables and 108,082 observations. Applied forward and backward selection, interaction terms, second-order polynomials, and variable transformations.</div>
        <div class="skills">
          <span class="skill-tag">R</span><span class="skill-tag">Regression</span><span class="skill-tag">Data Analysis</span><span class="skill-tag">Hypothesis Testing</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Data-Visualization/blob/main/DV/Final%20Report%20Data%20Vizards.pdf" target="_blank">
        <div class="project-title">Police Killing Dashboard</div>
        <div class="project-description">Multi-perspective visualizations on police killings. Sankey Plot for age/race/unarmed incidents, Bar Graph for unarmed killings by race, Star Plot for geographic risk, and Interactive Choropleth Map for dynamic exploration.</div>
        <div class="skills">
          <span class="skill-tag">R</span><span class="skill-tag">Tableau</span><span class="skill-tag">Data Visualization</span>
        </div>
      </a>

      <h3>Machine Learning</h3>

      <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank">
        <div class="project-title">Credit Risk</div>
        <div class="project-description">Engineered features and consolidated 30K+ loan purposes using TF-IDF + OpenAI API, enabling 94% accurate credit risk prediction. Trained and optimized Logistic Regression, Random Forest, and XGBoost using GridSearchCV.</div>
        <div class="skills">
          <span class="skill-tag">Python</span><span class="skill-tag">scikit-learn</span><span class="skill-tag">OpenAI API</span><span class="skill-tag">NLP</span><span class="skill-tag">TF-IDF</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank">
        <div class="project-title">Autism Screening</div>
        <div class="project-description">Used Mutual Information and Recursive Feature Elimination for feature selection. Evaluated XGBoost, SVM-RBF, Logistic Regression, Random Forest, and MLP. Achieved 97.2% CV accuracy and 1.0 sensitivity with SVM-RBF.</div>
        <div class="skills">
          <span class="skill-tag">Python</span><span class="skill-tag">scikit-learn</span><span class="skill-tag">XGBoost</span><span class="skill-tag">SVM</span><span class="skill-tag">MLP</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Generative-AI" target="_blank">
        <div class="project-title">Generative AI</div>
        <div class="project-description">Hands-on with RBMs, VAEs, GANs, and Transformers using TensorFlow 2. Built projects including image generation, deepfakes, music composition, and game agent training with GAIL.</div>
        <div class="skills">
          <span class="skill-tag">TensorFlow 2</span><span class="skill-tag">GAN</span><span class="skill-tag">VAE</span><span class="skill-tag">Transformers</span><span class="skill-tag">GAIL</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Obesity-Level-Classification" target="_blank">
        <div class="project-title">Obesity Level Classification</div>
        <div class="project-description">Collected, cleaned, and pre-processed data. Applied PCA and K-Means clustering. Achieved 92.95% accuracy using Decision Trees with pruning and KNN tuned for optimal k values.</div>
        <div class="skills">
          <span class="skill-tag">R</span><span class="skill-tag">PCA</span><span class="skill-tag">K-Means</span><span class="skill-tag">Decision Trees</span><span class="skill-tag">KNN</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Natural-Language-Processing-using-Python" target="_blank">
        <div class="project-title">Text Classification</div>
        <div class="project-description">Built a sentiment analysis pipeline using Bag of Words and TF-IDF with a Logistic Regression classifier. Trained on 2,000 samples and achieved 84.37% accuracy.</div>
        <div class="skills">
          <span class="skill-tag">Python</span><span class="skill-tag">NLP</span><span class="skill-tag">TF-IDF</span><span class="skill-tag">Logistic Regression</span>
        </div>
      </a>

      <a class="project-box" href="https://github.com/kavanamk/Programming-ML-Applications/blob/main/Final%20Project/Final_Project.ipynb" target="_blank">
        <div class="project-title">Heart Failure Prediction</div>
        <div class="project-description">Implemented SVM, Decision Trees, and ensemble methods. Developed a weighted voting model using Random Forest, Bagging, and Boosting, reaching 88% accuracy.</div>
        <div class="skills">
          <span class="skill-tag">Python</span><span class="skill-tag">scikit-learn</span><span class="skill-tag">SVM</span><span class="skill-tag">Ensemble Learning</span><span class="skill-tag">Random Forest</span><span class="skill-tag">Boosting</span>
        </div>
      </a>

      <h3>Software Development</h3>

      <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank">
        <div class="project-title">Distributed File Retrieval Engine</div>
        <div class="project-description">Built a distributed client-server file retrieval system with Java and ZeroMQ. Implemented multithreaded dispatcher/worker server with TF-based ranked search on Chameleon Cloud.</div>
        <div class="skills">
          <span class="skill-tag">Java</span><span class="skill-tag">ZeroMQ</span><span class="skill-tag">Multithreading</span><span class="skill-tag">Chameleon Cloud</span><span class="skill-tag">Distributed System</span>
        </div>
      </a>

    </div>

    <!-- ── CERTIFICATES ── -->
    <h2 id="certificates" class="section-heading">CERTIFICATES</h2>

  </div><!-- end section-wrap -->

  <div class="course-card">
    <h2>Machine Learning</h2>
    <p>The course includes supervised learning (linear regression, logistic regression, neural networks), unsupervised learning (clustering, dimensionality reduction), and key concepts like model evaluation, bias-variance tradeoff, and regularization. Emphasizes intuition behind algorithms and uses Octave/MATLAB for hands-on practice.</p>
    <div style="width:100%; height:260px; overflow:hidden; border-radius:6px; margin-top:1rem;">
      <img src="images/ml.jpg" alt="ML Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
    </div>
  </div>

  <div class="course-card">
    <h2>Developing Large Language Models (LLMs)</h2>
    <p>Completed a Skill Path in PyTorch and Deep Learning, covering tensors, neural networks, autograd, and optimization. Gained hands-on experience with GANs, transformers, and attention mechanisms, leading up to training and fine-tuning LLMs (e.g., BERT) for real-world NLP tasks.</p>
    <div style="width:100%; height:260px; overflow:hidden; border-radius:6px; margin-top:1rem;">
      <img src="images/Educative_DevelopingLLM.jpg" alt="LLM Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
    </div>
  </div>

  <div class="course-card">
    <h2>System Design</h2>
    <p>Abstractions, consistency models, distributed computing. Building block architecture — CDN, DNS, Load Balancers, Key-Value Store, Databases, NoSQL, Cache, BLOB, Monitoring, Distributed Search, Message Queues, Logging, Sequencer, Pub/Sub, Shared Counter. Extensive system design of 10+ concepts: YouTube, Instagram, Quora, Google Maps, TikTok, Uber, Uber Eats etc.</p>
    <div style="width:100%; height:260px; overflow:hidden; border-radius:6px; margin-top:1rem;">
      <img src="images/Educative_SysytemDesign.jpg" alt="System Design Certificate" style="width:100%; height:100%; object-fit:cover; display:block;" />
    </div>
  </div>

  <div class="footer">
    Built by <span>Kavana Manvi Krishnamurthy</span> · Hosted on GitHub Pages
  </div>

</body>
</html>
