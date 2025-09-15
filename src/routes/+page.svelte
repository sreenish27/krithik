<script>
  // --- Updated Data for your portfolio ---

  const experience = [
    {
      company: "Wurq (at the Harvard i-lab)",
      role: "Product Manager Intern (Sep 2023 – Apr 2024)",
      achievements: [
        "Conducted user research with over 30 athletes to define functional requirements for a new ML-powered pose correction feature.",
        "Guided the development of a CNN model that reduced latency from 800ms to under 40ms by translating user needs into detailed technical specifications.",
        "Reduced model inference costs by 28% by analyzing cloud computing data and presenting a successful proposal for on-device processing.",
        "Drove a 30% increase in form-correction accuracy and a 45% lift in monthly usage by synthesizing A/B test results and user feedback.",
        "Improved development velocity by 30% within a global agile team by refining sprint planning and documenting user stories."
      ]
    },
    {
      company: "ZS Associates",
      role: "Business Operations Associate (June 2021 – June 2022)",
      achievements: [
        "Drove workflow optimizations impacting $1.2M in client revenue by analyzing business processes for a $32M pharmaceutical compensation platform.",
        "Supported the rollout of an analytics dashboard to over 200 enterprise users, gathering feedback to maintain a 98% user satisfaction rate.",
        "Increased quarterly feature delivery by 26% by writing user stories and acceptance criteria within an Agile framework.",
        "Grew the active user base by 45% to 580 by providing data analysis on key platform adoption metrics within an OKR framework.",
        "Reduced monthly support tickets by 40% by analyzing ticket data to identify user pain points and inform a system redesign."
      ]
    },
    {
      company: "Kalo Labs",
      role: "Founder (Mar 2020 – Oct 2020)",
      achievements: [
        "Founded and scaled a solo-operated digital marketing agency from $0 to $15K in monthly recurring revenue (MRR).",
        "Acquired and closed a portfolio of 12+ retained clients with an average contract value of over $1,200/month by engineering and executing a full-cycle sales process.",
        "Delivered an average 25% increase in organic traffic and a 15% reduction in client Cost Per Acquisition (CPA) by directing multi-channel marketing strategies.",
        "Cut administrative overhead by over 50% by building a scalable operational framework with automated reporting and standardized workflows."
      ]
    }
  ];

  const projects = [
    {
      title: "Film Search 🎬",
      description: "Ever get frustrated trying to find a movie you can't quite name? This is the fix. I built a search engine that lets you talk to it like a person, using an LLM to understand what you mean, not just what you type.",
      details: [
          "Architected a scalable data pipeline using a crawler and PostgreSQL, enabling real-time search across 54k+ films.",
          "Built core search functionality using TF-IDF and BM25 ranking algorithms to deliver relevant and fast query results.",
          "Integrated a Llama 3.1 70B LLM to create a ”Film Chat” feature, allowing users to interact with film data."
      ],
      stack: "Node.js, React, Express.js, PostgreSQL, Python, TailwindCSS, Scrapy, Groq",
      links: [
          { name: "Live", url: "https://filmsearch-kappa.vercel.app/" },
          { name: "Demo", url: "https://www.youtube.com/watch?v=ULXZU1060UU" },
          { name: "Code", url: "https://github.com/sreenish27/filmsearch" }
      ]
    },
    {
      title: "ChuckleBox 🤖",
      description: "This project, built with the MIT AI Club, tackles a tough problem: analyzing hours of audio. I designed a scalable AWS backend and an asynchronous pipeline that can take massive audio files and process them for machine learning analysis, all without crashing.",
      details: [],
      stack: "Python, React, Flask, TensorFlow, Large Language Models (LLMs), AWS",
      links: [
          { name: "Project Page", url: "https://www.sundai.club/projects/bf3fd58f-0f07-4d9b-a2a0-01a4582ce3ae" }
      ]
    },
    {
      title: "Customer Churn Analysis 📉",
      description: "A practical application of data science to predict customer churn for a music player. This project uses a mix of regression, SVM, and PCA to identify users who are likely to leave, giving the business a chance to intervene.",
      details: [],
      stack: "Python, Scikit-learn, Pandas, SVM, PCA",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/Customer-Churn-Analysis" }
      ]
    },
    {
      title: "Voyantra ✈️",
      description: "A full-stack travel and tour booking website. I built the backend API with Node.js and Express for handling user authentication, tour bookings, and payments, and crafted the frontend with server-side templates.",
      details: [],
      stack: "Node.js, Express.js, MongoDB, Mongoose, Pug, JavaScript",
      links: [
          { name: "Code", url: "https://github.com/sreenish27/voyantra" }
      ]
    },
    {
      title: "YouTube Comment Analysis & Generation 💬",
      description: "This project analyzes sentiment in YouTube comments and uses a fine-tuned GPT-2 model to generate new, contextually relevant comments. It's a deep dive into NLP and generative AI.",
      details: [],
      stack: "Python, TensorFlow, Keras, Hugging Face Transformers, NLTK, Pandas",
      links: [
        { name: "Code", url: "https://github.com/sreenish27/YouTube-Comment-Analysis-and-Text-Generation" }
      ]
    }
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
      { title: "Empire of AI: Dreams and Nightmares in Sam Altman's OpenAI", author: "Karen Hao" },
      { title: "Amusing Ourselves to Death", author: "Neil Postman" },
      { title: "Asura: Tale of the Vanquished", author: "Anand Neelakantan" }
  ];

  const skills = [
    {
      category: "Product & Design",
      items: ["Agile Methodologies", "User Research", "Requirements Gathering", "Business Case Development", "A/B Testing", "Stakeholder Management", "JIRA", "Figma"]
    },
    {
      category: "Languages & Frameworks",
      items: ["Python", "SQL", "JavaScript/TypeScript", "React", "Node.js", "Express.js", "TailwindCSS"]
    },
    {
      category: "Data & DevOps",
      items: ["PostgreSQL", "MongoDB", "AWS", "Docker", "Git", "CI/CD", "dbt", "ETL", "Looker"]
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
      <span>·</span>
      <a href="#contact">Contact</a>
    </div>
  </header>

    <section>
      <h2>What I’m Working Toward</h2>
      <p class="mission-statement">
        I'm seeking a role where I can own the full product lifecycle on an AI-native team. My goal is to operate as a true product builder, fusing my skills in engineering, product, and design to ship solutions that solve meaningful user problems.
      </p>
  </section>

  <section>
    <h2>Professional Journey</h2>
    <div class="job-list">
      {#each experience as job}
        <div class="job-entry">
          <h3>{job.company}</h3>
          <p class="role">{job.role}</p>
          <ul class="achievements-list">
            {#each job.achievements as achievement}
              <li>{achievement}</li>
            {/each}
          </ul>
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
          
          {#if project.details && project.details.length > 0}
            <ul class="achievements-list project-details">
              {#each project.details as detail}
                <li>{detail}</li>
              {/each}
            </ul>
          {/if}

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

<footer id="contact" class="site-footer">
    <div class="footer-content">
        <h2 class="footer-heading">Let's build something together.</h2>
        <p>If you have a project in mind or just want to connect, feel free to get in touch.</p>
        <div class="contact-links">
            <a href="mailto:krithiksaisreenishg@gmail.com">krithiksaisreenishg@gmail.com</a>
            <a href="tel:+18576939815">+1 (857) 693-9815</a>
        </div>
    </div>
    <div class="footer-bottom">
