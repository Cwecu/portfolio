<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Nicholas Lawson | GIS Analyst Portfolio</title>
<style>
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    margin: 20px;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.6;
    color: #222;
  }
  img.profile {
    float: right;
    border-radius: 50%;
    width: 120px;
    margin-left: 20px;
    margin-bottom: 10px;
  }
  h2 {
    border-bottom: 2px solid #007acc;
    padding-bottom: 4px;
  }
  .slideshow-container {
    position: relative;
    max-width: 100%;
    margin: 20px auto 40px;
    overflow: hidden;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  .slideshow-container img {
    width: 100%;
    display: none;
  }
  .slideshow-container img.active {
    display: block;
  }
  /* Clear float */
  .clearfix::after {
    content: "";
    display: table;
    clear: both;
  }
  a {
    color: #007acc;
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
  }
  table {
    border-collapse: collapse;
    width: 100%;
    margin: 12px 0;
  }
  th, td {
    border: 1px solid #ccc;
    padding: 8px 12px;
    text-align: center;
  }
  th {
    background: #f0f0f0;
  }
  hr {
    border: none;
    border-top: 1px solid #ddd;
    margin: 40px 0;
  }
</style>
</head>
<body>

<h1>Nicholas Lawson | GIS Analyst Portfolio</h1>
<img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile" />

<section>
  <h2>👋 About Me</h2>
  <p>
    I am <strong>Nicholas Lawson</strong>, a recent Geography graduate with expertise in GIS, spatial analysis, and health geography. I leverage data-driven mapping and statistical modeling to inform public health policy, urban planning, and community development initiatives.
  </p>

  <h3>Core Competencies</h3>
  <ul>
    <li><strong>Software:</strong> ArcGIS Pro, QGIS, Python for GIS</li>
    <li><strong>Analysis:</strong> Geographically Weighted Regression (GWR), Network Analysis, Hotspot Analysis</li>
    <li><strong>Specializations:</strong> Health Geography, Urban Planning, LiDAR Processing</li>
  </ul>
</section>

<hr />

<section>
  <h2>🍎 Project 1: 🌆 Urbanization, Food Security & Spatial Access in DFW</h2>
  <p><strong>Challenge:</strong> Despite being part of a major metropolitan region, the urban cores of Dallas and Fort Worth continue to exhibit widespread food insecurity. Paradoxically, areas with high population density and infrastructure are home to some of the region's most persistent food deserts. Traditional definitions—based solely on proximity to supermarkets—fail to capture the lived realities of these communities, where cultural preferences, mobility limitations, and overlooked food retailers reshape access. This study addresses the spatial mismatch between where people live and where healthy food is truly available.</p>

  <p><strong>Approach:</strong> Comprehensive mapping that includes farmers' markets and ethnic grocery stores alongside traditional supermarkets to provide a more nuanced view of food access.</p>

  <p><strong>Tools Used:</strong> ArcGIS Pro, Network Analyst, USDA SNAP Retailer Locator, CDC PLACES, American Community Survey, Transport Network</p>

  <h3>Spatial Analysis:</h3>
  <ul>
    <li>Used Network Analyst to generate 1-mile service areas from food retailers.</li>
    <li>Expanded retailer dataset with ethnic stores and farmers' markets.</li>
  </ul>

  <h3>Summary Statistics:</h3>
  <ul>
    <li>Total food retailers: 1,023 (755 supermarkets, 241 small grocers, 27 farmers' markets)</li>
    <li>Census tracts analyzed: 1,536 (1,508 urban, 28 rural)</li>
    <li>Food desert tracts (traditional definition): 1,127</li>
    <li>Food desert tracts (expanded definition): 1,010 (10% reduction)</li>
    <li>Low-income food desert tracts dropped from 385 to 325 (16% reduction)</li>
  </ul>

  <div class="slideshow-container" id="slideshow1">
    <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map Analysis" class="active" />
    <img src="./Food Deserts hotspot.jpg" alt="Food Desert Hotspot Analysis" />
    <img src="./Food Access.jpg" alt="Food Access Comprehensive Map" />
  </div>
</section>

<hr />

<section>
  <h2>🍎 Project 2: Food Deserts and Chronic Disease in DFW: Association vs. Causality</h2>
  <p><strong>Objective:</strong> Examine the spatial relationship between food desert classification and the prevalence of obesity and diabetes using regression models.</p>
  <p><strong>Approach:</strong> Used Geographically Weighted Regression (GWR) to test local associations between food access and chronic disease rates across Dallas-Fort Worth census tracts.</p>

  <h3>Statistical Highlights:</h3>
  <ul>
    <li><strong>Obesity</strong>: R² = 0.52 (significant, p = 0.008)</li>
    <li><strong>Diabetes</strong>: R² = 0.40 (not significant, p = 0.12)</li>
    <li>Highest coefficients in southern Dallas and western Tarrant Counties</li>
  </ul>

  <h3>Factors:</h3>
  <ul>
    <li>Food deserts alone were <strong>not causal predictors</strong> of disease (p &gt; 0.27)</li>
    <li>Stronger predictors included:
      <ul>
        <li>Age 65+</li>
        <li>Education level</li>
        <li>Race/ethnicity (Black and Hispanic)</li>
        <li>Poverty</li>
      </ul>
    </li>
  </ul>

  <h3>Integrated Model Performance:</h3>
  <ul>
    <li>Obesity model R² = <strong>0.89</strong></li>
    <li>Diabetes model R² = <strong>0.82</strong></li>
  </ul>

  <div class="slideshow-container" id="slideshow2">
    <img src="./GWR and Obesity.jpg" alt="Geographically Weighted Regression - Obesity Analysis" class="active" />
    <img src="./GWR and Diabtes.jpg" alt="Geographically Weighted Regression - Diabetes Analysis" />
    <img src="./Obesity and Food Deserts.jpg" alt="Obesity and Food Deserts Correlation" />
    <img src="./Diabetes and Food deserts.jpg" alt="Diabetes and Food Deserts Correlation" />
  </div>

  <p><strong>Interpretation:</strong> Food access is <strong>associated</strong> with poor health outcomes in specific areas, but <strong>causality</strong> is best explained through a broader social determinants framework. Spatial modeling helps identify where food environments align with health risks, guiding targeted interventions.</p>
</section>

<hr />

<section>
  <h2>🏥 Project 3: Liver Disease Mortality Patterns in Texas</h2>
  <p><strong>Challenge:</strong> Understanding the geographic distribution and temporal trends of liver disease mortality to identify at-risk communities.</p>

  <p><strong>Approach:</strong> 20-year spatiotemporal analysis combining mortality data with socioeconomic and health indicators to identify hotspots and risk factors.</p>

  <p><strong>Tools Used:</strong> ArcGIS Pro, CDC WONDER, County Health Rankings, Geographically Weighted Regression (GWR)</p>

  <h3>Spatial Analysis:</h3>
  <ul>
    <li>Hotspot analysis identified persistent high mortality clusters.</li>
    <li>GWR analyzed local relationships between mortality and health/socioeconomic variables.</li>
  </ul>

  <h3>Summary Statistics:</h3>
  <ul>
    <li>Counties analyzed: 207</li>
    <li>Significant hotspots: 12 counties in south and west Texas</li>
    <li>Strongest variable correlations:
      <ul>
        <li>Diabetes (R² = 0.43)</li>
        <li>Hispanic population (R² = 0.32)</li>
        <li>Obesity (R² = 0.30)</li>
        <li>Income (R² = 0.25)</li>
      </ul>
    </li>
  </ul>

  <div class="slideshow-container" id="slideshow3">
    <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Mortality Hotspot Analysis" class="active" />
    <img src="./AADR 2001-2007.jpg" alt="Age-Adjusted Death Rates 2001-2007" />
    <img src="./AADR 2008-2014.jpg" alt="Age-Adjusted Death Rates 2008-2014" />
    <img src="./AADR 2015-2020.jpg" alt="Age-Adjusted Death Rates 2015-2020" />
    <img src="./Rate Change 1.jpg" alt="Mortality Rate Change Analysis 1" />
    <img src="./Rate change 2.jpg" alt="Mortality Rate Change Analysis 2" />
  </div>

  <p><strong>Interpretation:</strong> Public health risks are spatially clustered and vary regionally. Policy focus should be tailored for regions like South Texas where multiple risk factors converge.</p>
</section>

<hr />

<section>
  <h2>🏗️ Project 4: LiDAR Building Extraction in Waco, TX</h2>
  <p><strong>Challenge:</strong> Accurate building inventory and volume estimation for urban planning without costly field surveys.</p>

  <p><strong>Objective:</strong> Estimate small-area population using LiDAR-derived building metrics (count, area, volume) across 125 census blocks in Waco, Texas.</p>

  <p><strong>Study Area:</strong> Waco, a mid-sized city with 140,000 residents, offers a mix of urban, suburban, and semi-rural environments—ideal for testing population estimation models in transitional landscapes.</p>

  <p><strong>Approach:</strong> High-resolution LiDAR data (TNRIS) and 2020 Census block data were integrated using ArcGIS Pro. The methodology included:</p>
  <ul>
    <li>Generation of DSM, DTM, and DHM</li>
    <li>Building extraction (threshold &gt; 2.2m)</li>
    <li>Binary mask filtering and footprint vectorization</li>
    <li>Calculation of count, area, and volume metrics</li>
    <li>Population estimation using OLS regression models</li>
  </ul>

  <h3>Model Results:</h3>
  <table>
    <thead>
      <tr>
        <th>Model</th>
        <th>Metric Used</th>
        <th>R²</th>
        <th>Pop. Estimate</th>
        <th>Error (%)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td>Building Count</td>
        <td>0.6259</td>
        <td>5,713.01</td>
        <td>+0.0001%</td>
      </tr>
      <tr>
        <td>2</td>
        <td>Building Area</td>
        <td>0.5815</td>
        <td>5,709.54</td>
        <td>−0.06%</td>
      </tr>
      <tr>
        <td>3</td>
        <td>Building Volume</td>
        <td>0.1635</td>
        <td>5,656.80</td>
        <td>−0.98%</td>
      </tr>
    </tbody>
  </table>

  <h3>Key Takeaways:</h3>
  <ul>
    <li><strong>Building count</strong> was the most accurate and interpretable metric for population estimation in Waco's mixed-density environment.</li>
    <li><strong>Volume</strong> was the weakest predictor due to the influence of non-residential or tall commercial buildings.</li>
    <li>Results align with literature emphasizing building count and area as effective proxies in semi-urban contexts.</li>
  </ul>

  <h3>Implications:</h3>
  <ul>
    <li>Supports scalable LiDAR methods for urban planning, emergency response, and infrastructure management.</li>
    <li>Future work should incorporate land-use data, socio-demographic context, or machine learning for improved precision.</li>
  </ul>
</section>

<hr />

<section>
  <h2>📈 Technical Skills</h2>
  <h3>GIS & Spatial Analysis</h3>
  <ul>
    <li>Advanced cartography and spatial modeling</li>
    <li>Network analysis and service area optimization</li>
    <li>Regression, clustering, and spatial statistics</li>
    <li>Remote sensing and classification</li>
  </ul>

  <h3>Programming & Data</h3>
  <ul>
    <li>Python (ArcPy, Pandas, GeoPandas)</li>
    <li>SQL for spatial databases</li>
    <li>SPSS</li>
    <li>Web mapping: ArcGIS Pro, ArcGIS Online</li>
  </ul>

  <h3>Professional Experience</h3>
  <ul>
    <li>Project design, research, and execution</li>
    <li>Data visualization and report writing</li>
    <li>Public presentations and stakeholder engagement</li>
  </ul>
</section>

<hr />

<section>
  <h2>🎓 Education & Certifications</h2>
  <p><strong>Master of Science in Geography</strong><br />
  University of North Texas, 2025<br />
  Concentration: Geographic Information Systems &amp; Health and Medical Geography</p>

  <p><strong>Bachelor of Art in Geography and Resource Development</strong><br />
  University of Ghana, 2018<br />
  Concentration: Geographic Information Systems, Cities and Urbanisation, Transportation</p>

  <h3>Relevant Coursework</h3>
  <ul>
    <li>Advanced GIS Analysis</li>
    <li>Health Geography</li>
    <li>Urban Planning</li>
    <li>Spatial Statistics</li>
  </ul>
</section>

<hr />

<section>
  <h2>📞 Let's Connect</h2>
  <p>I'm actively seeking opportunities in GIS analysis, urban planning, and public health research. Let's discuss how spatial analysis can drive better decision-making in your organization.</p>
  <p>
    📧 <strong>Email:</strong> <a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a><br />
    💼 <strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank" rel="noopener noreferrer">Nicholas Lawson</a><br />
    💻 <strong>GitHub:</strong> <a href="https://github.com/cwecu" target="_blank" rel="noopener noreferrer">cwecu</a><br />
    📍 <strong>Location:</strong> Dallas-Fort Worth, Texas
  </p>
</section>

<hr />
<p><em>Portfolio last updated: June 2025</em></p>

<script>
  // Slideshow function for each slideshow container
  function initSlideshow(containerId, interval=
