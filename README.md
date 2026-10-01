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

 /* Main Profile Block Header Content Box - Edge-to-edge width, minimized vertical height */
.header-block { 
  background-color: #23272A !important; 
  color: #FFFFFF !important; 
  padding: 4px 20px !important; /* Cut top/bottom padding in half (from 8px to 4px) */
  border-radius: 0 !important; 
  margin: 0 !important; 
  border-left: 8px solid #FFD200;
  border-top: 3px solid #FFD200 !important; /* Slightly thinner top border to match the compact look */
  box-shadow: 0 4px 10px rgba(0,0,0,0.15);
  width: 100% !important; /* Keeps it stretching fully to the edges of the screen */
  height: auto !important; /* Allows it to shrink down completely to fit just the text */
  line-height: 1.2 !important; /* Tightens the spacing of the text inside */
  box-sizing: border-box !important;

  }
  .header-block h1 { color: #FFFFFF !important; margin: 0 !important; font-size: 26px; font-weight: 900; display: block !important; width: 100%; text-align: left; } 

/* Navigation Ribbon Strip - Tightened padding for a compact look */
.navbar { 
  background-color: #23272A !important; 
  padding: 0px 40px !important; /* Tightened vertical padding to make it slim */
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
    margin-right: 14px; 
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
    margin-top: 80px !important; 
    padding: 8px 0 65px 0 !important; 
    box-sizing: border-box !important;
    width: 100% !important;
    max-width: 100% !important;
    display: block !important;
    min-height: calc(100vh - 140px) !important; 
  }


 /* Content Cards Layout Parameters - Text top-aligned via tightened internal padding */
  .content-card {
    background-color: #D2F7FF !important; 
    padding: 5px 45px 5px 45px !important; 
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
  /* PURE CSS TAB SWITCH ENGINE RULES: Connects button selectors to views */
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
    <h1>Edna Ogutu | Consultant</h1>
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
<div id="home" class="content-card" style="padding: 20px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 20px; width: 100%; box-sizing: border-box; align-items: flex-start;">
    
    <!-- LEFT PANEL: DATA GRAPHIC CANVAS CONTAINER (COMPACT FRAME SCALE) -->
    <div style="flex: 0.5; min-width: 180px; max-width: 280px; box-sizing: border-box; margin: 0 auto !important;">
      <img width="800" height="800" alt="Edna Profile Picture" src="Edna Profile Picture.png" style="width: 100% !important; height: 100% !important; aspect-ratio: 1 / 1 !important; object-fit: cover !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
    </div>
    
    <!-- RIGHT PANEL: NAME & HEADLINES (VERTICALLY CENTERED WITH TIGHT RESOLVED WIDTH) -->
    <div style="flex: 1.8; min-width: 300px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; align-self: center !important; text-align: left !important;">
      <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 12px 0 !important; padding-bottom: 6px !important; text-transform: uppercase !important; display: block !important;"> Home</h2>
      <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">Edna Ogutu</p>
      <p style="font-size: 18px; color: #1A488E; font-weight: 700; margin-bottom: 15px;">Statistician | Data Analyst | Business Intelligence | Data Science | Workforce Analytics</p>
      <p style="line-height: 1.45; font-size: 16px; color: #1A1D20; font-weight: bold; margin-bottom: 0;">I engineer robust data pipelines, statistical frameworks, and automated dashboards that eliminate operational reporting blind spots, protect corporate budgets, and drive decision-ready intelligence.</p>
    </div>
    
  </div>

  <!-- TEXT BLOCK AUTOMATICALLY FLOWING ENTIRELY BELOW THE IMAGE ROW -->
  <div style="width: 100%; box-sizing: border-box; text-align: left !important; margin-top: 25px !important;">
    <p style="line-height: 1.45; font-size: 15.5px; color: #1A1D20; font-weight: 500; margin-bottom: 20px;">I am a Statistician and Data Analyst with a deep background in Biostatistics and experience working with workforce tracking metrics, research diagnostics, operational flows, survey matrices, and commercial business data. By bridging the gap between raw data complexity and executive strategy, I combine advanced data management, descriptive and inferential statistics, and modern business intelligence to transform disorganized data streams into high-integrity information, clear operational insights, and decision-ready executive reporting.</p>
    
    <p style="margin-top: 20px; font-weight: bold; font-size: 15px; color: #23272A;"> Explore My Portfolio: <label for="tab-projects" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">View Selected Projects Frameworks</label> | <label for="tab-services" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Explore Specialized Analytics Services</label> | <label for="tab-get-in-touch" style="color: #1A488E; cursor: pointer; text-decoration: underline; font-weight: bold;">Schedule a Data Solutions Consultation Session</label></p>
  </div>

</div>

<!-- ================================================ -->
<!-- 2. ABOUT CARD                                    -->
<!-- ================================================ -->
<div id="about" class="content-card" style="padding: 20px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 20px; width: 100%; box-sizing: border-box; align-items: center !important; margin-bottom: 25px !important;">
    
    <!-- LEFT PANEL: DATA GRAPHIC CONTAINER (REDUCED TO MATCH COMPACT PORTFOLIO DESIGN) -->
    <div style="flex: 0.5; min-width: 380px; max-width: 480px; box-sizing: border-box; margin: 0 auto !important;">
      <img width="800" height="800" alt="data" src="data.png" style="width: 100% !important; height: 100% !important; aspect-ratio: 1 / 1 !important; object-fit: cover !important; border-radius: 8px; border: 3px solid #23272A; box-shadow: 0 4px 14px rgba(0,0,0,0.15); display: inline-block !important;" />
    </div>
    
  <!-- RIGHT PANEL: CONTENT & VALUE PROPOSITION (VERTICALLY RE-CENTERED) -->
<div style="flex: 1.8; min-width: 300px; box-sizing: border-box; padding: 0 !important; margin: 0 !important; align-self: center !important; text-align: left !important;">
  <h2 style="color: #23272A !important; font-size: 26px !important; font-weight: 900 !important; border-bottom: 4px solid #23272A !important; margin: 0 0 12px 0 !important; padding-bottom: 6px !important; text-transform: uppercase !important; display: block !important;"> About Me</h2>
  <p style="font-size: 24px; color: #111314; font-weight: 900; margin: 0 0 15px 0; line-height: 1.35; letter-spacing: -0.5px;">I bridge the structural gap between messy, multi-source raw data and high-stakes executive strategy.</p>
  <p style="line-height: 1.45; font-size: 16px; color: #2D3748; font-weight: 500; margin-bottom: 15px;">My approach is centered on building high-integrity validation checks at the collection source, ensuring that every predictive model, regression script, or visualization dashboard is mathematically sound, audit-ready, and immediately actionable for corporate decision-makers.</p>
  
  <!-- STRATEGIC VALUE PROPOSITION BULLET LIST -->
  <ul style="padding-left: 20px !important; margin-top: 12px !important; margin-bottom: 0 !important; list-style-type: square !important;">
    <li style="font-size: 14.5px !important; line-height: 1.5 !important; color: #1A1D20 !important; font-weight: 500; margin-bottom: 8px !important;">
      <b>End-to-End Execution:</b> Operating across the entire analytical pipeline-from executing rigorous data cleaning and cross-system reconciliations to formulating diagnostic models and interactive reporting systems.
    </li>
    <li style="font-size: 14.5px !important; line-height: 1.5 !important; color: #1A1D20 !important; font-weight: 500; margin-bottom: 8px !important;">
      <b>Strategic Transformation:</b> Transforming highly complex numbers into simple, actionable, and strategic next steps for senior leadership.
    </li>
    <li style="font-size: 14.5px !important; line-height: 1.5 !important; color: #1A1D20 !important; font-weight: 500; margin-bottom: 0 !important;">
      <b>Data-Driven Efficiencies:</b> Grounding metrics in high-integrity data quality and asking the right analytical questions to generate long-term operational efficiencies.
    </li>
  </ul>
</div>

</div> <!-- Safely closes the top horizontal flex introduction row container block -->

  <!-- LOWER SECTION: FULL WIDTH ALIGNED COMPETENCIES MATRIX GRID -->
  <div style="width: 100%; box-sizing: border-box; margin-top: 25px !important;">
    <h3 style="margin-top: 0 !important; margin-bottom: 15px !important; font-size: 20px; font-weight: 900; color: #23272A !important; border-bottom: 2px solid rgba(35,39,42,0.15); padding-bottom: 6px; text-transform: uppercase; letter-spacing: 0.5px;"> Core Execution Domains</h3>
    
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(400px, 1fr)); gap: 15px; width: 100%; box-sizing: border-box; margin-bottom: 20px;">
      
      <!-- BOX 1: DATA ANALYTICS -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 12px 16px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 1. Data Analytics & Modeling</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Designing and deploying custom corporate KPI matrix tracking frameworks.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Executing comprehensive exploratory data analysis (EDA) algorithms.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Formulating historical trend forecasting and performance trend lines.</li>
        </ul>
      </div>

      <!-- BOX 2: DATA ENGINEERING -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 12px 16px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 2. Data Engineering & Management</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Architecting automated structural cleaning and parsing routines.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Enforcing cross-source database records validation parameters.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Executing multi-tier system ledger reconciliation and preparation.</li>
        </ul>
      </div>

      <!-- BOX 3: STATISTICAL INFERENCE -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 12px 16px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 3. Statistical Inference & Research</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Applying complex descriptive summaries and inferential metrics testing.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Constructing multivariable linear and logistic regression models.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Synthesizing field diagnostic evidence for strategic decision-making.</li>
        </ul>
      </div>

         <!-- BOX 4: BUSINESS INTELLIGENCE (NESTED CORRECTLY INSIDE THE CORE DOMAINS PARENT ROW) -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 12px 16px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 4. Business Intelligence Systems</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Engineering interactive, responsive Power BI business dashboards.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Formulating corporate cross-filtering visual performance matrix maps.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Generating automated executive management reporting frameworks.</li>
        </ul>
      </div>

    </div> <!-- Safely closes the single parent display grid container row -->

    <!-- RE-ENGINEERED OPTIMIZED TOOLSTACK RIBBON WITH CLEAN WRAPPING & LEGIBLE CONTRAST -->
    <div style="background-color: #23272A; padding: 12px 18px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box; overflow: visible !important; margin-top: 15px !important;">
      <span style="font-size: 13.5px; color: #FFFFFF !important; font-weight: bold; letter-spacing: 0.5px; display: block; margin-bottom: 6px; text-transform: uppercase;"> Statistical Tools Mastered</span>
      <span style="font-size: 14.5px !important; color: #FFD200 !important; font-weight: 900 !important; margin: 0 !important; padding: 0 !important; line-height: 1.5 !important; word-wrap: break-word !important; white-space: normal !important; display: block !important; font-family: 'Arial', sans-serif !important;">
        Excel &nbsp;|&nbsp; Power Query &nbsp;|&nbsp; Power BI &nbsp;|&nbsp; DAX &nbsp;|&nbsp; SQL &nbsp;|&nbsp; Python &nbsp;|&nbsp; R &nbsp;|&nbsp; STATA &nbsp;|&nbsp; SPSS
      </span>
    </div>

  </div> <!-- Safely closes the internal padding card content flex framework -->
</div> <!-- Safely closes the ABOUT Content Card Wrapper container box perfectly -->

<!-- ================================================ -->
<!-- 3. SERVICES CARD                                 -->
<!-- ================================================ -->
<div id="services" class="content-card" style="padding: 17px 37px 17px 37px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 6px !important;"> Consulting Services</h2>
  <p style="margin-top: 0 !important; margin-bottom: 20px !important; font-size: 12px; font-weight: bold; color: #23272A; line-height: 1.35;">Substituting manual error with high-integrity automation to protect corporate budgets and optimize scaling loops:</p>
  
  <!-- EXECUTIVE 2-COLUMN COMMERCIAL GRID FRAMEWORK -->
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(420px, 1fr)); gap: 15px; width: 100%; box-sizing: border-box; margin-bottom: 25px; align-items: stretch !important;">
    
    <!-- SERVICE CARD 1: ENTERPRISE DATA ANALYTICS -->
    <div style="background-color: rgba(255,255,255,0.75); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 18px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); display: flex !important; flex-direction: column !important; justify-content: space-between !important;">
      <div>
        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 6px;">
          <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 3px 10px; border-radius: 4px; font-family: 'Arial', sans-serif;">01</span>
          <h3 style="margin: 0 !important; font-size: 16px !important; font-weight: 900 !important; color: #1A488E !important; text-transform: uppercase; letter-spacing: 0.3px;">Data Analytics</h3>
        </div>
        <p style="font-size: 13.5px; color: #23272A; font-weight: 700; margin-bottom: 12px; line-height: 1.45;">I engineer scalable analytics frameworks that bridge the gap between complex enterprise operations and clear corporate strategy.</p>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 6px !important;"> Commercial Insights: <span style="font-weight: 500; color: #2D3748;">Transforming fragmented, cross-departmental data streams into clear localized market trends and actionable growth opportunities.</span></li>
          <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 0 !important;"> Performance Benchmarking: <span style="font-weight: 500; color: #2D3748;">Mapping disparate data pipelines into high-visibility corporate performance indicators (KPIs) to track organizational health in real time.</span></li>
        </ul>
      </div>
    </div>

    <!-- SERVICE CARD 2: DATABASE VALIDATION & AUDITING -->
    <div style="background-color: rgba(255,255,255,0.75); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 18px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); display: flex !important; flex-direction: column !important; justify-content: space-between !important;">
      <div>
        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 6px;">
          <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 3px 10px; border-radius: 4px; font-family: 'Arial', sans-serif;">02</span>
          <h3 style="margin: 0 !important; font-size: 16px !important; font-weight: 900 !important; color: #1A488E !important; text-transform: uppercase; letter-spacing: 0.3px;">Database Validation & Auditing</h3>
        </div>
        <p style="font-size: 13.5px; color: #23272A; font-weight: 700; margin-bottom: 12px; line-height: 1.45;">I deploy rigorous data governance protocols to establish a single, trusted source of truth for your business architecture.</p>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 6px !important;"> Automated Data Cleaning: <span style="font-weight: 500; color: #2D3748;">Designing custom validation routines that dynamically fix syntax discrepancies and catch format anomalies before they skew results.</span></li>
          <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 0 !important;"> Ledger Reconciliation: <span style="font-weight: 500; color: #2D3748;">Engineering cross-system auditing rules to completely eliminate duplicate tracking records and permanently isolate data leakages.</span></li>
        </ul>
      </div>
    </div>

    <!-- SERVICE CARD 3: EXECUTIVE BUSINESS INTELLIGENCE -->
    <div style="background-color: rgba(255,255,255,0.75); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 18px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); display: flex !important; flex-direction: column !important; justify-content: space-between !important;">
      <div>
        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 6px;">
          <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 3px 10px; border-radius: 4px; font-family: 'Arial', sans-serif;">03</span>
          <h3 style="margin: 0 !important; font-size: 16px !important; font-weight: 900 !important; color: #1A488E !important; text-transform: uppercase; letter-spacing: 0.3px;">Business Intelligence</h3>
        </div>
        <p style="font-size: 13.5px; color: #23272A; font-weight: 700; margin-bottom: 12px; line-height: 1.45;">I build high-impact visualization ecosystems that democratize data access and drive rapid executive decision-making.</p>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 6px !important;"> Dashboard Engineering: <span style="font-weight: 500; color: #2D3748;">Designing responsive Power BI and Advanced Excel suites tailored for immediate operational oversight and intuitive drill-down loops.</span></li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 0 !important;"> Live Decision Support: <span style="font-weight: 500; color: #2D3748;">Integrating interactive parameters, dynamic data filtering, and deep drill-down cross-filters for friction-free reporting.</span></li>
      </ul>
    </div>

    <!-- SERVICE CARD 4: ADVANCED COMMERCIAL ANALYTICS -->
    <div style="background-color: rgba(255,255,255,0.75); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 18px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); display: flex !important; flex-direction: column !important; justify-content: space-between !important;">
      <div>
        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 6px;">
          <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 3px 10px; border-radius: 4px; font-family: 'Arial', sans-serif;">04</span>
          <h3 style="margin: 0 !important; font-size: 16px !important; font-weight: 900 !important; color: #1A488E !important; text-transform: uppercase; letter-spacing: 0.3px;">Advanced Commercial Analytics</h3>
        </div>
        <p style="font-size: 13.5px; color: #23272A; font-weight: 700; margin-bottom: 12px; line-height: 1.45;">I apply advanced machine learning frameworks to customer data to optimize monetization, mitigate risk, and project revenue trends.</p>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 6px !important;"> Behavioral Segmentation: <span style="font-weight: 500; color: #2D3748;">Deploying multi-dimensional customer matrices and Recency, Frequency, Monetary (RFM) transaction clustering profiles to map intent.</span></li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 0 !important;"> Predictive Risk Modeling: <span style="font-weight: 500; color: #2D3748;">Building supervised machine learning classification pipelines to forecast market shifts, isolate churn risks, and drive proactive strategy blocks.</span></li>
      </ul>
    </div>

    <!-- SERVICE CARD 5: STATISTICAL RESEARCH & CONTROLS -->
    <div style="background-color: rgba(255,255,255,0.75); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 18px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); display: flex !important; flex-direction: column !important; justify-content: space-between !important; grid-column: 1 / -1 !important;">
      <div>
        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 6px;">
                   <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 3px 10px; border-radius: 4px; font-family: 'Arial', sans-serif;">05</span>
          <h3 style="margin: 0 !important; font-size: 16px !important; font-weight: 900 !important; color: #1A488E !important; text-transform: uppercase; letter-spacing: 0.3px;">Statistical Research & Controls</h3>
        </div>
        <p style="font-size: 13.5px; color: #23272A; font-weight: 700; margin-bottom: 12px; line-height: 1.45;">I leverage rigorous academic and empirical methodologies to ensure your research outcomes are bulletproof and mathematically sound.</p>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 6px !important;"> Quantitative Modeling: <span style="font-weight: 500; color: #2D3748;">Applying advanced population sampling controls, experimental regressions, and variance analysis (ANOVA) matrices to large survey datasets.</span></li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #1A1D20 !important; font-weight: bold; margin-bottom: 0 !important;"> Evidence-Based Reporting: <span style="font-weight: 500; color: #2D3748;">Synthesizing complex field data and deep inferential analytics into defensible, high-integrity executive reports for enterprise stakeholders.</span></li>
      </ul>
    </div>

  </div> <!-- Safely closes the display grid layout container -->

  <!-- HIGH-CONTRAST ACTION ACCENT BUTTON BAR -->
  <div style="background-color: #23272A; padding: 15px 25px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box; margin-top: 10px !important;">
    <p style="font-size: 15px; color: #FFFFFF !important; font-weight: bold; margin: 0; letter-spacing: 0.5px; font-family: 'Arial', sans-serif;">
       Explore - Projects: <label for="tab-projects" style="color: #FFD200; cursor: pointer; text-decoration: underline; font-weight: 900; margin-left: 5px;">Examine the active project briefs and structural overviews demonstrating these services in production →</label>
    </p>
  </div>

</div> <!-- Safely closes the services content-card panel wrapper container perfectly -->



<!-- ================================================ -->
<!-- 4. PROJECTS CARD                                 -->
<!-- ================================================ -->
<div id="projects" class="content-card" style="padding: 25px 45px 35px 45px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 4px !important;"> Projects Pool</h2>
  <p style="margin-top: 0 !important; margin-bottom: 20px !important; font-size: 15.5px; font-weight: bold; color: #23272A; line-height: 1.35;">A directory of production-ready analytical systems designed using a secure, standard, and unified enterprise specification format:</p>

  <!-- PROJECT 1 -->
  <details style="background-color: #FFFFFF; padding: 10px 20px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 10px; width: 100%; box-sizing: border-box;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; outline: none;"> 1. Enterprise HR Analytics & Workforce Stability Infrastructure</summary>
    <div style="margin-top: 12px; padding: 5px 0 0 0; width: 100%; box-sizing: border-box; border-top: 1px dashed #CBD5E0;">
      <table style="width: 100% !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 14px !important; margin-top: 10px; border: 1px solid #E2E8F0 !important;">
        <tbody>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; width: 25%; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Project Synopsis</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 4px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Engineered an end-to-end operational data processing and relational modeling database framework.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Aggregated and transformed highly fragmented employee files into centralized executive-ready assets.</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Focus & Production Scale</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;"><b>Workforce Scale Tracking:</b> Completed scale mapping for <b>1,048,575 total employees</b> across <b>734,439 active tracks</b>.</li>
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;"><b>Salary Intelligence:</b> Formulated interactive cohort analytics for a salary baseline of <b>$10,741.16</b> mapped by position role.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;"><b>Stability Analysis:</b> Isolated an exact **19.96% attrition rate variance** across core departments to flag risk areas.</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Specialized Tools Stack</td>
            <td style="padding: 12px 10px; color: #23272A; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Power BI Desktop &nbsp;|&nbsp; Power Query ETL &nbsp;|&nbsp; DAX Metric Modeling &nbsp;|&nbsp; Advanced Excel Data Structuring</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 0px !important;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Strategic Value & Output</td>
            <td style="padding: 12px 10px; color: #23272A !important; vertical-align: top; background-color: #FFFFFF !important;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #23272A !important; font-weight: 500 !important;">Delivered a responsive multi-tab dashboard layout spanning Overview, Workforce, Performance, and Attrition Analytics.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #23272A !important; font-weight: 500 !important;">Transforms messy operational feedback loops into audit-ready information for senior leadership decisions.</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </details>

  <!-- PROJECT 2 -->
  <details style="background-color: #FFFFFF; padding: 10px 20px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 10px; width: 100%; box-sizing: border-box;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; outline: none;"> 2. Administrative Ledger Data Quality & Reconciliation Engine</summary>
    <div style="margin-top: 12px; padding: 5px 0 0 0; width: 100%; box-sizing: border-box; border-top: 1px dashed #CBD5E0;">
      <table style="width: 100% !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 14px !important; margin-top: 10px; border: 1px solid #E2E8F0 !important;">
        <tbody>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; width: 25%; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Venture Track Status</td>
            <td style="padding: 12px 10px; color: #1A488E; font-weight: 800; vertical-align: top; background-color: #FFFFFF;">[PRODUCTION PIPELINE ACTIVE - IN PROGRESS / ONGOING]</td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Core Business Questions</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Where are the structural discrepancies and hidden financial leakages hiding inside multi-source ledger reporting arrays?</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">How can we construct an automated source of truth that guarantees ledger records are 100% audit-ready?</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Metrics & KPIs</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 4px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Record Completeness Score (%) &nbsp;|&nbsp; Exception Error Detection Rate</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Duplicate Tracking Volume &nbsp;|&nbsp; Reconciliation Processing Time</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Specialized Tools Stack</td>
            <td style="padding: 12px 10px; color: #23272A; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Advanced Excel &nbsp;|&nbsp; Power Query &nbsp;|&nbsp; SQL (PostgreSQL) &nbsp;|&nbsp; Python (Pandas/NumPy) &nbsp;|&nbsp; Exception Logs</li>
              </ul>
            </td>
          </tr>
                  <tr style="border-bottom: 0px !important;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Scope & Value</td>
            <td style="padding: 12px 10px; color: #23272A !important; vertical-align: top; background-color: #FFFFFF !important;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Ingesting multi-source administrative files, isolating formatting and structural metadata variances.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Compiles a verified clean database to eliminate financial risk parameters and mitigate leaks.</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </details>

  <!-- PROJECT 3 -->
  <details style="background-color: #FFFFFF; padding: 10px 20px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 10px; width: 100%; box-sizing: border-box;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; outline: none;"> 3. Employee Engagement Matrix & Quantitative Survey Diagnostics</summary>
    <div style="margin-top: 12px; padding: 5px 0 0 0; width: 100%; box-sizing: border-box; border-top: 1px dashed #CBD5E0;">
      <table style="width: 100% !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 14px !important; margin-top: 10px; border: 1px solid #E2E8F0 !important;">
        <tbody>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; width: 25%; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Venture Track Status</td>
            <td style="padding: 12px 10px; color: #1A488E; font-weight: 800; vertical-align: top; background-color: #FFFFFF;">[PRODUCTION PIPELINE ACTIVE - IN PROGRESS / ONGOING]</td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Core Business Questions</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">What specific workplace variables (tenure, shift, role) are mathematically correlated with satisfaction scores?</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Are feedback shifts statistically significant or due to minor baseline seasonal trend drops?</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Metrics & KPIs</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 4px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Average Engagement Score &nbsp;|&nbsp; Survey Response Rate (%)</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Sentiment Index Variance &nbsp;|&nbsp; Demographic Correlation Coefficient (r)</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Specialized Tools Stack</td>
            <td style="padding: 12px 10px; color: #23272A; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Excel &nbsp;|&nbsp; Power Query &nbsp;|&nbsp; Power BI &nbsp;|&nbsp; R Studio / Python &nbsp;|&nbsp; Statistical Analysis Inferences</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 0px !important;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Scope & Value</td>
            <td style="padding: 12px 10px; color: #23272A !important; vertical-align: top; background-color: #FFFFFF !important;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #23272A !important; font-weight: 500 !important;">Processing survey matrix arrays, building quantitative metrics distribution channels for analysis.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #23272A !important; font-weight: 500 !important;">Translates raw Likert feedback scales into defensible evidence paths to optimize performance models.</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </details>

  <!-- PROJECT 4 -->
  <details style="background-color: #FFFFFF; padding: 10px 20px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 10px rgba(0,0,0,0.02); margin-bottom: 0px; width: 100%; box-sizing: border-box;">
    <summary style="font-weight: bold; color: #1A488E; font-size: 17.5px; cursor: pointer; text-transform: uppercase; outline: none;"> 4. Customer & Commercial Predictive Churn Optimization Engine</summary>
    <div style="margin-top: 12px; padding: 5px 0 0 0; width: 100%; box-sizing: border-box; border-top: 1px dashed #CBD5E0;">
      <table style="width: 100% !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 14px !important; margin-top: 10px; border: 1px solid #E2E8F0 !important;">
        <tbody>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; width: 25%; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Venture Track Status</td>
            <td style="padding: 12px 10px; color: #1A488E; font-weight: 800; vertical-align: top; background-color: #FFFFFF;">[PRODUCTION PIPELINE ACTIVE - IN PROGRESS / ONGOING]</td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Core Business Questions</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Which high-value client segments are exhibiting behavioral patterns that signal an imminent risk of leaving?</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">What is the Projected Customer Lifetime Value (CLV) drop-off if customer retention drops by a specific percentage over the next quarter?</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Metrics & KPIs</td>
            <td style="padding: 12px 10px; color: #2D3748; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 4px !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Customer Churn Probability (%) &nbsp;|&nbsp; Projected Revenue At Risk</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; color: #2D3748 !important; font-weight: 500 !important;">Customer Lifetime Value (CLV) &nbsp;|&nbsp; Model Precision & Recall Accuracy Rate</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 1px solid #E2E8F0;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Specialized Tools Stack</td>
            <td style="padding: 12px 10px; color: #23272A; vertical-align: top; background-color: #FFFFFF;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                              <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Advanced Excel &nbsp;|&nbsp; Power Query &nbsp;|&nbsp; SQL (PostgreSQL) &nbsp;|&nbsp; Python (Pandas/NumPy) &nbsp;|&nbsp; Exception Logs</li>
              </ul>
            </td>
          </tr>
          <tr style="border-bottom: 0px !important;">
            <td style="padding: 12px 10px; font-weight: bold; color: #1A488E; vertical-align: top; background-color: #F8FAFC; border-right: 1px solid #E2E8F0;"> Target Scope & Value</td>
            <td style="padding: 12px 10px; color: #23272A !important; vertical-align: top; background-color: #FFFFFF !important;">
              <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
                <li style="margin-bottom: 6px !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Ingesting multi-source administrative files, isolating formatting and structural metadata variances.</li>
                <li style="margin-bottom: 0 !important; line-height: 1.45; font-weight: 500; color: #23272A !important;">Compiles a verified clean database to eliminate financial risk parameters and mitigate leaks.</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </details>
</div>


<!-- ================================================ -->
<!-- 5. PORTFOLIO CARD                                -->
<!-- ================================================ -->
<div id="portfolio-hub" class="content-card" style="padding: 25px 45px 35px 45px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 4px !important;"> Enterprise Portfolio Directory</h2>
  <p style="margin-top: 0 !important; margin-bottom: 20px !important; font-size: 15.5px; font-weight: bold; color: #23272A; line-height: 1.35;">A technical asset directory cataloging relational ingestion sources, production scales, and integrity validation constraints across active data modules:</p>
  
  <!-- DATA ENGINEERING COMPLIANCE LEDGER MATRIX TABLE -->
  <div style="width: 100% !important; overflow-x: auto !important; margin-bottom: 0px; border-radius: 8px; border: 1px solid #CBD5E0; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <table style="width: 100% !important; min-width: 950px !important; border-collapse: collapse !important; background-color: #FFFFFF !important; color: #23272A !important; font-size: 13.5px !important; margin: 0;">
      <thead>
        <tr style="background-color: #23272A !important; color: #FFFFFF !important; font-weight: bold;">
          <th style="padding: 12px 10px; border-right: 1px solid #3A3F44; text-align: center; width: 4%;">#</th>
          <th style="padding: 12px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 22%;">Active System Asset Module</th>
          <th style="padding: 12px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 18%;">Relational DB Ingestion Source</th>
          <th style="padding: 12px 12px; border-right: 1px solid #3A3F44; text-align: left; width: 26%;">Pipeline Ingestion Scale</th>
          <th style="padding: 12px 12px; text-align: left; width: 30%;">Integrity Verification Logic Check</th>
        </tr>
      </thead>
      <tbody>
        <!-- MODULE 1 -->
        <tr style="background-color: #FFFFFF; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 12px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">1</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Module_01: HR_Core_Analytics</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #2D3748; font-weight: 500;">Multi-Source CSV Datasets & Excel Arrays</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #1A488E; font-weight: bold;">1,048,575 Row Frameworks (734,439 Active)</td>
          <td style="padding: 12px 12px; font-weight: 500; color: #2D3748;">Calculated Measures, Schema Validation & DAX Checksums</td>
        </tr>
        <!-- MODULE 2 -->
        <tr style="background-color: #F8FAFC; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 12px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">2</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Module_02: Recon_Engine</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #2D3748; font-weight: 500;">Administrative SQL Ledgers & Flat Files</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #718096; font-style: italic; font-weight: 500;">[System Scale Load Testing Underway]</td>
          <td style="padding: 12px 12px; font-weight: 500; color: #2D3748;">Automated Cross-System Key Matching & Duplicate Scrubbing</td>
        </tr>
        <!-- MODULE 3 -->
        <tr style="background-color: #FFFFFF; border-bottom: 1px solid #E2E8F0;">
          <td style="padding: 12px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">3</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Module_03: Sentiment_Matrix</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #2D3748; font-weight: 500;">Survey Management API Feedback Streams</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #718096; font-style: italic; font-weight: 500;">[Data Schema Engineering Underway]</td>
          <td style="padding: 12px 12px; font-weight: 500; color: #2D3748;">Cron-Scheduled Syntax Outlier Cleaning & Range Constraints</td>
        </tr>
        <!-- MODULE 4 -->
        <tr style="background-color: #F8FAFC; border-bottom: 0;">
          <td style="padding: 12px 10px; border-right: 1px solid #E2E8F0; text-align: center; font-weight: bold; color: #4A5568;">4</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; font-weight: bold; color: #1A488E;">Module_04: Predictive_Monetization</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #2D3748; font-weight: 500;">Live Commercial Transaction Record Blocks</td>
          <td style="padding: 12px 12px; border-right: 1px solid #E2E8F0; color: #718096; font-style: italic; font-weight: 500;">[Machine Learning Model Tuning Underway]</td>
          <td style="padding: 12px 12px; font-weight: 500; color: #2D3748;">Supervised Classification Hyperplane Validation Bounds Loops</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>


<!-- ================================================ -->
<!-- 6. EXPERIENCE CARD                               -->
<!-- ================================================ -->
<div id="experience" class="content-card" style="padding: 17px 37px 17px 37px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 4px !important;"> Professional Experience Track</h2>
  <p style="margin-top: 0 !important; margin-bottom: 25px !important; font-size: 15.5px; font-weight: bold; color: #23272A; line-height: 1.35;">My consulting track spans advanced statistical modeling, cross-source data engineering, and predictive commercial business intelligence across high-stakes corporate environments:</p>

  <!-- TIMELINE GRID ENGINE DECK -->
  <div style="display: flex; flex-direction: column; gap: 20px; width: 100%; box-sizing: border-box; margin-bottom: 25px;">
    
    <!-- ROLE 1: INFOTRAK -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 12px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif;"> 1. ENGAGEMENT TRACK - 2026</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Data Analyst - Infotrak Research & Consulting</h3>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 0 15px 0 !important; list-style-type: square !important;">
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 6px !important;">Managing research, survey, and commercial business data pipelines across end-to-end data management, data validation, inferential statistical testing, and executive reporting.</li>
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Automating the transformation of massive raw field research tracking arrays into high-integrity, decision-ready information assets for strategic stakeholders.</li>
      </ul>
      <div style="font-size: 12px; color: #1A488E; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px;"> Core Focus: Pipeline Automation &nbsp;|&nbsp; Inferential Statistics &nbsp;|&nbsp; Executive Briefs</div>
    </div>

    <!-- ROLE 2: CALLTRONIX -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 12px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif;"> 2. CORPORATE TRACK - 2024–2025</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Workforce & Data Analyst - Calltronix Kenya Ltd</h3>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 0 15px 0 !important; list-style-type: square !important;">
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 6px !important;">Analysed and reconciled cross-functional workforce, HR, finance, and system operations data to audit productivity, validate incentive parameters, and support payroll processing for 350+ FTE.</li>
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Integrated multiple disjointed operational data platforms to eliminate tracking variances and generate automated performance dashboards for leadership support teams.</li>
      </ul>
      <div style="font-size: 12px; color: #1A488E; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px;"> Core Focus: Data Reconciliation &nbsp;|&nbsp; HR Analytics &nbsp;|&nbsp; Workfoce Planning &nbsp;|&nbsp; Payroll Planning and Auditing</div>
    </div>

    <!-- ROLE 3: HAMASISHA AFRICA -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 12px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif;"> 3. SYSTEMS TRACK - 2025</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Data & Research Analyst - Hamasisha Africa</h3>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 0 15px 0 !important; list-style-type: square !important;">
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Supported quantitative project research through data preparation, multi-variable statistical analysis, narrative interpretation, and stakeholder reporting, directly enabling evidence-based funding deployments.</li>
      </ul>
      <div style="font-size: 12px; color: #1A488E; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px;"> Core Focus: Quantitative Research &nbsp;|&nbsp; Multi-Variable Regressions &nbsp;|&nbsp; Funding Metrics</div>
    </div>

    <!-- ROLE 4: ASSIGNMENTS -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 12px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif;"> 4. FIELD TRACK</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Research, MEAL & Data Operations Assignments</h3>
      </div>
      <ul style="padding-left: 20px !important; margin: 0 0 15px 0 !important; list-style-type: square !important;">
        <li style="font-size: 14px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Undertook specialized contract assignments involving quantitative data capture monitoring, digital questionnaire skip-logic engineering, descriptive summaries, and field-based information management assets.</li>
      </ul>
      <div style="font-size: 12px; color: #1A488E; font-weight: 800; text-transform: uppercase; letter-spacing: 0.5px;"> Core Focus: Skip-Logic Engineering &nbsp;|&nbsp; MEAL Compliance &nbsp;|&nbsp; Field Data Capture</div>
    </div>

  </div>

  <!-- PREMIUM LOWER BRAND FIELD RIBBON BUTTON BAR -->
  <div style="background-color: #23272A; padding: 15px 25px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box; margin-top: 10px !important;">
    <p style="font-size: 14.5px; color: #FFFFFF !important; font-weight: bold; margin: 0; letter-spacing: 0.5px; font-family: 'Arial', sans-serif; text-transform: uppercase;">
       Primary Specialty Execution Fields: <span style="color: #FFD200; font-weight: 900; margin-left: 5px;">Data Analytics &nbsp;|&nbsp; Statistics &nbsp;|&nbsp; Business Intelligence &nbsp;|&nbsp; Data Management &nbsp;|&nbsp; Research Analytics &nbsp;|&nbsp; Workforce Analytics</span>
    </p>
  </div>

</div>


<!-- ================================================ -->
<!-- 7. EDUCATION CARD                                -->
<!-- ================================================ -->
<div id="education" class="content-card" style="padding: 17px 37px 17px 37px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 4px !important;"> Academic Foundations</h2>
  <p style="margin-top: 0 !important; margin-bottom: 25px !important; font-size: 15.5px; font-weight: bold; color: #23272A; line-height: 1.35;">Advanced graduate data track training and rigorous quantitative biostatistics core competencies:</p>

  <!-- ACADEMIC TIMELINE CONTAINER DECK -->
  <div style="display: flex; flex-direction: column; gap: 20px; width: 100%; box-sizing: border-box;">
    
    <!-- DEGREE 1: DATA SCIENCE -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 11.5px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif; text-transform: uppercase; letter-spacing: 0.5px;"> 1. MSC PROGRAM TRACK</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Master of Science in Data Science</h3>
      </div>
      <span style="font-size: 13.5px; color: #23272A; font-weight: bold; display: block; margin-bottom: 12px; font-family: 'Arial', sans-serif;"> Open University of Kenya &nbsp;|&nbsp; <span style="color: #1A488E; font-weight: 800;">[Ongoing]</span></span>
      <span style="font-size: 13px; color: #1A488E; font-weight: 800; display: block; margin-bottom: 6px; text-transform: uppercase; letter-spacing: 0.5px;"> Advanced Graduate Competencies Deployed:</span>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 4px !important;">Active development of advanced capabilities in predictive analytics, computational machine learning classification, and model precision mapping.</li>
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Architecting big data engineering frameworks, data warehousing systems, cloud science pipelines, and senior corporate governance blocks.</li>
      </ul>
    </div>

    <!-- DEGREE 2: BIOSTATISTICS -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 11.5px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif; text-transform: uppercase; letter-spacing: 0.5px;">  2. BSC ACADEMIC FOUNDATION</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;"> Bachelor of Science in Biostatistics</h3>
      </div>
      <span style="font-size: 13.5px; color: #23272A; font-weight: bold; display: block; margin-bottom: 12px; font-family: 'Arial', sans-serif;"> Jomo Kenyatta University of Agriculture and Technology (JKUAT) &nbsp;|&nbsp; <span style="color: #2D3748; font-weight: 800;">Class of 2022 - Second Class Upper Division</span></span>
      <span style="font-size: 13px; color: #1A488E; font-weight: 800; display: block; margin-bottom: 6px; text-transform: uppercase; letter-spacing: 0.5px;"> Core Academic Disciplines Mastered:</span>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 4px !important;">Advanced training in foundational biostatistics, complex mathematical modeling arrays, and deep inferential quantitative methodology.</li>
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;">Formulating rigorous research design rules, multi-variable regression diagnostics, population sampling tracks, and relational data analysis.</li>
      </ul>
    </div>

  </div>
</div>


<!-- ================================================ -->
<!-- 8. CERTIFICATIONS CARD                           -->
<!-- ================================================ -->
<div id="certifications" class="content-card" style="padding: 17px 37px 17px 37px !important;">
  <h2 style="margin: 0 0 4px 0 !important; padding-bottom: 6px !important;"> Certifications & Professional Development</h2>
  <p style="margin-top: 10 !important; margin-bottom: 25px !important; font-size: 15.5px; font-weight: bold; color: #23272A; line-height: 1.35;">Validated global credentials and specialized industry training tracking advanced data systems engineering and project governance:</p>

  <!-- PREMIUM SINGLE COLUMN STACKED CREDENTIALS FRAMEWORK -->
  <div style="display: flex; flex-direction: column; gap: 20px; width: 100%; box-sizing: border-box; margin-bottom: 25px;">
    
    <!-- CREDENTIAL 1: IBM DATA SCIENCE & AI -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15 rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: 900; font-size: 11.5px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif; letter-spacing: 0.5px;"> 1. ADVANCED ANALYTICS & AI</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">IBM Data Science & AI Professional</h3>
      </div>
      <span style="font-size: 13.5px; color: #23272A; font-weight: bold; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;"> IBM Authorized Industry Credential</span>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important;">Validated global validation training covering enterprise data science operations, machine learning classification algorithms, and predictive trends forecasting workflows.</li>
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important;">Engineering interactive computational scripts and executing multi-tiered dataset cleaning routines using Python data analysis frameworks.</li>
      </ul>
    </div>

    <!-- CREDENTIAL 2: HUMANITARIAN MEAL & PROJECT SYSTEMS -->
    <div style="background-color: rgba(255,255,255,0.7); border: 1px solid rgba(35,39,42,0.18); border-radius: 10px; padding: 22px; box-shadow: 0 4px 15px rgba(0,0,0,0.02); box-sizing: border-box; width: 100%;">
      <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px; border-bottom: 2px solid rgba(26,72,142,0.15); padding-bottom: 8px; flex-wrap: wrap;">
        <span style="background-color: #23272A; color: #FFD200; font-weight: bold; font-size: 11.5px; padding: 4px 12px; border-radius: 4px; font-family: 'Arial', sans-serif; letter-spacing: 0.5px;"> 2. METRICS & PROJECT GOVERNANCE</span>
        <h3 style="margin: 0 !important; font-size: 17px !important; font-weight: 900 !important; color: #1A488E !important; letter-spacing: 0.3px;">Humanitarian MEAL & Project Management Essentials</h3>
      </div>
      <span style="font-size: 13.5px; color: #23272A; font-weight: bold; display: block; margin-bottom: 12px; font-family: 'Arial', sans-serif;"> DisasterReady / Humanitarian Leadership Academy</span>
      <span style="font-size: 13px; color: #1A488E; font-weight: 800; display: block; margin-bottom: 6px; text-transform: uppercase; letter-spacing: 0.5px;"> Specialized Dual-Track Endorsements Mastered:</span>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 6px !important;"><b>MEAL Essentials Professional:</b> Specialized training in multi-variable monitoring tracking arrays, quantitative dataset validation loops, program evaluation metrics, and system accountability frameworks.</li>
        <li style="font-size: 13.5px !important; line-height: 1.5 !important; color: #2D3748 !important; font-weight: 500 !important; margin-bottom: 0 !important;"><b>Project Management Essentials Track:</b> Certified operational proficiency spanning advanced project planning structures, lifecycle milestones layout, and active project implementation governance models.</li>
      </ul>
    </div>

  </div>


   <!-- HIGH-CONTRAST LOWER TRACK ENGINE RE-LINKED BLOCK -->
  <div style="background-color: #23272A; padding: 15px 25px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box; margin-top: 10px !important;">
    <p style="font-size: 14.5px; color: #FFFFFF !important; font-weight: bold; margin: 0; letter-spacing: 0.5px; font-family: 'Arial', sans-serif; text-transform: uppercase;">
       Primary Specialty Execution Fields: <span style="color: #FFD200; font-weight: 900; margin-left: 5px;">Data Analytics &nbsp;|&nbsp; Statistics &nbsp;|&nbsp; Business Intelligence &nbsp;|&nbsp; Data Management &nbsp;|&nbsp; Research Analytics &nbsp;|&nbsp; Workforce planning and Analytics;|&nbsp; Payroll Analytics</span>
    </p>
  </div>

</div>


<!-- ================================================ -->
<!-- 9. GET IN TOUCH CARD (FULLY FUNCTIONAL FORM)     -->
<!-- ================================================ -->
<div id="get-in-touch" class="content-card" style="background-color: #FFFFFF !important; color: #23272A !important; padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; margin: 0;">
    
    <!-- LEFT PANEL: VALUE PROPOSITION -->
    <div style="flex: 1; min-width: 320px; box-sizing: border-box; padding: 0 !important; margin: 0 !important;">
      <span style="color: #1A488E; font-weight: bold; text-transform: uppercase; font-size: 13px; letter-spacing: 0.5px; display: block; margin-bottom: 5px; text-align: left !important;">Get in touch</span>
      <h2 style="color: #23272A !important; font-size: 36px !important; font-weight: 900 !important; border: none !important; margin: 0 0 15px 0 !important; padding: 0 !important; text-transform: none !important; display: block !important; text-align: left !important;">Let's Build Something Together</h2>
      <p style="line-height: 1.5; font-size: 16px; color: #4A5568 !important; margin-bottom: 20px; text-align: left !important;">Need an interactive executive dashboard, an automated data cleaning script, or a rigorous statistical analysis model?</p>
      <p style="line-height: 1.5; font-size: 15px; color: #4A5568 !important; margin-bottom: 25px; text-align: left !important;">I engineer custom, high-integrity data infrastructure designed to eliminate manual business errors and power smart corporate strategies. Fill out your requirements to map out your operational goals.</p>
    </div>
    
    <!-- RIGHT PANEL: INTERACTIVE INTAKE FORM -->
    <div style="flex: 1.2; min-width: 360px; background-color: #FFFFFF; border: 1px solid #E2E8F0; padding: 35px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); box-sizing: border-box; margin: 0 !important;">
      
      <form action="https://web3forms.com" method="POST" style="width: 100%; margin: 0; padding: 0; display: flex; flex-direction: column; gap: 15px; text-align: left;">
        
        <!-- INTEGRATED UNIQUE ACCESS KEY -->
        <input type="hidden" name="access_key" value="0b458d02-f50e-4cbe-b729-c441817646df">
        
        <!-- AUTOMATIC REDIRECT HOOK: Bounces clients straight back to your portfolio page -->
        <input type="hidden" name="redirect" value="https://github.io"> 
        
        <!-- EMAIL SUBJECT CONFIG -->
        <input type="hidden" name="subject" value="New Portfolio Consulting Inquiry">
        
        <div style="display: flex; flex-direction: column; gap: 5px;">
          <label style="font-size: 13px; font-weight: bold; color: #23272A;">Your Name</label>
          <input type="text" name="name" required style="width: 100%; padding: 10px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; font-size: 14px; background-color: #F8FAFC;">
        </div>

        <div style="display: flex; flex-direction: column; gap: 5px;">
          <label style="font-size: 13px; font-weight: bold; color: #23272A;">Email Address</label>
          <input type="email" name="email" required style="width: 100%; padding: 10px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; font-size: 14px; background-color: #F8FAFC;">
        </div>

        <div style="display: flex; flex-direction: column; gap: 5px;">
          <label style="font-size: 13px; font-weight: bold; color: #23272A;">Inquiry Summary & Project Scope</label>
          <textarea name="message" rows="4" required placeholder="Describe your data challenges or timeline metrics..." style="width: 100%; padding: 10px; border: 1px solid #CBD5E0; border-radius: 6px; box-sizing: border-box; font-size: 14px; font-family: sans-serif; resize: vertical; background-color: #F8FAFC;"></textarea>
        </div>

        <button type="submit" style="background-color: #1A488E !important; color: #FFFFFF !important; padding: 14px !important; border: none !important; border-radius: 6px; font-weight: bold; font-size: 14px; cursor: pointer; text-transform: uppercase; letter-spacing: 0.5px; box-shadow: 0 4px 10px rgba(26,72,142,0.2); width: 100%; text-align: center; margin-top: 5px;">
           Submit Inquiry
        </button>
        
      </form>
      
    </div>
    
  </div>
</div>

</div> <!-- Closes scroll-content layout engine -->
</div> <!-- Closes portfolio-container outer window -->
