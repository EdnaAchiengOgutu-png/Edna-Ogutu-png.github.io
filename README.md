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
    background-color: #D2F7FF !important; 
    margin: 0 !important;
    padding: 0 !important;
  }

  /* HIDES THE RADIO MECHANISM BUTTONS OUT OF SIGHT */
  input[type="radio"].tab-toggle {
    display: none !important;
  }
  
  /* MASTER FIXED TOP HEADER WRAPPER */
  .master-sticky-header {
    position: fixed !important;
    top: 0 !important;
    left: 0 !important;
    width: 100% !important;
    z-index: 999999 !important; 
    background-color: #D2F7FF !important; 
    padding: 15px 4% 0 4% !important; 
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
    padding: 12px 40px !important; 
    border-radius: 8px 8px 0 0;
    margin: 0 !important; 
    border-left: 8px solid #FFD200;
    box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    width: 100% !important;
    box-sizing: border-box !important;
  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 24px; font-weight: 900; display: block !important; width: 100%; text-align: left; } 

  /* Navigation Ribbon Strip */
  .navbar { 
    background-color: #23272A !important; 
    padding: 10px 40px !important; 
    margin: 0 !important;
    text-align: left !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44; 
    border-radius: 0 0 8px 8px; 
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  }
  
  .navbar label { 
    color: #FFFFFF !important; 
    margin-right: 22px; 
    font-weight: 800; 
    font-size: 12px; 
    text-transform: uppercase;
    letter-spacing: 0.5px;
    cursor: pointer !important;
    display: inline-block !important;
  }
  .navbar label:hover { color: #FFD200 !important; }

  /* FIXED BOTTOM FROZEN BAR */
  .fixed-footer-container {
    position: fixed !important;
    bottom: 0 !important;
    left: 0 !important;
    width: 100% !important;
    z-index: 999999 !important;
    background-color: #D2F7FF !important; 
    padding: 0 4% 10px 4% !important; 
    box-sizing: border-box !important;
  }

  .footer-bar {
    background-color: #23272A !important;
    padding: 8px 30px !important; 
    border-radius: 8px;
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 3px solid #FFD200; 
    display: flex !important;
    justify-content: space-between !important;
    align-items: center !important;
    box-shadow: 0 -4px 15px rgba(0,0,0,0.15);
  }
  .footer-bar p { color: #E5E7EB !important; margin: 0 !important; font-size: 14px; font-weight: bold; }
  .footer-bar a { color: #FFD200 !important; text-decoration: underline !important; font-weight: bold; }
  .footer-bar a:hover { color: #FFFFFF !important; }

  /* Fluid Scrolling Content Layer Layout - OPTIMIZED WITH EXTRA BOTTOM CUSHION FOR RESPONSIVENESS */
  .scroll-content {
    margin-top: 115px !important; /* Pulls cards tighter right up to top header */
    padding: 0 4% 75px 4% !important; /* Fixed bottom padding buffer room for frozen footer */
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
  }

  /* Section Content Cards: INTEGRATED WITH INTUITIVE INNER HEIGHT AUTO-SCROLL CONTROLS */
  .content-card {
    background-color: #97B2DE !important; 
    padding: 25px 35px !important; 
    border-radius: 8px;
    margin-bottom: 10px !important; 
    box-shadow: 0 4px 14px rgba(0,0,0,0.12);
    position: relative;
    width: 100% !important;
    max-width: 100% !important;
    box-sizing: border-box !important;
    display: none !important; 
    
    /* THE SMART CUSHION FIX: Automatically adds a scrollbar inside the card if text or forms are too tall */
    max-height: calc(100vh - 195px) !important; 
    overflow-y: auto !important; 
  }

  /* THE ENGINE LINK: Show only the checked tab card */
  #tab-about:checked ~ .scroll-content #about,
  #tab-services:checked ~ .scroll-content #services,
  #tab-projects:checked ~ .scroll-content #projects,
  #tab-experience:checked ~ .scroll-content #experience,
  #tab-education:checked ~ .scroll-content #education,
  #tab-certifications:checked ~ .scroll-content #certifications,
  #tab-get-in-touch:checked ~ .scroll-content #get-in-touch {
    display: block !important; 
  }

  /* Highlight Active Menu Label Item */
  #tab-about:checked ~ .master-sticky-header .navbar label[for="tab-about"],
  #tab-services:checked ~ .master-sticky-header .navbar label[for="tab-services"],
  #tab-projects:checked ~ .master-sticky-header .navbar label[for="tab-projects"],
  #tab-experience:checked ~ .master-sticky-header .navbar label[for="tab-experience"],
  #tab-education:checked ~ .master-sticky-header .navbar label[for="tab-education"],
  #tab-certifications:checked ~ .master-sticky-header .navbar label[for="tab-certifications"],
  #tab-get-in-touch:checked ~ .master-sticky-header .navbar label[for="tab-get-in-touch"] {
    color: #FFD200 !important;
    border-bottom: 2px solid #FFD200;
  }

  /* Background Grid Elements */
  .skills-bg-card {
    background: linear-gradient(rgba(151, 178, 222, 0.94), rgba(151, 178, 222, 0.94)), 
                url('https://dreamstime.com') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* Typographic controls with flush top alignment overrides */
  .content-card > h2:first-child, .content-card > div:first-child { margin-top: 0 !important; padding-top: 0 !important; }
  h2 { color: #23272A !important; font-size: 24px; font-weight: 900; margin: 0 0 15px 0 !important; padding-bottom: 8px; border-bottom: 4px solid #23272A; text-transform: uppercase; letter-spacing: 1px; display: block !important; }
  h3 { color: #111314 !important; font-size: 20px; font-weight: 900; margin-top: 18px !important; margin-bottom: 5px !important; padding-top: 0 !important; display: block !important; }
  h2 + h3, .content-card > h3:first-of-type { margin-top: 5px !important; }
  .job-meta { color: #23272A !important; font-style: normal; font-size: 14px; margin-top: 0 !important; margin-bottom: 12px !important; display: block; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px; }

  /* COMPRESSED READABILITY TEXT METRICS */
  ul { padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 2px !important; }
  li { margin-top: 0 !important; margin-bottom: 4px !important; line-height: 1.35 !important; color: #1A1D20 !important; font-size: 15.5px; font-weight: 500; } 
  p { margin-top: 0 !important; margin-bottom: 6px !important; line-height: 1.35 !important; }
  .skill-title { font-weight: 700; color: #1A488E; font-size: 16px; }
  .badge-pill { background-color: #23272A; color: #FFD200; padding: 3px 10px; border-radius: 20px; font-size: 12px; font-weight: bold; display: inline-block; margin-right: 5px; }
</style>

<div class="portfolio-container">

<!-- MASTER CSS REGISTER RADIO BUTTONS -->
<input type="radio" name="page-tabs" id="tab-about" class="tab-toggle" checked />
<input type="radio" name="page-tabs" id="tab-services" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-projects" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-experience" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-education" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-certifications" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-get-in-touch" class="tab-toggle" />

<!-- FIXED TOP HEADER STRIP PANEL -->
<div class="master-sticky-header">
  <div class="header-block">
    <h1>Edna Ogutu | Enterprise Solutions Consultant</h1>
  </div>

  <div class="navbar">
    <label for="tab-about">🏠 ABOUT</label>
    <label for="tab-services">💼 SERVICES</label>
    <label for="tab-projects">📊 PROJECTS</label>
    <label for="tab-experience">📈 EXPERIENCE</label>
    <label for="tab-education">🎓 EDUCATION</label>
    <label for="tab-certifications">🏆 CERTIFICATIONS</label>
    <label for="tab-get-in-touch">📞 GET IN TOUCH</label>
  </div>
</div>

<!-- FIXED BOTTOM FROZEN FOOTER BAR -->
<div class="fixed-footer-container">
  <div class="footer-bar">
    <p>📍 Nairobi, Kenya</p>
    <p>💼 <a href="https://linkedin.com" target="_blank">Connect on LinkedIn</a></p>
  </div>
</div>

<!-- SCROLLING CONTENT LAYER VIEWPORT -->
<div class="scroll-content">


<!-- 1. ABOUT CARD -->
<div id="about" class="content-card">
  <h2>👤 About & Value Proposition</h2>
  <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Stop guessing. Start growing. I turn your raw enterprise data into clear dashboards and smart analytics that turn complex numbers into simple next steps.</p>
  <p style="font-size: 18px; color: #23272A; font-weight: 700; margin: 15px 0 20px 0; line-height: 1.4; font-style: italic;">"You collect the data. I find the money and operational efficiencies hidden inside it."</p>
  <hr style="border: 0; height: 1px; background: #23272A; margin-bottom: 20px; opacity: 0.3;">
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500;">Statistician and Data Analyst with extensive experience supporting Monitoring, Evaluation, Accountability and Learning (MEL), research, and development programs. Specialized in quantitative and qualitative analysis, database validation, and building centralized business intelligence frameworks that translate messy field research targets into clear institutional insights.</p>
</div>

<!-- 2. SERVICES CARD -->
<div id="services" class="content-card skills-bg-card">
  <h2>💼 Operational Consulting Services</h2>
  <h3 style="margin-top: 0 !important;">Data Packages I Offer:</h3>
  <ul>
    <li><span class="skill-title">Business Intelligence & Sales Analysis:</span> Engineering interactive Power BI and Advanced Excel dashboard suites to audit real-time revenue targets, monitor project status, and optimize shift parameters.</li>
    <li><span class="skill-title">MEL Systems & Data Architecture:</span> Constructing indicator logs, target tracking registers, and quality assurance checkpoints for program verification.</li>
    <li><span class="skill-title">Database Reconciliation & Auditing:</span> Running strict diagnostic sweeps to isolate structural entry gaps and inconsistencies across complex biometric, CRM, and payroll databases.</li>
    <li><span class="skill-title">Field Operations & Digital Scripting:</span> Scripting logical digital surveys (KoboCollect/SurveyCTO), coordinating remote enumerator actions, and synthesizing qualitative thematic reports.</li>
    <li><span class="skill-title">Documentation & Learning:</span> Synthesizing research evidence, documenting lessons learned, managing knowledge networks, and implementing strict data protection workflows.</li>
  </ul>
</div>

<!-- 3. PROJECTS SHOWCASE CARD -->
<div id="projects" class="content-card">
  <h2>📊 Strategic Projects Portfolio</h2>
  <h3 style="margin-top: 0 !important;">Production-Ready Analytics & Dashboards</h3>
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; margin-bottom: 15px;">A selection of data systems designed to optimize business operations, increase sales visibility, and automate reporting metrics:</p>
  
  <ul>
    <li><span class="skill-title">Enterprise Sales & Attendance Dashboard (Power BI):</span> Fully automated reporting suite built to monitor cross-project capacity planning and performance forecasting. <i>[Project Assets Coming Soon]</i></li>
    <li><span class="skill-title">Biostatistical Health Survey Pipeline (Stata):</span> Custom advanced regression scripts engineered for massive data cleaning, outlier isolation, and quantitative evidence synthesis. <i>[Project Assets Coming Soon]</i></li>
    <li><span class="skill-title">Algorithmic Payroll & Database Reconciliation Engine (Excel):</span> Advanced data macro matrix optimized for multi-project validation and compliance checks for 350+ FTE. <i>[Project Assets Coming Soon]</i></li>
  </ul>
</div>

<!-- 4. TOOLS SHOWCASE MATRIX -->
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

  <h3>Mobile Data Collection & Field Systems</h3>
  <ul>
    <li><span class="skill-title">KoboCollect & SurveyCTO:</span> Building field questionnaires with complex digital validation logic, automated conditions, and structured mobile data capture modules.</li>
    <li><span class="skill-title">Enterprise Ecosystems:</span> Integrating analytics workflows across CRM platforms, telephony metrics logs, Microsoft Teams, PowerPoint, and Excel.</li>
  </ul>
</div>

<!-- 5. EXPERIENCE CARD -->
<div id="experience" class="content-card">
  <h2>📈 Consulting & Analytics Engagement History</h2>

  <h3 style="margin-top: 0 !important;">📍 PASGR - African Youth Pathways to Systems Change (AYPS)</h3>
  <span class="job-meta">Field Coordinator | Research, Data Quality & Monitoring Track — (Jun 2026 - Aug 2026)</span>
  <ul>
    <li>Coordinated large-scale data operations, supervising enumerator deployment, field research communication, and strict protocol tracking.</li>
    <li>Designed and delivered field briefings on digital survey methodology, research ethics validation, and quantitative/qualitative data capture tools.</li>
    <li>Managed live database auditing, monitoring real-time digital entries for completeness, logic consistency, and entry gaps.</li>
    <li>Headed post-field documentation workflows, data validation, qualitative coding metrics, and thematic research synthesis.</li>
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
  <span class="job-meta">Data Systems Specialist (Institutional Internship) — (Nov 2023 - Jan 2024)</span>
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
  <span class="job-meta">IBM Data Science Specialist (Applied Attachment Track) — (Aug 2021 - Dec 2021)</span>
  <ul>
    <li>Engineered foundational data routines, building exploration models and analytical dashboards during an intensive SCIT industry partnership track.</li>
  </ul>
</div>

<!-- 6. EDUCATION CARD -->
<div id="education" class="content-card">
  <h2>🎓 Academic Background</h2>
  <h3 style="margin-top: 0 !important;">Degrees</h3>
  <ul>
    <li><span class="skill-title">Master of Science in Data Science</span> | Open University of Kenya <i>(In Progress | Expected 2028)</i></li>
    <li><span class="skill-title">Bachelor Of Science in Biostatistics</span> | Jomo Kenyatta University of Agriculture and Technology (JKUAT)</li>
  </ul>
</div>

<!-- 7. CERTIFICATIONS CARD -->
<div id="certifications" class="content-card">
  <h2>🏆 Professional Accreditations</h2>
  <h3 style="margin-top: 0 !important;">Specialized Certifications</h3>
  <ul>
    <li><b>MEAL Essentials Professional Certificate</b> – DisasterReady / Humanitarian Leadership Academy</li>
    <li><b>Project Management Essentials</b> – DisasterReady</li>
    <li><b>IBM Data Science, Artificial Intelligence & Machine Learning Certificate</b></li>
  </ul>
</div>

<!-- 8. GET IN TOUCH ACTIVE SUBMISSION ENGINE - SYMMETRIC SPLIT ENGINE LAYOUT -->
<div id="get-in-touch" class="content-card" style="background-color: #FFFFFF !important; color: #23272A !important; padding: 40px !important;">
  <form action="https://formspree.io" method="POST" style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; margin: 0;">
    
    <!-- LEFT SIDE DETAILS COLUMN PANEL -->
    <div style="flex: 1; min-width: 320px; box-sizing: border-box; padding: 0 !important; margin: 0 !important;">
      <span style="color: #1A488E; font-weight: bold; text-transform: uppercase; font-size: 13px; letter-spacing: 0.5px; display: block; margin-bottom: 5px; text-align: left !important;">Get in touch</span>
      <h2 style="color: #23272A !important; font-size: 36px !important; font-weight: 900 !important; border: none !important; margin: 0 0 15px 0 !important; padding: 0 !important; text-transform: none !important; display: block !important; text-align: left !important;">Let's talk</h2>
      <p style="line-height: 1.5; font-size: 16px; color: #4A5568 !important; margin-bottom: 30px; text-align: left !important;">Request a data solutions session below. I confirm by email within one business day with a meeting link and any prep notes.</p>
      
      <!-- Box Info Fragment 1 -->
      <div style="background-color: #F8FAFC; padding: 20px; border-radius: 8px; margin-bottom: 20px; border: 1px solid #E2E8F0; width: 100%; box-sizing: border-box;">
        <h4 style="margin: 0 0 8px 0; font-size: 15px; font-weight: bold; color: #23272A; display: block; text-align: left !important;">How booking works</h4>
        <p style="margin: 0; font-size: 14px; line-height: 1.5; color: #4A5568 !important; text-align: left !important;">Suggest your target slots below. When you hit submit, the operational data is packaged and securely sent directly to my workspace email inbox.</p>
      </div>
      
      <!-- Box Info Fragment 2 -->
      <div style="background-color: #F8FAFC; padding: 20px; border-radius: 8px; border: 1px solid #E2E8F0; width: 100%; box-sizing: border-box;">
        <h4 style="margin: 0 0 8px 0; font-size: 15px; font-weight: bold; color: #23272A; display: block; text-align: left !important;">Prefer direct messaging?</h4>
        <p style="margin: 0; font-size: 14px; line-height: 1.5; color: #4A5568 !important; text-align: left !important;">Utilize the floating WhatsApp sync portal button on the right column frame for real-time consultation.</p>
      </div>
    </div>
    
    <!-- RIGHT SIDE ACTIVE TYPEABLE BOOKING FORM CONTAINER -->
    <div style="flex: 1.2; min-width: 360px; background-color: #FFFFFF; border: 1px solid #E2E8F0; padding: 35px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); box-sizing: border-box; margin: 0 !important;">
      
      <!-- Form Input Row 1 -->
      <div style="display: flex; gap: 20px; margin-bottom: 20px; width: 100%; box-sizing: border-box;">
        <div style="flex: 1;">
          <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">Full name</label>
          <input type="text" name="Client Name" placeholder="Enter name" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px;" />
        </div>
        <div style="flex: 1;">
          <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">Email address</label>
          <input type="email" name="Client Email" placeholder="name@company.com" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px;" />
        </div>
      </div>
      
      <!-- Form Input Row 2 -->
      <div style="display: flex; gap: 20px; margin-bottom: 20px; width: 100%; box-sizing: border-box;">
        <div style="flex: 1;">
          <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">Preferred date</label>
          <input type="text" name="Requested Date" placeholder="dd/mm/yyyy" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px;" />
        </div>
        <div style="flex: 1;">
          <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">What is this about?</label>
          <select name="Consultancy Scope" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px; height: 45px;">
            <option value="">Select a consultancy topic</option>
            <option value="Business Intelligence & Power BI Dashboards">Business Intelligence & Power BI Dashboards</option>
            <option value="Advanced Excel Automation & Reconciliation">Advanced Excel Automation & Reconciliation</option>
            <option value="Stata / Biostatistical Survey Scripting">Stata / Biostatistical Survey Scripting</option>
            <option value="MEL Systems Architecture">MEL Systems Architecture</option>
          </select>
        </div>
      </div>
      
      <!-- Form Input Row 3 -->
      <div style="margin-bottom: 20px; width: 50%; box-sizing: border-box;">
        <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">Preferred time</label>
        <input type="text" name="Requested Time" placeholder="e.g., 2:00 PM EAT" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px;" />
      </div>
      
      <!-- Form Input Row 4 -->
      <div style="margin-bottom: 25px; width: 100%; box-sizing: border-box;">
        <label style="display: block; font-size: 13px; font-weight: bold; color: #4A5568; margin-bottom: 6px; text-align: left !important;">Tell me a little more</label>
        <textarea name="Project Context Details" placeholder="Provide a line or two of context: the target data challenge, your timeline, and what a successful outcome looks like..." rows="3" required style="width: 100%; padding: 12px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; background-color: #FFFFFF; color: #23272A; font-size: 14px; resize: none;"></textarea>
      </div>

      <!-- TRANSMISSION SUBMIT BUTTONS -->
      <div style="text-align: center; display: flex; gap: 15px; width: 100%; box-sizing: border-box;">
        <button type="submit" style="flex: 1; background-color: #1A488E !important; color: #FFFFFF !important; padding: 14px 20px !important; border: none !important; border-radius: 6px; font-weight: bold; font-size: 14px; cursor: pointer; box-shadow: 0 4px 10px rgba(0,0,0,0.1); text-transform: uppercase; letter-spacing: 0.5px; text-align: center; height: 45px;">✉️ Submit Booking Request</button>
        <a href="https://whatsapp.com" target="_blank" style="flex: 1; background-color: #23272A !important; color: #FFD200 !important; padding: 14px 20px !important; border-radius: 6px; font-weight: bold; text-decoration: none; font-size: 14px; display: inline-block; box-shadow: 0 4px 10px rgba(0,0,0,0.1); text-transform: uppercase; letter-spacing: 0.5px; text-align: center; line-height: 45px; height: 45px; box-sizing: border-box;">Sync via WhatsApp</a>
      </div>
      
    </div>
  </form>
</div>

</div> <!-- Closes scroll-content layout engine -->
</div> <!-- Closes portfolio-container outer window -->
