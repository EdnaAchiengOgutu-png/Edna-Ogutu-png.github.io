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


<!-- 3. PROJECTS SHOWCASE CARD - EXECUTIVE PORTFOLIO SYNOPSIS HUB -->
<div id="projects" class="content-card">
  <h2>📊 Strategic Projects Portfolio</h2>
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; margin-bottom: 25px;">Select an enterprise solutions tracking system from the index directory rows below to expand its high-level business objective, specialized tool-stack framework, and strategic data value:</p>

  <!-- PROJECT 1: WORKFORCE ANALYTICS -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">💼 Project 1: Enterprise Workforce & HR Analytics System</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Fragmented, desktop-siloed employee logs and shift registers prevented real-time tracking of escalating workforce fulfillment gaps and unmonitored early attrition trends across 350+ FTE.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Engineered a unified Star Schema data model inside <b>Advanced Excel (Power Query)</b> and <b>Power BI (DAX)</b> to isolate moving Headcount, cohort Attrition rates, and department Absenteeism loss metrics.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Enabled leadership teams to shift raw budget parameters away from high-churn operational channels into proactive milestone retention incentives, cutting localized turnover risk profiles.</p>
    </div>
  </details>

  <!-- PROJECT 2: EMPLOYEE ENGAGEMENT SURVEY -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">📊 Project 2: Employee Engagement Survey Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Administrative delays in compiling annual manual survey text feedback left executive teams blind to shifting company culture scores and growing team dissatisfaction trends across off-peak branches.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Unpivoted multi-layered question fields using <b>Power BI ETL</b> to script interactive dashboards tracking Employee Net Promoter Scores (eNPS) and cross-filtering Likert-scale sentiment parameters.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Isolated a severe 22% drop in organizational engagement metrics inside nighttime operations blocks, driving targeted facility benefit restructures that recovered team retention by 12%.</p>
    </div>
  </details>

  <!-- PROJECT 3: DATA QUALITY & RECONCILIATION -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🔍 Project 3: Data Quality & Reconciliation Analysis</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Biometric entry omissions, text mismatching string errors, and transaction record inconsistencies created severe data variances that distorted quarterly payroll ledger audits.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Architected backend cross-system data quality verification engines in <b>Python (pandas)</b> and relational <b>SQL</b> to monitor automated Validation Pass Rates and database Duplication frequencies.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Exposed a critical 4.2% data leak trail caused by misaligned shift calendar ID overrides, permanently standardizing administrative master data governance channels.</p>
    </div>
  </details>

  <!-- PROJECT 4: SALES & COMMERCIAL ANALYTICS -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">💰 Project 4: Sales & Commercial Analytics System</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Samped multi-branch POS receipts and promotional markdown records lacked unified tracking, leaving executives without granular profit leakage visibility across geographic trade sectors.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Scripted optimized multi-table data pipelines in <b>SQL relational queries</b> and <b>Power BI</b> to track Gross Profit Margins %, Average Order Values, and dynamic Customer Contribution variables.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Isolated an 11% margin slippage in regional logistics routes, enabling the immediate removal of low-yielding stock units to maximize core retail revenue channels.</p>
    </div>
  </details>

  <!-- PROJECT 5: STATISTICAL MODELING -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">📈 Project 5: Statistical Analysis & Modelling Track</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Program evaluation networks relied exclusively on raw descriptive means to report project trajectories, failing to validate whether treatment outcomes were statistically significant for donor verification.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Programmed reproducible quantitative scripts using <b>R Programming</b> and <b>Python (scipy.stats)</b> to map Model Fit Diagnostics (R²), regression coefficients, and hypothesis test boundaries.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Formulated empirical proof confirming a 18.5% net programmatic indicator improvement over baseline tracks, unblocking secondary capital funding expansion extensions.</p>
    </div>
  </details>

  <!-- PROJECT 6: CUSTOMER SEGMENTATION -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">👥 Project 6: Customer Segmentation & Analytics Engine</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Inefficient marketing ad spend allocations and dropping purchase frequencies occurred because diverse consumer cohorts were lumped into unsegmented baseline customer databases.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Formulated advanced <b>SQL windowing operations</b> and <b>Power BI</b> clustering logic to construct an automated RFM matrix mapping Recency, Frequency, Monetary data values, and Customer Lifetime Value (CLV).</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Proved that a core 14% group of "Champions" generated 52% of total transaction revenue, enabling personalized loyalty campaigns while establishing early win-back churn alerts.</p>
    </div>
  </details>

  <!-- PROJECT 7: PREDICTIVE ANALYTICS -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🤖 Project 7: Predictive Analytics / Machine Learning Framework</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Reactive corporate account management models struggled to identify churning client profiles early enough to deploy retention offers, ballooning customer acquisition costs.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Engineered a supervised machine learning classification model using <b>Python (scikit-learn)</b> and Jupyter notebooks to calculate Feature Importance weightings, ROC-AUC curve tracks, and F1-scores.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Achieved a high-precision 0.89 model classification score, feeding proactive user data indicators straight to customer success squads to resolve accounts at risk.</p>
    </div>
  </details>

 <!-- PROJECT 8: FINANCIAL TRACKER -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 0px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px;">🏦 Project 8: Banking & Financial Analytics Asset Tracker</summary>
    <div style="margin-top: 15px; padding-left: 10px; line-height: 1.5; font-size: 14.5px; color: #2D3748;">
      <p><b>🎯 Business Problem & Objective:</b> Credit underwriting and asset teams lacked interactive, unified dashboard accounting to monitor high-frequency outstanding volumes, portfolio values, and active loan default scales.</p>
      <p><b>🛠️ Tools & KPI Framework Deployed:</b> Scripted financial measure code strings leveraging <b>Advanced Excel models</b> and relational <b>SQL server views</b> to map Non-Performing Loans (NPL) ratios and asset volume trajectories.</p>
      <p><b>🏆 Strategic Business Value Proven:</b> Flagged an unmonitored default trend in an unsecured loan category early, enabling credit managers to recalibrate pricing thresholds and secure core banking margins.</p>
    </div>
  </details>
  
  <p style="font-size: 14px; font-style: italic; color: #23272A; margin: 20px 0 0 0; font-weight: 500;">📌 Note: Technical file layers, proprietary algorithms, and raw database schema logic are omitted to protect client data rights. Full system reproducibility assets are reviewed upon proposal contract screen verification.</p>
</div> <!-- Closes the master projects card wrapper safely -->



















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

