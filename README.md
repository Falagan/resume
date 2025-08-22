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
**Software Developer**

**Contact**  
Email: ep.falagan@outlook.es  
Phone: +34 671 323 914  
Location: Monforte de Lemos, Spain  
LinkedIn: [linkedin.com/in/eloyperezotero](https://linkedin.com/in/eloyperezotero)  
Github: [github.com/Falagan](https://github.com/Falagan)


## About

Framework-agnostic software developer focused on fundamentals and scalable solutions. A software developer should adhere to best practices by writing clean, efficient, scalable, well-tested, documented, and maintainable code. Easy to say, hard to accomplish. To achieve these goals, I follow the well-known SOLID principles, keeping in mind the balance between KISS and DRY, while also reflecting on YAGNI recursively. I aim to reduce the level of uncertainty to the minimum possible level in the analysis phase, enjoy the design and coding process, feel confident with testing, endure the deployment phase, and then start over again. What a ride!

## Soft Skills

Communication • Team collaboration • Analytical thinking • Continuous learning • Team management • Mentoring & Coaching • Problem solving • Adaptability

## Technical Stack

**Backend:** Node.js, Express, NestJS, Go.  
**Databases:** MySQL, MongoDB, Redis, Mongoose, TypeORM, GORM.  
**Testing:** Jest, Cypress.  
**DevOps:** Jenkins, Azure, PM2.
**Architecture:** Clean Architecture, Vertical Slice, REST, Microservices, DDD.
**Observability:** OpenTelemetry, Prometheus, Grafana.
**Code Versioning:** Git, Gitflow, Trunk Based.  
**Project Management:** Azure Devops, Jira.  
**Message Brokers:** Kafka, Azure Service Bus.  
**API Documentation:** OpenAPI.  
**Frontend:** Angular 2+, React, TypeScript, JavaScript, Redux, S/CSS, Bootstrap, Angular Material, PrimeNG, Tailwind.  

<div class="page-break-before"></div>

## Experience

### **Mapal Software** — Software Developer
*May 2024 – Present*

- Being part of a squad of 5 developers working with scrum.
- Developing from scratch a complete migration of a legacy web app that handles and covers all the hospitality industry features as staff management, documentation, analytics, logistics etc.
- Using Angular as main framework with DDD frontend architecture and working closely with the team of the company custom design system which is also developed with Angular tools.
- Design of backend services built Go with different architectures solutions such as REST and Microservices through the clean architecture principles.

**Technologies:** Go, Angular 2+, Azure, Redis, SQL.

### **Sngular Europe** — Software Developer
*Apr 2023 – May 2024*

- Full-Stack development focused on designing front-end and back-end software solutions best suited to each project.
- Design of front-end apps in Angular and React, combining components reuse, rendering optimization and simple, styled and fluid UI's, taken in advance of a set composed for mono-repos, lazy loading, micro-front-ends, web-components, CSR, SSR, SSG, Redux Pattern.
- Design of backend services built in Node.js (Express/NestJS) and Go with different architectures solutions such as REST and Microservices through the clean architecture principles.
- Coaching junior developers joining the team, doing frequent pair and mob programming sessions, while working with senior engineers to define road-maps and feature priorities.

**Technologies:** Go, Node.js, Angular 2+, React, Angular Universal, Redis, SQL, Azure.

### **AtSistemas** — Software Developer
*Dec 2021 – Apr 2023*

- Full-Stack development focused on designing front-end and back-end software solutions best suited to each project.
- Design of front-end apps in Angular and React, combining components reuse, rendering optimization and simple, styled and fluid UI's, taken in advance of a set composed for mono-repos, lazy loading, micro-front-ends, web-components, CSR, SSR, SSG, Redux Pattern.
- Design of backend services built in Node.js (Express/NestJS) and Go with different architectures solutions such as REST and Microservices through the clean architecture principles.
- Coaching junior developers joining the team, doing frequent pair and mob programming sessions, while working with senior engineers to define road-maps and feature priorities.
- Part of the core team responsible for company Node Community, given support for projects, creating training content and coaching junior developers through node core and NestJS training.

**Technologies:** Go, Node.js, Angular 2+, React, NestJS, MongoDB, Mongoose, SQL, Azure.

### **CtGalega de Software** — Software Developer
*Nov 2019 – Dec 2021*

- Full-stack developer on charge of a five senior developers team, responsible for the architecture, design, development, and testing of custom software built from scratch and integrated with our main ERP product.
- Create a complete development environment for a team-based software production, defining tools, protocols, work-flows and timelines.
- Design of front-end apps in Angular and React with Redux Pattern, combining components reuse, rendering optimization and simple, styled and fluid UI's.
- Design of back-end services built in Node.js (Express/NestJS) with MySQL, MongoDB and Redis with different architectures solutions such as REST and Microservices.
- Distribution of software with custom CI/CD with Jenkins on a self-administration host, supported with Azure DevOps.
- Coaching of junior developers joining the team, doing frequent pair and mob programming sessions, while working with senior engineers to define road-maps and feature priorities.

**Technologies:** Angular 2+, SQL, MongoDB, Mongoose, Jenkins, Azure, NestJS.

### **IgmWeb - Grupo HOTUSA** — Software Developer
*Jan 2018 – Dec 2019*

- Full-stack developer focused in a full web applications design and development, built front-ends with Angular and back-ends with Node.js and JavaEE. Responsible for the entire process from analysis, design and development to deploy and maintenance support.
- Initially focused on front-end, single-handedly led the efforts to re-build our front-ends for Hotels Bookings migrating from Knockout.js to Angular. Later on, perform API integration and developments with JavaEE to provide functionality to other front-ends.
- Built, in a back-end scope with Node.js and NestJS, a service with a high availability requirements and a heavy file treatment process, taking advantage of microservices with RabbitMQ as a queues broker.

**Technologies:** Node.js, Angular 2+, Jenkins, RabbitMQ, MongoDB, SQL.

### **CtGalega de Software** — Software Trainer
*Nov 2016 – Jan 2018*

- Integration of ERP software and new work-flows for companies in a digitalization evolution process.
- Technical coaching for the advance users of the ERP Software delivered to business customers.
- Actively participated in ERP support to help users to maximize performance and leverage our software.
- Managed communication with customers and developer teams to provide all the needed information about the software usage and testing results.
- Evaluate new client requirements and defined use cases.

### **Anthony Perry Designs & Builds** — Software Developer
*Feb 2016 – Jul 2016*

- Built virtual tours to create different showcases to share an immersive experience in custom-built homes designed by Anthony Perry's team.
- Developed a simple and functional web app to handle customers agenda and reports and projects evolution monitoring, using Java with Spring and JSP.

**Technologies:** Java, JSP.

### **Falagan Web** — Software Developer
*Nov 2015 – Feb 2016*

- Fullstack junior developer, building web apps with Spring (Boot, Security, Data JPA), JSP, JavaScript, MySQL and Bootstrap.

**Technologies:** Java, Spring, MySQL, Bootstrap, JSP.


## Education

**Certificate of Higher Education: Software Development**  
*IES San Clemente, Santiago de Compostela (2013-2015)*

**Erasmus Exchange**  
*Uniwersytet Warmińsko-Mazurski, Poland (2009-2010)*


## Certifications

- **English B2 (FCE)** — University of Cambridge (2012).
- **Scrum Master & Foundations** — EuropeanScrum.org (2022).
- **NestJS Fundamentals** — NestJS (2020).
- **Testing JavaScript with Jest** — Vitae Consultores (2020).
- **Angular: Advanced and Scalable** — TrainingIT (2019).
- **Big Data Technologies** — Derivalya Business & Training (2019).


## Languages

**Spanish:** Native  
**English:** Fluent
