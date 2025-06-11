<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nicholas Lawson | GIS Analyst Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            text-align: center;
        }

        .profile-container {
            display: flex;
            align-items: center;
            gap: 30px;
            margin-bottom: 20px;
        }

        .profile-img {
            border-radius: 50%;
            width: 120px;
            height: 120px;
            object-fit: cover;
            border: 4px solid #667eea;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        .profile-content h1 {
            color: #2c3e50;
            font-size: 2.5em;
            margin-bottom: 10px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .profile-content h2 {
            color: #34495e;
            font-size: 1.3em;
            margin-bottom: 15px;
        }

        /* Tab Navigation */
        .tab-nav {
            display: flex;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 10px;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            overflow-x: auto;
            gap: 5px;
        }

        .tab-btn {
            flex: 1;
            padding: 15px 20px;
            background: transparent;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            color: #64748b;
            white-space: nowrap;
            min-width: 120px;
        }

        .tab-btn.active {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .tab-btn:hover:not(.active) {
            background: rgba(102, 126, 234, 0.1);
            transform: translateY(-1px);
        }

        /* Tab Content */
        .tab-content {
            display: none;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            animation: fadeIn 0.5s ease;
        }

        .tab-content.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h2 {
            color: #2c3e50;
            font-size: 1.8em;
            margin-bottom: 25px;
            padding-bottom: 10px;
            border-bottom: 3px solid;
            border-image: linear-gradient(135deg, #667eea, #764ba2) 1;
        }

        h3 {
            color: #2c3e50;
            margin: 25px 0 15px 0;
            font-size: 1.3em;
        }

        .competencies {
            background: linear-gradient(135deg, #f8f9ff, #e8f0fe);
            padding: 25px;
            border-radius: 15px;
            margin: 25px 0;
            border-left: 5px solid #667eea;
        }

        .competencies ul {
            margin: 0;
            padding-left: 20px;
        }

        .competencies li {
            margin-bottom: 8px;
        }

        /* Project Navigation */
        .project-nav {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-bottom: 30px;
            justify-content: center;
        }

        .project-nav-btn {
            padding: 12px 20px;
            background: linear-gradient(135deg, #f8f9ff, #e8f0fe);
            border: 2px solid #667eea;
            border-radius: 10px;
            cursor: pointer;
            font-weight: 600;
            color: #2c3e50;
            transition: all 0.3s ease;
            white-space: nowrap;
        }

        .project-nav-btn.active {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .project-nav-btn:hover:not(.active) {
            background: rgba(102, 126, 234, 0.1);
            transform: translateY(-1px);
        }

        /* Project Styles */
        .project-grid {
            display: grid;
            gap: 30px;
        }

        .project-card {
            background: linear-gradient(135deg, #f8f9ff, #e8f0fe);
            padding: 30px;
            border-radius: 20px;
            border-left: 6px solid #667eea;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: none;
        }

        .project-card.active {
            display: block;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .project-card h3 {
            color: #2c3e50;
            font-size: 1.4em;
            margin-bottom: 20px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .highlight-box {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            padding: 20px;
            border-radius: 15px;
            margin: 20px 0;
            border-left: 4px solid #2196f3;
        }

        .stats-table {
            background: white;
            border-radius: 15px;
            padding: 25px;
            margin: 25px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .stats-table table {
            width: 100%;
            border-collapse: collapse;
        }

        .stats-table th,
        .stats-table td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid #e0e0e0;
        }

        .stats-table th {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            font-weight: 600;
        }

        /* Slideshow Styles */
        .slideshow-container {
            position: relative;
            width: 100%;
            max-width: 800px;
            margin: 25px auto;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
            background: #f8f9fa;
        }

        .slideshow-container img {
            width: 100%;
            height: 500px;
            object-fit: contain;
            position: absolute;
            top: 0;
            left: 0;
            opacity: 0;
            transition: opacity 1s ease-in-out;
            background: white;
        }

        .slideshow-container img.active {
            opacity: 1;
        }

        .slideshow-container img:first-child {
            position: relative;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .skill-category {
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-top: 4px solid #667eea;
            transition: transform 0.3s ease;
        }

        .skill-category:hover {
            transform: translateY(-5px);
        }

        .skill-category h3 {
            color: #2c3e50;
            font-size: 1.2em;
            margin-bottom: 15px;
        }

        /* Experience Styles */
        .experience-item {
            background: linear-gradient(135deg, #f8f9ff, #e8f0fe);
            padding: 25px;
            border-radius: 15px;
            margin: 20px 0;
            border-left: 5px solid #667eea;
            transition: transform 0.3s ease;
        }

        .experience-item:hover {
            transform: translateX(5px);
        }

        .job-title {
            font-size: 1.3em;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 5px;
        }

        .company-info {
            color: #667eea;
            font-weight: 600;
            margin-bottom: 10px;
        }

        .date-range {
            color: #64748b;
            font-style: italic;
            margin-bottom: 15px;
        }

        .job-responsibilities {
            list-style: none;
            padding-left: 0;
        }

        .job-responsibilities li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }

        .job-responsibilities li:before {
            content: "▸";
            color: #667eea;
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* Contact Section */
        .contact-section {
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            margin-top: 40px;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .contact-item {
            padding: 15px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            transition: background 0.3s ease;
        }

        .contact-item:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        .contact-section a {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
        }

        .contact-section a:hover {
            color: #5dade2;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .profile-container {
                flex-direction: column;
                text-align: center;
            }

            .container {
                padding: 10px;
            }

            .tab-content {
                padding: 25px;
            }

            .slideshow-container img {
                height: 300px;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .tab-nav {
                flex-wrap: wrap;
            }

            .tab-btn {
                min-width: 100px;
                font-size: 0.9em;
            }

            .project-nav {
                flex-direction: column;
                align-items: center;
            }

            .project-nav-btn {
                width: 100%;
                max-width: 300px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="profile-container">
                <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
                <div class="profile-content">
                    <h1>Nicholas Lawson</h1>
                    <h2>🗺️ GIS Analyst & Spatial Data Scientist</h2>
                    <p>Geography graduate specializing in GIS analysis, spatial modeling, and health geography. Combining advanced geospatial technologies with statistical analysis to solve complex urban planning and public health challenges.</p>
                </div>
            </div>
        </div>

        <div class="tab-nav">
            <button class="tab-btn active" onclick="showTab('welcome')">🏠 Welcome</button>
            <button class="tab-btn" onclick="showTab('projects')">📊 Projects</button>
            <button class="tab-btn" onclick="showTab('experience')">💼 Experience</button>
        </div>

        <!-- Welcome Tab -->
        <div id="welcome" class="tab-content active">
            <h2>Welcome to My Portfolio</h2>
            
            <p>I am <strong>Nicholas Lawson</strong>, a Geography graduate specializing in GIS analysis, spatial modeling, and health geography. I combine advanced geospatial technologies with statistical analysis to solve complex urban planning and public health challenges, delivering actionable insights that drive evidence-based decision making.</p>
            
            <div class="competencies">
                <h3>Core Competencies</h3>
                <ul>
                    <li><strong>GIS Software:</strong> ArcGIS Pro, ArcGIS Online, QGIS, Python (ArcPy, GeoPandas)</li>
                    <li><strong>Spatial Analysis:</strong> Geographically Weighted Regression, Network Analysis, Hotspot Analysis, Service Area Modeling</li>
                    <li><strong>Data Management:</strong> SQL, PostgreSQL/PostGIS, Feature Class Design, Geodatabase Management</li>
                    <li><strong>Remote Sensing:</strong> LiDAR Processing, Image Classification, Digital Elevation Models</li>
                </ul>
            </div>

            <div class="skills-grid">
                <div class="skill-category">
                    <h3>🗺️ GIS & Spatial Analysis</h3>
                    <ul>
                        <li><strong>Enterprise GIS:</strong> ArcGIS Pro, ArcGIS Online, Portal for ArcGIS</li>
                        <li><strong>Advanced Analysis:</strong> Network Analyst, Spatial Analyst, 3D Analyst, Geostatistical Analyst</li>
                        <li><strong>Statistical Methods:</strong> Geographically Weighted Regression, Hotspot Analysis, Spatial Autocorrelation</li>
                        <li><strong>Remote Sensing:</strong> LiDAR processing, Image classification, Change detection</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h3>💻 Programming & Data Management</h3>
                    <ul>
                        <li><strong>Python GIS:</strong> ArcPy, GeoPandas, Shapely, Rasterio, GDAL</li>
                        <li><strong>Database Management:</strong> PostgreSQL/PostGIS, SQL Server, File Geodatabase</li>
                        <li><strong>Statistical Software:</strong> R (spatial packages), SPSS, SAS</li>
                        <li><strong>Web Development:</strong> ArcGIS JavaScript API, Leaflet, HTML/CSS</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h3>📊 Business & Communication</h3>
                    <ul>
                        <li><strong>Project Management:</strong> Requirements gathering, timeline development, stakeholder coordination</li>
                        <li><strong>Data Visualization:</strong> Dashboard creation, executive reporting, cartographic design</li>
                        <li><strong>Client Relations:</strong> Technical presentation, training delivery, solution consulting</li>
                        <li><strong>Documentation:</strong> Technical writing, methodology documentation, user guides</li>
                    </ul>
                </div>
            </div>

            <h2>🎓 Education & Certifications</h2>
            
            <div class="highlight-box">
                <h3>Master of Science in Geography</h3>
                <p><em>University of North Texas, 2025</em><br>
                <em>Concentration: Geographic Information Systems & Health and Medical Geography</em></p>
            </div>

            <div class="highlight-box">
                <h3>Bachelor of Art in Geography and Resource Development</h3>
                <p><em>University of Ghana, 2018</em><br>
                <em>Concentration: Geographic Information Systems, Cities and Urbanisation, Transportation</em></p>
            </div>

            <h3>Relevant Coursework</h3>
            <ul>
                <li>Advanced GIS Analysis</li>
                <li>Health Geography</li>
                <li>Urban Planning</li>
                <li>Spatial Statistics</li>
            </ul>
        </div>

        <!-- Projects Tab -->
        <div id="projects" class="tab-content">
            <h2>📊 Featured Projects</h2>
            
            <div class="project-nav">
                <button class="project-nav-btn active" onclick="showProject('project1')">🍎 Food Access Analysis</button>
                <button class="project-nav-btn" onclick="showProject('project2')">📊 Health Analysis</button>
                <button class="project-nav-btn" onclick="showProject('project3')">🏥 Mortality Study</button>
                <button class="project-nav-btn" onclick="showProject('project4')">🏗️ LiDAR Analysis</button>
            </div>

            <!-- Project 1 -->
            <div id="project1" class="project-card active">
                <h3>🍎 Multi-Criteria Food Access Analysis - Dallas-Fort Worth Metroplex</h3>
                
                <p><strong>Business Problem:</strong> Traditional food desert mapping underestimates food accessibility in diverse urban communities by excluding culturally-relevant retailers and alternative food sources. This creates gaps in public health planning and community development resource allocation across the 1,536 census tracts in the DFW region.</p>

                <p><strong>GIS Solution:</strong> Developed a comprehensive spatial analysis framework integrating Network Analyst with expanded retailer datasets to create more accurate food accessibility models. Enhanced traditional USDA methodology by incorporating ethnic grocery stores, farmers' markets, and culturally-specific food retailers.</p>

                <p><strong>Technical Implementation:</strong>
                <br>• <strong>Data Integration:</strong> Merged USDA SNAP retailer data with custom-geocoded ethnic grocers and farmers' markets (1,023 total locations)
                <br>• <strong>Network Analysis:</strong> Generated 1-mile walking and driving service areas using ArcGIS Network Analyst with real-time traffic data
                <br>• <strong>Spatial Join Operations:</strong> Calculated population-weighted accessibility metrics for 1,536 census tracts
                <br>• <strong>Statistical Validation:</strong> Applied chi-square tests to validate improved classification accuracy</p>

                <div class="highlight-box">
                    <h3>Quantifiable Results:</h3>
                    <ul>
                        <li><strong>16% reduction</strong> in low-income food desert classification (385 → 325 tracts)</li>
                        <li><strong>10% improvement</strong> in overall food access mapping accuracy (1,127 → 1,010 desert tracts)</li>
                        <li><strong>Enhanced data quality:</strong> Expanded retailer database by 268 previously unmapped locations</li>
                        <li><strong>Policy Impact:</strong> Results adopted by Dallas County Health Department for resource allocation planning</li>
                    </ul>
                </div>

                <div class="stats-table">
                    <h3>Summary Statistics:</h3>
                    <ul>
                        <li>Total food retailers: 1,023 (755 supermarkets, 241 small grocers, 27 farmers' markets)</li>
                        <li>Census tracts analyzed: 1,536 (1,508 urban, 28 rural)</li>
                        <li>Food desert tracts (traditional definition): 1,127</li>
                        <li>Food desert tracts (expanded definition): 1,010 (10% reduction)</li>
                        <li>Low-income food desert tracts dropped from 385 to 325 (16% reduction)</li>
                    </ul>
                </div>

                <div class="slideshow-container" id="slider1">
                    <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map Analysis" class="active">
                    <img src="./Food Deserts hotspot.jpg" alt="Food Desert Hotspot Analysis">
                    <img src="./Food Access.jpg" alt="Food Access Comprehensive Map">
                </div>
            </div>

            <!-- Project 2 -->
            <div id="project2" class="project-card">
                <h3>📊 Geographically Weighted Regression Analysis - Chronic Disease & Food Environment</h3>
                
                <p><strong>Business Problem:</strong> Public health agencies needed to understand the spatial relationship between food environment and chronic disease prevalence to optimize intervention strategies and resource deployment across diverse Dallas-Fort Worth communities.</p>

                <p><strong>Analytical Approach:</strong> Applied advanced spatial statistics using Geographically Weighted Regression (GWR) to model local variations in obesity and diabetes rates, moving beyond traditional global correlation models to identify spatially-varying relationships.</p>

                <p><strong>Technical Implementation:</strong>
                <br>• <strong>Data Preparation:</strong> Integrated CDC PLACES health data with ACS demographic variables across 1,400+ census tracts
                <br>• <strong>GWR Modeling:</strong> Executed local regression analysis using ArcGIS Pro to identify spatial heterogeneity in disease-environment relationships
                <br>• <strong>Model Validation:</strong> Applied Akaike Information Criterion (AIC) and residual analysis for model selection
                <br>• <strong>Hotspot Analysis:</strong> Used Getis-Ord Gi* statistics to identify significant disease clusters</p>

                <div class="highlight-box">
                    <h3>Statistical Results & Model Performance:</h3>
                    <ul>
                        <li><strong>GWR Obesity Model:</strong> R² = 0.52, statistically significant (p < 0.01)</li>
                        <li><strong>GWR Diabetes Model:</strong> R² = 0.40, moderate correlation (p = 0.12)</li>
                        <li><strong>Integrated Multi-Variable Model:</strong> R² = 0.89 (obesity), R² = 0.82 (diabetes)</li>
                        <li><strong>Spatial Clustering:</strong> Highest disease coefficients concentrated in southern Dallas and western Tarrant Counties</li>
                    </ul>
                </div>

                <div class="stats-table">
                    <h3>Key Analytical Findings:</h3>
                    <ul>
                        <li><strong>Primary Discovery:</strong> Food environment shows spatial association but not direct causality with chronic disease (p > 0.27)</li>
                        <li><strong>Significant Predictors Identified:</strong>
                            <ul>
                                <li>Population aged 65+ (β = 0.34, p < 0.001)</li>
                                <li>Educational attainment (β = -0.28, p < 0.01)</li>
                                <li>Race/ethnicity composition (β = 0.31, p < 0.01)</li>
                                <li>Poverty rate (β = 0.42, p < 0.001)</li>
                            </ul>
                        </li>
                        <li><strong>Business Value:</strong> Analysis informed targeted intervention strategies for Dallas County Health Department, prioritizing social determinants over food access alone</li>
                    </ul>
                </div>

                <div class="slideshow-container" id="slider2">
                    <img src="./GWR and Obesity.jpg" alt="Geographically Weighted Regression - Obesity Analysis" class="active">
                    <img src="./GWR and Diabtes.jpg" alt="Geographically Weighted Regression - Diabetes Analysis">
                    <img src="./Obesity and Food Deserts.jpg" alt="Obesity and Food Deserts Correlation">
                    <img src="./Diabetes and Food deserts.jpg" alt="Diabetes and Food Deserts Correlation">
                </div>

                <p><strong>Strategic Impact:</strong> This spatial analysis framework enabled public health agencies to shift from food-access-only interventions to comprehensive social determinants approaches, improving resource allocation efficiency and community health outcomes measurement.</p>
            </div>

            <!-- Project 3 -->
            <div id="project3" class="project-card">
                <h3>🏥 Spatiotemporal Mortality Analysis - Texas Liver Disease Surveillance</h3>
                
                <p><strong>Business Problem:</strong> State health departments required comprehensive mortality surveillance system to identify emerging geographic clusters of liver disease and allocate prevention resources across Texas's 254 counties over a 20-year period.</p>

                <p><strong>GIS Solution:</strong> Developed automated spatiotemporal analysis workflow combining CDC WONDER mortality data with County Health Rankings to identify persistent disease hotspots and quantify risk factor relationships using advanced spatial statistics.</p>

                <p><strong>Technical Implementation:</strong>
                <br>• <strong>Data Integration:</strong> Processed 20 years of age-adjusted death rates across 207 counties with complete datasets
                <br>• <strong>Hotspot Analysis:</strong> Applied Getis-Ord Gi* statistics with temporal weighting to identify persistent clusters
                <br>• <strong>GWR Analysis:</strong> Modeled local relationships between mortality and 15+ socioeconomic/health variables
                <br>• <strong>Trend Analysis:</strong> Calculated rate-of-change statistics across three temporal periods (2001-2007, 2008-2014, 2015-2020)</p>

                <div class="highlight-box">
                    <h3>Quantifiable Results:</h3>
                    <ul>
                        <li><strong>12 persistent hotspot counties</strong> identified in South and West Texas regions</li>
                        <li><strong>87% prediction accuracy</strong> for high-mortality areas using integrated risk model</li>
                        <li><strong>4 distinct geographic clusters</strong> identified with different risk factor profiles</li>
                        <li><strong>Policy Impact:</strong> Analysis directly supported Texas Department of State Health Services regional resource allocation for liver disease prevention programs</li>
                    </ul>
                </div>

                <div class="stats-table">
                    <h3>Statistical Analysis Results:</h3>
                    <ul>
                        <li><strong>Dataset:</strong> 207 counties analyzed with complete 20-year mortality records</li>
                        <li><strong>Spatial Autocorrelation:</strong> Moran's I = 0.34 (p < 0.001), confirming significant clustering</li>
                        <li><strong>Top Predictive Variables (GWR coefficients):</strong>
                            <ul>
                                <li>Diabetes prevalence: R² = 0.43, β = 0.38</li>
                                <li>Hispanic population percentage: R² = 0.32, β = 0.29</li>
                                <li>Adult obesity rate: R² = 0.30, β = 0.26</li>
                                <li>Median household income: R² = 0.25, β = -0.22</li>
                            </ul>
                        </li>
                        <li><strong>Temporal Trends:</strong> 23% increase in mortality rates in hotspot counties vs. 8% statewide average</li>
                    </ul>
                </div>

                <div class="slideshow-container" id="slider3">
                    <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Mortality Hotspot Analysis" class="active">
                    <img src="./AADR 2001-2007.jpg" alt="Age-Adjusted Death Rates 2001-2007">
                    <img src="./AADR 2008-2014.jpg" alt="Age-Adjusted Death Rates 2008-2014">
                    <img src="./AADR 2015-2020.jpg" alt="Age-Adjusted Death Rates 2015-2020">
                    <img src="./Rate Change 1.jpg" alt="Mortality Rate Change Analysis 1">
                    <img src="./Rate change 2.jpg" alt="Rate Change Analysis 2">
                </div>

                <p><strong>Strategic Impact:</strong> This comprehensive surveillance system enabled state health officials to implement region-specific prevention strategies, resulting in 15% improvement in early detection programs and more efficient deployment of limited public health resources across high-risk geographic areas.</p>
            </div>

            <!-- Project 4 -->
            <div id="project4" class="project-card">
                <h3>🏗️ Automated Population Estimation Using LiDAR Remote Sensing</h3>
                
                <p><strong>Business Problem:</strong> Municipal planning departments needed cost-effective method for small-area population estimation without expensive field surveys. Traditional census data becomes outdated quickly, creating gaps in infrastructure planning and emergency response preparation.</p>

                <p><strong>GIS Solution:</strong>
