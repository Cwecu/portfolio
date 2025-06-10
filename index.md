<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nicholas Lawson | GIS Analyst Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
    }

    .header {
      background-color: #343a40;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .content {
      padding: 20px;
      margin: 20px;
    }

    .slider1, .slider2, .slider3 {
      position: relative;
      width: 100%;
      max-width: 800px;
      margin: 20px auto;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      background-color: #f8f9fa;
    }

    .slider1 img, .slider2 img, .slider3 img {
      width: 100%;
      height: auto;
      display: none;
      border-radius: 10px;
    }

    .slider1 img:first-child, .slider2 img:first-child, .slider3 img:first-child {
      display: block;
      animation: fadeSlide3 15s infinite;
    }

    .slider2 img:first-child {
      animation: fadeSlide4 20s infinite;
    }

    .slider3 img:first-child {
      animation: fadeSlide6 30s infinite;
    }

    .slider1 img:nth-child(2) {
      animation: fadeSlide3 15s infinite 5s;
    }

    .slider1 img:nth-child(3) {
      animation: fadeSlide3 15s infinite 10s;
    }

    .slider2 img:nth-child(2) {
      animation: fadeSlide4 20s infinite 5s;
    }

    .slider2 img:nth-child(3) {
      animation: fadeSlide4 20s infinite 10s;
    }

    .slider2 img:nth-child(4) {
      animation: fadeSlide4 20s infinite 15s;
    }

    .slider3 img:nth-child(2) {
      animation: fadeSlide6 30s infinite 5s;
    }

    .slider3 img:nth-child(3) {
      animation: fadeSlide6 30s infinite 10s;
    }

    .slider3 img:nth-child(4) {
      animation: fadeSlide6 30s infinite 15s;
    }

    .slider3 img:nth-child(5) {
      animation: fadeSlide6 30s infinite 20s;
    }

    .slider3 img:nth-child(6) {
      animation: fadeSlide6 30s infinite 25s;
    }

    @keyframes fadeSlide3 {
      0%, 30% { opacity: 1; display: block; }
      33%, 100% { opacity: 0; display: none; }
    }

    @keyframes fadeSlide4 {
      0%, 22% { opacity: 1; display: block; }
      25%, 100% { opacity: 0; display: none; }
    }

    @keyframes fadeSlide6 {
      0%, 14% { opacity: 1; display: block; }
      16%, 100% { opacity: 0; display: none; }
    }

  </style>
</head>
<body>

  <header class="header">
    <h1>Nicholas Lawson | GIS Analyst Portfolio</h1>
    <img src="./profile.jpg.jfif" style="float: right; border-radius: 50%; width: 120px; margin-left: 20px;" alt="Profile Picture">
  </header>

  <div class="content">
    <section>
      <h2>👋 About Me</h2>
      <p>I am <strong>Nicholas Lawson</strong>, a recent Geography graduate with expertise in GIS, spatial analysis, and health geography. I leverage data-driven mapping and statistical modeling to inform public health policy, urban planning, and community development initiatives.</p>

      <h3>Core Competencies</h3>
      <ul>
        <li><strong>Software:</strong> ArcGIS Pro, QGIS, Python for GIS</li>
        <li><strong>Analysis:</strong> Geographically Weighted Regression (GWR), Network Analysis, Hotspot Analysis</li>
        <li><strong>Specializations:</strong> Health Geography, Urban Planning, LiDAR Processing</li>
      </ul>
    </section>

    <section>
      <h2>🍎 Project 1: 🌆 Urbanization, Food Security & Spatial Access in DFW</h2>
      <p><strong>Challenge:</strong> Despite being part of a major metropolitan region, the urban cores of Dallas and Fort Worth continue to exhibit widespread food insecurity...</p>

      <div class="slider1">
        <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map Analysis">
        <img src="./Food Deserts hotspot.jpg" alt="Food Desert Hotspot Analysis">
        <img src="./Food Access.jpg" alt="Food Access Comprehensive Map">
      </div>
    </section>

    <section>
      <h2>🍎 Project 2: Food Deserts and Chronic Disease in DFW: Association vs. Causality</h2>
      <p><strong>Objective:</strong> Examine the spatial relationship between food desert classification and the prevalence of obesity and diabetes using regression models.</p>

      <div class="slider2">
        <img src="./GWR and Obesity.jpg" alt="Geographically Weighted Regression - Obesity Analysis">
        <img src="./GWR and Diabtes.jpg" alt="Geographically Weighted Regression - Diabetes Analysis">
        <img src="./Obesity and Food Deserts.jpg" alt="Obesity and Food Deserts Correlation">
        <img src="./Diabetes and Food deserts.jpg" alt="Diabetes and Food Deserts Correlation">
      </div>
    </section>

    <section>
      <h2>🏥 Project 3: Liver Disease Mortality Patterns in Texas</h2>
      <p><strong>Challenge:</strong> Understanding the geographic distribution and temporal trends of liver disease mortality to identify at-risk communities.</p>

      <div class="slider3">
        <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Mortality Hotspot Analysis">
        <img src="./AADR 2001-2007.jpg" alt="Age-Adjusted Death Rates 2001-2007">
        <img src="./AADR 2008-2014.jpg" alt="Age-Adjusted Death Rates 2008-2014">
        <img src="./AADR 2015-2020.jpg" alt="Age-Adjusted Death Rates 2015-2020">
        <img src="./Rate Change 1.jpg" alt="Mortality Rate Change Analysis 1">
        <img src="./Rate change 2.jpg" alt="Mortality Rate Change Analysis 2">
      </div>
    </section>

    <section>
      <h2>🏗️ Project 4: LiDAR Building Extraction in Waco, TX</h2>
      <p><strong>Challenge:</strong> Accurate building inventory and volume estimation for urban planning without costly field surveys...</p>
    </section>

    <section>
      <h2>📈 Technical Skills</h2>
      <ul>
        <li><strong>GIS & Spatial Analysis:</strong> Advanced cartography and spatial modeling, Network analysis and service area optimization, Regression, clustering, and spatial statistics, Remote sensing and classification</li>
        <li><strong>Programming & Data:</strong> Python (ArcPy, Pandas, GeoPandas), SQL for spatial databases, SPSS, Web mapping: ArcGIS Pro, ArcGIS Online</li>
      </ul>
    </section>

    <section>
      <h2>🎓 Education & Certifications</h2>
      <p><strong>Master of Science in Geography</strong><br>University of North Texas, 2025</p>
      <p><strong>Bachelor of Art in Geography and Resource Development</strong><br>University of Ghana, 2018</p>
    </section>

    <section>
      <h2>📞 Let's Connect</h2>
      <p>I'm actively seeking opportunities in GIS analysis, urban planning, and public health research...</p>
      <p><strong>Email:</strong> <a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a></p>
      <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank">Nicholas Lawson</a></p>
      <p><strong>GitHub:</strong> <a href="https://github.com/cwecu" target="_blank">cwecu</a></p>
      <p><strong>Location:</strong> Dallas-Fort Worth, Texas</p>
    </section>
  </div>

  <footer>
    <p>Portfolio last updated: June 2025</p>
  </footer>

</body>
</html>
