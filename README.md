<style>
  /* Force hide default GitHub template elements */
  header, #header, .title, h1:first-of-type:not(.header-block h1) {
    display: none !important;
  }
  
  /* Overrides GitHub's secret default wrapper settings to allow full width stretch */
  .wrapper, #main_content, .main-content, #content, .container-lg, .markdown-body {
    max-width: 100% !important;
    width: 100% !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  body, h1, h2, h3, p, a, li, span, div { 
    font-family: 'Arial', sans-serif !important; 
  }

  body { 
    background-color: #1A488E !important; 
    margin: 0 !important;
    padding: 0 !important;
  }
  
  /* FIXED COMPACT TOP LAYOUT LAYER - FORCED FULL SCREEN WIDTH */
  .fixed-header-container {
    position: fixed !important;
    top: 0 !important;
    left: 0 !important;
    width: 100% !important;
    z-index: 9999 !important;
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
    padding: 15px 40px !important; 
    border-radius: 8px 8px 0 0;
    margin: 0 !important; 
    border-left: 8px solid #FFD200;
    box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    width: 100% !important;
    box-sizing: border-box !important;
    display: flex !important;
    justify-content: space-between !important;
    align-items: center !important;
    flex-wrap: wrap !important;
  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 26px; font-weight: 900; display: inline-block !important; } 
  .header-block p { color: #E5E7EB !important; margin: 0 !important; font-size: 14px; font-weight: bold; display: inline-block !important; }

  /* Navigation Ribbon Strip */
  .navbar { 
    background-color: #23272A !important; 
    padding: 12px 30px !important; 
    border-radius: 0 0 8px 8px;
    margin: 0 !important;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44; 
  }
  .navbar a { 
    color: #FFFFFF !important; 
    margin: 0 35px; 
    text-decoration: none !important; 
    font-weight: 800; 
    font-size: 15px; 
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  .navbar a:hover { color: #FFD200 !important; }

  /* Fluid Scrolling Content Layer Layout - SHIFTED DOWN SO IT NEVER HIDES */
  .scroll-content {
    margin-top: 200px !important; /* Fixed padding buffer so cards load below the header */
    padding: 0 4% 40px 4% !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
  }

  /* Section Content Cards: FULL SCREEN WIDE MODE ONLY */
  .content-card {
    background-color: #97B2DE !important; 
    padding: 30px 40px !important; 
    border-radius: 8px;
    margin-bottom: 35px !important; /* Clean structural blue separation gaps */
    box-shadow: 0 6px 18px rgba(0,0,0,0.25);
    position: relative;
    overflow: hidden;
    scroll-margin-top: 220px !important; /* Prevents overlap when clicking links */
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

  /* Typographic text layout controls with flush top alignment overrides */
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
</style>

<div class="portfolio-container">

<!-- FIXED CONTAINER BLOCK -->
<div class="fixed-header-container">
  <div class="header-block">







    
    <h1>Edna Ogutu</h1>
    <p>📍 Nairobi, Kenya | 📧 hednaogutuh@gmail.com | 💼 <a href="Your-LinkedIn-URL-Here" style="color: #FFD200 !important; text-decoration: underline; font-weight: bold;">Connect on LinkedIn</a></p>
  </div>

  <div class="navbar">
    <a href="#summary">🏠 Home</a>
    <a href="#skills">🛠️ Skills</a>
    <a href="#experience">💼 Experience</a>
    <a href="#education">🎓 Education</a>
  </div>
</div>

<!-- SCROLLING CONTENT LAYER -->
<div class="scroll-content">

<div id="summary" class="content-card">
  <h2>📋 Professional Summary & Strategy</h2>
  <p style="font-size: 19px; color: #111314; font-weight: 800; margin: 0 0 15px 0; line-height: 1.4;">Data Analyst & Statistician | Data Management, Reconciliation & BI | Excel, Power BI, SQL, Python, R & Stata | Turning complex data into reliable insights and practical decisions</p>
  <hr style="border: 0; height: 1px; background: #23272A; margin-bottom: 20px; opacity: 0.3;">
  <p style="line-height: 1.7; font-size: 17px; color: #1A1D20; font-weight: 500;">Statistician and Data Analyst with experience supporting Monitoring, Evaluation, Accountability and Learning, research and development programs through data collection, data quality assurance, data management, statistical analysis, reporting, and field coordination.</p>
  <p style="line-height: 1.7; font-size: 17px; color: #1A1D20; font-weight: 500;">Trained in Biostatistics with hands-on experience across the research and program cycle, including digital data collection, field-team coordination, data validation, monitoring progress against targets, evidence generation, and reporting. Experienced in analyzing quantitative and qualitative data, identifying data gaps and inconsistencies, and translating program and research data into accurate reports, summaries, and visualizations. Combines strong statistical and analytical capability with practical development-sector and field research experience.</p>
</div>

<div id="skills" class="content-card skills-bg-card">
  <h2>🛠️ Core Expertise & Technical Skills</h2>
  
  <h3 style="margin-top: 0 !important;">Core Areas of Expertise</h3>
  <ul>
    <li><span class="skill-title">MEL & Program Monitoring:</span> Program monitoring | Indicator & target tracking | Monitoring data collection | Field monitoring | Progress tracking | Evidence generation</li>
    <li><span class="skill-title">Data Collection & Quality Assurance:</span> Digital data collection | Data capture | Data validation | Data cleaning | Data reconciliation | Completeness & consistency checks | Discrepancy resolution</li>
    <li><span class="skill-title">Research & Field Operations:</span> Research implementation | Field coordination | Enumerator supervision | Surveys | KIIs | FGDs | Field documentation</li>
    <li><span class="skill-title">Data Analysis & Reporting:</span> Statistical analysis | Quantitative & qualitative analysis | Data summaries | Tables | Visualisations | Dashboards | Report preparation</li>
    <li><span class="skill-title">Documentation & Learning:</span> Research documentation | Evidence synthesis | Lessons learned | Knowledge management | Stakeholder coordination | Data protection</li>
  </ul>

  <h3>Technical Tools</h3>
  <ul>
    <li><span class="skill-title">Data & Analytics:</span> Excel (Advanced) | Power BI | Stata | R | SPSS | SQL | Python</li>
    <li><span class="skill-title">Data Collection & Reporting:</span> KoboCollect | SurveyCTO | Digital survey platforms | Microsoft Word | PowerPoint | Teams | Outlook</li>
  </ul>
</div>

<div id="experience" class="content-card">
   <h2>💼 Professional Experience</h2>

  <h3 style="margin-top: 5px !important;">📍 PASGR - African Youth Pathways to Systems Change (AYPS)</h3>
  <span class="job-meta">Field Coordinator | Research, Data Quality & Monitoring Support (Jun 2026 - Aug 2026)</span>
  <ul>
    <li>Coordinated field implementation, including enumerator deployment, field communication, progress monitoring, and adherence to approved study procedures.</li>
    <li>Facilitated enumerator training and field briefings on quantitative and qualitative methodologies, digital data collection, research ethics, and field protocols.</li>
    <li>Supported household surveys, Key Informant Interviews (KIIs), and Focus Group Discussions (FGDs) in accordance with approved research protocols.</li>
    <li>Monitored live digital data submissions, identifying completeness, consistency, and submission issues requiring follow-up.</li>
    <li>Reported field progress, emerging challenges, data-quality issues, and implementation gaps to the Principal Investigator and research team.</li>
    <li>Supported field documentation, transcription, data cleaning, qualitative coding, thematic analysis, and preliminary quantitative analysis.</li>
    <li>Coordinated enumerator attendance and daily payment administration, maintaining accurate participation records and supporting timely disbursement.</li>
  </ul>

  <h3>📍 Hamasisha Africa</h3>
  <span class="job-meta">Research & Data Operations Analyst (Remote - Project-Based Consultancy) | (Mar 2022 - Apr 2026)</span>
  <ul>
    <li>Supported monitoring, evaluation and research activities across youth empowerment and community development programs, including baseline and monitoring studies.</li>
    <li>Coordinated and supervised field teams, providing guidance on questionnaires, field procedures, research ethics and data-quality requirements.</li>
    <li>Supported recruitment, orientation, deployment and day-to-day coordination of field teams while monitoring progress against agreed schedules and targets.</li>
    <li>Supported the design and refinement of structured questionnaires, digital data-collection tools and qualitative interview guides.</li>
    <li>Conducted and supported KIIs and FGDs, including participant engagement, field coordination, documentation and qualitative data organization.</li>
    <li>Performed data cleaning, validation, coding and quantitative and qualitative analysis, contributing to interpretation of findings.</li>
    <li>Prepared research reports, monitoring summaries, presentations and evidence briefs for program and research teams.</li>
    <li>Maintained research documentation and supported ethical research, confidentiality, data protection and accurate field-team records.</li>
  </ul>

  <h3>📍 Calltronix Kenya Limited</h3>
  <span class="job-meta">Data Analyst (Contract) | (Jan 2025 - Feb 2026)</span>
  <ul>
    <li>Provided analytical and operational support across 37+ customer and workforce programs, using data to monitor performance and support operational decision-making.</li>
    <li>Conducted data cleaning, validation, reconciliation, and quality assurance across biometric, CRM, telephony, and workforce data sources.</li>
    <li>Managed payroll processes for 350+ FTE across multiple projects, incorporating attendance, overtime, incentives, and benefits.</li>
    <li>Reconciled workforce and attendance records across multiple systems, identifying discrepancies and validating payroll inputs.</li>
    <li>Developed and automated Power BI and Excel dashboards for attendance, shift adherence, and KPI monitoring, reducing reporting time by 80%.</li>
    <li>Conducted volume forecasting, capacity planning, and schedule optimization to support workforce allocation.</li>
    <li>Partnered with HR and Finance to validate timesheets, reconcile payroll information, and prepare operational and compliance reports.</li>
  </ul>

  <h3>📍 SGS Kenya</h3>
  <span class="job-meta">Data Officer Intern | (Nov 2023 - Jan 2024)</span>
  <ul>
    <li>Supported data collection, compilation, cleaning, validation, and database management for operational and research data.</li>
    <li>Conducted data-quality checks and reconciled discrepancies across multiple data sources.</li>
    <li>Prepared routine and ad-hoc reports, data tables, summaries, and Excel-based reporting tools.</li>
    <li>Performed descriptive analysis and supported data visualization for internal reporting and decision-making.</li>
  </ul>

  <h3>📍 GAIN-AGRA Project</h3>
  <span class="job-meta">Research Assistant - Nutrition Survey Project (Project-Based) | (Apr 2023 - May 2023)</span>
  <ul>
    <li>Implemented household surveys using structured digital data-collection tools and approved field procedures.</li>
    <li>Administered questionnaires while maintaining informed consent, confidentiality, and participant-protection requirements.</li>
    <li>Conducted field-level data validation and quality checks to identify incomplete or inconsistent submissions.</li>
    <li>Supported field reporting, data cleaning, and preparation of collected data for analysis.</li>
  </ul>

  <h3>📍 Adaptive Model for Research and Empowerment in Communities (AMREC)</h3>
  <span class="job-meta">Research Analyst – Intern | (Jan 2023 - Mar 2023)</span>
  <ul>
    <li>Analyzed health research and program datasets using Stata and SPSS to generate statistical summaries and research outputs.</li>
    <li>Cleaned, coded, and validated datasets to produce analysis-ready research data.</li>
    <li>Conducted data-quality checks and supported preparation of statistical reports and research summaries.</li>
    <li>Assisted research and program teams with interpretation and synthesis of quantitative findings.</li>
  </ul>

  <h3>📍 JKUAT - School of Computing and Information Technology (SCIT)</h3>
  <span class="job-meta">IBM Data Science - Attachment Program | (Aug 2021 - Dec 2021)</span>
  <ul>
    <li>Completed a structured four-month IBM Data Science learning program delivered in partnership with JKUAT's School of Computing and Information Technology.</li>
    <li>Applied data science concepts through practical exercises involving data preparation, exploration, analysis, and visualization.</li>
    <li>Developed foundational skills in data-driven problem solving and communicating analytical findings through reports and visualizations.</li>
  </ul>
</div>

<div id="education" class="content-card education-bg-card">
  <h2>🎓 Education & Certifications</h2>

  <h3 style="margin-top: 5px !important;">Education</h3>
  <ul>
    <li><span class="skill-title">Master of Science in Data Science</span> | Open University of Kenya <i>(In Progress | Expected 2028)</i></li>
    <li><span class="skill-title">Bachelor Of Science in Biostatistics</span> | Jomo Kenyatta University of Agriculture and Technology (JKUAT)</li>
  </ul>

  <h3>Professional Certifications</h3>
  <ul>
    <li><b>MEAL Essentials Professional Certificate</b> – DisasterReady / Humanitarian Leadership Academy</li>
    <li><b>Project Management Essentials</b> – DisasterReady</li>
    <li><b>IBM Data Science, Artificial Intelligence & Machine Learning Certificate</b></li>
  </ul>
</div>

</div> <!-- Closes scroll-content -->
</div> <!-- Closes portfolio-container -->
