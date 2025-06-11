<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nicholas Lawson | GIS Analyst Portfolio</title>
  <style>
    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      margin: 0;
      background-color: #f9f9f9;
    }
    .tabs {
      display: flex;
      background-color: #2c3e50;
      overflow: hidden;
    }
    .tablink {
      flex: 1;
      padding: 14px 16px;
      background-color: inherit;
      color: white;
      text-align: center;
      text-decoration: none;
      border: none;
      outline: none;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    .tablink:hover {
      background-color: #1abc9c;
    }
    .tabcontent {
      display: none;
      padding: 30px;
      background-color: white;
    }
    .active-tab {
      background-color: #1abc9c;
    }
    h2 {
      color: #34495e;
      border-bottom: 3px solid #3498db;
      padding-bottom: 10px;
    }
    ul {
      padding-left: 20px;
    }
    li {
      margin-bottom: 8px;
    }
  </style>
</head>
<body>

<div class="tabs">
  <button class="tablink active-tab" onclick="openTab(event, 'About')">About Me</button>
  <button class="tablink" onclick="openTab(event, 'Projects')">Projects</button>
  <button class="tablink" onclick="openTab(event, 'Experience')">Professional Experience</button>
</div>

<div id="About" class="tabcontent" style="display: block;">
  <h2>👋 About Me</h2>
  <p>I am <strong>Nicholas Lawson</strong>, a Geography graduate passionate about GIS and spatial analysis. My skills include ArcGIS Pro, QGIS, spatial statistics, and remote sensing. I enjoy developing data-driven maps and solutions to address real-world problems.</p>
  <h3>Core Skills</h3>
  <ul>
    <li>GIS Software: ArcGIS Pro, QGIS, ArcGIS Online</li>
    <li>Programming: Python (ArcPy, GeoPandas), SQL</li>
    <li>Spatial Analysis: Network Analysis, Hotspot Mapping, GWR</li>
    <li>Remote Sensing: LiDAR, Raster Analysis</li>
  </ul>
</div>

<div id="Projects" class="tabcontent">
  <h2>📊 GIS Projects</h2>

  <h3>Project 1: Multi-Criteria Food Access Analysis - Dallas-Fort Worth Metroplex</h3>
  <p>Mapped food accessibility by integrating ethnic grocers, farmers' markets, and supermarkets using ArcGIS Network Analyst and service area modeling.</p>
  <ul>
    <li>Enhanced USDA methodology with 1,023 total retailer locations</li>
    <li>Reduced low-income food desert tracts by 16%</li>
    <li>Presented at the 2025 North Texas Climate Symposium</li>
  </ul>

  <h3>Project 2: Geographically Weighted Regression - Chronic Disease & Food Environment</h3>
  <p>Used GWR to explore the spatial variability in obesity and diabetes rates across DFW in relation to food access and social determinants.</p>
  <ul>
    <li>R² = 0.89 (obesity), R² = 0.82 (diabetes)</li>
    <li>Spatial clusters identified in southern Dallas & western Tarrant Counties</li>
    <li>Model guided Dallas County's health intervention strategies</li>
  </ul>

  <h3>Project 3: Texas Liver Disease Surveillance - Spatiotemporal Analysis</h3>
  <p>Analyzed mortality trends using 20 years of liver disease death rates to detect hotspots using Getis-Ord Gi* and spatial autocorrelation.</p>
  <ul>
    <li>12 persistent hotspot counties identified</li>
    <li>87% predictive accuracy for high-mortality areas</li>
    <li>Supported DSHS resource allocation</li>
  </ul>

  <h3>Project 4: Automated Population Estimation Using LiDAR</h3>
  <p>Used 3D building metrics from LiDAR data to estimate population in Waco, TX through regression analysis compared with census data.</p>
  <ul>
    <li>99.99% accuracy using building count model</li>
    <li>Processed 3,247 footprints across 125 census blocks</li>
    <li>Reduced analysis time from weeks to 6 hours</li>
  </ul>
</div>

<div id="Experience" class="tabcontent">
  <h2>💼 Professional Experience</h2>
  <ul>
    <li><strong>Teaching Assistant</strong> – University of North Texas, Denton, TX (Aug 2023 – May 2025)
      <ul>
        <li>Used ArcGIS tools in instructional labs to support spatial learning outcomes.</li>
        <li>Assisted in spatial data review, quality checks, and database updates for research activities.</li>
        <li>Managed student submissions and resolved technical issues in GIS software.</li>
      </ul>
    </li>
    <li><strong>Business Development Officer</strong> – Sambus Geospatial Ltd., Accra, Ghana (Nov 2021 – Jul 2023)
      <ul>
        <li>Delivered custom GIS solutions using ArcGIS, resulting in 30% growth in client accounts.</li>
        <li>Led training sessions and technical support for clients, improving GIS application rates.</li>
        <li>Advised on spatial data accuracy and usage across industries.</li>
      </ul>
    </li>
    <li><strong>Field Supervisor</strong> – Ghana Statistical Service (May 2021 – Aug 2021)
      <ul>
        <li>Supervised census enumeration teams and achieved 98% accuracy.</li>
        <li>Managed logistical issues and ensured full coverage of assigned areas.</li>
      </ul>
    </li>
    <li><strong>Customer Service Executive</strong> – Sporty Group, Accra (Dec 2020 – Nov 2021)
      <ul>
        <li>Monitored and resolved technical issues with 95% customer satisfaction.</li>
        <li>Implemented QA for support calls and ticket management.</li>
      </ul>
    </li>
    <li><strong>Communication/Administrative Assistant</strong> – University of Ghana (2018 – 2019)</li>
    <li><strong>GIS & Transportation Intern</strong> – GAPTE (Jun 2017 – Aug 2017)</li>
    <li><strong>Vital Records Intern</strong> – Birth and Death Registry (Jun 2016 – Aug 2016)</li>
  </ul>
</div>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active-tab", "");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active-tab";
}
</script>

</body>
</html>
