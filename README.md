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



  /* Fluid Scrolling Content Layer Layout - Calibrated to tighten the top gap metrics */
  .scroll-content {
    margin-top: 72px !important; /* Draws your blue cards up up beautifully underneath the bar */
    padding: 10px 0 75px 0 !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
    min-height: calc(100vh - 180px) !important; 
  }
    
    /* THE SMART CUSHION BUFFER: Keeps short tabs open wide enough to cleanly reveal your footer bar layout */
    min-height: calc(100vh - 220px) !important; 
  }

    /* Content Cards Layout Parameters */
  .content-card {
    background-color: #97B2DE !important; 
    padding: 35px 45px !important; 
    border-radius: 8px; 
    margin-left: 20px !important; 
    margin-right: 20px !important; 
    margin-top: 0 !important; /* Forces cards flush to eliminate whitespace gaps */
    margin-bottom: 0 !important; 
    box-shadow: 0 4px 12px rgba(0,0,0,0.1) !important;
    position: relative;
    overflow: hidden;
    scroll-margin-top: 100px !important; 
    width: calc(100% - 40px) !important; 
    max-width: calc(100% - 40px) !important; 
    box-sizing: border-box !important;
    display: none !important; 
    overflow-y: visible !important;
    z-index: 100 !important; 
  }
  /* THE PURE CSS INTERACTIVE ENGINE RULES: Connects nav buttons to view cards */
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

  /* Background Grid Graphical Canvas Elements */
  .skills-bg-card {
    background: linear-gradient(rgba(151, 178, 222, 0.94), rgba(151, 178, 222, 0.94)), 
                url('https://dreamstime.com') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* Typography metrics controllers */
  .content-card > h2:first-child, .content-card > div:first-child { margin-top: 0 !important; padding-top: 0 !important; }
  h2 { color: #23272A !important; font-size: 26px; font-weight: 900; margin: 0 0 20px 0 !important; padding-bottom: 10px; border-bottom: 4px solid #23272A; text-transform: uppercase; letter-spacing: 1px; display: block !important; }
  h3 { color: #111314 !important; font-size: 21px; font-weight: 900; margin-top: 22px !important; margin-bottom: 6px !important; padding-top: 0 !important; display: block !important; }
  h2 + h3, .content-card > h3:first-of-type { margin-top: 5px !important; }
  .job-meta { color: #23272A !important; font-style: normal; font-size: 15px; margin-top: 0 !important; margin-bottom: 14px !important; display: block; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px; }

  ul { padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 2px !important; }
  li { margin-top: 0 !important; margin-bottom: 4px !important; line-height: 1.35 !important; color: #1A1D20 !important; font-size: 16px; font-weight: 500; } 
  p { margin-top: 0 !important; margin-bottom: 8px !important; line-height: 1.35 !important; }
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
    <label for="tab-home">🏠 HOME</label>
    <label for="tab-about">👤 ABOUT</label>
    <label for="tab-services">💼 SERVICES</label>
    <label for="tab-projects">📊 PROJECTS</label>
    <label for="tab-portfolio">📈 PORTFOLIO</label>
    <label for="tab-experience">💼 EXPERIENCE</label>
    <label for="tab-education">🎓 EDUCATION</label>
    <label for="tab-certifications">🏆 CERTIFICATIONS</label>
    <label for="tab-get-in-touch">📞 GET IN TOUCH</label>
  </div>
</div>
<!-- FIXED EDGE-TO-EDGE BOTTOM FROZEN FOOTER BAR -->
<div class="fixed-footer-container">
  <div class="footer-bar">
    <p>📍 <span class="footer-highlight">Nairobi, Kenya</span> | 💬 <a href="https://whatsapp.com" target="_blank">WhatsApp: +254 741 937074</a></p>
    <p>💼 <a href="https://linkedin.com" target="_blank">Connect on LinkedIn</a></p>
  </div>
</div>

<div class="scroll-content">

<div class="scroll-content">


<!-- ================================================ -->
<!-- 1. HOME CARD                                     -->
<!-- ================================================ -->
<div id="home" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
   <!-- LEFT PANEL: UNBLOCKABLE SECURE PORTRAIT CONTAINER WITH RECENT CORRECT LINK -->
<div style="flex: 0.8; min-width: 260px; max-width: 320px; box-sizing: border-box; margin: 0 auto !important;">
  <img width="800" height="800" alt="Edna Profile Picture" src="data.png" style="width: 100% !important; height: auto !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
</div>

    
    <!-- RIGHT PANEL: HOME BRIEF CONTENT -->
    <div style="flex: 1.5; min-width: 340px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 20px 0 !important; padding-bottom: 10px !important; text-transform: uppercase !important; display: block !important;">🏠 Welcome</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Edna Achieng Ogutu</p>
      <p style="font-size: 18px; color: #1A488E; font-weight: 700; margin-bottom: 15px;">Statistician | Data Analyst | Business Intelligence | Data Science</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 15px;">Turning data into reliable insights and better decisions.</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 20px;">I am a Statistician and Data Analyst with a background in Biostatistics and experience working with workforce, research, operational, survey and business data. I combine data management, statistical analysis and business intelligence to transform data into reliable information, meaningful insights and decision-ready reporting.</p>
      
      <p style="margin-top: 25px; font-weight: bold; font-size: 15px;">👉 Explore My Portfolio: <label for="tab-projects" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">View Projects</label> | <label for="tab-services" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Explore Services</label> | <label for="tab-get-in-touch" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Get in Touch</label></p>
    </div>
    
  </div>
</div>



<!-- ================================================ -->
<!-- 2. ABOUT CARD                                    -->
<!-- ================================================ -->
<div id="about" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
   <!-- LEFT PANEL: UNBLOCKABLE SECURE PORTRAIT CONTAINER WITH RECENT CORRECT LINK -->
<div style="flex: 0.8; min-width: 260px; max-width: 320px; box-sizing: border-box; margin: 0 auto !important;">
  <img width="800" height="800" alt="Edna Profile Picture" src="Edna Profile Picture.png" style="width: 100% !important; height: auto !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
</div>

    
    <!-- RIGHT PANEL: ABOUT & VALUE PROPOSITION CONTENT -->
    <div style="flex: 1.5; min-width: 340px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 20px 0 !important; padding-bottom: 10px !important; text-transform: uppercase !important; display: block !important;">👤 About Me</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">I am a Statistician and Data Analyst focused on transforming data into reliable, understandable and useful insights.</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 15px;">My work combines data management, statistical analysis, business intelligence and research analytics. I work across the analytical process—from preparing and validating data to analysing, visualising and communicating results.</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: 500; margin-bottom: 20px;">I believe effective analytics starts with reliable data. My approach is therefore centred on understanding the data, asking the right questions and producing outputs that are both technically sound and useful to decision-makers.</p>
      
      <h3 style="margin-top: 22px !important; margin-bottom: 6px !important; font-size: 21px; font-weight: 900; color: #111314 !important;">🎯 Core Areas</h3>
      <ul style="padding-left: 25px !important; margin-top: 2px !important; margin-bottom: 15px !important;">
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Data Analytics:</span> Exploratory analysis, KPI development, trends and performance analysis.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Data Management:</span> Data cleaning, validation, reconciliation and preparation.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Statistics:</span> Descriptive and inferential analysis, statistical testing and modelling.</li>
        <li style="margin-bottom: 4px !important; line-height: 1.35 !important; font-size: 16px;"><span class="skill-title">Business Intelligence:</span> Dashboards, visualisation and management reporting.</li>
      </ul>
      <p style="font-size: 15px; color: #1A488E; font-weight: bold; margin: 0;">🧰 Tools: Excel | Power Query | Power BI | DAX | SQL | Python | R | STATA | SPSS</p>
    </div>
    
  </div>
</div>


<!-- ================================================ -->
<!-- 3. SERVICES CARD                                 -->
<!-- ================================================ -->
<div id="services" class="content-card skills-bg-card">
  <h2>💼 What I Do</h2>
  <ul>
    <li><span class="skill-title">Data Analytics:</span> Transforming structured data into meaningful insights, trends and performance indicators.</li>
    <li><span class="skill-title">Data Management & Quality:</span> Cleaning, validating, reconciling and preparing data for reliable analysis and reporting.</li>
    <li><span class="skill-title">Business Intelligence:</span> Developing interactive dashboards, KPI reports and data visualisations for decision support.</li>
    <li><span class="skill-title">Statistical & Research Analytics:</span> Applying statistical methods to quantitative, survey and research data to generate evidence-based insights.</li>
    <li><span class="skill-title">Advanced Analytics:</span> Customer segmentation, predictive modelling and other advanced analytical approaches.</li>
  </ul>
  <p style="margin-top: 20px; font-weight: bold;"><label for="tab-projects" style="color: #23272A; cursor: pointer; text-decoration: underline;">View My Projects →</label></p>
</div>

<!-- ================================================ -->
<!-- 4. PROJECTS CARD                                 -->
<!-- ================================================ -->
<div id="projects" class="content-card">
  <h2>📊 Selected Projects</h2>
  <p style="margin-bottom: 25px;">A selection of analytical projects demonstrating my capabilities across data management, business intelligence, statistics and advanced analytics. Expand below to read project frameworks:</p>

  <!-- PROJECT 1 -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;">💼 1. Workforce & HR Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      <p><b>📝 Synopsis:</b> Developed an interactive workforce analytics solution to transform structured employee data into management-ready insights on workforce composition, departmental distribution, salary patterns, employee performance, workforce trends and attrition. The project demonstrates practical application of data preparation, analytical modelling, KPI development and interactive visualisation to support workforce monitoring and management reporting.</p>
      <p><b>🔍 Analytical Focus:</b> Workforce composition and distribution | Department and role analysis | Salary and compensation patterns | Employee performance | Workforce trends | Attrition and workforce stability</p>
      <p><b>⚙️ Tools Stack:</b> Excel | Power Query | Power BI | DAX | Statistical Analysis</p>
      <p><b>🖥️ Key Output:</b> Interactive Power BI workforce dashboard with filtering and drill-down capabilities.</p>
      <p><b>📈 Analytical Value:</b> Provides a consolidated view of workforce characteristics and trends to support workforce monitoring, management reporting and identification of areas requiring further analysis.</p>
    </div>
  </details>

  <!-- PROJECT 2 -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;">🧽 2. Data Quality & Reconciliation</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      <p><b>📝 Synopsis:</b> Developed a data quality and reconciliation solution to combine information from multiple sources, identify inconsistencies, validate records and prepare reliable datasets for reporting and analysis. The project demonstrates practical application of data cleaning, transformation, matching and validation techniques when working with incomplete, duplicated and inconsistent information.</p>
      <p><b>🔍 Analytical Focus:</b> Data completeness and consistency | Duplicate and missing-record identification | Cross-source record matching | Data validation and reconciliation | Standardisation and transformation | Data quality assessment</p>
      <p><b>⚙️ Tools Stack:</b> Excel | Power Query | SQL | Python | Statistical Analysis</p>
      <p><b>🖥️ Key Output:</b> A validated and reconciled analytical dataset supported by data-quality checks and exception reporting.</p>
      <p><b>📈 Analytical Value:</b> Improves the reliability and usability of data by identifying and resolving quality issues before information is used for reporting, analysis or decision-making.</p>
    </div>
  </details>

  <!-- PROJECT 3 -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 20px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;">📊 3. Employee Engagement & Statistical Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      <p><b>🎯 Synopsis:</b> Developed an employee survey analytics solution to examine engagement patterns, response behaviour and relationships across key employee characteristics. The project demonstrates the application of statistical analysis, survey analytics and data visualisation to transform quantitative survey data into interpretable evidence and actionable insights.</p>
      <p><b>🔍 Analytical Focus:</b> Employee engagement patterns | Survey response analysis | Engagement across employee groups | Relationships between key variables | Descriptive and inferential statistics | Statistical interpretation and visualisation</p>
      <p><b>🛠️ Tools:</b> Excel | Power Query | Power BI | Python/R | Statistical Analysis</p>
      <p><b>🖥️ Key Output:</b> Interactive employee engagement dashboard supported by statistical analysis of survey responses and key employee characteristics.</p>
      <p><b>📈 Analytical Value:</b> Provides a structured view of employee engagement patterns and statistical relationships to support evidence-based workforce analysis and identify areas requiring further investigation.</p>
    </div>
  </details>

  <!-- PROJECT 4 -->
  <details style="background-color: #F8FAFC; padding: 20px 25px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 0px;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase;">📊 4. Customer & Commercial Predictive Analytics</summary>
    <div style="margin-top: 15px; padding-left: 10px;">
      <p><b>🎯 Synopsis:</b> Developed an end-to-end customer and commercial analytics solution to examine customer behaviour, commercial performance and customer segments while applying predictive analytical techniques. The project demonstrates progression from descriptive and diagnostic analysis to segmentation and predictive modelling using structured business data.</p>
      <p><b>🔍 Analytical Focus:</b> Customer behaviour and purchasing patterns | Sales and commercial performance | Customer segmentation | Customer value and retention patterns | Predictive modelling | Model evaluation and interpretation</p>
      <p><b>🛠️ Tools:</b> Excel | SQL | Python | Power BI | scikit-learn</p>
      <p><b>🖥️ Key Output:</b> Interactive commercial analytics dashboard supported by customer segmentation and predictive modelling outputs.</p>
      <p><b>📈 Analytical Value:</b> Combines business intelligence and advanced analytics to identify customer patterns, segment customers and generate evidence that can support commercial analysis and customer-focused decision-making.</p>
    </div>
  </details>
</div> <!-- Closes the master projects card wrapper safely -->

<!-- ================================================ -->
<!-- 5. PORTFOLIO CARD                                -->
<!-- ================================================ -->
<div id="portfolio-hub" class="content-card">
  <h2>📈 Enterprise Portfolio Directory</h2>
  <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; margin-bottom: 25px;">A metric tracking directory summarizing alignment profiles and operational capability targets for my core data modules:</p>
  
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
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Excel, Power Query, Power BI, DAX</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Headcount, Department Distribution, Attrition Rate</td>
          <td style="padding: 14px 12px; font-weight: 500;">Analytical Modelling, KPI Development, Corporate Management Reporting</td>
        </tr>
        <tr style="background-color: #F8FAFC; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">2</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Data Quality & Reconciliation</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Excel, Power Query, SQL, Python</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Record Completeness, Duplicate Tracking, Gaps Validation</td>
          <td style="padding: 14px 12px; font-weight: 500;">Cross-Source Record Matching, Dataset Cleaning, Exception Reporting</td>
        </tr>
        <tr style="background-color: #FFFFFF; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 14px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">3</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Employee Survey Analytics</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Excel, Power BI, Python, R</td>
          <td style="padding: 14px 12px; border-right: 1px solid #E2E8F0; color: #2D3748;">Engagement Score, Response Rates, Variable Correlations</td>
          <td style="padding: 14px 12px; font-weight: 500;">Inferential Statistics, Survey Array Processing, Evidence-Based Insights</td>
        </tr>
        <tr style="background-color: #F8FAFC; border-bottom: 1px solid #E2E8F0;">
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
  <h2>💼 Experience</h2>
  <h3 style="margin-top: 0 !important;">Professional Experience</h3>
  <p style="line-height: 1.45; font-size: 15.5px; color: #1A1D20; margin-bottom: 25px;">My experience spans data analytics, workforce analytics, research, data management and quantitative analysis across research, business and development-focused environments.</p>

  <h3>📍 Data Analyst — Infotrak Research & Consulting</h3>
  <span class="job-meta">Active Engagement — (2026)</span>
  <ul>
    <li>Working with research and business data across data management, validation, statistical analysis, reporting and analytical outputs.</li>
    <li>Supporting the transformation of raw data into reliable information for research and decision-making.</li>
  </ul>

  <h3>📍 Workforce & Data Analyst — Calltronix Kenya Ltd</h3>
  <span class="job-meta">Corporate Operations — (2024–2025)</span>
  <ul>
    <li>Analysed workforce, HR, finance and operational data to support employee management, payroll validation, productivity analysis and reporting.</li>
    <li>Worked across multiple operational data sources to reconcile information and produce reliable analytical outputs.</li>
  </ul>

  <h3>📍 Data & Research Analyst — Hamasisha Africa</h3>
  <span class="job-meta">Research Systems Analyst Track — (2025)</span>
  <ul>
    <li>Supported quantitative research through data preparation, analysis, interpretation and reporting, contributing to evidence generation and research-related decision-making.</li>
  </ul>

   <h3>📍 Research, MEAL & Data Assignments — Various Projects</h3>
  <span class="job-meta">Independent Field Consultations Track</span>
  <ul>
    <li>Undertook research, monitoring, evaluation and data-related assignments involving quantitative data collection, data quality, analysis, reporting and field-based information management.</li>
  </ul>
  
  <p style="margin-top: 25px; font-weight: bold; color: #1A488E;">🎯 Professional Focus Track: Data Analytics | Statistics | Business Intelligence | Data Management | Research Analytics | Workforce Analytics</p>
</div>

<!-- ================================================ -->
<!-- 7. EDUCATION CARD                                -->
<!-- ================================================ -->
<div id="education" class="content-card">
  <h2>🎓 Education</h2>
  
  <h3>📍 Master of Science in Data Science</h3>
  <span class="job-meta">Open University of Kenya — (Ongoing)</span>
  
  <h3>📍 BSc Biostatistics</h3>
  <span class="job-meta">Jomo Kenyatta University of Agriculture and Technology (JKUAT) — (2022 | Second Class Upper)</span>
  
  <p style="line-height: 1.5; font-size: 15px; color: #1A1D20; font-weight: 500; margin-top: 15px; background: rgba(255,255,255,0.4); padding: 15px; border-radius: 6px;"><b>📚 Academic Foundation Matrix:</b> Academic foundation in biostatistics, statistical analysis, quantitative methods, research methodology and data analysis.</p>
</div>

<!-- ================================================ -->
<!-- 8. CERTIFICATIONS CARD                           -->
<!-- ================================================ -->
<div id="certifications" class="content-card">
  <h2>🏆 Certifications & Professional Development</h2>
  <ul>
    <li><span class="skill-title">IBM Data Science & AI:</span> Training in data science and AI-related analytical concepts and practical data workflows.</li>
    <li><span class="skill-title">MEAL Essentials Professional Certificate:</span> Professional development in Monitoring, Evaluation, Accountability and Learning.</li>
  </ul>
  
  <div style="background-color: rgba(23, 27, 28, 0.05); padding: 15px; border-radius: 6px; margin-top: 20px; border-left: 4px solid #1A488E;">
    <h4 style="margin: 0 0 5px 0; color: #23272A; font-weight: bold;">🔄 Continuous Learning Track Focus</h4>
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
      <p style="line-height: 1.5; font-size: 16px; color: #4A5568 !important; margin-bottom: 20px; text-align: left !important;">Have a data, analytics or research problem?</p>
      <p style="line-height: 1.5; font-size: 15px; color: #4A5568 !important; margin-bottom: 25px; text-align: left !important;">I am open to opportunities involving data analytics, statistics, business intelligence, data management, research analytics and quantitative analysis.</p>
      <p style="line-height: 1.5; font-size: 15px; color: #4A5568 !important; margin-bottom: 30px; text-align: left !important;">Whether you are looking for analytical support, a data professional to join your team, or help turning data into useful insights, I would be interested in discussing the opportunity.</p>
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


