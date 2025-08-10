<script>
  // --- Data for your portfolio ---

  const education = [
    {
      university: "Northeastern University – Boston, MA",
      degree: "Master of Science, Engineering Management",
      dates: "Sep 2022 – Dec 2024",
      courses: "Courses: Digital Product Design, Data Mining for Engineering, Natural Language Processing, Operations Research"
    },
    {
      university: "Visvesvaraya National Institute of Technology – Nagpur, India",
      degree: "Bachelor of Technology in Engineering",
      dates: "July 2017 – May 2021",
      courses: null
    }
  ];

  const professionalPath = [
    {
      title: "Product Manager Intern",
      company: "Wurq",
      location: "Cambridge, MA",
      dates: "Sept 2023 – Apr 2024",
      duties: [
        "Drove product strategy for an ML-powered fitness analytics platform, growing active users to 24,500 (40% increase) by launching sensor-to-insight features that translated raw data into actionable workout feedback.",
        "Reduced pose correction feature latency from 800ms to 40ms using CNN model distillation and on-device computing, boosting daily active users to 13,500 (35% growth) while slashing monthly cloud costs to $18,000 (28% drop).",
        "Led cross-functional agile development with teams in Boston, Frankfurt, and Milan, shortening sprint cycles to 7 weeks (30% faster) and maintaining defect rates below 5% by enforcing rigorous code reviews and testing protocols.",
        "Conducted user testing with over 30 athletes and ran A/B experiments, raising form accuracy to 91% (30% improvement) and increasing monthly feature activations to 7,250 (45% up) by refining algorithms based on real-world feedback.",
        "Built Go-To-Market partnerships with sports programs, retaining 8,500 subscribers (85% retention) and securing product-market fit.",
        "Applied the RICE prioritization framework to feature development, delivering 26 high-impact features on time per quarter (30% more).",
      ],
    },
    {
      title: "Business Operations Associate",
      company: "ZS Associates",
      location: "Pune, India",
      dates: "June 2021 – June 2022",
      duties: [
        "Owned end-to-end development of $32M pharmaceutical compensation platform, driving $1.2M revenue impact through optimized workflows for enterprise clients.",
        "Scaled analytics dashboard from pilot to 200+ enterprise users across neuroscience and nephrology divisions, maintaining 98% satisfaction.",
        "Introduced agile methodologies and automated SQL/Python data pipelines, delivering 24 features per quarter (26% increase) to support quarterly compensation cycles with faster, data-driven updates.",
        "Established an OKR framework to align business objectives with technical execution, growing platform active users to 580 (45% growth) across sales teams by focusing on key adoption metrics.",
        "Mentored junior team members on product methodology, boosting their feature prioritization accuracy to 90% (40% increase) and reducing backlog refinement time to 4 hours per sprint (50% decrease).",
        "Designed and built a hierarchical access control system for the MBO tool, reducing monthly support tickets to 300 (40% drop) by creating intuitive workflows that minimized user errors.",
      ],
    },
  ];

  const whatIBuilt = [
    {
      title: "Film Search",
      link: "#",
      description: "Architected a scalable data pipeline using a Python crawler and PostgreSQL, enabling real-time search across 54k+ films. Built core search functionality using TF-IDF and BM25 ranking algorithms to deliver relevant and fast query results. Integrated a Llama 3.1 70B LLM to create a ”Film Chat” feature, allowing users to interact with film data conversationally.",
      stack: "Node.js, React, Express.js, PostgreSQL, Postman, TailwindCSS, Python, Scrapy (Crawler), Groq (llama 70b 3.1 LLM)",
    },
    {
      title: "Voyantra: Budget Based Trip Planner",
      link: "#",
      description: "Analyzed user survey data to quantify traveler pain points and define the core project problem statement. Modeled the travel booking workflow to identify inefficiencies and design a more streamlined user process. Developed a quantitative model to score and prioritize features based on projected user impact. Synthesized market and user analysis into an MVP definition to secure project development resources.",
      stack: "Node.js, React, Express.js, MongoDB, Postman, TailwindCSS",
    },
  ];
</script>

<main>
  <header>
    <h1>KRITHIK SAI SREENISH GOPINATH</h1>
    <div class="contact-info">
        <span>krithiksaisreenishg@gmail.com</span>
        <span>&nbsp;|&nbsp;</span>
        <span>+1 857-693-9815</span>
        <span>&nbsp;|&nbsp;</span>
        <span>San Jose, CA</span>
    </div>
    <div class="header-links">
      <a href="#" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <a href="#" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </header>

  <section>
    <h2>Education</h2>
    <div class="education-list">
      {#each education as edu}
        <div class="degree-entry">
          <h3>{edu.degree}</h3>
          <p class="university">{edu.university} | {edu.dates}</p>
          {#if edu.courses}
            <p class="details">{edu.courses}</p>
          {/if}
        </div>
      {/each}
    </div>
  </section>

  <section>
    <h2>Professional Path</h2>
    <div class="job-list">
      {#each professionalPath as job}
        <div class="job-entry">
          <h3>{job.title}</h3>
          <p class="company">{job.company} | {job.location} | {job.dates}</p>
          <ul>
            {#each job.duties as duty}
              <li>{duty}</li>
            {/each}
          </ul>
        </div>
      {/each}
    </div>
  </section>

  <section>
    <h2>What I've Built</h2>
    <div class="project-grid">
      {#each whatIBuilt as project}
        <a
          href={project.link}
          target="_blank"
          rel="noopener noreferrer"
          class="project-card"
        >
          <h3>{project.title}</h3>
          <p class="description">{project.description}</p>
          <p class="stack"><strong>Tech Stack:</strong> {project.stack}</p>
        </a>
      {/each}
    </div>
  </section>

  <section>
    <h2>Skills</h2>
    <div class="skills-container">
        <div class="skill-category">
            <h3>Technical Stack</h3>
            <p>Python (Data Pipelines, Web Crawling), JavaScript/TypeScript, React, Node.js, Express.js, TailwindCSS, SQL (PostgreSQL), MongoDB, Natural Language Processing (NLP)</p>
        </div>
        <div class="skill-category">
            <h3>Infrastructure & DevOps</h3>
            <p>AWS (S3, EC2, Lambda), Docker, Git, CI/CD</p>
        </div>
        <div class="skill-category">
            <h3>Engineering Fundamentals</h3>
            <p>Data Structures, Algorithms, System Design, Microservices Architecture, Test-Driven Development (TDD)</p>
        </div>
        <div class="skill-category">
            <h3>Developer Tools</h3>
            <p>JIRA, Figma, Postman, Looker Studio, Tableau</p>
        </div>
    </div>
  </section>
</main>

<style>
  /* Base Styles */
  main {
    max-width: 800px;
    margin: 0 auto;
    padding: 4rem 2rem;
    display: flex;
    flex-direction: column;
    gap: 4rem;
  }
  h2 {
    font-size: 1.5rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 2rem;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 0.75rem;
  }
  h3 {
    font-size: 1.25rem;
  }
  p {
    margin: 0 0 1rem 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  /* Header Section */
  header {
    text-align: left;
    border-bottom: 1px solid var(--text-color);
    padding-bottom: 2rem;
  }
  header h1 {
    font-size: 2.25rem;
    margin-bottom: 0.5rem;
  }
  .contact-info {
      display: flex;
      flex-wrap: wrap;
      gap: 0.25rem;
      color: #555;
      margin-bottom: 1rem;
  }
  .header-links {
    margin-top: 1rem;
    display: flex;
    gap: 1.5rem;
    font-size: 1rem;
  }
  .header-links a {
    font-weight: 700;
  }

  /* Education Section */
  .education-list {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
  }
  .university {
      color: #555;
      font-weight: 700;
      margin-top: 0.25rem;
      margin-bottom: 0.25rem;
  }
  .details {
      font-size: 0.9rem;
      color: #333;
      margin: 0;
  }

  /* Experience Section */
  .job-list {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
  }
  .company {
    color: #555;
    font-size: 1rem;
    font-weight: 700;
    margin-top: 0.25rem;
  }
  .job-entry ul {
    margin-top: 1rem;
    padding-left: 1.2rem;
    list-style-type: disc;
  }
  .job-entry li {
    margin-bottom: 0.75rem;
  }

  /* Projects Section */
  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  .project-card {
    display: block;
    padding: 1.5rem;
    border: 1px solid var(--border-color);
    border-radius: 4px;
    background-color: var(--bg-color);
  }
  .project-card:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.15);
    border-color: var(--accent-color);
    text-shadow: none;
  }
  .project-card:hover h3 {
    color: var(--accent-color);
  }
  .description {
    color: #333;
    margin: 0.5rem 0;
  }
  .stack {
    font-size: 0.9rem;
    color: #555;
    margin: 0.5rem 0 0 0;
  }
  
  /* Skills Section */
  .skills-container {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
  }
  .skill-category h3 {
      font-size: 1.1rem;
      margin-bottom: 0.5rem;
      border-bottom: 1px solid var(--border-color);
      padding-bottom: 0.25rem;
  }
  .skill-category p {
      margin: 0;
      line-height: 1.7;
      color: #333;
  }
</style>
