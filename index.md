<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Nicholas Lawson | GIS Analyst Portfolio</title>
  <style>
    body { font-family: Arial, sans-serif; line-height: 1.6; margin: 0; padding: 20px; background: #f4f4f4; color: #333; }
    .container { max-width: 900px; margin: auto; background: #fff; padding: 30px; border-radius: 8px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
    header h1, section h2 { color: #0056b3; }
    header h1 { border-bottom: 2px solid #0056b3; padding-bottom: 10px; margin-bottom: 20px; }
    img.profile-img { float: right; width: 120px; height: auto; border-radius: 50%; margin-left: 20px; }
    hr { border: none; border-top: 1px solid #eee; margin: 40px 0; }
    section { margin-bottom: 30px; }
    section h3 { margin-top: 10px; }
    ul { list-style: none; padding: 0; }
    ul li { margin: 6px 0; }
    .slider { position: relative; width: 100%; max-width: 800px; margin: 20px auto; background: #f8f9fa; overflow: hidden; padding-bottom: 56.25%; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); }
    .slider img { position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: cover; opacity: 0; transition: opacity 1.5s ease-in-out; border-radius: 10px; }
    .slider img:first-child { opacity: 1; }
    footer { text-align: center; margin-top: 40px; font-size: 0.9em; color: #666; border-top: 1px solid #eee; padding-top: 20px; }
    a { color: #0056b3; text-decoration: none; }
    a:hover { text-decoration: underline; }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Nicholas Lawson | GIS Analyst Portfolio</h1>
      <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img"/>
    </header>

    <section id="about">
      <h2>👋 About Me</h2>
      <p><strong>Nicholas Lawson</strong> is a Geography graduate specializing in GIS, spatial analysis, and health geography. He utilizes data-driven mapping and statistical modeling to support public health policy, urban planning, and community development.</p>
      <h3>Core Competencies</h3>
      <ul>
        <li><strong>Software:</strong> ArcGIS Pro, QGIS, Python (ArcPy, GeoPandas)</li>
        <li><strong>Analysis:</strong> Geographically Weighted Regression, Network/Hotspot Analysis</li>
        <li><strong>Specializations:</strong> Health Geography, Urban Planning, LiDAR Processing</li>
      </ul>
    </section>

    <hr/>

    <section id="project1">
      <h2>🍎 Project 1: Urbanization, Food Security & Spatial Access in DFW</h2>
      <p><strong>Challenge:</strong> Despite strong infrastructure in Dallas and Fort Worth, food insecurity persists. Traditional measures of food deserts miss cultural, mobility, and store-type factors.</p>
      <p><strong>Approach:</strong> Expanded mapping to include farmers' markets and ethnic grocers for a fuller picture of food access.</p>
      <p><strong>Tools:</strong> ArcGIS Pro, Network Analyst, USDA SNAP Locator, CDC PLACES, ACS, transport networks.</p>
      <ul>
        <li>Created 1 mile service areas via Network Analyst.</li>
        <li>Identified 1,023 food retailers (755 supermarkets, 241 small grocers, 27 farmers' markets).</li>
        <li>Traditional food desert tracts: 1,127 → 1,010 (10% reduction).</li>
        <li>Low‑income food desert tracts dropped from 385 to 325 (16% reduction).</li>
      </ul>
      <div class="slider slider1">
        <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map"/>
        <img src="./Food Deserts hotspot.jpg" alt="Hotspot Analysis"/>
        <img src="./Food Access.jpg" alt="Comprehensive Food Access Map"/>
      </div>
    </section>

    <hr/>

    <section id="project2">
      <h2>🍎 Project 2: Food Deserts and Chronic Disease in DFW</h2>
      <p><strong>Objective:</strong> Assess the spatial link between food desert presence and obesity/diabetes rates using regression methods.</p>
      <p><strong>Approach:</strong> Employed Geographically Weighted Regression to evaluate local-level associations across DFW census tracts.</p>
      <h3>Key Results</h3>
      <ul>
        <li><strong>Obesity:</strong> R² = 0.52 (p = 0.008)</li>
        <li><strong>Diabetes:</strong> R² = 0.40 (p = 0.12, not significant)</li>
        <li>Strongest coefficients found in southern Dallas and western Tarrant counties.</li>
        <li>Food deserts alone not causal predictors (P > 0.27); stronger predictors included age 65+, education, race/ethnicity, poverty.</li>
      </ul>
      <h3>Integrated Model Performance</h3>
      <ul>
        <li>Obesity model: R² = 0.89</li>
        <li>Diabetes model: R² = 0.82</li>
      </ul>
      <div class="slider slider2">
        <img src="./GWR and Obesity.jpg" alt="GWR Obesity Analysis"/>
        <img src="./GWR and Diabtes.jpg" alt="GWR Diabetes Analysis"/>
        <img src="./Obesity and Food Deserts.jpg" alt="Obesity vs Food Deserts"/>
        <img src="./Diabetes and Food deserts.jpg" alt="Diabetes vs Food Deserts"/>
      </div>
      <p><strong>Interpretation:</strong> Food access shows strong associations with certain health outcomes locally, but causation is best explained via social determinants of health. Spatial modeling helps target public health interventions.</p>
    </section>

    <hr/>

    <section id="project3">
      <h2>🏥 Project 3: Liver Disease Mortality Patterns in Texas</h2>
      <p><strong>Challenge:</strong> Identify geographic and temporal liver disease mortality trends to pinpoint at-risk Texas communities.</p>
      <p><strong>Approach:</strong> Conducted a 20-year spatiotemporal analysis combining mortality data with socioeconomic and health metrics.</p>
      <h3>Spatial Analysis & Findings</h3>
      <ul>
        <li>Analyzed 207 Texas counties; detected 12 persistent hotspots in South & West Texas.</li>
        <li>Correlation strengths: diabetes (R² = 0.43), Hispanic population (R² = 0.32), obesity (R² = 0.30), income (R² = 0.25).</li>
      </ul>
      <div class="slider slider3">
        <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Hotspots"/>
        <img src="./AADR 2001-2007.jpg" alt="AADR 2001–2007"/>
        <img src="./AADR 2008-2014.jpg" alt="AADR 2008–2014"/>
        <img src="./AADR 2015-2020.jpg" alt="AADR 2015–2020"/>
        <img src="./Rate Change 1.jpg" alt="Mortality Rate Change Ⅰ"/>
        <img src="./Rate change 2.jpg" alt="Mortality Rate Change Ⅱ"/>
      </div>
      <p><strong>Interpretation:</strong> Liver disease risk is spatially concentrated. Regions such as South Texas, where multiple risk factors intersect, should guide policy and intervention focus.</p>
    </section>

    <hr/>

    <section id="project4">
      <h2>🏗️ Project 4: LiDAR Building Extraction in Waco, TX</h2>
      <p><strong>Challenge:</strong> Derive accurate building inventories and volume estimates for population modeling, avoiding expensive field surveys.</p>
      <p><strong>Objective:</strong> Estimate small-area population across 125 census blocks using LiDAR-derived building attributes.</p>
      <p><strong>Methodology:</strong> Processed high-resolution LiDAR (DSM/DTM/DHM) from TNRIS with ArcGIS Pro to extract building footprints, then calculated counts, areas, volumes; modeled population using OLS regression.</p>
      <table>
        <thead>
          <tr><th>Model</th><th>Metric</th><th>R²</th><th>Pop. Estimate</th><th>Error (%)</th></tr>
        </thead>
        <tbody>
          <tr><td>1</td><td>Building Count</td><td>0.6259</td><td>5,713.01</td><td>+0.0001%</td></tr>
          <tr><td>2</td><td>Building Area</td><td>0.5815</td><td>5,709.54</td><td>−0.06%</td></tr>
          <tr><td>3</td><td>Building Volume</td><td>0.1635</td><td>5,656.80</td><td>−0.98%</td></tr>
        </tbody>
      </table>
      <p><strong>Key Takeaways:</strong> Building count was the most reliable proxy for population in mixed-density Waco. Volume underperformed likely due to non-residential structures. Results align with literature on urban estimation proxies.</p>
      <p><strong>Implications:</strong> LiDAR-based methods show promise for urban planning, emergency response, and infrastructure. Future enhancements could include land-use data, sociodemographic context, or ML approaches.</p>
    </section>

    <hr/>

    <section id="skills">
      <h2>📈 Technical Skills</h2>
      <h3>GIS & Spatial Analysis</h3>
      <ul><li>Advanced cartography, spatial modeling, network & hotspot analysis, remote sensing, classification</li></ul>
      <h3>Programming & Data</h3>
      <ul><li>Python (ArcPy, Pandas, GeoPandas), SQL, SPSS, ArcGIS Online</li></ul>
      <h3>Professional Experience</h3>
      <ul><li>Project design & execution, data visualization, report writing, presentations & stakeholder engagement</li></ul>
    </section>

    <hr/>

    <section id="education">
      <h2>🎓 Education & Certifications</h2>
      <ul>
        <li><strong>M.S. in Geography</strong>, University of North Texas, 2025 (GIS & Health Geography)</li>
        <li><strong>B.A. in Geography & Resource Development</strong>, University of Ghana, 2018 (GIS, Urbanisation, Transport)</li>
      </ul>
      <p><strong>Relevant Coursework:</strong> Advanced GIS Analysis; Health Geography; Urban Planning; Spatial Statistics</p>
    </section>

    <hr/>

    <section id="contact">
      <h2>📞 Let's Connect</h2>
      <p>Seeking roles in GIS analysis, urban planning, and public health research. Let’s discuss how spatial insights can drive better decisions for your organization.</p>
      <p>
        📧 <strong>Email:</strong> <a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a><br/>
        💼 <strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/">Nicholas Lawson</a><br/>
        💻 <strong>GitHub:</strong> <a href="https://github.com/cwecu">cwecu</a><br/>
        📍 <strong>Location:</strong> Dallas–Fort Worth, TX
      </p>
    </section>

    <footer>
      <p><em>Portfolio last updated: June 2025</em></p>
    </footer>

  </div>

  <script>
    function setupSlideshow(selector, interval) {
      const sliders = document.querySelectorAll(selector);
      sliders.forEach(slider => {
        const imgs = slider.querySelectorAll("img");
        let i = 0;
        setInterval(() => {
          imgs[i].style.opacity = 0;
          i = (i + 1) % imgs.length;
          imgs[i].style.opacity = 1;
        }, interval);
      });
    }
    setupSlideshow(".slider1", 5000);
    setupSlideshow(".slider2", 6000);
    setupSlideshow(".slider3", 7000);
  </script>
</body>
</html>
