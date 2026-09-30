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
    <h1>Edna Ogutu | KenData Consultant</h1>
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
<div id="about" class="content-card" style="padding: 40px !important;">
  <div style="display: flex; flex-wrap: wrap; gap: 40px; width: 100%; box-sizing: border-box; align-items: center !important; margin-bottom: 25px !important;">
    
    <!-- LEFT PANEL: DATA GRAPHIC CONTAINER (REDUCED TO MATCH COMPACT PORTFOLIO DESIGN) -->
    <div style="flex: 0.5; min-width: 280px; max-width: 380px; box-sizing: border-box; margin: 0 auto !important;">
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
      <b>End-to-End Execution:</b> Operating across the entire analytical pipeline—from executing rigorous data cleaning and cross-system reconciliations to formulating diagnostic models and interactive reporting systems.
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
      <div style="background-color: rgba(255,255,255,0.6); padding: 14px 18px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 1. Data Analytics & Modeling</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Designing and deploying custom corporate KPI matrix tracking frameworks.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Executing comprehensive exploratory data analysis (EDA) algorithms.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Formulating historical trend forecasting and performance trend lines.</li>
        </ul>
      </div>

      <!-- BOX 2: DATA ENGINEERING -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 14px 18px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 2. Data Engineering & Management</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Architecting automated structural cleaning and parsing routines.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Enforcing cross-source database records validation parameters.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Executing multi-tier system ledger reconciliation and preparation.</li>
        </ul>
      </div>

      <!-- BOX 3: STATISTICAL INFERENCE -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 14px 18px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 3. Statistical Inference & Research</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Applying complex descriptive summaries and inferential metrics testing.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Constructing multivariable linear and logistic regression models.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Synthesizing field diagnostic evidence for strategic decision-making.</li>
        </ul>
      </div>

         <!-- BOX 4: BUSINESS INTELLIGENCE (NESTED CORRECTLY INSIDE THE CORE DOMAINS PARENT ROW) -->
      <div style="background-color: rgba(255,255,255,0.6); padding: 14px 18px; border-radius: 8px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
        <span style="font-weight: 800; color: #1A488E; font-size: 15px; display: block; margin-bottom: 8px;"> 4. Business Intelligence Systems</span>
        <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Engineering interactive, responsive Power BI business dashboards.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 4px !important;">Formulating corporate cross-filtering visual performance matrix maps.</li>
          <li style="font-size: 13px !important; line-height: 1.4 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;">Generating automated executive management reporting frameworks.</li>
        </ul>
      </div>

    </div> <!-- Safely closes the single parent display grid container row -->

    <!-- RE-ENGINEERED OPTIMIZED TOOLSTACK RIBBON WITH CLEAN WRAPPING & LEGIBLE CONTRAST -->
    <div style="background-color: #23272A; padding: 14px 20px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box; overflow: visible !important; margin-top: 15px !important;">
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
<div id="services" class="content-card" style="padding: 40px !important;">
  <h2>💼 Operational Consulting Services</h2>
  <p style="margin-bottom: 25px; font-size: 16.5px; font-weight: bold; color: #23272A; line-height: 1.4;">Speaking directly to organizational pain points—substituting manual error with high-integrity automation:</p>
  
  <!-- PERSUASIVE BENTO GRID SYSTEM WITH NEW STRATEGIC CONTENT -->
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(290px, 1fr)); gap: 20px; width: 100%; box-sizing: border-box; margin-bottom: 30px;">
    
    <!-- CARD 1: ENTERPRISE DATA ANALYTICS -->
    <div style="background-color: rgba(255,255,255,0.7); padding: 22px; border-radius: 10px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 12px rgba(0,0,0,0.03); display: flex; flex-direction: column; justify-content: flex-start;">
      <span style="font-size: 26px; display: block; margin-bottom: 8px;">💼</span>
      <span style="font-weight: 900; color: #1A488E; font-size: 16.5px; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;">Enterprise Data Analytics</span>
      <p style="font-size: 13.5px; margin: 0 0 10px 0; line-height: 1.45; color: #2D3748; font-weight: 600;">I engineer scalable analytics frameworks that bridge the gap between complex enterprise operations and clear corporate strategy.</p>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 6px !important;"><b>Commercial Insights:</b> Transforming fragmented, cross-departmental data streams into clear localized market trends and actionable growth opportunities.</li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;"><b>Performance Benchmarking:</b> Mapping disparate data pipelines into high-visibility corporate performance indicators (KPIs) to track organizational health in real time.</li>
      </ul>
    </div>

    <!-- CARD 2: DATABASE VALIDATION & AUDITING -->
    <div style="background-color: rgba(255,255,255,0.7); padding: 22px; border-radius: 10px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 12px rgba(0,0,0,0.03); display: flex; flex-direction: column; justify-content: flex-start;">
      <span style="font-size: 26px; display: block; margin-bottom: 8px;">🔍</span>
      <span style="font-weight: 900; color: #1A488E; font-size: 16.5px; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;">Database Validation & Auditing</span>
      <p style="font-size: 13.5px; margin: 0 0 10px 0; line-height: 1.45; color: #2D3748; font-weight: 600;">I deploy rigorous data governance protocols to establish a single, trusted source of truth for your business architecture.</p>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 6px !important;"><b>Automated Data Cleaning:</b> Designing custom validation routines that dynamically fix syntax discrepancies and catch format anomalies.</li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;"><b>Ledger Reconciliation:</b> Engineering cross-system auditing rules to completely eliminate duplicate tracking records and permanently isolate data leakages.</li>
      </ul>
    </div>

    <!-- CARD 3: EXECUTIVE BUSINESS INTELLIGENCE -->
    <div style="background-color: rgba(255,255,255,0.7); padding: 22px; border-radius: 10px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 12px rgba(0,0,0,0.03); display: flex; flex-direction: column; justify-content: flex-start;">
      <span style="font-size: 26px; display: block; margin-bottom: 8px;">📊</span>
      <span style="font-weight: 900; color: #1A488E; font-size: 16.5px; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;">Executive Business Intelligence</span>
      <p style="font-size: 13.5px; margin: 0 0 10px 0; line-height: 1.45; color: #2D3748; font-weight: 600;">I build high-impact visualization ecosystems that democratize data access and drive rapid executive decision-making.</p>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 6px !important;"><b>Dashboard Engineering:</b> Designing responsive Power BI and Advanced Excel suites tailored for immediate operational oversight.</li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;"><b>Live Decision Support:</b> Integrating interactive parameters, dynamic filtering, and deep drill-down analytics for friction-free reporting.</li>
      </ul>
    </div>

    <!-- CARD 4: ADVANCED COMMERCIAL ANALYTICS -->
    <div style="background-color: rgba(255,255,255,0.7); padding: 22px; border-radius: 10px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 12px rgba(0,0,0,0.03); display: flex; flex-direction: column; justify-content: flex-start;">
      <span style="font-size: 26px; display: block; margin-bottom: 8px;">📈</span>
      <span style="font-weight: 900; color: #1A488E; font-size: 16.5px; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;">Advanced Commercial Analytics</span>
      <p style="font-size: 13.5px; margin: 0 0 10px 0; line-height: 1.45; color: #2D3748; font-weight: 600;">I apply advanced machine learning frameworks to customer data to optimize monetization, mitigate risk, and project revenue.</p>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 6px !important;"><b>Behavioral Segmentation:</b> Deploying multi-dimensional customer matrices and Recency, Frequency, Monetary (RFM) clustering profiles.</li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;"><b>Predictive Risk Modeling:</b> Building supervised machine learning pipelines to forecast market shifts, flag churn risks, and drive proactive strategy.</li>
      </ul>
    </div>

    <!-- CARD 5: STATISTICAL RESEARCH & CONTROLS -->
    <div style="background-color: rgba(255,255,255,0.7); padding: 22px; border-radius: 10px; border: 1px solid rgba(35,39,42,0.2); box-shadow: 0 4px 12px rgba(0,0,0,0.03); display: flex; flex-direction: column; justify-content: flex-start;">
      <span style="font-size: 26px; display: block; margin-bottom: 8px;">🔬</span>
      <span style="font-weight: 900; color: #1A488E; font-size: 16.5px; display: block; margin-bottom: 10px; font-family: 'Arial', sans-serif;">Statistical Research & Controls</span>
      <p style="font-size: 13.5px; margin: 0 0 10px 0; line-height: 1.45; color: #2D3748; font-weight: 600;">I leverage rigorous academic and empirical methodologies to ensure your research outcomes are bulletproof and mathematically sound.</p>
      <ul style="padding-left: 20px !important; margin: 0 !important; list-style-type: square !important;">
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 6px !important;"><b>Quantitative Modeling:</b> Applying advanced population sampling controls, experimental regressions, and variance analysis (ANOVA) to survey datasets.</li>
        <li style="font-size: 13px !important; line-height: 1.45 !important; color: #2D3748 !important; font-weight: 500; margin-bottom: 0 !important;"><b>Evidence-Based Reporting:</b> Synthesizing complex field data and deep analytics into defensible, high-integrity executive reports for stakeholders.</li>
      </ul>
    </div>

  </div>

  <!-- HIGH-CONTRAST ACTION ACCENT BUTTON BAR (PORTFOLIO SYNOPSES GATE) -->
  <div style="background-color: #23272A; padding: 15px 25px; border-radius: 8px; border-left: 6px solid #FFD200; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; box-sizing: border-box;">
    <p style="font-size: 15px; color: #FFFFFF !important; font-weight: bold; margin: 0; letter-spacing: 0.5px; font-family: 'Arial', sans-serif;">
      🛠️ Portfolio Synopses: <label for="tab-projects" style="color: #FFD200; cursor: pointer; text-decoration: underline; font-weight: 900; margin-left: 5px;">Examine the active project briefs and structural overviews demonstrating these services in production →</label>
    </p>
  </div>

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
    <br><br>
  
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




