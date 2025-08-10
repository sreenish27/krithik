<!-- 
  File: src/routes/+page.svelte
  Instructions: 
  1. Create a new SvelteKit project.
  2. Replace the entire content of 'src/routes/+page.svelte' with this code.
  3. Create 'src/app.css' and add the global styles provided in the instructions.
  4. Update 'src/app.html' to include the 'Inter' font.
-->

<script>
  // --- Data for your portfolio ---

  const professionalPath = [
    {
      title: "Senior Software Engineer",
      company: "Tech Corp",
      location: "San Francisco, CA",
      dates: "Jan 2022 - Present",
      duties: [
        "Led the development of a major feature from conception to launch, resulting in a 20% increase in user engagement.",
        "Mentored junior engineers, improving team productivity by 15%.",
        "Architected and implemented a new microservice for data processing.",
      ],
    },
    {
      title: "Software Engineer",
      company: "Innovate LLC",
      location: "Austin, TX",
      dates: "Jun 2019 - Dec 2021",
      duties: [
        "Developed and maintained front-end components using React and TypeScript.",
        "Collaborated with UX/UI designers to create a seamless user experience.",
        "Reduced API response times by 30% through performance optimization.",
      ],
    },
  ];

  const whatIBuilt = [
    {
      title: "Project Alpha",
      link: "https://github.com",
      description: "A data visualization dashboard that helps users understand complex datasets through interactive charts and graphs.",
      stack: "SvelteKit, D3.js, Node.js",
    },
    {
      title: "Portfolio Site",
      link: "https://github.com",
      description: "A minimalist, single-page portfolio built to showcase professional work and skills, with a focus on clean design.",
      stack: "SvelteKit, CSS",
    },
  ];

  const writings = [
    {
      title: "Understanding Svelte's Reactivity Model",
      link: "#",
      date: "Aug 2025",
      readTime: "7 min read",
    },
    {
      title: "CSS Techniques for Minimalist Design",
      link: "#",
      date: "Jul 2025",
      readTime: "5 min read",
    },
  ];
</script>

<main>
  <!-- =================================================================
  HEADER SECTION
  ================================================================== -->
  <header>
    <h1>Hi, I am Krithik.</h1>
    <p class="subtitle">
      I am a Software Engineer specializing in building scalable and beautiful
      web applications.
    </p>
    <div class="header-links">
      <a href="#" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <a href="#" target="_blank" rel="noopener noreferrer">GitHub</a>
      <a href="#" target="_blank">Resume</a>
    </div>
  </header>

  <!-- =================================================================
  PROFESSIONAL PATH SECTION
  ================================================================== -->
  <section>
    <h2>Professional Path</h2>
    <div class="job-list">
      {#each professionalPath as job}
        <div class="job-entry">
          <h3>{job.title}</h3>
          <p class="company">{job.company} | {job.location} — {job.dates}</p>
          <ul>
            {#each job.duties as duty}
              <li>{duty}</li>
            {/each}
          </ul>
        </div>
      {/each}
    </div>
  </section>

  <!-- =================================================================
  WHAT I'VE BUILT SECTION
  ================================================================== -->
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
          <p class="stack">Stack: {project.stack}</p>
        </a>
      {/each}
    </div>
  </section>

  <!-- =================================================================
  WRITINGS SECTION
  ================================================================== -->
  <section>
    <h2>Writings</h2>
    <div class="post-list">
      {#each writings as post}
        <a
          href={post.link}
          class="post-entry"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class="post-title">{post.title}</span>
          <span class="post-meta">{post.date} • {post.readTime}</span>
        </a>
      {/each}
    </div>
  </section>

  <!-- =================================================================
  ACADEMIC FOUNDATION SECTION
  ================================================================== -->
  <section>
    <h2>Academic Foundation</h2>
    <div class="degree-entry">
      <h3>Bachelor of Science in Computer Science</h3>
      <p class="university">University of California, Berkeley | Graduated May 2019</p>
      <p class="details">Honors: Magna Cum Laude</p>
    </div>
  </section>

  <!-- =================================================================
  MILESTONES SECTION
  ================================================================== -->
  <section>
    <h2>Milestones & Recognition</h2>
    <ul class="milestones-list">
      <li>AWS Certified Solutions Architect - Associate, 2023</li>
      <li>1st Place Winner - Bay Area Hackathon, 2022</li>
      <li>Tech Corp 'Innovator of the Year' Award, 2022</li>
    </ul>
  </section>

  <!-- =================================================================
  GET IN TOUCH SECTION (FOOTER)
  ================================================================== -->
  <footer class="footer-section">
    <h2>Get In Touch</h2>
    <p>Feel free to reach out for collaboration or inquiries.</p>
    <a href="mailto:your.email@example.com" class="email-link">your.email@example.com</a>
    <p class="copyright">© 2025 Krithik. Built with SvelteKit.</p>
  </footer>
</main>

<!-- =================================================================
  STYLES
================================================================== -->
<style>
  /* Base Styles */
  main {
    max-width: 800px;
    margin: 0 auto;
    padding: 4rem 2rem;
    display: flex;
    flex-direction: column;
    gap: 5rem;
  }
  h2 {
    font-size: 1.75rem;
    margin-bottom: 2rem;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 0.5rem;
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
  }
  .subtitle {
    font-size: 1.2rem;
    color: #555;
    max-width: 60ch;
  }
  .header-links {
    margin-top: 1.5rem;
    display: flex;
    gap: 1.5rem;
    font-size: 1rem;
  }
  .header-links a {
    font-weight: 700;
  }

  /* Professional Path Section */
  .job-list {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
  }
  .company {
    color: #555;
    font-size: 1rem;
    margin-top: 0.25rem;
  }
  .job-entry ul {
    margin-top: 1rem;
    padding-left: 1.2rem;
    list-style-type: disc;
  }
  .job-entry li {
    margin-bottom: 0.5rem;
  }

  /* What I've Built Section */
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
    color: #555;
    margin: 0.5rem 0;
  }
  .stack {
    font-size: 0.9rem;
    color: #333;
    font-weight: 700;
    margin: 0.5rem 0 0 0;
  }

  /* Writings Section */
  .post-list {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  .post-entry {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    border: 1px solid var(--border-color);
    border-radius: 4px;
  }
  .post-entry:hover {
    transform: translateX(5px);
    border-color: var(--accent-color);
    text-shadow: none;
  }
  .post-title {
    font-weight: 700;
  }
  .post-entry:hover .post-title {
    color: var(--accent-color);
  }
  .post-meta {
    font-size: 0.9rem;
    color: #555;
    flex-shrink: 0;
    margin-left: 1rem;
  }

  /* Academic Foundation Section */
  .university {
    color: #555;
    margin-top: 0.25rem;
  }
  .details {
    font-size: 0.9rem;
  }
  
  /* Milestones Section */
  .milestones-list li {
      padding: 0.5rem 0;
      border-bottom: 1px solid var(--border-color);
  }
  .milestones-list li:last-child {
      border-bottom: none;
  }

  /* Footer Section */
  .footer-section {
    text-align: center;
    border-top: 1px solid var(--border-color);
    padding-top: 4rem;
  }
  .email-link {
    font-size: 1.25rem;
    font-weight: 700;
    display: inline-block;
    margin: 1rem 0;
  }
  .copyright {
    margin-top: 2rem;
    font-size: 0.9rem;
    color: #555;
  }
</style>
