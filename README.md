<style>
  /* Force hide default GitHub template elements */
  header, #header, .title, h1:first-of-type:not(.header-block h1) {
    display: none !important;
  }
  
  /* Overrides GitHub's default wrapper padding parameters to force true edge-to-edge stretch */
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
  
  /* MASTER FIXED TOP HEADER WRAPPER - MAXIMUM CEILING LAYER PRIORITY */
  .master-sticky-header {
    position: fixed !important;
    top: 0 !important;
    left: 0 !important;   
    right: 0 !important;  
    width: 100% !important;
    z-index: 999999 !important; 
    background-color: #23272A !important; 
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

  /* Main Profile Block Header Content Box - Height reduced to make the bar compact */
  .header-block { 
    background-color: #23272A !important; 
    color: #FFFFFF !important; 
    padding: 8px 40px !important; /* Reduced vertical padding */
    border-radius: 0 !important; 
    margin: 0 !important; 
    border-left: 8px solid #FFD200;
    border-top: 4px solid #FFD200 !important; 
    box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    width: 100% !important;
    box-sizing: border-box !important;
  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 26px; font-weight: 900; display: block !important; width: 100%; text-align: left; } 

  /* Navigation Ribbon Strip - Padding tightened down */
  .navbar { 
    background-color: #23272A !important; 
    padding: 8px 40px !important; /* Tightened from 12px down to 8px */
    margin: 0 !important;
    text-align: left !important; 
    width: 100% !important;
    box-sizing: border-box !important;
    border-left: 8px solid #FFD200;
    border-top: 1px solid #3A3F44; 
    border-bottom: 4px solid #FFD200 !important; 
    border-radius: 0 !important; 
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  }
  
  .navbar label { 
    color: #FFFFFF !important; 
    margin-right: 20px; 
    font-weight: 800; 
    font-size: 12px; 
    text-transform: uppercase;
    letter-spacing: 0.5px;
    cursor: pointer !important;
    display: inline-block !important;
  }
  .navbar label:hover { color: #FFD200 !important; }

  /* FIXED BOTTOM FROZEN FOOTER BAR - FORCED MAXIMUM PRIORITY LAYER */
  .fixed-footer-container {
    position: fixed !important;
    bottom: 0 !important;
    left: 0 !important;
    right: 0 !important;
    width: 100% !important;
    z-index: 9999999 !important; 
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
    box-shadow: 0 -5px 20px rgba(0,0,0,0.25) !important;
  }
  .footer-bar p { color: #FFFFFF !important; margin: 0 !important; font-size: 14px; font-weight: bold; }
  .footer-bar span.footer-highlight { color: #FFD200 !important; font-weight: bold; }
  .footer-bar a { color: #FFD200 !important; text-decoration: underline !important; font-weight: bold; }
  .footer-bar a:hover { color: #FFFFFF !important; }

  /* Scrolling Content Layout Core Layer Workspace - Tightened Top Spacing Option */
  .scroll-content {
    margin-top: 125px !important; 
    padding: 10px 0 95px 0 !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
    min-height: calc(100vh - 160px) !important; 
  }


    /* Content Cards Layout Parameters - Text top-aligned via tightened internal padding */
  .content-card {
    background-color: #D2F7FF !important; 
    padding: 10px 45px 35px 45px !important; /* Top padding reduced to 10px to align words to the top */
    border-radius: 12px !important; 
    margin-left: 20px !important; 
    margin-right: 20px !important; 
    margin-top: 0 !important;
    margin-bottom: 0 !important; 
    border: 2px solid #23272A !important;
    box-shadow: 0 10px 25px rgba(0,0,0,0.15), 0 4px 10px rgba(0,0,0,0.12), inset 0 1px 0 rgba(255,255,255,0.2) !important;
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



  /* PURE CSS TAB SWITCH MECHANISM - CONNECTS NAV BUTTONS TO CARDS */
  #tab-home:checked ~ .scroll-content #home,
  #tab-about:checked ~ .scroll-content #about,
  #tab-services:checked ~ .scroll-content #services,
  #tab-projects:checked ~ .scroll-content #projects,
  #tab-portfolio:checked ~ .scroll-content #portfolio-hub,
  #tab-experience:checked ~ .scroll-content #experience,
  #tab-education:checked ~ .scroll-content #education,
  #tab-certifications:checked ~ .scroll-content #certifications,
  #tab-get-in-touch:checked ~ .scroll-content #get-in-touch {
    display: block !important; 
  }

  /* Highlights active menu labels inside the navbar array */
  #tab-home:checked ~ .master-sticky-header .navbar label[for="tab-home"],
  #tab-about:checked ~ .master-sticky-header .navbar label[for="tab-about"],
  #tab-services:checked ~ .master-sticky-header .navbar label[for="tab-services"],
  #tab-projects:checked ~ .master-sticky-header .navbar label[for="tab-projects"],
  #tab-portfolio:checked ~ .master-sticky-header .navbar label[for="tab-portfolio"],
  #tab-experience:checked ~ .master-sticky-header .navbar label[for="tab-experience"],
  #tab-education:checked ~ .master-sticky-header .navbar label[for="tab-education"],
  #tab-certifications:checked ~ .master-sticky-header .navbar label[for="tab-certifications"],
  #tab-get-in-touch:checked ~ .master-sticky-header .navbar label[for="tab-get-in-touch"] {
    color: #FFD200 !important;
    border-bottom: 2px solid #FFD200;
  }

  /* Typography metrics controllers */
  .content-card > h2:first-child, .content-card > div:first-child { margin-top: 0 !important; padding-top: 0 !important; }
  h2 { color: #23272A !important; font-size: 26px; font-weight: 900; margin: 0 0 20px 0 !important; padding-bottom: 10px; border-bottom: 4px solid #23272A; text-transform: uppercase; letter-spacing: 1px; display: block !important; }
  h3 { color: #111314 !important; font-size: 21px; font-weight: 900; margin-top: 22px !important; margin-bottom: 6px !important; padding-top: 0 !important; display: block !important; }
  h2 + h3, .content-card > h3:first-of-type { margin-top: 5px !important; }
  .job-meta { color: #23272A !important; font-style: normal; font-size: 15px; margin-top: 0 !important; margin-bottom: 14px !important; display: block; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px; }

  ul { padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 2px !important; }
  li { margin-top: 0 !important; margin-bottom: 6px !important; line-height: 1.4 !important; color: #1A1D20 !important; font-size: 15.5px; font-weight: 500; } 
  p { margin-top: 0 !important; margin-bottom: 12px !important; line-height: 1.45 !important; font-size: 15.5px; color: #1A1D20 !important; }
  .skill-title { font-weight: 700; color: #1A488E; font-size: 16.5px; }
  .area-badge { background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 13.5px; padding: 4px 12px; border-radius: 4px; display: inline-block; margin-bottom: 8px; }
</style>

<div class="portfolio-container">

<!-- MASTER REGISTER INPUT RADIO CONTROLLERS -->
<input type="radio" name="page-tabs" id="tab-home" class="tab-toggle" checked />
<input type="radio" name="page-tabs" id="tab-about" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-services" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-projects" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-portfolio" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-experience" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-education" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-certifications" class="tab-toggle" />
<input type="radio" name="page-tabs" id="tab-get-in-touch" class="tab-toggle" />

<!-- FIXED EDGE-TO-EDGE TOP HEADER BLOCK AND NAVIGATION CONTROL BAR -->
<div class="master-sticky-header">
  <div class="header-block">
    <h1>Edna Achieng Ogutu</h1>
  </div>

  <div class="navbar">
    <label for="tab-home"> HOME</label>
    <label for="tab-about"> ABOUT</label>
    <label for="tab-services"> SERVICES</label>
    <label for="tab-projects"> PROJECTS</label>
    <label for="tab-portfolio"> PORTFOLIO</label>
    <label for="tab-experience"> EXPERIENCE</label>
    <label for="tab-education"> EDUCATION</label>
    <label for="tab-certifications"> CERTIFICATIONS</label>
    <label for="tab-get-in-touch"> GET IN TOUCH</label>
  </div>
</div>
<!-- FIXED EDGE-TO-EDGE BOTTOM FROZEN FOOTER BAR -->
<div class="fixed-footer-container">
  <div class="footer-bar">
    <p> <span class="footer-highlight">Nairobi, Kenya</span> | 💬 <a href="https://whatsapp.com" target="_blank">WhatsApp: +254 741 937074</a></p>
    <p> <a href="https://www.linkedin.com/in/edna-achieng-ogutu/" target="_blank">Connect on LinkedIn</a></p>
  </div>
</div>

<div class="scroll-content">

<!-- ================================================ -->
<!-- 1. HOME CARD                                     -->
<!-- ================================================ -->
<div id="home" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
    <!-- LEFT PANEL: DATA GRAPHIC CANVAS CONTAINER -->
    <div style="flex: 0.8; min-width: 260px; max-width: 320px; box-sizing: border-box; margin: 0 auto !important;">
      <img width="488" height="800" alt="data" src="data.png" style="width: 100% !important; height: auto !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
    </div>
    
    <!-- RIGHT PANEL: HOME BRIEF CONTENT -->
    <div style="flex: 1.5; min-width: 340px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 20px 0 !important; padding-bottom: 10px !important; text-transform: uppercase !important; display: block !important;"> Welcome</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Edna Achieng Ogutu</p>
      <p style="font-size: 18px; color: #1A488E; font-weight: 700; margin-bottom: 15px;">Statistician | Data Analyst | Business Intelligence | Data Science | Workforce Analytics</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: bold; margin-bottom: 15px;">I engineer robust data pipelines, statistical frameworks, and automated dashboards that eliminate operational reporting blind spots, protect corporate budgets, and drive decision-ready intelligence.</p>
      <p style="line-height: 1.45; font-size: 15.5px; color: #1A1D20; font-weight: 500; margin-bottom: 20px;">I am a Statistician and Data Analyst with a deep background in Biostatistics and experience working with workforce tracking metrics, research diagnostics, operational flows, survey matrices, and commercial business data. By bridging the gap between raw data complexity and executive strategy, I combine advanced data management, descriptive and inferential statistics, and modern business intelligence to transform disorganized data streams into high-integrity information, clear operational insights, and decision-ready executive reporting.</p>
      
      <p style="margin-top: 25px; font-weight: bold; font-size: 15px; color: #23272A;"> Explore My Portfolio: <label for="tab-projects" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">View Selected Projects Frameworks</label> | <label for="tab-services" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Explore Specialized Analytics Services</label> | <label for="tab-get-in-touch" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Schedule a Data Solutions Consultation Session</label></p>
    </div>
    
  </div>
</div>

<!-- ================================================ -->
<!-- 2. ABOUT CARD                                    -->
<!-- ================================================ -->
<div id="about" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
    <!-- LEFT PANEL: UNBLOCKABLE SECURE PORTRAIT CONTAINER -->
    <div style="flex: 0.8; min-width: 260px; max-width: 320px; box-sizing: border-box; margin: 0 auto !important;">
      <img width="800" height="800" alt="Edna Profile Picture" src="Edna Profile Picture.png" style="width: 100% !important; height: auto !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
    </div>
    
    <!-- RIGHT PANEL: ABOUT PROPOSITION CONTENT -->
    <div style="flex: 1.5; min-width: 340px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 20px 0 !important; padding-bottom: 10px !important; text-transform: uppercase !important; display: block !important;"> About Me</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">I bridge the structural gap between messy, multi-source raw data and high-stakes executive strategy.</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 15px;">My approach is centered on building high-integrity validation checks at the collection source, ensuring that every predictive model, regression script, or visualization dashboard is mathematically sound, audit-ready, and immediately actionable for corporate decision-makers.</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 20px;">Operating across the entire analytical pipeline—from executing rigorous data cleaning and cross-system reconciliations to formulating diagnostic models and interactive reporting systems—I transform complex numbers into simple, strategic next steps. I believe effective analytics begins with absolute data quality, requiring the right analytical questions to generate long-term operational efficiencies.</p>
      
      <h3 style="margin-top: 22px !important; margin-bottom: 6px !important; font-size: 21px; font-weight: 900; color: #111314 !important;"> Core Execution Domains</h3>
      <ul style="padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 15px !important;">
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Data Analytics & Modeling:</span> Designing custom KPI matrix systems, executing exploratory data analysis (EDA), trend forecasting, and diagnostic performance tracking.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Data Engineering & Management:</span> Building automated data cleaning pipelines, cross-source record validation, system reconciliation, and database preparation tracks.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Statistical Inference & Research:</span> Deployed descriptive and inferential statistics, multivariable regression modeling, diagnostic testing, and empirical evidence synthesis.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Business Intelligence Systems:</span> Developing responsive, enterprise-grade data dashboards, interactive corporate visual maps, and executive management report frameworks.</li>
      </ul>
      <p style="font-size: 15px; color: #1A488E; font-weight: bold; margin: 0;"> Data Analytical Tools Mastered: Excel | Power Query | Power BI | DAX | SQL | Python | R | STATA | SPSS</p>
    </div>
    
  </div>
</div>

<!-- ================================================ -->
<!-- 3. SERVICES CARD                                 -->
<!-- ================================================ -->
<div id="services" class="content-card">
  <h2> Operational Consulting Services</h2>
  <p style="margin-bottom: 20px; font-weight: bold; color: #1A488E;">Speaking directly to organizational pain points—substituting manual error with high-integrity automation:</p>
  <ul>
    <li><span class="skill-title">Enterprise Data Analytics:</span> Transforming disparate, structured data into clear commercial insights, localized market trends, and high-visibility corporate performance indicators.</li>
    <li><span class="skill-title">Database Validation & Auditing:</span> Implementing automated cleaning routines and cross-system ledger reconciliation to eliminate duplicate tracking records, fix syntax discrepancies, and isolate data leakages.</li>
    <li><span class="skill-title">Executive Business Intelligence:</span> Engineering responsive Power BI and Advanced Excel dashboard suites equipped with dynamic filtering and deep drill-down analytics for live decision support.</li>
    <li><span class="skill-title">Statistical & Research Analytics:</span> Applying advanced quantitative methods, population sampling controls, and experimental regressions to survey and field research data to output sound, evidence-based reporting.</li>
        <li><span class="skill-title">Advanced Commercial Analytics:</span> Deploying customer behavioral segmentation matrices, RFM clustering profiles, supervised machine learning pipelines, and predictive risk modeling.</li>
  </ul>
  <p style="margin-top: 25px; font-weight: bold;"><label for="tab-projects" style="color: #1A488E; cursor: pointer; text-decoration: underline;"> Review the Live Infrastructure Systems Powered by These Services →</label></p>
</div>

<!-- ================================================ -->
<!-- 4. PROJECTS CARD                                 -->
<!-- ================================================ -->
<div id="projects" class="content-card">
  <h2> Selected Projects Portfolio</h2>
  <p style="margin-bottom: 25px;">A directory of production-ready analytical systems designed to optimize business operations, increase tracking visibility, and automate multi-source data processing pipelines using a protective synopsis format:</p>

  <!-- PROJECT 1 -->
  <details style="background-color: #FFFFFF; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;"> 1. Workforce & HR Analytics System</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b> Project Synopsis:</b> Developed an interactive workforce analytics system to transform fragmented employee records into management-ready insights tracking workforce composition, departmental distributions, salary bands, and performance metrics across large employee cohorts.</p>
      <p><b> Analytical Focus:</b> Workforce scale tracking | Department and role distribution | Salary compression and equity patterns | Shift performance variables | Attrition and stability trends.</p>
      <p><b> Specialized Tools Stack:</b> Excel | Power Query | Power BI | DAX | Statistical Analysis</p>
      <p><b> Strategic Value & Output:</b> Interactive Power BI report dashboard featuring multi-dimensional cross-filtering. Delivers a consolidated view of workforce health parameters to support executive monitoring, compliance audits, and strategic resource forecasting.</p>
    </div>
  </details>

  <!-- PROJECT 2 -->
  <details style="background-color: #FFFFFF; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;"> 2. Data Quality & Reconciliation Engine</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b> Project Synopsis:</b> Architected a data validation and reconciliation module to ingest multi-source administrative files, isolate structural data discrepancies, match missing parameters, and compile a verified clean database for secure corporate financial reporting.</p>
      <p><b> Analytical Focus:</b> Data completeness metrics | Duplicate and missing-value isolation | Cross-system key matching | Automated ledger reconciliation | Schema standardization | Exception reporting logs.</p>
      <p><b> Specialized Tools Stack:</b> Excel | Power Query | SQL | Python | Statistical Analysis</p>
      <p><b> Strategic Value & Output:</b> A fully validated, reconciled relational dataset backed by automated exception tracking scripts. Mitigates financial and reporting risk by identifying and resolving structural database anomalies before files are used for audits.</p>
    </div>
  </details>

  <!-- PROJECT 3 -->
  <details style="background-color: #FFFFFF; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;"> 3. Employee Engagement & Statistical Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b> Project Synopsis:</b> Engineered a quantitative survey analytics system to process corporate sentiment tracking files, evaluating feedback distributions, response behaviors, and demographic correlations across dynamic organizational blocks.</p>
      <p><b> Analytical Focus:</b> Engagement pattern tracking | Survey response trends | Cohort sentiment analysis | Multi-variable correlation | Descriptive and inferential statistics diagnostics | Analytical data visualization.</p>
      <p><b> Specialized Tools Stack:</b> Excel | Power Query | Power BI | Python / R | Statistical Analysis</p>
      <p><b> Strategic Value & Output:</b> Interactive sentiment matrix dashboard supported by inferential statistical tests. Translates raw Likert-scale feedback metrics into structured evidence to support proactive team management and isolate operational friction points.</p>
    </div>
  </details>

  <!-- PROJECT 4 -->
  <details style="background-color: #FFFFFF; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 0px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;"> 4. Customer & Commercial Predictive Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b> Project Synopsis:</b> Developed an end-to-end commercial optimization pipeline using business transactions to group buyer cohorts and apply supervised machine learning classification algorithms to predict churn risks.</p>
      <p><b> Analytical Focus:</b> Purchasing pattern trends | Gross profit margins % | Customer behavioral segmentation | Customer Lifetime Value (CLV) tracks | Supervised predictive modeling | Model precision and performance evaluation.</p>
      <p><b> Specialized Tools Stack:</b> Excel | SQL | Python | Power BI | Scikit-Learn</p>
      <p><b> Strategic Value & Output:</b> Enterprise business intelligence dashboard connected directly to statistical clustering and churn risk classifiers. Combines visual reporting with advanced predictive diagnostics to identify high-value customer groups and mitigate revenue drop-offs.</p>
    </div>
  </details>
</div>

<!-- ================================================ -->
<!-- 5. PORTFOLIO CARD                                -->
<!-- ================================================ -->
<div id="portfolio-hub" class="content-card">
  <h2> Portfolio Directory</h2>
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; margin-bottom: 25px;">A directory summarizing alignment profiles and operational capability targets for my core data modules:</p>
  
  <div style="width: 100% !important; overflow-x: auto !important; margin-bottom: 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <table style="width: 100% !important; min-width: 950px !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 13.5px !important; margin: 0;">
      <thead>
        <tr style="background-color: #23272A !important; color: #FFFFFF !important; font-weight: bold;">
          <th style="padding: 14px 10px; border-right: 1px solid #3A3F44; text-align: center; width: 4%;">#</th>
          <th style="padding: 14px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 22%;">Venture Track Name Focus</th>
          <th style="padding: 14px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 18%;">Specialized Tools Stack</th>
          <th style="padding: 14px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 26%;">Core Enterprise Metrics Deployed</th>
          <th style="padding: 14px 12px; text-align: left; width: 30%;">Target Operational Capability Value</th>
        </tr>
      </thead>
      <tbody>
        <tr style="background-color: #FFFFFF; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">1</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Workforce & HR Analytics</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0;">Excel, Power Query, Power BI, DAX</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0;">Headcount, Department Distribution, Attrition Rate</td>
          <td style="padding: 14px 12px; font-weight: 500;">Analytical Modelling, KPI Development, Corporate Management Reporting</td>
        </tr>
        <tr style="background-color: #F8FAFC; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">2</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Data Quality & Reconciliation</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0;">Excel, Power Query, SQL, Python</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0;">Record Completeness, Duplicate Tracking, Gaps Validation</td>
          <td style="padding: 14px 12px; font-weight: 500;">Cross-Source Record Matching, Dataset Cleaning, Exception Reporting</td>
        </tr>
        <tr style="background-color: #FFFFFF; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">3</td>
                    <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Employee Survey Analytics</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Excel, Power BI, Python, R</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Engagement Score, Response Rates, Variable Correlations</td>
          <td style="padding: 14px 12px; font-weight: 500;">Inferential Statistics, Survey Array Processing, Evidence-Based Insights</td>
        </tr>
        <tr style="background-color: #F8FAFC; border-bottom: 0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">4</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Customer & Commercial Analytics</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Excel, SQL, Python, Power BI, scikit-learn</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Purchasing Patterns, CLV, Predictive Churn Probability</td>
          <td style="padding: 14px 12px; font-weight: 500;">Customer Behavior Segmentation, Supervised ML, Business Intelligence Support</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<!-- ================================================ -->
<!-- 6. EXPERIENCE CARD                               -->
<!-- ================================================ -->
<div id="experience" class="content-card">
  <h2> Experience</h2>
  <h3 style="margin-top: 0 !important;">Professional Experience</h3>
  <p style="line-height: 1.45; font-size: 15.5px; color: #1A1D20; margin-bottom: 25px;">My consulting track spans data engineering, workforce analytics, research operations, and quantitative biostatistics across research, corporate, and international development environments.</p>

  <h3> Data Analyst - Infotrak Research & Consulting</h3>
  <span class="job-meta">Active Engagement Track - (2026)</span>
  <ul>
    <li>Managing research, survey, and commercial business data pipelines across end-to-end data management, data validation, inferential statistical testing, and executive reporting.</li>
    <li>Automating the transformation of massive raw field research tracking arrays into high-integrity, decision-ready information assets for strategic stakeholders.</li>
  </ul>

  <h3> Workforce & Data Analyst - Calltronix Kenya Ltd</h3>
  <span class="job-meta">Corporate Operations Track - (2024–2025)</span>
  <ul>
    <li>Analysed and reconciled cross-functional workforce, HR, finance, and system operations data to audit productivity, validate incentive parameters, and support payroll processing for 350+ FTE.</li>
    <li>Integrated multiple disjointed operational data platforms to eliminate tracking variances and generate automated performance dashboards for leadership.</li>
  </ul>

  <h3> Data & Research Analyst - Hamasisha Africa</h3>
  <span class="job-meta">Research Systems Analyst Track - (2025)</span>
  <ul>
    <li>Supported quantitative project research through data preparation, multi-variable statistical analysis, narrative interpretation, and stakeholder reporting, directly enabling evidence-based funding deployments.</li>
  </ul>

  <h3> Research, MEAL & Data Assignments - Various Projects</h3>
  <span class="job-meta">Independent Field Consultations Track</span>
  <ul>
    <li>Undertook specialized contract assignments involving quantitative data capture monitoring, digital questionnaire skip-logic engineering, descriptive summaries, and field-based information management.</li>
  </ul>

  
  <p style="margin-top: 25px; font-weight: bold; color: #1A488E;"> Primary Specialty Fields: Data Analytics | Statistics | Business Intelligence | Data Management | Research Analytics | Workforce Analytics</p>
</div>


<!-- ================================================ -->
<!-- 7. EDUCATION CARD                                -->
<!-- ================================================ -->
<div id="education" class="content-card">
  <h2> Education</h2>
  
  <h3> Master of Science in Data Science</h3>
  <span class="job-meta">Open University of Kenya - (Ongoing / In Progress)</span>
  <p style="line-height: 1.5; font-size: 15px; color: #1A1D20; font-weight: 500; margin-bottom: 20px; background: rgba(255,255,255,0.4); padding: 15px; border-radius: 6px;">
    <b> Advanced Graduate Competencies:</b> Active development of advanced capabilities in predictive analytics, computational machine learning algorithms, big data engineering, data warehousing architecture, cloud-based data science pipelines, and senior-level data governance frameworks.
  </p>
  
  <h3> Bachelor of Science in Biostatistics</h3>
  <span class="job-meta">Jomo Kenyatta University of Agriculture and Technology (JKUAT) - (2022 | Second Class Upper Division)</span>
  <p style="line-height: 1.5; font-size: 15px; color: #1A1D20; font-weight: 500; background: rgba(255,255,255,0.4); padding: 15px; border-radius: 6px;">
    <b> Core Academic Competencies Mastered:</b> Advanced training in biostatistics, mathematical modeling, inferential quantitative methods, research design methodology, regression diagnostics, and relational data analysis.
  </p>
</div>

<!-- ================================================ -->
<!-- 8. CERTIFICATIONS CARD                           -->
<!-- ================================================ -->
<div id="certifications" class="content-card">
  <h2> Certifications & Professional Development</h2>
  <ul>
    
    <li><span class="skill-title">IBM Data Science & AI Professional:</span> Validated industry training in data science operations, machine learning classification, predictive algorithms, and Python data analysis workflows.</li>
    <li><span class="skill-title">MEAL Essentials Professional Certificate (DisasterReady / Humanitarian Leadership Academy):</span> Specialized global certification in Monitoring, Evaluation, Accountability, and Learning systems.</li>
  </ul>
  
  <div style="background-color: rgba(23, 27, 28, 0.05); padding: 15px; border-radius: 6px; margin-top: 20px; border-left: 4px solid #1A488E;">
    <h4 style="margin: 0 0 5px 0; color: #23272A; font-weight: bold;"> Continuous Capabilities Integration</h4>
    <p style="margin: 0; font-size: 14px; color: #1A488E; font-weight: bold;">Data Analytics | Statistics | Business Intelligence | Data Science | Research Analytics</p>
  </div>
</div>

<!-- ================================================ -->
<!-- 9. GET IN TOUCH CARD                             -->
<!-- ================================================ -->
<div id="get-in-touch" class="content-card" style="background-color: #FFFFFF !important; color: #23272A !important; padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; margin: 0;">
    
    <div style="flex: 1; min-width: 320px; box-sizing: border-box; padding: 0 !important; margin: 0 !important;">
      <span style="color: #1A488E; font-weight: bold; text-transform: uppercase; font-size: 13px; letter-spacing: 0.5px; display: block; margin-bottom: 5px; text-align: left !important;">Get in touch</span>
      <h2 style="color: #23272A !important; font-size: 36px !important; font-weight: 900 !important; border: none !important; margin: 0 0 15px 0 !important; padding: 0 !important; text-transform: none !important; display: block !important; text-align: left !important;">Let's Work With Data</h2>
      <p style="line-height: 1.5; font-size: 16px; color: #4A5568 !important; margin-bottom: 20px; text-align: left !important;">Do you have an enterprise data management, business intelligence dashboard, or quantitative research analysis challenge?</p>
      <p style="line-height: 1.5; font-size: 15px; color: #4A5568 !important; margin-bottom: 25px; text-align: left !important;">I am open to consulting engagements, project-based assignments, and corporate team positions involving data analytics, statistics, business intelligence, data management, research analytics, and workforce analysis. Whether you need support trouble-shooting a messy database, automating your executive KPI tracking metrics, or turning field research data into decision-ready insights, I am interested in discussing your operational goals.</p>
    </div>
    
    <div style="flex: 1.2; min-width: 360px; background-color: #FFFFFF; border: 1px solid #E2E8F0; padding: 45px 35px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); box-sizing: border-box; margin: 0 !important; display: flex; flex-direction: column; justify-content: center; text-align: center !important;">
      <div style="border: 2px dashed #CBD5E0; border-radius: 8px; padding: 25px; background-color: #F8FAFC; text-align: center !important; width: 100%; box-sizing: border-box;">
        <span style="font-size: 40px; display: block; margin-bottom: 10px; text-align: center !important;">📧</span>
        <h4 style="margin: 0 0 8px 0; font-size: 18px; font-weight: bold; color: #23272A; text-align: center !important;">Launch Project Inquiry</h4>
        <p style="margin: 0 0 20px 0; font-size: 15px; font-weight: bold; color: #1A488E; text-align: center !important;">hednaogutuh@gmail.com</p>
        <p style="margin: 0 0 25px 0; font-size: 14px; line-height: 1.45; color: #4A5568; text-align: center !important;">Click below to automatically generate an explicit analytics project proposal brief directly inside your default mail app securely.</p>
        <a href="mailto:hednaogutuh@://gmail.com" style="background-color: #1A488E !important; color: #FFFFFF !important; padding: 15px 30px !important; border-radius: 6px; font-weight: bold; text-decoration: none; font-size: 14px; display: inline-block; box-shadow: 0 4px 10px rgba(26,72,142,0.2); text-transform: uppercase; letter-spacing: 0.5px; text-align: center !important;">✉️ Submit Proposal Brief</a>
      </div>
    </div>
    
  </div>
</div>

</div> <!-- Closes scroll-content layout engine -->
</div> <!-- Closes portfolio-container outer window -->




