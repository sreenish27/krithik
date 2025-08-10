<script>
  // --- Data for your portfolio ---

  const experience = [
    {
      company: "Wurq (at the Harvard i-lab)",
      role: "Product Manager Intern (Sep 2023 – Apr 2024)",
      summary: "Shaped the product strategy for an ML-powered fitness platform, translating raw sensor data into actionable workout feedback based on direct athlete testing."
    },
    {
      company: "ZS Associates",
      role: "Business Operations Associate (June 2021 – June 2022)",
      summary: "Scaled a pharmaceutical compensation platform from pilot to hundreds of enterprise users by introducing agile workflows and automating data pipelines to improve efficiency."
    },
    {
      company: "Kalo Labs",
      role: "Founder (Mar 2020 – Oct 2020)",
      summary: "Founded a digital marketing agency where I led the full customer lifecycle from outreach to contract, and built a custom automation platform to streamline client notifications and lead management."
    }
  ];

  const projects = [
    {
      title: "Film Search 🎬",
      description: "Ever get frustrated trying to find a movie you can't quite name? This is the fix. I built a search engine from the ground up that lets you talk to it like a person. It uses a custom data pipeline and a 70B parameter LLM to understand what you mean, not just what you type.",
      stack: "Node.js, React, Express.js, PostgreSQL, Python, TailwindCSS, Scrapy, Groq",
      links: [
          { name: "Live", url: "https://filmsearch-kappa.vercel.app/" },
          { name: "Demo", url: "https://www.loom.com/share/df7dfc3116654913bf5fe05c97d909b7?sid=1323dae3-f9d0-4783-a884-a66ed147e8af" },
          { name: "Code", url: "https://github.com/sreenish27/filmsearch" }
      ]
    },
    {
      title: "ChuckleBox 🤖",
      description: "This project, built with the MIT AI Club, tackles a tough problem: analyzing hours of audio. I designed a scalable AWS backend and an asynchronous pipeline that can take massive audio files and process them for machine learning analysis, all without crashing.",
      stack: "Python, React, Flask, TensorFlow, Large Language Models (LLMs), AWS",
      links: [
          { name: "Project Page", url: "https://www.sundai.club/projects/bf3fd58f-0f07-4d9b-a2a0-01a4582ce3ae" }
      ]
    },
    {
      title: "YouTube Comment Analyzer 📊",
      description: "An NLP exploration that visualizes YouTube comment sections as a word cloud and uses the data to train a text generation model. It's a quick way to get the pulse of a comment section and see what the hive mind is thinking.",
      stack: "Python, NLP, Machine Learning",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/YouTube-Comment-Analysis-and-Text-Generation" }
      ]
    },
    {
      title: "Customer Churn Analysis 📉",
      description: "A practical application of data science to predict customer churn for a music player. This project uses a mix of regression, SVM, and PCA to identify users who are likely to leave, giving the business a chance to intervene.",
      stack: "Python, Scikit-learn, Pandas, SVM, PCA",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/Customer-Churn-Analysis" }
      ]
    },
    {
      title: "Ball Classifier 🏀",
      description: "A fun computer vision project that uses a neural network to recognize different kinds of sports balls. It's a simple but effective demonstration of building and training a custom image classifier.",
      stack: "Python, TensorFlow, Keras, Computer Vision",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/ball_classifier" }
      ]
    },
    {
      title: "Voyantra 🌍",
      description: "A no-nonsense trip planner for when your wallet has the final say. Instead of endless scrolling, you just tell it your budget, and it generates a full travel itinerary. It’s all about making travel accessible by putting the financial constraints first.",
      stack: "Node.js, React, Express.js, MongoDB, TailwindCSS",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/voyantra" }
      ]
    },
  ];
  
  const education = [
    {
        university: "Northeastern University – Boston, MA",
        degree: "Master of Science, Engineering Management (2022–2024)",
        notes: [
            "Secured 2nd place representing the university's chess team.",
            "Explored Boston and have visited 10+ states across the US (and counting)."
        ]
    },
    {
        university: "Visvesvaraya National Institute of Technology – Nagpur, India",
        degree: "Bachelor of Technology in Engineering (2017–2021)",
        notes: [
            "Secured admission by placing in the top 1% of the national JEE Mains entrance exam.",
            "Represented the university on the competitive dance team."
        ]
    }
  ];

  const bookshelf = [
      { title: "Empire of AI: Dreams and Nightmares in Sam Altman's OpenAI", author: "Walter Isaacson" },
      { title: "Amusing Ourselves to Death", author: "Neil Postman" },
      { title: "Asura: Tale of the Vanquished", author: "Anand Neelakantan" }
  ];

  const skills = [
    {
        category: "Product & Design",
        items: ["UX/UI Design", "Figma", "Stakeholder Management", "JIRA", "Agile Methodologies", "Go-to-Market Strategy"]
    },
    {
        category: "Languages & Frameworks",
        items: ["Python", "JavaScript/TypeScript", "React", "Node.js", "Express.js", "TailwindCSS"]
    },
    {
        category: "Databases & DevOps",
        items: ["PostgreSQL", "MongoDB", "AWS", "Docker", "Git", "CI/CD"]
    },
    {
        category: "Engineering Fundamentals",
        items: ["System Design", "Microservices", "TDD", "Algorithms", "Data Structures"]
    }
  ];

</script>

<main>
  <header class="intro-header">
    <h1 class="greeting">Hi, I’m Krithik 👋</h1>
    <p class="intro-text">
        I’m a <strong>product builder</strong> who bridges the gap between ambitious technical goals and real-world business needs. I thrive in roles that demand full ownership—from initial strategy and design to engineering execution and stakeholder management. I'm the person you bring in when you need to not only build a product right, but also build the right product.
        <br><br>
        Based in San Jose, CA, and ready to relocate for the right opportunity. Outside of work, you’ll usually find me hitting the gym, playing chess, diving into a good non-fiction book, or reading up about the latest tech advancements on Twitter.
    </p>
    <div class="header-links">
      <a href="https://www.linkedin.com/in/krithiksai/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <span>·</span>
      <a href="https://github.com/sreenish27" target="_blank" rel="noopener noreferrer">GitHub</a>
      <span>·</span>
      <a href="https://x.com/SaiSreenish" target="_blank" rel="noopener noreferrer">Twitter</a>
      <span>·</span>
      <a href="https://medium.com/@krithikintl" target="_blank" rel="noopener noreferrer">Writings</a>
      <span>·</span>
      <a href="resume.pdf" target="_blank">Resume</a>
    </div>
  </header>

  <section>
      <h2>What I’m Working Toward</h2>
      <p class="mission-statement">
        I’m seeking a role where I can own the <strong>end-to-end product vision</strong>, combining strategy, design, and engineering into solutions that stick. I'm actively looking for positions like <strong>Product Manager, Product Engineer, Design Engineer, Product Analyst,</strong> or <strong>Product Associate</strong> in the tech industry at large.
      </p>
  </section>

  <section>
    <h2>Professional Journey</h2>
    <div class="job-list">
      {#each experience as job}
        <div class="job-entry">
          <h3>{job.company}</h3>
          <p class="role">{job.role}</p>
          <p class="job-summary">{job.summary}</p>
        </div>
      {/each}
    </div>
  </section>

  <section>
    <h2>What I’ve Built</h2>
    <div class="project-grid">
      {#each projects as project}
        <div class="project-card">
          <h3>{project.title}</h3>
          <p class="description">{project.description}</p>
          <p class="stack"><strong>Stack:</strong> {project.stack}</p>
          <div class="project-links">
            {#each project.links as link}
                <a href={link.url} target="_blank" rel="noopener noreferrer">{link.name}</a>
            {/each}
          </div>
        </div>
      {/each}
    </div>
  </section>

  <section>
    <h2>Education & Milestones</h2>
    <div class="job-list">
        {#each education as school}
            <div class="job-entry">
                <h3>{school.university}</h3>
                <p class="role">{school.degree}</p>
                <ul class="notes-list">
                    {#each school.notes as note}
                        <li>{note}</li>
                    {/each}
                </ul>
            </div>
        {/each}
    </div>
  </section>

  <section>
      <h2>From the Bookshelf</h2>
      <div class="bookshelf">
          {#each bookshelf as book}
              <div class="book-entry">
                  <span class="book-title">{book.title}</span>
                  <span class="book-author">by {book.author}</span>
              </div>
          {/each}
      </div>
      <a href="https://www.goodreads.com/user/show/172059882-krithik" target="_blank" rel="noopener noreferrer" class="goodreads-link">
          View all on Goodreads →
      </a>
  </section>

  <section>
    <h2>Skills at a Glance</h2>
    <div class="skills-section-container">
      {#each skills as category}
        <div class="skill-group">
            <h4>{category.category}</h4>
            <div class="skills-tag-container">
                {#each category.items as skill}
                    <span class="skill-tag">{skill}</span>
                {/each}
            </div>
        </div>
      {/each}
    </div>
  </section>
</main>

<style>
  :root {
      --accent-color: #FF3B30; /* Red Accent Color */
      --bg-color: #f7f7f7; /* Very light grey */
      --border-color: #ddd;
      --selection-bg: #FBBF24; /* Gold/Yellow selection color */
  }

  /* --- Custom Cursor & Selection --- */
  html {
      cursor: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><line x1="22" y1="12" x2="18" y2="12"></line><line x1="6" y1="12" x2="2" y2="12"></line><line x1="12" y1="6" x2="12" y2="2"></line><line x1="12" y1="22" x2="12" y2="18"></line></svg>') 12 12, auto;
  }

  ::selection {
      background-color: var(--selection-bg);
      color: #111;
      text-shadow: none;
  }
  ::-moz-selection { /* For Firefox */
      background-color: var(--selection-bg);
      color: #111;
      text-shadow: none;
  }
  /* --- End of Custom Styles --- */


  /* Base Styles */
  body {
      background-color: var(--bg-color);
      margin: 0;
      padding: 0;
      font-family: 'Manrope', sans-serif;
      color: #333;
  }
  main {
    max-width: 800px;
    margin: 0 auto;
    padding: 6rem 2rem 4rem 2rem;
    display: flex;
    flex-direction: column;
    gap: 4rem;
  }
  h2 {
    font-size: 1.25rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 1.5rem;
    border-bottom: 2px solid var(--border-color);
    padding-bottom: 0.5rem;
  }
  h3 {
    font-size: 1.25rem;
    font-weight: 700;
  }
  p {
    margin: 0 0 1rem 0;
  }

  /* Header / Intro Section */
  .intro-header {
    text-align: left;
    padding-bottom: 2rem;
  }
  .greeting {
      font-size: 2.5rem;
      font-weight: 800;
      margin-bottom: 1rem;
  }
  .intro-text {
      font-size: 1.2rem;
      line-height: 1.7;
      color: #333;
      max-width: 70ch;
  }
  .header-links {
    margin-top: 2rem;
    display: flex;
    align-items: center;
    gap: 0.75rem;
    font-size: 1rem;
  }
  .header-links a {
    font-weight: 700;
    padding-bottom: 2px;
    border-bottom: 2px solid transparent;
    color: #111;
    text-decoration: none;
  }
  .header-links a:hover {
      color: var(--accent-color);
      border-bottom-color: var(--accent-color);
      transform: translate(-2px, -2px);
  }
  .header-links span {
      color: var(--border-color);
  }

  /* Mission Statement Section */
  .mission-statement {
      font-size: 1.2rem;
      line-height: 1.7;
      color: #333;
  }

  /* Professional Journey & Education Sections */
  .job-list {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }
  .role {
    color: #555;
    font-size: 1rem;
    font-weight: 700;
    margin: 0.25rem 0 0.5rem 0;
  }
  .job-summary {
      color: #333;
      line-height: 1.7;
      margin: 0;
  }
  .notes-list {
      list-style-type: '→ ';
      padding-left: 1.2rem;
      color: #333;
      line-height: 1.7;
      margin-top: 1rem;
  }
  .notes-list li {
      margin-bottom: 0.5rem;
  }

  /* What I've Built Section */
  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  .project-card {
    padding: 1.5rem;
    border: 2px solid var(--border-color);
    border-radius: 4px;
    background-color: white;
    transition: all 0.2s ease-out;
  }
  .project-card:hover {
    transform: translate(-4px, -4px) scale(1.01);
    box-shadow: 4px 4px 0px #111;
    border-color: #111;
    background-color: rgba(255, 59, 48, 0.05);
  }
  .description {
    color: #333;
    margin: 0.5rem 0 1.5rem 0;
    line-height: 1.7;
  }
  .stack {
    font-size: 0.9rem;
    color: #555;
    margin: 0;
  }
  .project-links {
      margin-top: 1.5rem;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
  }
  .project-links a {
      font-weight: 700;
      font-size: 0.9rem;
      padding: 0.25rem 0.75rem;
      border: 2px solid #111;
      border-radius: 4px;
      color: #111;
      transition: all 0.2s ease-out;
      text-decoration: none;
  }
  .project-links a:hover {
      background-color: #111;
      color: white;
      transform: translateY(-2px);
  }

  /* Bookshelf Section */
  .bookshelf {
      display: flex;
      flex-direction: column;
      gap: 1rem;
  }
  .book-entry {
      display: flex;
      flex-direction: column;
      padding: 0.75rem 0;
      border-bottom: 1px solid var(--border-color);
  }
  .book-title {
      font-weight: 700;
      color: #111;
  }
  .book-author {
      font-size: 0.9rem;
      color: #555;
  }
  .goodreads-link {
      margin-top: 1.5rem;
      font-weight: 700;
      display: inline-block;
      color: #111;
      text-decoration: none;
  }
  .goodreads-link:hover {
      color: var(--accent-color);
  }

  /* Skills at a Glance Section */
  .skills-section-container {
      display: grid;
      grid-template-columns: 1fr;
      gap: 2rem;
  }
  .skill-group h4 {
      font-size: 1rem;
      font-weight: 700;
      margin: 0 0 1rem 0;
      color: #111;
  }
  .skills-tag-container {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
  }
  .skill-tag {
    background-color: #e9e9e9;
    padding: 0.5rem 1rem;
    border-radius: 2rem;
    font-size: 0.9rem;
    font-weight: 700;
    color: #333;
    transition: all 0.2s ease-out;
  }
  .skill-tag:hover {
      background-color: var(--accent-color);
      color: white;
      transform: translateY(-2px);
  }
</style>
