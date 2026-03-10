<!-- Navigation Bar -->
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

  * { box-sizing: border-box; }

  body {
    background-color: #0a0a0a;
    color: #f0f0f0;
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0 1rem;
  }

  html {
    scroll-padding-top: 80px;
  }

  h1, h2, h3 { color: #ff2d78; }

  a { color: #ff2d78; }

  .navbar {
    display: flex;
    justify-content: center;
    gap: 2rem;
    background-color: #0a0a0a;
    padding: 1rem 0;
    font-family: "Poppins", sans-serif;
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
    transition: color 0.3s ease;
  }

  .navbar a:hover {
    color: #ffffff;
  }
</style>

<div class="navbar">
  <a href="#work-experience">Work</a>
  <a href="#skills">Skills</a>
  <a href="#projects">Projects</a>
  <a href="#certificates">Certificates</a>
</div>

<img src="images/LLM-13.jpg" style="vertical-align:middle; display:block; margin: 2rem auto; max-width: 100%; border-radius: 12px;"/>

<h3 style="text-align: center; color: #ff2d78;">
  I'd be a great fit for these roles
</h3>

<!-- Data Roles Section -->
<style>
  .data-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    font-family: "Poppins", sans-serif;
    margin: 40px 0;
  }

  .data-box {
    background-color: #111111;
    color: white;
    border-radius: 16px;
    padding: 20px 25px;
    box-shadow: 0 4px 10px rgba(255, 45, 120, 0.1);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    width: 80%;
    border-top: 3px solid #ff2d78;
  }

  .data-box:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 20px rgba(255, 45, 120, 0.25);
  }

  .data-title {
    font-size: 1.4em;
    font-weight: 600;
    margin-bottom: 5px;
    color: #ff2d78;
  }

  .data-subtitle {
    font-size: 0.95em;
    color: #aaaaaa;
    margin-bottom: 12px;
  }

  .data-bubbles {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .skill-tag {
    background-color: #1e1e1e;
    color: #ff2d78;
    border: 1px solid #ff2d7855;
    padding: 6px 12px;
    border-radius: 20px;
    font-size: 0.85em;
    font-weight: 500;
    white-space: nowrap;
    transition: background-color 0.2s ease, transform 0.2s ease;
  }

  .skill-tag:hover {
    background-color: #ff2d7822;
    transform: scale(1.05);
  }
</style>

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
      <span class="skill-tag">Spark / Pyspark</span>
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

<!-- Link Boxes Style -->
<style>
  .link-boxes {
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    margin: 2rem auto;
    max-width: 1200px;
    flex-wrap: nowrap;
  }

  .link-box {
    flex: 1 1 20%;
    background-color: #111111;
    border: 1px solid #ff2d7844;
    border-radius: 8px;
    padding: 1.5rem;
    text-align: center;
    font-family: 'Helvetica Neue', sans-serif;
    font-size: 1.1rem;
    color: #ff2d78;
    text-decoration: none;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .link-box:hover {
    transform: translateY(-4px);
    box-shadow: 0 6px 16px rgba(255, 45, 120, 0.2);
  }
</style>

<!-- EDUCATION -->
<h2 id="education" style="color: #ff2d78; padding-top: 3rem;">EDUCATION</h2>

<style>
  .edu-block {
    background: #111111;
    border: 1px solid #1f1f1f;
    border-left: 3px solid #ff2d78;
    border-radius: 10px;
    padding: 1.5rem 2rem;
    margin-bottom: 1.5rem;
    max-width: 860px;
  }
  .edu-block h3 { color: #ff2d78; margin: 0 0 0.3rem 0; }
  .edu-block h4 { color: #cccccc; font-weight: 500; margin: 0 0 0.8rem 0; }
  .edu-block p { color: #999999; font-size: 0.9rem; line-height: 1.7; margin: 0.3rem 0; }
  .edu-block strong { color: #dddddd; }
</style>

<div class="edu-block">
  <h3>Master of Science, Computer Science</h3>
  <h4><img src="images/depaul.jpg" width="20" style="vertical-align:middle; margin-right:6px;"/>DePaul University, Chicago &nbsp;·&nbsp; GPA: 3.86</h4>
  <p><strong>Foundational CS:</strong> Object Oriented Programming, Distributed Systems, Database Management, Algorithms & Data Structures</p>
  <p><strong>Foundational Data Science:</strong> Fundamentals of Data Science in R, Data Visualization, Data Regression & Analysis, Image Processing</p>
  <p><strong>Advanced Data Science:</strong> Programming ML Algorithms, Advanced Machine Learning, Computer Vision</p>
</div>

<div class="edu-block">
  <h3>Bachelor of Science, Computer Science</h3>
  <h4><img src="images/nieit.jpg" width="20" style="vertical-align:middle; margin-right:6px;"/>NIE, India</h4>
  <p><strong>Courses:</strong> Mathematics, Statistics, Data Structures, Algorithms, Compiler Design, Cybersecurity, IoT, Microprocessor & Assembly, Java, J2EE, Database, Computer Architecture, OpenGL, Big Data, Data Mining, AI, Software Engineering, Unix</p>
</div>

<!-- WORK EXPERIENCE -->
<h2 id="work-experience" style="color: #ff2d78;">WORK EXPERIENCE</h2>

<style>
  .exp-block {
    background: #111111;
    border: 1px solid #1f1f1f;
    border-left: 3px solid #ff2d78;
    border-radius: 10px;
    padding: 1.5rem 2rem;
    margin-bottom: 1.5rem;
    max-width: 860px;
  }
  .exp-block h3 { color: #ff2d78; margin: 0 0 1rem 0; }
  .exp-block ul { margin: 0; padding-left: 1.2rem; }
  .exp-block li { color: #cccccc; font-size: 0.95rem; line-height: 1.7; margin-bottom: 0.5rem; }
  .exp-block li strong { color: #ffffff; }
</style>

<div class="exp-block">
  <h3><img src="images/oracle.jpg" width="22" style="vertical-align:middle; margin-right:8px;"/>Software Engineer — Oracle</h3>
  <ul>
    <li>Performed defect correction and management of ETL scripts and reports using SQL, OCI and Tableau.</li>
    <li>Led full-stack development for <strong>75+ Jira tickets</strong>, handling issue analysis, design, implementation, and testing.</li>
    <li><strong>Improved code runtime from 6–7 hours to 40 seconds</strong>, earning 2022 "Innovate and Simplify" Quarterly Award.</li>
    <li>Recognised twice as <strong>"Star of the Sprint"</strong> for exceeding expectations with additional testing alongside sprint deliverables, removing roadblocks.</li>
    <li>Conducted <strong>35+ client issue investigations</strong> over 6 months to identify root causes.</li>
  </ul>
</div>

<div class="exp-block">
  <h3><img src="images/oracle.jpg" width="22" style="vertical-align:middle; margin-right:8px;"/>Software Intern — Oracle</h3>
  <ul>
    <li>Developed full-stack web features for internal business performance application (eBoard) using ReactJS, Spring Boot, PHP, SQL, HTML, CSS, JavaScript, jQuery, and AJAX.</li>
    <li>Delivered <strong>6+ data visualization dashboards</strong> displaying Jenkins job execution status, improving visibility for 30+ revenue cycle teams. Recognized by senior leadership for impact and design quality.</li>
    <li>Created summary and drill-down analytics reports used by directors and senior managers for performance oversight.</li>
  </ul>
</div>

<!-- SKILLS -->
<h2 id="skills" style="color: #ff2d78;">SKILLS</h2>

<style>
  .skills-block {
    background: #111111;
    border: 1px solid #1f1f1f;
    border-radius: 10px;
    padding: 1.5rem 2rem;
    max-width: 860px;
    margin-bottom: 2rem;
  }
  .skills-block ul { margin: 0; padding-left: 1.2rem; }
  .skills-block li { color: #cccccc; font-size: 0.95rem; line-height: 1.9; }
  .skills-block li strong { color: #ff2d78; }
</style>

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

<h2 style="color: #ff2d78;">I'm also an Expert in Data Structures, Algorithms and System Design</h2>

<div class="link-boxes" style="max-width:600px;">
  <a class="link-box" href="https://github.com/kavanamk/Educative-DSA" target="_blank">DSA</a>
  <a class="link-box" href="https://github.com/kavanamk/Educative-System-Design" target="_blank">System Design</a>
</div>

<!-- ML BLOG -->
<h2 id="ml-blog" style="color: #ff2d78; padding-top: 3rem;">MACHINE LEARNING BLOG</h2>

<style>
  .project-box {
    background-color: #111111;
    border: 1px solid #1f1f1f;
    border-radius: 12px;
    padding: 1.5rem;
    font-family: 'Poppins', sans-serif;
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
    font-size: 1.2rem;
    font-weight: 600;
    color: #ff2d78;
    margin-bottom: 0.5rem;
  }
  .project-description {
    font-size: 0.95rem;
    margin-bottom: 1rem;
    color: #aaaaaa;
    line-height: 1.7;
  }
  .skills {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }
</style>

<div class="project-box" style="max-width: 860px; margin: 2rem auto;">
  <div style="width: 100%; height: 300px; overflow: hidden; border-radius: 10px; margin: 0 0 1rem 0;">
    <img src="images/MLblog.jpg" alt="ML Blog Flowchart" style="width: 100%; height: 100%; object-fit: cover; display: block;" />
  </div>
  <div class="project-description">
    As a Machine Learning practitioner, I translate complex data into actionable, intelligent solutions. My expertise spans the entire ML lifecycle — from rigorous data preparation and statistical modeling to implementing cutting-edge Deep Learning and Generative AI architectures. I focus on building and deploying scalable models, including Supervised, Unsupervised, and Reinforcement Learning systems.
  </div>
  <a href="https://kavanamlstuff.blogspot.com/" target="_blank" class="skill-tag" style="margin-top: 0.5rem; display: inline-block;">Read Full Blog →</a>
</div>

<!-- PROJECTS -->
<h2 id="projects" style="color: #ff2d78;">PROJECTS</h2>

<style>
  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    max-width: 860px;
    margin: 2rem auto;
  }
  .project-grid h3 {
    color: #ff2d78;
    margin: 1.5rem 0 0.5rem 0;
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    border-bottom: 1px solid #1f1f1f;
    padding-bottom: 0.5rem;
  }
</style>

<div class="project-grid">

  <h3>Data Analysis & Visualization</h3>

  <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank">
    <div class="project-title">Predicting Birth Weight</div>
    <div class="project-description">Built a Regression model for dataset with 36 explanatory variables and 108,082 observations. Applied forward and backward selection, interaction terms, second-order polynomials, and variable transformations.</div>
    <div class="skills">
      <div class="skill-tag">R</div>
      <div class="skill-tag">Regression</div>
      <div class="skill-tag">Data Analysis</div>
      <div class="skill-tag">Hypothesis Testing</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Data-Visualization/blob/main/DV/Final%20Report%20Data%20Vizards.pdf" target="_blank">
    <div class="project-title">Police Killing Dashboard</div>
    <div class="project-description">Multi-perspective visualizations on police killings. Sankey Plot for age/race/unarmed incidents, Bar Graph for unarmed killings by race, Star Plot for geographic risk, and Interactive Choropleth Map for dynamic exploration.</div>
    <div class="skills">
      <div class="skill-tag">R</div>
      <div class="skill-tag">Tableau</div>
      <div class="skill-tag">Data Visualization</div>
    </div>
  </a>

  <h3>Machine Learning</h3>

  <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank">
    <div class="project-title">Credit Risk</div>
    <div class="project-description">Engineered features and consolidated 30K+ loan purposes using TF-IDF + OpenAI API, enabling 94% accurate credit risk prediction. Trained and optimized Logistic Regression, Random Forest, and XGBoost using GridSearchCV.</div>
    <div class="skills">
      <div class="skill-tag">Python</div>
      <div class="skill-tag">scikit-learn</div>
      <div class="skill-tag">OpenAI API</div>
      <div class="skill-tag">NLP</div>
      <div class="skill-tag">TF-IDF</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning/blob/main/AML/FinalProject/Kavana%20Autism%20Word%20doc.pdf" target="_blank">
    <div class="project-title">Autism Screening</div>
    <div class="project-description">Used Mutual Information and Recursive Feature Elimination for feature selection. Evaluated XGBoost, SVM-RBF, Logistic Regression, Random Forest, and MLP. Achieved 97.2% CV accuracy and 1.0 sensitivity with SVM-RBF.</div>
    <div class="skills">
      <div class="skill-tag">Python</div>
      <div class="skill-tag">scikit-learn</div>
      <div class="skill-tag">XGBoost</div>
      <div class="skill-tag">SVM</div>
      <div class="skill-tag">MLP</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Generative-AI" target="_blank">
    <div class="project-title">Generative AI</div>
    <div class="project-description">Hands-on with RBMs, VAEs, GANs, and Transformers using TensorFlow 2. Built projects including image generation, deepfakes, music composition, and game agent training with GAIL.</div>
    <div class="skills">
      <div class="skill-tag">TensorFlow 2</div>
      <div class="skill-tag">GAN</div>
      <div class="skill-tag">VAE</div>
      <div class="skill-tag">Transformers</div>
      <div class="skill-tag">GAIL</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Obesity-Level-Classification" target="_blank">
    <div class="project-title">Obesity Level Classification</div>
    <div class="project-description">Collected, cleaned, and pre-processed data. Applied PCA and K-Means clustering. Achieved 92.95% accuracy using Decision Trees with pruning and KNN tuned for optimal k values.</div>
    <div class="skills">
      <div class="skill-tag">R</div>
      <div class="skill-tag">PCA</div>
      <div class="skill-tag">K-Means</div>
      <div class="skill-tag">Decision Trees</div>
      <div class="skill-tag">KNN</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Natural-Language-Processing-using-Python" target="_blank">
    <div class="project-title">Text Classification</div>
    <div class="project-description">Built a sentiment analysis pipeline using Bag of Words and TF-IDF with a Logistic Regression classifier. Trained on 2,000 samples and achieved 84.37% accuracy.</div>
    <div class="skills">
      <div class="skill-tag">Python</div>
      <div class="skill-tag">NLP</div>
      <div class="skill-tag">TF-IDF</div>
      <div class="skill-tag">Logistic Regression</div>
    </div>
  </a>

  <a class="project-box" href="https://github.com/kavanamk/Programming-ML-Applications/blob/main/Final%20Project/Final_Project.ipynb" target="_blank">
    <div class="project-title">Heart Failure Prediction</div>
    <div class="project-description">Implemented SVM, Decision Trees, and ensemble methods. Developed a weighted voting model using Random Forest, Bagging, and Boosting, reaching 88% accuracy.</div>
    <div class="skills">
      <div class="skill-tag">Python</div>
      <div class="skill-tag">scikit-learn</div>
      <div class="skill-tag">SVM</div>
      <div class="skill-tag">Ensemble Learning</div>
      <div class="skill-tag">Random Forest</div>
      <div class="skill-tag">Boosting</div>
    </div>
  </a>

  <h3>Software Development</h3>

  <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank">
    <div class="project-title">Distributed File Retrieval Engine</div>
    <div class="project-description">Built a distributed client-server file retrieval system with Java and ZeroMQ. Implemented multithreaded dispatcher/worker server with TF-based ranked search on Chameleon Cloud.</div>
    <div class="skills">
      <div class="skill-tag">Java</div>
      <div class="skill-tag">ZeroMQ</div>
      <div class="skill-tag">Multithreading</div>
      <div class="skill-tag">Chameleon Cloud</div>
      <div class="skill-tag">Distributed System</div>
    </div>
  </a>

</div>

<!-- CERTIFICATES -->
<h2 id="certificates" style="color: #ff2d78;">CERTIFICATES</h2>

<style>
  .course-card {
    border: 1px solid #1f1f1f;
    background: #111111;
    padding: 1.5rem;
    border-radius: 10px;
    max-width: 700px;
    margin: 2rem auto;
    box-shadow: 0 2px 12px rgba(255, 45, 120, 0.08);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .course-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 20px rgba(255, 45, 120, 0.15);
  }
  .course-card h2 { color: #ff2d78; margin-bottom: 0.5rem; font-size: 1.2rem; }
  .course-card p { color: #999999; font-size: 0.92rem; line-height: 1.6; }
</style>

<div class="course-card">
  <h2>Machine Learning</h2>
  <p>The course includes supervised learning (linear regression, logistic regression, neural networks), unsupervised learning (clustering, dimensionality reduction), and key concepts like model evaluation, bias-variance tradeoff, and regularization. Emphasizes intuition behind algorithms and uses Octave/MATLAB for hands-on practice.</p>
  <div style="width: 100%; height: 280px; overflow: hidden; border-radius: 6px; margin-top: 1rem;">
    <img src="images/ml.jpg" alt="Machine Learning Certificate" style="width: 100%; height: 100%; object-fit: cover; display: block;" />
  </div>
</div>

<div class="course-card">
  <h2>Developing Large Language Models (LLMs)</h2>
  <p>Completed a Skill Path in PyTorch and Deep Learning, covering tensors, neural networks, autograd, and optimization. Gained hands-on experience with GANs, transformers, and attention mechanisms, leading up to training and fine-tuning LLMs (e.g., BERT) for real-world NLP tasks.</p>
  <div style="width: 100%; height: 280px; overflow: hidden; border-radius: 6px; margin-top: 1rem;">
    <img src="images/Educative_DevelopingLLM.jpg" alt="LLM Certificate" style="width: 100%; height: 100%; object-fit: cover; display: block;" />
  </div>
</div>

<div class="course-card">
  <h2>System Design</h2>
  <p>Abstractions, consistency models, distributed computing. Building block architecture — CDN, DNS, Load Balancers, Key-Value Store, Databases, NoSQL, Cache, BLOB, Monitoring, Distributed Search, Message Queues, Logging, Sequencer, Pub/Sub, Shared Counter. Extensive system design of 10+ concepts: YouTube, Instagram, Quora, Google Maps, TikTok, Uber, Uber Eats etc.</p>
  <div style="width: 100%; height: 280px; overflow: hidden; border-radius: 6px; margin-top: 1rem;">
    <img src="images/Educative_SysytemDesign.jpg" alt="System Design Certificate" style="width: 100%; height: 100%; object-fit: cover; display: block;" />
  </div>
</div>

<!-- FOOTER -->
<style>
  .footer {
    text-align: center;
    padding: 2rem 0 3rem;
    color: #444444;
    font-size: 0.8rem;
    font-family: 'Poppins', sans-serif;
    border-top: 1px solid #1a1a1a;
    margin-top: 4rem;
  }
  .footer span { color: #ff2d78; }
</style>
<div class="footer">
  Built by <span>Kavana Manvi Krishnamurthy</span> · Hosted on GitHub Pages
</div>
