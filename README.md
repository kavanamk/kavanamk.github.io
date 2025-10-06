<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kavana Manvi Krishnamurthy - Portfolio</title>
  <style>
    html {
      scroll-behavior: smooth;
      font-family: 'Helvetica Neue', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #fff;
      color: #333;
    }

    h2, h3 {
      color: #2a7ae2;
    }

    img {
      max-width: 100%;
      height: auto;
    }

    .link-boxes {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin: 2rem auto;
      max-width: 600px;
      flex-wrap: wrap;
    }

    .link-box {
      flex: 1 1 45%;
      background-color: #f3f3f3;
      border: 1px solid #ccc;
      border-radius: 8px;
      padding: 1.5rem;
      text-align: center;
      font-size: 1.1rem;
      color: #2a7ae2;
      text-decoration: none;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .link-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 10px rgba(0, 0, 0, 0.08);
    }

    .project-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 2rem;
      max-width: 900px;
      margin: 2rem auto;
    }

    .project-box {
      background-color: #f3f3f3;
      border: 1px solid #ccc;
      border-radius: 12px;
      padding: 1.5rem;
      color: #333;
      transition: transform 0.3s ease;
      text-decoration: none;
      display: block;
    }

    .project-box:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 10px rgba(0, 0, 0, 0.08);
    }

    .project-title {
      font-size: 1.2rem;
      font-weight: 600;
      color: #2a7ae2;
      margin-bottom: 0.5rem;
    }

    .project-description {
      font-size: 1rem;
      margin-bottom: 1rem;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .skill-tag {
      background-color: #dce6f9;
      color: #2a7ae2;
      font-size: 0.85rem;
      padding: 0.3rem 0.6rem;
      border-radius: 999px;
      font-weight: 500;
    }

    .course-card {
      border: 1px solid #ddd;
      padding: 1rem;
      border-radius: 8px;
      max-width: 600px;
      margin: 2rem auto;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
      transition: transform 0.2s ease;
    }

    @media (max-width: 768px) {
      .link-boxes {
        flex-direction: column;
        align-items: center;
      }

      .link-box {
        width: 80%;
      }

      .project-grid {
        grid-template-columns: 1fr;
        padding: 0 1rem;
      }

      h2, h3 {
        text-align: center;
      }
    }
  </style>
</head>
<body>

  <img src="images/LLM-13.jpg" style="display:block;margin:auto;" alt="Profile Banner" />

  <h3 style="text-align: center; color: #2a7ae2;">
    I'd be a great fit for these roles
  </h3>

  <h2 style="color: #2a7ae2; padding-top: 3rem;">EDUCATION</h2>

  <h3>Master of Science, Computer Science</h3>
  <h3><img src="images/depaul.jpg" width="30" style="vertical-align:middle;"/> Depaul University, Chicago (GPA - 3.86)</h3>

  <p><strong>Foundational CS courses:</strong> Object Oriented Programming, Distributed Systems, Database Management Systems, Algorithms and Data Structures</p>
  <p><strong>Data Science courses:</strong> Data Visualization, Regression & Analysis, Image Processing, Machine Learning, Computer Vision</p>

  <h3>Bachelor of Science, Computer Science</h3>
  <h3><img src="images/nieit.jpg" width="30" style="vertical-align:middle;"/> NIE, India</h3>

  <p><strong>Courses:</strong> Mathematics, Physics, Data Structures, Algorithms, Cybersecurity, IoT, UI Design, AI, Big Data, Software Engineering, OpenGL, Compiler Design</p>

  <h2 style="color: #2a7ae2;">WORK EXPERIENCE</h2>

  <h3><img src="images/oracle.jpg" width="30" style="vertical-align:middle;"/> Software Engineer at Oracle</h3>
  <ul>
    <li>Performed defect correction and ETL management using SQL, OCI, and Tableau.</li>
    <li>Led full-stack development for 75+ Jira tickets; reduced runtime from 6–7 hrs to 40s.</li>
    <li>Received “Innovate and Simplify” Award and “Star of the Sprint” twice.</li>
    <li>Investigated 35+ client issues to identify root causes.</li>
  </ul>

  <h3><img src="images/oracle.jpg" width="30" style="vertical-align:middle;"/> Software Intern at Oracle</h3>
  <ul>
    <li>Developed web features using ReactJS, Spring Boot, PHP, SQL, HTML, CSS, JS, and AJAX.</li>
    <li>Created 6+ dashboards visualizing Jenkins job execution for 30+ teams.</li>
    <li>Implemented UI enhancements recognized by senior leadership.</li>
  </ul>

  <h2 style="color: #2a7ae2;">SKILLS</h2>
  <ul>
    <li><strong>Languages:</strong> C, C++, Java, SQL, Python, Scala, Spark, R, MySQL</li>
    <li><strong>Web:</strong> HTML, CSS, JS, PHP, ReactJS, jQuery, AJAX</li>
    <li><strong>ML:</strong> TensorFlow, PyTorch, Tableau, MATLAB</li>
    <li><strong>Others:</strong> Git, Jenkins, Agile, CI/CD</li>
  </ul>

  <h2 style="color: #2a7ae2;">Expert in DSA and System Design</h2>
  <div class="link-boxes">
    <a class="link-box" href="https://github.com/kavanamk/Educative-DSA" target="_blank">DSA</a>
    <a class="link-box" href="https://github.com/kavanamk/Educative-System-Design" target="_blank">System Design</a>
  </div>

  <h2 style="color: #2a7ae2;">PROJECTS</h2>
  <div class="project-grid">

    <a class="project-box" href="https://github.com/kavanamk/Distributed-Systems" target="_blank">
      <div class="project-title">Predicting Birth Weight</div>
      <div class="project-description">Built regression model on 108k observations using variable selection and transformation.</div>
      <div class="skills">
        <div class="skill-tag">R</div><div class="skill-tag">Regression</div>
      </div>
    </a>

    <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning" target="_blank">
      <div class="project-title">Credit Risk</div>
      <div class="project-description">Used TF-IDF + OpenAI API to engineer features for credit loan classification (94% accuracy).</div>
      <div class="skills">
        <div class="skill-tag">Python</div><div class="skill-tag">TF-IDF</div><div class="skill-tag">NLP</div>
      </div>
    </a>

    <a class="project-box" href="https://github.com/kavanamk/Advanced-Machine-Learning" target="_blank">
      <div class="project-title">Autism Screening</div>
      <div class="project-description">SVM-RBF achieved 97.2% accuracy and perfect sensitivity using RFE and MI.</div>
      <div class="skills">
        <div class="skill-tag">Python</div><div class="skill-tag">SVM</div><div class="skill-tag">XGBoost</div>
      </div>
    </a>
  </div>

  <h2 style="color: #2a7ae2;">CERTIFICATES</h2>

  <div class="course-card">
    <h2>Machine Learning</h2>
    <p>Covered supervised and unsupervised learning using Octave/MATLAB with focus on intuition.</p>
    <img src="images/ml.jpg" alt="Machine Learning Certificate" />
  </div>

  <div class="course-card">
    <h2>Developing Large Language Models (LLMs)</h2>
    <p>Hands-on with PyTorch, Transformers, BERT fine-tuning, and attention mechanisms.</p>
    <img src="images/Educative_DevelopingLLM.jpg" alt="LLM Certificate" />
  </div>

  <div class="course-card">
    <h2>System Design</h2>
    <p>Designed scalable systems like YouTube, Uber, Instagram with real-world distributed systems concepts.</p>
    <img src="images/Educative_SysytemDesign.jpg" alt="System Design Certificate" />
  </div>

</body>
</html>
