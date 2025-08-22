<style>
/* Professional Resume Typography */
@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;1,400&family=Source+Sans+Pro:wght@300;400;600;700&display=swap');

body {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;
  font-size: 16px;
  line-height: 1.5;
  color: #2c3e50;
  max-width: 850px;
  margin: 0 auto;
  padding: 3rem 2rem;
  background: #ffffff;
  font-weight: 400;
}

/* Name and title */
h1 {
  font-family: 'Crimson Text', Georgia, serif;
  font-size: 3rem;
  font-weight: 600;
  color: #1a202c;
  margin-bottom: 0.25rem;
  letter-spacing: -0.02em;
  line-height: 1.1;
}

h1 + p strong {
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 1.25rem;
  font-weight: 300;
  color: #4a5568;
  letter-spacing: 0.05em;
}

/* Section headers */
h2 {
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 1.4rem;
  font-weight: 700;
  color: #1a202c;
  margin-top: 3rem;
  margin-bottom: 1.5rem;
  border-bottom: 2px solid #3182ce;
  padding-bottom: 0.5rem;
  letter-spacing: 0.02em;
}

/* Job titles and subsections */
h3 {
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 1.15rem;
  font-weight: 600;
  color: #2d3748;
  margin-top: 2rem;
  margin-bottom: 0.5rem;
  line-height: 1.3;
}

/* Dates and locations */
em {
  font-family: 'Source Sans Pro', sans-serif;
  font-style: italic;
  color: #718096;
  font-size: 0.95rem;
  font-weight: 400;
}

/* Body text */
p {
  margin-bottom: 1rem;
  text-align: left;
  hyphens: auto;
}

/* Strong text (company names, etc.) */
strong {
  font-weight: 600;
  color: #1a202c;
}

/* Lists */
ul, ol {
  margin-bottom: 1.25rem;
  padding-left: 0;
  list-style: none;
}

li {
  margin-bottom: 0.75rem;
  line-height: 1.6;
  position: relative;
  padding-left: 1.25rem;
}

li::before {
  content: "•";
  color: #3182ce;
  font-weight: 600;
  position: absolute;
  left: 0;
  top: 0;
}

/* Links */
a {
  color: #3182ce;
  text-decoration: none;
  font-weight: 500;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s ease;
}

a:hover {
  border-bottom-color: #3182ce;
}

/* Contact section */
body > p:nth-of-type(2) {
  font-size: 1rem;
  line-height: 1.8;
  margin-bottom: 2.5rem;
  color: #4a5568;
}

/* Skills section - inline styling */
h2:contains("Soft Skills") + p,
h2:contains("Technical Stack") + p {
  font-size: 0.95rem;
  line-height: 1.7;
}

/* Technologies in experience */
p:contains("Technologies:") {
  font-size: 0.9rem;
  color: #718096;
  font-style: italic;
  margin-top: 0.75rem;
}

/* Print styles */
@media print {
  .print-button {
    display: none !important;
  }
  
  body {
    font-size: 12pt;
    line-height: 1.4;
    padding: 1rem;
    max-width: none;
  }
  
  /* Page break controls */
  .page-break-before {
    page-break-before: always;
  }
  
  .page-break-after {
    page-break-after: always;
  }
  
  .no-page-break {
    page-break-inside: avoid;
  }
  
  /* Keep job entries together */
  h3 {
    page-break-after: avoid;
  }
  
  /* Avoid breaking between job title and content */
  h3 + p,
  h3 + ul {
    page-break-before: avoid;
  }
  
  /* Keep experience sections together when possible */
  .experience-item {
    page-break-inside: avoid;
  }
  
  /* Force page break before Experience section */
  h2:contains("Experience") {
    page-break-before: always;
  }
  
  h1 {
    font-size: 24pt;
    margin-bottom: 6pt;
  }
  
  h2 {
    font-size: 14pt;
    margin-top: 18pt;
    margin-bottom: 8pt;
    border-bottom: 1.5pt solid #000;
  }
  
  h3 {
    font-size: 12pt;
    margin-top: 12pt;
    margin-bottom: 4pt;
  }
  
  p, li {
    margin-bottom: 4pt;
  }
  
  a {
    color: #000;
    text-decoration: underline;
  }
}

/* Mobile responsive */
@media (max-width: 768px) {
  body {
    padding: 1.5rem 1rem;
    font-size: 15px;
  }
  
  h1 {
    font-size: 2.25rem;
  }
  
  h2 {
    font-size: 1.25rem;
    margin-top: 2.5rem;
  }
  
  h3 {
    font-size: 1.1rem;
  }
}

.print-button {
  position: fixed;
  top: 20px;
  right: 20px;
  background: #3182ce;
  color: white;
  border: none;
  padding: 12px 24px;
  border-radius: 8px;
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  box-shadow: 0 4px 12px rgba(49, 130, 206, 0.3);
  transition: all 0.2s ease;
  z-index: 1000;
}

.print-button:hover {
  background: #2c5282;
  transform: translateY(-2px);
  box-shadow: 0 6px 16px rgba(49, 130, 206, 0.4);
}

.print-button:active {
  transform: translateY(0);
}
</style>

<button class="print-button" onclick="window.print()">🖨️ Print Resume</button>

# Eloy Pérez
**SOFTWARE DEVELOPER**

**Contact**  
Email: ep.falagan@outlook.es  
Phone: +34 671 323 914  
Location: Monforte de Lemos, Spain  
LinkedIn: [linkedin.com/in/eloyperezotero](https://linkedin.com/in/eloyperezotero)  
Github: [github.com/Falagan](https://github.com/Falagan)

## About

Framework-agnostic software developer with **6+ years of experience** building scalable solutions across hospitality, ERP, and consulting domains. Passionate about clean architecture, **leading technical teams**, and delivering maintainable code following SOLID principles. Proven track record in **mentoring developers**, driving digital transformation projects, and implementing modern development practices. Expertise in both frontend and backend technologies with a focus on performance optimization and architectural decision-making.

## Technical Stack

**Backend:** Node.js, Express, NestJS, Go.  
**Frontend:** Angular 2+, React, TypeScript, JavaScript, Redux, SCSS, Bootstrap, Angular Material, PrimeNG, Tailwind.  
**Databases:** MySQL, MongoDB, Redis, Mongoose, TypeORM, GORM.  
**Testing:** Jest, Cypress, Testify, Unit Testing, Integration Testing, E2E Testing.  
**Code Quality & Security:** ESLint, Prettier, TSLint, go vet, go fmt, staticcheck, SonarQube, Snyk.  
**DevOps:** Jenkins, Azure, PM2, Docker, CI/CD Pipelines.  
**Architecture:** Clean Architecture, Vertical Slice, REST, Microservices, DDD.  
**Observability:** OpenTelemetry, Prometheus, Grafana.  
**Code Versioning:** Git, Gitflow, Trunk-based Development.  
**Project Management:** Azure DevOps, Jira.  
**Message Brokers:** Kafka, Azure Service Bus.  
**API Documentation:** OpenAPI, Swagger.

<div class="page-break-before"></div>

## Key Projects

### **Hospitality Management Platform Migration** — Mapal Software
*May 2024 – Present*

- Leading complete modernization of legacy hospitality management system serving 10,000+ daily users
- Implementing Angular frontend with DDD architecture and Go backend microservices
- Achieved 40% performance improvement and 90% code coverage through comprehensive testing strategy

### **Go-Kit Cross-Organization Libraries** — Open Source Initiative
*2024*

- Architected reusable Go microservice toolkit supporting cross-organizational collaboration with 15+ shared libraries
- Implemented standardized authentication, logging, monitoring, and circuit breaker patterns using go-kit principles
- Achieved 30% faster development cycles across multiple teams through consistent service patterns and interfaces
- Built comprehensive testing suite with Testify achieving 95% code coverage and integrated OpenTelemetry observability

### **Go-DS Design System Framework** — Personal Project
*2024*

- Developed production-ready design system combining Go backend APIs with Tailwind CSS, HTMX, and DaisyUI components
- Created 50+ reusable UI components with SSR capabilities, reducing frontend development time by 60%
- Implemented dynamic theming system and accessibility standards (WCAG 2.1 AA compliance)
- Built comprehensive documentation site with live component playground and integration examples

<div class="page-break-before"></div>

### **RunCode-OS: Mechanical Workshop ERP System** — Enterprise Solution
*2024*

- Designed comprehensive ERP system for automotive repair shops managing 5,000+ client records and inventory integration
- Built modular Go microservices architecture handling client management, estimate generation, work order tracking, and supplier integration
- Implemented real-time parts sourcing with automated supplier API integrations reducing procurement time by 70%
- Created responsive dashboard using HTMX and Tailwind with invoice generation, payment tracking, and comprehensive reporting

### **Multi-Client Consulting Solutions** — Sngular Europe
*2023 – 2024*

- Delivered 12+ full-stack projects using Angular, React, Node.js, and Go across various industries
- Implemented micro-frontend architecture supporting 50,000+ concurrent users
- Achieved 60% faster page loads through SSR/SSG optimization techniques

### **Enterprise ERP Integration Platform** — CtGalega de Software
*2019 – 2021*

- Architected and led development of custom ERP integration platform processing 1M+ daily transactions
- Managed team of 5 senior developers with €2M+ project budget
- Reduced deployment time from 4 hours to 30 minutes through CI/CD implementation

<div class="page-break-before"></div>

## Experience

### **Mapal Software** — Software Developer
*May 2024 – Present*

- Leading a **5-developer scrum team** specializing in hospitality industry software solutions
- Spearheading the complete migration of a **legacy web application serving 10,000+ daily users** with comprehensive hospitality operations including staff management, documentation, analytics, and logistics
- Implementing scalable frontend solutions using Angular with Domain-Driven Design (DDD) architecture while **reducing load times by 40%** through optimization techniques
- Architecting high-performance backend services in Go using clean architecture principles with REST API design and microservices patterns
- Successfully mentoring **3 junior developers** with 100% team retention through structured pair programming and mob programming sessions

*Technologies: Go, Angular 2+, Azure, Redis, SQL*

### **Sngular Europe** — Software Developer
*Apr 2023 – May 2024*

- Delivered full-stack consulting solutions across **12+ client projects** with focus on optimal technology selection and rapid deployment
- Built responsive frontend applications using Angular and React, implementing advanced patterns including mono-repos, lazy loading, micro-frontends, and web components, **improving development efficiency by 30%**
- Developed scalable backend services using Node.js (Express/NestJS) and Go with clean architecture and microservices patterns, **handling 50,000+ concurrent users**
- Utilized modern rendering techniques including CSR, SSR, SSG, and Angular Universal for **optimal SEO performance and 60% faster initial page loads**
- Collaborated with senior engineers on technical roadmaps while mentoring **4 junior developers** across multiple project teams

*Technologies: Go, Node.js, Angular 2+, React, Angular Universal, Redis, SQL, Azure*

<div class="page-break-before"></div>

### **AtSistemas** — Software Developer
*Dec 2021 – Apr 2023*

- Specialized in full-stack development with emphasis on selecting optimal architectural patterns for each project's requirements across **8+ enterprise projects**
- Created dynamic frontend solutions using Angular and React with advanced component reusability and rendering optimization, **achieving 95% component reusability rate**
- Architected robust backend services using Node.js, Express, NestJS, and Go with microservices and clean architecture approaches, **reducing system downtime by 80%**
- Served as **core team member for the company's Node.js Community** of 50+ developers, providing project support and creating comprehensive training materials
- Led technical mentoring initiatives and delivered NestJS training programs, **successfully upskilling 15+ junior developers** with measurable performance improvements

*Technologies: Go, Node.js, Angular 2+, React, NestJS, MongoDB, Mongoose, SQL, Azure*

### **CtGalega de Software** — Software Developer
*Nov 2019 – Dec 2021*

- Led a **team of 5 senior developers**, overseeing architecture, design, development, and testing of custom software integrated with the main ERP product, **managing €2M+ project budget**
- Established comprehensive development environment including tools, protocols, workflows, and project timelines, **reducing deployment time from 4 hours to 30 minutes**
- Designed frontend applications using Angular and React with Redux pattern, focusing on component reusability and performance optimization, **achieving 99.9% uptime**
- Built backend services with Node.js (Express/NestJS) integrated with MySQL, MongoDB, and Redis using REST and microservices architectures, **processing 1M+ daily transactions**
- Implemented custom CI/CD pipelines using Jenkins with self-hosted infrastructure, supported by Azure DevOps integration, **increasing deployment frequency by 300%**
- Provided technical leadership through mentoring, pair programming, and strategic roadmap planning, **achieving 100% team retention and 25% productivity increase**

*Technologies: Angular 2+, SQL, MongoDB, Mongoose, Jenkins, Azure, NestJS*

<div class="page-break-before"></div>

### **IgmWeb - Grupo HOTUSA** — Software Developer
*Jan 2018 – Dec 2019*

- Delivered end-to-end web application development using Angular frontend and Node.js/JavaEE backend technologies for **Europe's leading hotel group**
- Single-handedly led the complete migration of hotel booking frontend applications from Knockout.js to Angular architecture, **serving 500,000+ monthly bookings**
- Developed high-availability file processing service using Node.js and NestJS with microservices architecture and RabbitMQ message queuing, **achieving 99.95% uptime and processing 100,000+ files daily**
- Integrated APIs and developed JavaEE solutions to support multiple frontend applications, **reducing API response time by 50%**
- Managed full software lifecycle from analysis and design through deployment and maintenance, **delivering projects 20% under budget**

*Technologies: Node.js, Angular 2+, Jenkins, RabbitMQ, MongoDB, SQL*

### **CtGalega de Software** — Software Trainer
*Nov 2016 – Jan 2018*

- Facilitated ERP software integration and digital transformation workflows for enterprise clients
- Provided technical training and coaching to advanced users of ERP systems
- Delivered comprehensive software support to maximize client performance and software utilization
- Coordinated communication between customers and development teams for requirements gathering and testing feedback
- Analyzed client requirements and defined detailed use cases for software enhancements

### **Anthony Perry Designs & Builds** — Software Developer
*Feb 2016 – Jul 2016*

- Developed immersive virtual tour applications to showcase custom-built home designs
- Built customer management web application for agenda handling, project monitoring, and progress reporting using Java Spring framework and JSP

*Technologies: Java, Spring, JSP*

### **Falagan Web** — Software Developer
*Nov 2015 – Feb 2016*

- Developed full-stack web applications using Spring framework (Boot, Security, Data JPA) with JSP frontend and MySQL database integration

*Technologies: Java, Spring, MySQL, Bootstrap, JSP*

<div class="page-break-before"></div>

## Soft Skills

**Leadership & Mentoring:** Successfully led teams of up to 5 senior developers, mentored 22+ junior developers with 100% retention rate  
**Communication & Collaboration:** Facilitated cross-functional teams, client presentations, and technical training sessions  
**Problem Solving & Analysis:** Architected solutions for complex technical challenges, optimized performance by up to 60%  
**Continuous Learning & Adaptability:** Rapidly adopted new technologies, frameworks, and methodologies to meet project requirements  

## Education

**Certificate of Higher Education: Software Development**  
*IES San Clemente, Santiago de Compostela (2013-2015)*

**Erasmus Exchange**  
*Uniwersytet Warmińsko-Mazurski, Poland (2009-2010)*

## Certifications

- **English B2 (FCE)** — University of Cambridge (2012)
- **Scrum Master & Foundations** — EuropeanScrum.org (2022)
- **NestJS Fundamentals** — NestJS (2020)
- **Testing JavaScript with Jest** — Vitae Consultores (2020)
- **Angular: Advanced and Scalable** — TrainingIT (2019)
- **Big Data Technologies** — Derivalya Business & Training (2019)

## Languages

**Spanish:** Native  
**English:** Fluent
