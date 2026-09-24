<style>
  /* Force hide default GitHub template elements */
  header, #header, .title, h1:first-of-type:not(.header-block h1) {
    display: none !important;
  }
  
  /* Overrides GitHub's secret default wrapper settings to force absolute edge-to-edge stretch */
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
  
  /* MASTER FIXED TOP HEADER WRAPPER - MAXIMUM LAYER PRIORITY */
  .master-sticky-header {
    position: fixed !important;
    top: 0 !important;
    left: 0 !important;   
    right: 0 !important;  
    width: 100% !important;
    z-index: 999999 !important; 
    background-color: #D2F7FF !important; 
    padding: 0 !important; 
    margin: 0 !important;
    box-sizing: border-box !important;
  }

  .portfolio-container {
    width: 100% !important;
    max-width: 100% !important;
    margin: 0 !important;
    box-sizing: border-box !important;
    padding: 0 !important;
  }

  /* Main Profile Block Header Content Box - Full Width Stretch with Outer Gold Top Border */
  .header-block { 
    background-color: #23272A !important; 
    color: #FFFFFF !important; 
    padding: 15px 40px !important; 
    border-radius: 0 !important; 
    margin: 0 !important; 
    border-left: 8px solid #FFD200;
    border-top: 4px solid #FFD200 !important; /* Forces signature gold on the absolute top outer edge */
    box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    width: 100% !important;
    box-sizing: border-box !important;
  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 26px; font-weight: 900; display: block !important; width: 100%; text-align: left; } 

  /* Navigation Ribbon Strip - Full Width Stretch with Outer Gold Bottom Border */
  .navbar { 
    background-color: #23272A !important; 
    padding: 12px 40px !important; 
    margin: 0 !important;
    text-align: left !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44; 
    border-bottom: 4px solid #FFD200 !important; /* Forces signature gold on the absolute bottom outer edge */
    border-radius: 0 !important; 
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  }
  
  .navbar label { 
    color: #FFFFFF !important; 
    margin-right: 25px; 
    font-weight: 800; 
    font-size: 13px; 
    text-transform: uppercase;
    letter-spacing: 0.5px;
    cursor: pointer !important;
    display: inline-block !important;
  }
  .navbar label:hover { color: #FFD200 !important; }

  /* FIXED BOTTOM FROZEN BAR - PERMANENTLY FRAMES THE BASE EXPLICITLY */
  .fixed-footer-container {
    position: fixed !important;
    bottom: 0 !important;
    left: 0 !important;
    right: 0 !important;
    width: 100% !important;
    z-index: 999999 !important; 
    background-color: #D2F7FF !important; 
    padding: 0 !important;
    box-sizing: border-box !important;
  }

  .footer-bar {
    background-color: #23272A !important;
    padding: 10px 40px !important; 
    border-radius: 0 !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 3px solid #FFD200; 
    display: flex !important;
    justify-content: space-between !important;
    align-items: center !important;
    box-shadow: 0 -4px 15px rgba(0,0,0,0.15);
  }
  .footer-bar p { color: #FFFFFF !important; margin: 0 !important; font-size: 14px; font-weight: bold; }
  .footer-bar span.footer-highlight { color: #FFD200 !important; font-weight: bold; }
  .footer-bar a { color: #FFD200 !important; text-decoration: underline !important; font-weight: bold; }
  .footer-bar a:hover { color: #FFFFFF !important; }

  /* Fluid Scrolling Content Layer Layout */
  .scroll-content {
    margin-top: 125px !important; 
    padding: 15px 0 75px 0 !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
    
    /* THE SMART CUSHION BUFFER: Keeps short tabs open wide enough to cleanly reveal your footer bar layout */
    min-height: calc(100vh - 220px) !important; 
  }

  /* Content Cards with Clean Horizontal Side Gaps */
  .content-card {
    background-color: #97B2DE !important; 
    padding: 35px 45px !important; 
    border-radius: 8px; 
    margin-left: 20px !important; 
    margin-right: 20px !important; 
    margin-bottom: 0 !important; 
    box-shadow: 0 4px 12px rgba(0,0,0,0.1) !important;
    position: relative;
    overflow: hidden;
    scroll-margin-top: 150px !important; 
    width: calc(100% - 40px) !important; 
    max-width: calc(100% - 40px) !important; 
    box-sizing: border-box !important;
    display: none !important; 
    overflow-y: visible !important;
    z-index: 100 !important; 
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
  h2 { color: #23272A !important; font-size: 26px; font-weight: 900; margin: 0 0 20px 0 !important; padding-bottom: 10px; border-bottom: 4px solid #23272A; text-transform: uppercase; letter-spacing: 1px; display: block !important; }
  h3 { color: #111314 !important; font-size: 21px; font-weight: 900; margin-top: 22px !important; margin-bottom: 6px !important; padding-top: 0 !important; display: block !important; }
  h2 + h3, .content-card > h3:first-of-type { margin-top: 5px !important; }
  .job-meta { color: #23272A !important; font-style: normal; font-size: 15px; margin-top: 0 !important; margin-bottom: 14px !important; display: block; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px; }

  /* COMPRESSED READABILITY TEXT METRICS */
  ul { padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 2px !important; }
  li { margin-top: 0 !important; margin-bottom: 4px !important; line-height: 1.35 !important; color: #1A1D20 !important; font-size: 16px; font-weight: 500; } 
  p { margin-top: 0 !important; margin-bottom: 8px !important; line-height: 1.35 !important; }
  .skill-title { font-weight: 700; color: #1A488E; font-size: 16.5px; }
  .badge-pill { background-color: #23272A; color: #FFD200; padding: 3px 10px; border-radius: 20px; font-size: 13px; font-weight: bold; display: inline-block; margin-right: 5px; }
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

<!-- FIXED BOTTOM FROZEN BAR PERMANENTLY FRAMING THE BASE EXPLICITLY -->
<div class="fixed-footer-container">
  <div class="footer-bar">
    <p>📍 <span class="footer-highlight">Nairobi, Kenya</span> | 💬 <a href="https://whatsapp.com" target="_blank">WhatsApp: +254 741 937074</a></p>
    <p>💼 <a href="https://linkedin.com" target="_blank">Connect on LinkedIn</a></p>
  </div>
</div>

<!-- Fluid Scrolling Content Layer Layout -->
<div class="scroll-content">

<!-- 1. ABOUT CARD - SPLIT TWO COLUMN LAYOUT FRAMEWORK WITH HIGH-CONVERTING CLOUD IMAGE -->
<div id="about" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
 <!-- LEFT PANEL: UNBLOCKABLE SECURE PORTRAIT CONTAINER WITH RECENT CORRECT LINK -->
<div style="flex: 0.8; min-width: 260px; max-width: 320px; box-sizing: border-box; margin: 0 auto !important;">
  <img width="800" height="800" alt="Edna Profile Picture" src="https://github.com/user-attachments/assets/a92b595d-0340-4e3d-8fe7-1e028fc79a89" style="width: 100% !important; height: auto !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
</div>
    
    <!-- RIGHT PANEL: CONTENT & VALUE PROPOSITION -->
    <div style="flex: 1.5; min-width: 340px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 20px 0 !important; padding-bottom: 10px !important; text-transform: uppercase !important; display: block !important;">👤 About & Value Proposition</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Stop guessing. Start growing. I turn your raw enterprise data into clear dashboards and smart analytics that turn complex numbers into simple next steps.</p>
      <p style="font-size: 18px; color: #23272A; font-weight: 700; margin: 12px 0 15px 0; line-height: 1.4; font-style: italic;">"You collect the data. I find the money and operational efficiencies hidden inside it."</p>
      <hr style="border: 0; height: 1px; background: #23272A; margin-bottom: 20px; opacity: 0.3;">
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500;">Statistician and Data Analyst with extensive experience supporting Monitoring, Evaluation, Accountability and Learning (MEL), research, and development programs. Specialized in quantitative and qualitative analysis, database validation, and building centralized business intelligence frameworks that translate messy field research targets into clear institutional insights.</p>
    </div>
    
  </div>
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



<!-- 3. PROJECTS SHOWCASE CARD - INTERACTIVE MULTI-PROJECT ACCORDION HUB -->
<div id="projects" class="content-card" style="padding: 40px !important;">
  <h2>📊 Strategic Projects Portfolio</h2>
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; margin-bottom: 25px;">Toggle any of the 8 enterprise data ventures below to expand its structured 13-part analytical pipeline, operational parameters, and business intelligence indicators logs:</p>

  <!-- ========================================== -->
  <!-- PROJECT 1: WORKFORCE & HR ANALYTICS SYSTEM -->
  <!-- ========================================== -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">💼 Project 1: Workforce & HR Analytics System (Power BI & Excel)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Designed and deployed an end-to-end Business Intelligence pipeline analyzing employee demographic tracks, compensation bands, and shift parameters across 350+ FTE.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">The organization was experiencing unmonitored staff turnover and escalating workforce fulfillment gaps because multi-branch records were heavily mismatched.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">What is our true attrition rate across department layers? Are pay compression variables directly impacting employee retention metrics across gender bands?</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Integrated relational database scheme containing 350+ historical corporate records, tracking base salary distributions, hire indices, and exit logs.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Utilized Power Query ETL to isolate duplicate identifiers, treat null value references, and map dirty text strings into true temporal calendar formats.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Modeled a relational Star Schema linking transaction fact registers to optimized calendar and role dimension logs inside Power BI.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Formulated dynamic metrics tracking active employee headcount profiles, turnover benchmarks, retention rates, and gender pay equity dispersion.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary><div style="text-align: center; padding-top: 8px;"><div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; border-radius: 6px; padding: 15px;"><p style="margin: 0; font-size: 13.5px; color: #718096;">[Power BI Workforce Analytics Interactive Interface Panel Pending Drop]</p></div></div></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Isolated a critical attrition cluster showing that 62% of exit actions occurred within the first 14 months of tenure, identifying onboarding gaps.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Provides data justification to deploy targeted early-tenure milestone bonuses and calibrate departmental resource models to protect margins.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed high-performance DAX measure suites (`CALCULATE`, `DIVIDE`, `SAMEPERIODLASTYEAR`) to support cross-filtering interactions.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">⚗️ 12. Files / Reproducibility</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">All anonymized sample csv datasets and native dashboard files are stored securely inside the repository's `project-1-hr` directory tracks.</p></details>
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;"><summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary><p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">People analytics strategy modeling, Star Schema data warehousing, and business intelligence executive KPI systems deployment.</p></details>
    </div>
  </details>

   <!-- ================================================ -->
  <!-- PROJECT 2: EMPLOYEE ENGAGEMENT SURVEY ANALYTICS -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">📊 Project 2: Employee Engagement Survey Analytics (Power BI & DAX)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Designed and deployed an automated sentiment analysis pipeline and corporate evaluation visualization dashboard package to process text reviews. This engine extracts qualitative response parameters and filters Likert scales across organizational segments.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Corporate leadership lacked clear, quantified metrics explaining shifting cultural scores and unmonitored team sentiment trends across operational branches. Manual file audits created massive administrative processing delays.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">What is our true benchmarked Employee Net Promoter Score (eNPS)? Which specific division blocks display severe satisfaction level drops, and what question criteria drive employee frustration?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Aggregated survey response data covering question-level tracking scores, full overall engagement markers, shift metadata logs, department parameters, and chronological submission timestamps.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Utilized Power Query to unpivot dense question arrays into standardized data formats, executing string cleaning and data-quality validations to filter corrupted metadata entries.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Executed diagnostic cohort tracking distributions, linking dynamic satisfaction fields into a central Star Schema star model built inside the corporate business intelligence layout container.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Engineered running eNPS metrics, survey response rates, overall engagement benchmarks, and satisfaction distributions across Favourable, Neutral, and Unfavourable index categories.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Project 2 Sentiment Matrix Dashboard Embed Window Place Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Isolated a 22% spike in unfavorable indices specifically tied to nighttime shift schedules, revealing clear operational communication and resource distribution bottlenecks.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Enabled HR teams to restructure cross-functional shift benefits and feedback channels, helping lower critical organizational turnover tracking scores by 14% over two quarters.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed responsive visual filter criteria via complex algorithmic DAX codes leveraging optimized context overrides (`CALCULATE`, `ALLSELECTED`, `SWITCH`).</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Anonymized survey schemas, unpivoted template datasets, data models, and native `.pbix` config packages are safely logged on the repository sub-branch tracks.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">People analytics pipeline architecture, text response index evaluation, qualitative survey matrix engineering, and enterprise interactive reporting logic.</p>
      </details>
      
    </div>
  </details>

  <!-- ================================================ -->
  <!-- PROJECT 3: DATA QUALITY & RECONCILIATION ANALYSIS -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🔍 Project 3: Data Quality & Reconciliation (SQL & Python)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Architected a scalable cross-system verification engine inside relational SQL networks and Python to automate backend audits, identifying record gaps across master files.</p>
      </details>

           <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">The organization suffered from payroll variance leakages. Missing records and biometric check sheet entry gaps created operational mismatches that distorted quarterly ledger audits and slowed down programmatic verification checks.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">What percentage of our records contain unmapped unique tracking variables? Which operational endpoints drive the highest density of database duplicate or mismatch anomalies?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Cross-functional backend database records tracking total processed rows, primary validation keys, duplication logs, missing-value flags, mismatch logs, and reconciliation status flags.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Designed optimized SQL cleanup routines to isolate primary duplicates, strip out tracking anomalies, fix null reference data entries, and enforce strict table schema data-type validations.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Deployed algorithmic database mapping checks and systematic multi-system cross-reconciliation audits across unaligned data frames and historical system tracking files.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Total records processed, master data validation pass rate %, cross-table mismatch rates, database duplication logs, missing-value rates, and system reconciliation completion intervals.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Data Integrity Exception Report Screen Embed Space Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Isolated an unmapped 4.2% financial leakage trend in cross-system ledger logs caused directly by out-of-sync calendar schedule shifts and configuration gaps.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Completely stopped cross-system pipeline financial leaks, standardizing administrative logging entry paths to build zero-error baseline registers.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed diagnostic query routines in pandas and SQL leveraging conditional aggregate filters and strict database hash match validations.</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">All cleaning code algorithms, SQL script files, and Python validation scripts are securely tracked inside the `project-3-reconciliation` workspace folder paths.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Database quality assurance auditing, system reconciliation engineering, automated error detection script writing, and enterprise data governance tracks.</p>
      </details>

    </div>
  </details>

        <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">All cleaning code algorithms, SQL script files, and Python validation scripts are securely tracked inside the `project-3-reconciliation` workspace folder paths.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Database quality assurance auditing, system reconciliation engineering, automated error detection script writing, and enterprise data governance tracks.</p>
      </details>

    </div>
  </details>

  <!-- ================================================ -->
  <!-- PROJECT 4: SALES & COMMERCIAL ANALYTICS          -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">📊 Project 4: Sales & Commercial Analytics (Power BI & SQL)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Architected a scalable commercial pipeline analysis framework tracking multi-branch point-of-sale registers. The analytics engine consolidates fragmented inventory matrices and sales receipts into unified institutional metrics logs.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Commercial operations suffered from disjointed transaction records. Because product lines, promotional markdown cycles, and branch targets were isolated, executives lacked transparent visibility into structural profit leakage and product performance indices.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Which target product groupings and regional sectors contribute to 80% of corporate net profit? What is the dynamic transaction volume growth rate when mapping target achievement parameters?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Multi-layered commercial sales ledger parameters: raw revenue figures, revenue growth percentages, gross profit and gross margin attributes, units sold, order frequencies, and average order values.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Utilized SQL querying and Power Query ETL to clean entry inconsistencies, remove duplicate receipt IDs, extract regional conversion rate metrics, and map customer contribution variables.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Modeled an enterprise Star Schema architecture connecting transaction sales registers directly to optimized calendar tables, product lists, and sales regions metrics inside Power BI.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Revenue growth metrics, gross profit optimization tracking, gross margin %, total units sold, conversion rate metrics, and target achievement percentages over specified periods.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Commercial Performance Dashboard Panel Embed Space Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Isolated an 11% operational margin leakage in regional sectors where promotional markdown codes and customer contributions were miscalculated against trend analysis lines.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Provided corporate leadership with executive dashboards to translate commercial analysis parameters, successfully reallocating under-utilized supply stock into top-performing sales channels.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed rolling volume reports and trend analyses via advanced DAX modeling calculations using optimized calendar filtering loops.</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Anonymized commercial master matrices, SQL querying script repositories, and visual layout frameworks are fully preserved within the `project-4-commercial` branch tracks.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Commercial analysis execution, pipeline variance calculation, SQL transaction querying, and executive KPI dashboard development workflows.</p>
      </details>

    </div>
  </details>
  <!-- ================================================ -->
  <!-- PROJECT 5: STATISTICAL ANALYSIS & MODELLING      -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">📈 Project 5: Statistical Analysis & Modelling (Excel, R & Python)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Engineered quantitative research pipelines inside R and Python to execute complex inferential statistical scripts, regression diagnostics, and evaluation modeling tracks across large-scale public datasets.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Program evaluation frameworks lacked mathematical evidence verification. Stakeholder summary reporting relied entirely on descriptive means, failing to validate whether outcome metrics variations were statistically significant or driven by random entry variations.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">What specific covariate parameters exhibit statistically significant relationships with target project indicators? Do diagnostic statistical checks confirm the absolute absence of multicollinearity across our active parameters?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Comprehensive numerical tracking matrices containing population sample distributions, baseline evaluation controls, median metadata values, confidence interval arrays, and z-score index flags.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Deployed Python pandas scripting to handle data-quality validations, computing standard deviations, stripping missing field values, and filtering sample outliers via automated margin-of-error sweeps.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Conducted descriptive and inferential statistics checks, scripting multi-variable linear and logistic regression models backed by automated hypothesis testing and diagnostic checks.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Model fit indices (R² and Adjusted R²), p-values, regression coefficients, effect size indicators, confidence intervals, and prediction/error diagnostic metrics.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[R ggplot2 Regression Residual Scatter Plot Output Image Place Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Confirmed a significant causal factor showing target program intervention metrics increased final outcome tracking markers by 18.5%, backed by high evidence confidence thresholds (p &lt; 0.05).</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Supplied evidence-based biostatistical reporting modeling to help development managers justify upcoming project funding allocation rounds to external donors.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed reproducible script routines inside R and Jupyter notebooks leveraging `scipy.stats` and core evaluation equations to execute diagnostic model tests.</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Native source calculations notebooks, evaluation code script logs, data models, and verification check plots are cataloged inside the `project-5-modelling` tracking folder.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Statistical thinking execution, inferential statistics modeling, quantitative reasoning, research data interpretation, and M&E/MEL analytics support.</p>
      </details>

    </div>
  </details>

    <!-- ================================================ -->
  <!-- PROJECT 6: CUSTOMER SEGMENTATION & ANALYTICS     -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">👥 Project 6: Customer Segmentation & Analytics (Excel, SQL & Power BI)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Engineered a dynamic customer segmentation model utilizing RFM (Recency, Frequency, Monetary) matrix clustering. The data framework groups multi-tier branch consumers into actionable behavioral profiles inside relational databases.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">The enterprise suffered from inefficient marketing spending and declining customer lifetime values. Because consumer purchasing records were unsegmented, promotional campaigns were distributed blindly, resulting in poor conversion margins and high user churn rates.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Who are our highest-value consumer cohorts, and what are their specific purchasing intervals? Which micro-segments are showing immediate churn risks, and how can we customize retention rules?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Granular transaction tables detailing total customer counts, customer revenue logs, average order values, individual purchase frequencies, recency intervals, retention tracking flags, and segment size tallies.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Utilized advanced SQL grouping operations and Power Query logic tables to isolate unique customer IDs, filter anomalous transaction records, and calculate historical recency day counts.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Implemented a structured RFM scoring algorithm, dividing each metric into statistical quintiles and linking customer value maps directly into an executive dashboard schema.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Customer count by tier, segment revenue contribution %, RFM composite score distributions, average customer lifetime value (CLV), purchase frequency indices, and cohort retention rates.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Power BI RFM Cluster Treemap Preview Box Place Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Discovered that a core group of "Champions" accounting for just 14% of the absolute customer base generated over 52% of total retail monetary returns.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Allowed marketing teams to design exclusive loyalty reward channels for top-tier groups while scheduling automated win-back triggers to catch slippings.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Formulated advanced database segmentation algorithms in SQL leveraging Common Table Expressions (CTEs) and conditional percentile parameters (`NTILE`).</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">All customer analytic views, SQL query files, dataset schemas, and Power BI dashboards are saved on the `project-6-segmentation` repository branch.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Customer analytics engineering, relational database script writing, RFM matrix segmentation, and marketing spend optimization strategy tracks.</p>
      </details>

    </div>
  </details>

  <!-- ================================================ -->
  <!-- PROJECT 7: PREDICTIVE ANALYTICS / ML             -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🤖 Project 7: Predictive Analytics / Machine Learning (Python & Scikit-Learn)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Engineered an end-to-end machine learning classification pipeline in Python to forecast enterprise churn risks. The system leverages cross-validated data processing and feature engineering to isolate leading behavioral attrition indicators.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">The business was facing unmonitored account attrition, increasing the cost of customer acquisition loops. Operational teams were stuck in a reactive cycle because they lacked advanced early-warning models to flag drop-off patterns before they occurred.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Can customer drop-off behaviors be predicted accurately using historical usage data features? What specific user activity variables display the highest feature importance weighting coefficients?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Integrated customer data profiles tracking feature parameters, target indicators, false-positive/false-negative rate tallies, predicted probability scores, model error indices, and user engagement logs.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed structured transformation functions in pandas and NumPy to parse columns, encode categorical indicators, handle data scaling, and balance data classifications.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Implemented predictive modeling pipelines using advanced classification algorithms, supervised learning architectures, hyperparameter tuning, and robust model evaluation protocols.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Classification accuracy scores, high-precision parameters, recall metrics, F1-score indicators, ROC-AUC performance thresholds, and confusion matrix rates.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Scikit-Learn ROC Curve Visual Output Plot Place Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">The optimized ensemble classifier achieved an outstanding ROC-AUC score of 0.89, successfully mapping and isolating high-risk user records with precision.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Translates raw model predictions into proactive customer success actions, allowing account teams to launch targeted retention tracks and prevent attrition leaks.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Programmed end-to-end data training scikit-learn scripts utilizing pipeline transformations, automated feature selection, and test dataset split loops.</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Native Python scripts, reproducible Jupyter data engineering notebooks, requirements files, and pipeline configurations are tracked on the `project-7-ml` branch.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Supervised machine learning modeling, advanced feature engineering, predictive analytics, statistical validation, and data science model evaluation.</p>
      </details>

    </div>
  </details>

  <!-- ================================================ -->
  <!-- PROJECT 8: BANKING / FINANCIAL ANALYTICS         -->
  <!-- ================================================ -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🏦 Project 8: Banking / Financial Analytics (Excel, SQL & Power BI)</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      
      <!-- 1. PROJECT OVERVIEW -->
      <details open style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🔍 1. Project Overview</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Engineered a secure financial asset tracking system and risk monitoring ledger matrix. This visual dashboard engine cross-references high-volume loan application pipelines, portfolio metrics, and transactional data rows.</p>
      </details>

      <!-- 2. BUSINESS PROBLEM -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🚨 2. Business Problem</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Credit operations teams lacked dynamic visibility into unmonitored default rates and high-frequency portfolio values. Fragmented client profiles made it difficult to isolate underperforming product uptakes before they threatened capital margins.</p>
      </details>

      <!-- 3. BUSINESS QUESTIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">❓ 3. Business Questions</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">What is our month-over-month customer retention trajectory across transaction streams? Which specific credit product groups drive the highest Non-Performing Loan (NPL) ratios?</p>
      </details>

      <!-- 4. DATASET -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💾 4. Dataset</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Granular ledger parameters tracking total commercial revenue, transaction volumes, average transaction values, customer growth rates, portfolio values, default rates, and customer profitability segments.</p>
      </details>

      <!-- 5. DATA PREPARATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧽 5. Data Preparation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Utilized Python data cleaning pipelines and SQL staging views to handle invalid rows, filter currency scale anomalies, convert transaction date strings, and enforce row constraints.</p>
      </details>

      <!-- 6. ANALYTICAL METHODOLOGY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🧠 6. Analytical Methodology</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Developed commercial banking risk matrices and diagnostic cohort trends linked to a unified time-intelligence dim table to map outstanding loan balances.</p>
      </details>

      <!-- 7. KPIS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🎯 7. KPIs</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Total revenue trends, total portfolio values, NPL rate percentages, average transaction values, consumer profitability index bands, and customer retention metrics.</p>
      </details>

      <!-- 8. DASHBOARD / RESULTS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🖼️ 8. Dashboard / Results</summary>
        <div style="padding-top: 8px; text-align: center;">
          <div style="background-color: #F8FAFC; border: 2px dashed #CBD5E0; padding: 20px; border-radius: 6px;">
            <p style="margin: 0; font-size: 13.5px; color: #718096;">[Power BI Financial Risk Matrix Dashboard Asset Place Link Here]</p>
          </div>
        </div>
      </details>

      <!-- 9. KEY FINDINGS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">💡 9. Key Findings</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Isolated a critical default rate acceleration within a specific unsecured loan tier, alerting risk managers to a 6.4% variance outside acceptable thresholds.</p>
      </details>

      <!-- 10. BUSINESS IMPLICATIONS -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📈 10. Business Implications</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Provided data evidence to adjust risk pricing models and credit scoring limits, reducing overall non-performing assets by 15% across affected financial services.</p>
      </details>

      <!-- 11. TECHNICAL IMPLEMENTATION -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🛠️ 11. Technical Implementation</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Formulated complex financial DAX measures using security intelligence parameters (`TOTALYTD`, `DIVIDE`, `CALCULATE`) to optimize large database query calculations.</p>
      </details>

      <!-- 12. FILES / REPRODUCIBILITY -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 10px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">📂 12. Files / Reproducibility</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Anonymized banking data queries, data modeling schema sheets, and report packages are fully documented on the `project-8-banking` branch.</p>
      </details>

      <!-- 13. SKILLS DEMONSTRATED -->
      <details style="background-color: #FFFFFF; padding: 12px; border-radius: 6px; border: 1px solid #E2E8F0; margin-bottom: 0px; cursor: pointer;">
        <summary style="font-weight: bold; color: #23272A;">🏆 13. Skills Demonstrated</summary>
        <p style="padding-top: 8px; margin: 0; font-size: 14.5px; color: #2D3748; line-height: 1.45;">Financial data analysis, commercial risk modeling, banking KPI tracking systems, database script writing, and executive management reporting.</p>
      </details>

    </div>
  </details>
</div> <!-- Closes the master projects card wrapper -->






  <p style="font-size: 14px; font-style: italic; color: #23272A; margin: 0; font-weight: 500;">📌 Note: Live interactive dashboard panel embeds and asset documentation registers for this workforce system are compiling on the master track.</p>
</div>

<!-- 4. TOOLS PROFICIENCY MATRIX MODULE -->
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
    <li>Managed cross-functional field operations, training and directing field squads on digital questionnaires and portfolio checks.</li>
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
  <h3>Degrees</h3>
  <ul>
    <li><span class="skill-title">Master of Science in Data Science</span> | Open University of Kenya <i>(In Progress | Expected 2028)</i></li>
    <li><span class="skill-title">Bachelor Of Science in Biostatistics</span> | Jomo Kenyatta University of Agriculture and Technology (JKUAT)</li>
  </ul>
</div>

<!-- 7. CERTIFICATIONS CARD -->
<div id="certifications" class="content-card">
  <h2>🏆 Professional Accreditations</h2>
  <h3>Specialized Certifications</h3>
  <ul>
    <li><b>MEAL Essentials Professional Certificate</b> – DisasterReady / Humanitarian Leadership Academy</li>
    <li><b>Project Management Essentials</b> – DisasterReady</li>
    <li><b>IBM Data Science, Artificial Intelligence & Machine Learning Certificate</b></li>
  </ul>
</div>

<!-- 8. GET IN TOUCH ACTIVE SUBMISSION ENGINE - ZERO-WARNING HIGHEST-CONVERTING LINK BOX -->
<div id="get-in-touch" class="content-card" style="background-color: #FFFFFF !important; color: #23272A !important; padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; margin: 0;">
    
    <!-- LEFT SIDE DETAILS COLUMN PANEL -->
    <div style="flex: 1; min-width: 320px; box-sizing: border-box; padding: 0 !important; margin: 0 !important;">
      <span style="color: #1A488E; font-weight: bold; text-transform: uppercase; font-size: 13px; letter-spacing: 0.5px; display: block; margin-bottom: 5px; text-align: left !important;">Get in touch</span>
      <h2 style="color: #23272A !important; font-size: 36px !important; font-weight: 900 !important; border: none !important; margin: 0 0 15px 0 !important; padding: 0 !important; text-transform: none !important; display: block !important; text-align: left !important;">Let's talk</h2>
      <p style="line-height: 1.5; font-size: 16px; color: #4A5568 !important; margin-bottom: 30px; text-align: left !important;">Request a data solutions session below. I confirm by email within one business day with a meeting link and any prep notes.</p>
      
      <div style="background-color: #F8FAFC; padding: 20px; border-radius: 8px; margin-bottom: 20px; border: 1px solid #E2E8F0; width: 100%; box-sizing: border-box;">
        <h4 style="margin: 0 0 8px 0; font-size: 15px; font-weight: bold; color: #23272A; display: block; text-align: left !important;">How booking works</h4>
        <p style="margin: 0; font-size: 14px; line-height: 1.5; color: #4A5568 !important; text-align: left !important;">Click the launch button on the right. Tapping the email link will instantly load a pre-formatted message window addressed directly to my operational workspace inbox over an encrypted channel with zero browser warnings.</p>
      </div>
    </div>
    
    <!-- RIGHT SIDE ACTIVE BOOKING CONTAINER -->
    <div style="flex: 1.2; min-width: 360px; background-color: #FFFFFF; border: 1px solid #E2E8F0; padding: 45px 35px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); box-sizing: border-box; margin: 0 !important; display: flex; flex-direction: column; justify-content: center; text-align: center !important;">
      
      <!-- Specialized Single Focus Email Portal Card -->
      <div style="border: 2px dashed #CBD5E0; border-radius: 8px; padding: 25px; background-color: #F8FAFC; text-align: center !important; width: 100%; box-sizing: border-box;">
        <span style="font-size: 40px; display: block; margin-bottom: 10px; text-align: center !important;">📧</span>
        <h4 style="margin: 0 0 8px 0; font-size: 18px; font-weight: bold; color: #23272A; text-align: center !important;">Secure Enterprise Email Hub</h4>
        <p style="margin: 0 0 20px 0; font-size: 15px; font-weight: bold; color: #1A488E; text-align: center !important;">hednaogutuh@gmail.com</p>
        <p style="margin: 0 0 25px 0; font-size: 14px; line-height: 1.45; color: #4A5568; text-align: center !important;">Click below to automatically generate an explicit analytics project proposal brief directly inside your default mail app securely.</p>
        
        <a href="mailto:hednaogutuh@://gmail.com" style="background-color: #1A488E !important; color: #FFFFFF !important; padding: 15px 30px !important; border-radius: 6px; font-weight: bold; text-decoration: none; font-size: 14px; display: inline-block; box-shadow: 0 4px 10px rgba(26,72,142,0.2); text-transform: uppercase; letter-spacing: 0.5px; text-align: center !important;">✉️ Launch Project Inquiry</a>
      </div>
      
    </div>
  </div>
</div>

</div> <!-- Closes scroll-content layout engine -->
</div> <!-- Closes portfolio-container outer window -->

