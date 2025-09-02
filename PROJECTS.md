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

<button class="print-button" onclick="window.print()">🖨️ Print Resume Projects</button>

## Key Projects

### **Hospitality Management Platform Migration** — Mapal Software
*May 2024 – Present*

- Leading complete modernization of legacy hospitality management system serving 10,000+ daily users
- Implementing Angular frontend with DDD architecture and Go backend microservices
- Achieved 40% performance improvement and 80% code coverage through comprehensive testing strategy

### **Go-Kit Cross-Organization Libraries** — Enterprise Solution
*2024*

- Architected reusable Go microservice toolkit supporting cross-organizational collaboration with 15+ shared libraries
- Implemented standardized authentication, logging, monitoring, and circuit breaker patterns using go-kit principles
- Achieved faster development cycles across multiple teams through consistent service patterns and interfaces
- Built comprehensive testing suite with Testify achieving 95% code coverage and integrated OpenTelemetry observability

<div class="page-break-before"></div>

### **SSR Design System Framework** — Enterprise Solution
*2023*

- Developed production-ready design system combining Go backend APIs with Tailwind CSS, HTMX, and DaisyUI components
- Created 20+ reusable UI components with SSR capabilities, reducing frontend development time and providing UI standarization.
- Implemented dynamic theming system
- Built comprehensive documentation site with live component playground and integration examples

### **Mechanical Workshop ERP System** — Enterprise Solution
*2023*

- Designed comprehensive ERP system for automotive repair shops
- Built modular Go services with vertical slicing and microservices architecture handling client management, estimate generation, work order tracking, billing and supplier integration
- Implemented providers parts API integrations
- Created responsive dashboard using HTMX and Tailwind with SSR strategy.

### **Backend Service for Mobile Bank App** — AtSistemas
*2022*

- Provide a backend service in Nodejs for mobile App Bank Albiliad
- Modular project with users, auth, payments, wallets and actions authorization flow
- Integration with different API'S from Bank Albilad, like payments, clients and wallets.

### **Enterprise ERP Integration Platform** — CtGalega de Software
*2019 – 2021*

- Architected and led development of custom ERP integration platform for a electric sector client
- Modular project with users, auth, clients, estimates, billing, mobility, signature and issues tracker management
- Managed team of 5 mixed junior and senior developers
- Reduced deployment time through CI/CD flow implementation


