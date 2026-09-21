<style>
  /* Force hide default GitHub template elements */
  header, #header, .title, h1:first-of-type:not(.header-block h1) {
    display: none !important;
  }
  
  /* Overrides GitHub's secret default wrapper settings to allow full width stretch */
  html, body, .wrapper, #main_content, .main-content, #content, .container-lg, .markdown-body, .portfolio-container, .scroll-content, div, section, main {
    max-width: 100% !important;
    width: 100% !important;
    padding: 0 !important;
    margin: 0 !important;
    box-sizing: border-box !important;
  }

  body, h1, h2, h3, p, a, li, span, div { 
    font-family: 'Arial', sans-serif !important; 
  }

  body { 
    background-color: #1A488E !important; 
    margin: 0 !important;
    padding: 0 !important;
  }
  
  /* MASTER FIXED WRAPPER - HIGHEST LAYER */
  .master-sticky-header {
    position: fixed !important;
    top: 0 !important;
    left: 0 !important;
    width: 100% !important;
    z-index: 999999 !important; 
    background-color: #1A488E !important; 
    padding: 20px 4% 5px 4% !important;
    box-sizing: border-box !important;
  }

  .portfolio-container {
    width: 100% !important;
    max-width: 100% !important;
    margin: 0 auto !important;
    box-sizing: border-box !important;
    padding: 0 !important;
  }

  /* Main Profile Block Header Content Box */
  .header-block { 
    background-color: #23272A !important; 
    color: #FFFFFF !important; 
    padding: 20px 40px 10px 40px !important; 
    border-radius: 8px 8px 0 0;
    margin: 0 !important; 
    border-left: 8px solid #FFD200;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    width: 100% !important;
    box-sizing: border-box !important;
  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 28px; font-weight: 900; display: block !important; width: 100%; text-align: left; } 

  /* Navigation Ribbon Strip: ALIGNED TO THE FAR LEFT */
  .navbar { 
    background-color: #23272A !important; 
    padding: 12px 40px !important; 
    margin: 0 !important;
    text-align: left !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44; 
  }
  .navbar a { 
    color: #FFFFFF !important; 
    margin-right: 45px; 
    margin-left: 0 !important;
    text-decoration: none !important; 
    font-weight: 800; 
    font-size: 15px; 
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  .navbar a:hover { color: #FFD200 !important; }

  /* Contact Information Bar: ALIGNED TO THE FAR RIGHT */
  .contact-bar {
    background-color: #23272A !important;
    padding: 12px 40px !important;
    border-radius: 0 0 8px 8px;
    margin-bottom: 10px;
    text-align: right !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44;
  }
  .contact-bar p { color: #E5E7EB !important; margin: 0 !important; font-size: 15px; font-weight: bold; }
  .contact-bar a { color: #FFFFFF !important; text-decoration: none !important; }
  .contact-bar a:hover { color: #FFD200 !important; text-decoration: underline !important; }

  /* Fluid Scrolling Content Layer Layout */
  .scroll-content {
    margin-top: 240px !important; 
    padding: 0 4% 40px 4% !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
  }

  /* Section Content Cards */
  .content-card {
    background-color: #97B2DE !important; 
    padding: 30px 40px !important; 
    border-radius: 8px;
    margin-bottom: 35px !important; 
    box-shadow: 0 6px 18px rgba(0,0,0,0.25);
    position: relative;
    overflow: hidden;
    scroll-margin-top: 250px !important; 
    width: 100% !important;
    max-width: 100% !important;
    box-sizing: border-box !important;
    display: block !important;
  }

  /* Background Grid Elements */
  .skills-bg-card {
    background: linear-gradient(rgba(151, 178, 222, 0.94), rgba(151, 178, 222, 0.94)), 
                url('https://dreamstime.com') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  .education-bg-card {
    background: linear-gradient(rgba(151, 178, 222, 0.94), rgba(151, 178, 222, 0.94)), 
                url('https://pinimg.com') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* Typographic controls with flush top alignment overrides */
  .content-card > h2:first-child, .content-card > div:first-child { margin-top: 0 !important; padding-top: 0 !important; }
  
  h2 { 
    color: #23272A !important; 
    font-size: 26px; 
    font-weight: 900; 
    margin: 0 0 20px 0 !important; 
    padding-top: 0 !important; 
    padding-bottom: 10px; 
    border-bottom: 4px solid #23272A; 
    text-transform: uppercase; 
    letter-spacing: 1px; 
    display: block !important; 
  }

  h3 { 
    color: #111314 !important; 
    font-size: 21px; 
    font-weight: 900; 
    margin-top: 22px !important; 
    margin-bottom: 6px !important; 
    padding-top: 0 !important; 
    display: block !important; 
  }

  h2 + h3, .content-card > h3:first-of-type { margin-top: 5px !important; }
  
  .job-meta { 
    color: #23272A !important; 
    font-style: normal; 
    font-size: 15px; 
    margin-top: 0 !important; 
    margin-bottom: 14px !important; 
    display: block; 
    font-weight: 800; 
    text-transform: uppercase; 
    letter-spacing: 0.5px; 
  }

  /* COMPRESSED SENTENCE & PARAGRAPH SPACING OVERRIDES */
  ul { 
    padding-left: 25px !important; 
    margin-top: 2px !important; 
    margin-bottom: 2px !important; 
  }
  li { 
    margin-top: 0 !important;
    margin-bottom: 4px !important; 
    line-height: 1.35 !important;  
    color: #1A1D20 !important; 
    font-size: 16px; 
    font-weight: 500; 
  } 
  p {
    margin-top: 0 !important;
    margin-bottom: 8px !important; 
    line-height: 1.35 !important;
  }
  .skill-title { font-weight: 700; color: #1A488E; font-size: 16.5px; }
  
  /* Business Matrix Style Pill Labels */
  .badge-pill {
    background-color: #23272A;
    color: #FFD200;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 13px;
    font-weight: bold;
    display: inline-block;
    margin-right: 5px;
  }
</style>

<div class="portfolio-container">

<!-- FIXED NAVIGATION HEADER BLOCK -->
<div class="master-sticky-header">
  <div class="header-block">
    <h1>Edna Ogutu | Enterprise Solutions Consultant</h1>
  </div>

  <div class="navbar">
    <a href="#summary">🏠 SOLUTIONS</a>
    <a href="#capabilities">🛠️ CAPABILITIES</a>
    <a href="#experience">💼 CONSULTING HISTORY</a>
    <a href="#education">🎓 CREDENTIALS</a>
  </div>

  <div class="contact-bar">
    <p>
      📍 Nairobi, Kenya | 
      💬 <a href="https://whatsapp.com" target="_blank" style="color: #FFFFFF !important; font-weight: bold;">Instant Chat</a> | 
      📧 <a href="mailto:hednaogutuh@gmail.com" style="color: #FFFFFF !important; font-weight: bold;">Book Consulting Call</a> | 
      💼 <a href="https://linkedin.com" target="_blank" style="color: #FFD200 !important; text-decoration: underline; font-weight: bold;">LinkedIn Profile</a>
    </p>
  </div>
</div>

<!-- SCROLLING CONTENT LAYER -->
<div class="scroll-content">

<div id="summary" class="content-card">
  <h2>🚀 Core Solutions Portfolio</h2>
  <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Stop guessing. Start growing. I turn your raw enterprise data into clear dashboards and smart analytics that turn complex numbers into simple next steps.</p>
  
  <p style="font-size: 18px; color: #23272A; font-weight: 700; margin: 15px 0 20px 0; line-height: 1.4; font-style: italic;">"You collect the data. I find the money and operational efficiencies hidden inside it."</p>
  
  <hr style="border: 0; height: 1px; background: #23272A; margin-bottom: 25px; opacity: 0.3;">
  
  <h3 style="margin-top: 0 !important;">💡 Consulting Engagement Matrix</h3>
  <p style="line-height: 1.45; font-size: 17px; color: #1A1D20; margin-bottom: 15px;">I partner with organizations across two distinct target operational tracks to solve specific analytics problems without corporate overhead:</p>
  
  <ul>
    <li><span class="badge-pill">Freelance & Consultancy Contracts</span> <b>Immediate ROI & Project Scope:</b> I optimize your business conversion rates, engineer automated customer sales pipelines, and clean up messy, disconnected program databases on a project-by-project basis.</li>
    <li><span class="badge-pill">Full-Time Institutional Growth</span> <b>Scalability & Culture Alignment:</b> I build long-term scalable data pipelines, design centralized business intelligence frameworks, and drive cross-department operations.</li>
  </ul>
</div>

<div id="capabilities" class="content-card skills-bg-card">
  <h2>📊 Strategic Analytics & Field Systems</h2>
  <h3 style="margin-top: 0 !important;">Operational Consulting Specializations</h3>
  <ul>
    <li><span class="skill-title">Business Intelligence & Sales Analysis:</span> Building automated Power BI and Excel dashboards to track real-time revenue targets, shift performance, and performance patterns.</li>
    <li><span class="skill-title">MEL Systems & Data Architecture:</span> Designing indicator tracking logs, managing quality assurance layers, and translating field research targets into insights.</li>
    <li><span class="skill-title">Data Validation & Reconciliation:</span> Identifying structural entry gaps, inconsistencies, and discrepancies across complex biometric, CRM, and financial databases.</li>
    <li><span class="skill-title">Field Operations Coordination:</span> Scripting digital forms (KoboCollect/SurveyCTO), supervising large enumerator operations, and documenting qualitative thematic insights.</li>
    <li><span class="skill-title">Documentation & Learning:</span> Synthesizing research evidence, documenting lessons learned, managing knowledge networks, and implementing strict data protection workflows.</li>
  </ul>
</div>

<div id="tools-proficiency" class="content-card">
  <h2>🛠️ Specialized Solutions & Tools Matrix</h2>
  
  <h3 style="margin-top: 0 !important;">Business Intelligence & Advanced Analytics</h3>
  <ul>
    <li><span class="skill-title">Power BI Architecture:</span> Building automated corporate dashboards, real-time KPI tracking models, volume forecasting engines, and call-centre shift optimizations.</li>
    <li><span class="skill-title">Stata Scripting & Biostatistics:</span> Advanced quantitative research scripting, regression modeling, biostatistical evidence synthesis, and large-scale survey data cleansing.</li>
    <li><span class="skill-title">Advanced Microsoft Excel:</span> Designing complex algorithmic payroll engines for 350+ FTE, biometric check sheet validations, automated lookup scripts, and database reconciliations.</li>
    <li><span class="skill-title">R Programming & SPSS:</span> Implementing descriptive dataset workflows, healthcare program summaries, qualitative data metrics, and graphic data visualizations.</li>
    <li><span class="skill-title">SQL & Python Data Science:</span> Formulating back-end relational database management routines, data cleaning pipelines, and structured problem-solving models.</li>
  </ul>

  <h3>Mobile Data Collection & Operational Operations</h3>
  <ul>
    <li><span class="skill-title">KoboCollect & SurveyCTO:</span> Building field questionnaires with complex digital validation logic, automated conditions, and structured mobile data capture modules.</li>
    <li><span class="skill-title">Enterprise Ecosystems:</span> Integrating analytics workflows across CRM platforms, telephony metrics logs, Microsoft Teams, PowerPoint, and Excel.</li>
  </ul>
</div>

<div id="experience" class="content-card">
  <h2>💼 Consulting & Analytics Engagement History</h2>

  <h3 style="margin-top: 5px !important;">📍 PASGR - African Youth Pathways to Systems Change (AYPS)</h3>
  <span class="job-meta">Field Coordinator | Research, Data Quality & Monitoring Track — (Jun 2026 - Aug 2026)</span>
  <ul>
    <li>Coordinated large-scale data operations, supervising enumerator deployment, field research communication, and strict protocol tracking.</li>
    <li>Designed and delivered field briefings on digital survey methodology, research ethics validation, and quantitative/qualitative data capture tools.</li>
    <li>Managed live database auditing, monitoring real-time digital entries for completeness, logic consistency, and entry gaps.</li>
    <li>Engineered post-field documentation workflows, data validation, qualitative coding metrics, and thematic research synthesis.</li>
  </ul>

  <h3>📍 Hamasisha Africa</h3>
  <span class="job-meta">Research & Data Operations Consultant (Remote - Project Contract) — (Mar 2022 - Apr 2026)</span>
  <ul>
    <li>Architected monitoring, evaluation, and research layers for community development frameworks, delivering baseline metrics and evidence synthesis.</li>
    <li>Managed cross-functional field operations, training and directing field squads on digital questionnaires and rigorous quality control checks.</li>
    <li>Scripted structured mobile survey tools, qualitative research modules, and Key Informant Interview (KII) tracking logs.</li>
    <li>Delivered end-to-end data processing, handling data cleaning pipelines, validation criteria, and qualitative analysis reports for stakeholders.</li>
  </ul>

  <h3>📍 Calltronix Kenya Limited</h3>
  <span class="job-meta">Workforce Data Analyst (Corporate Contract) — (Jan 2025 - Feb 2026)</span>
  <ul>
    <li>Provided enterprise intelligence across 37+ customer programs, translating biometric, CRM, and telephony logs into actionable decisions.</li>
    <li>Designed and automated scalable Power BI and Advanced Excel dashboards, cutting routine operations reporting turnaround times by 80%.</li>
    <li>Managed complex database reconciliations, auditing attendance grids, shift adherence, and incentives to process payroll configurations for 350+ FTE.</li>
    <li>Executed volume capacity forecasting and schedule optimization metrics to maximize workforce resource allocations.</li>
  </ul>

  <h3>📍 SGS Kenya</h3>
  <span class="job-meta">Data Systems Specialist (Internship Contract) — (Nov 2023 - Jan 2024)</span>
  <ul>
    <li>Supported institutional databases by structuring routine data collections, compilation pipelines, and database management engines.</li>
    <li>Executed rigorous descriptive statistical sweeps and designed Excel-based reporting toolsets to eliminate data gaps.</li>
  </ul>

  <h3>📍 GAIN-AGRA Project</h3>
  <span class="job-meta">Research Analytics Assistant (Project Contract) — (Apr 2023 - May 2023)</span>
  <ul>
    <li>Deployed digital survey frameworks for household research metrics, validating entry completeness directly on the field.</li>
  </ul>

  <h3>📍 Adaptive Model for Research and Empowerment in Communities (AMREC)</h3>
  <span class="job-meta">Research Systems Analyst (Internship Contract) — (Jan 2023 - Mar 2023)</span>
  <ul>
    <li>Analyzed health research datasets inside Stata and SPSS to produce validated data summaries and statistical reports.</li>
  </ul>

  <h3>📍 JKUAT - School of Computing and Information Technology (SCIT)</h3>
  <span class="job-meta">IBM Data Science Specialist (Applied Training) — (Aug 2021 - Dec 2021)</span>
  <ul>
    <li>Engineered foundational data routines, building exploration models and analytical dashboards during an intensive SCIT industry partnership track.</li>
  </ul>
</div>

<div id="education" class="content-card education-bg-card">
  <h2>🎓 Academic Credentials & Strategic Accreditations</h2>
  <h3 style="margin-top: 5px !important;">Academic Background</h3>
  <ul>
    <li><span class="skill-title">Master of Science in Data Science</span> | Open University of Kenya <i>(In Progress | Expected 2028)</i></li>
    <li><span class="skill-title">Bachelor Of Science in Biostatistics</span> | Jomo Kenyatta University of Agriculture and Technology (JKUAT)</li>
  </ul>

  <h3>Strategic Accreditations</h3>
  <ul>
    <li><b>MEAL Essentials Professional Certificate</b> – DisasterReady / Humanitarian Leadership Academy</li>
    <li><b>Project Management Essentials</b> – DisasterReady</li>
    <li><b>IBM Data Science, Artificial Intelligence & Machine Learning Certificate</b></li>
  </ul>
</div>

</div> <!-- Closes scroll-content layout engine -->
</div> <!-- Closes portfolio-container outer window -->
