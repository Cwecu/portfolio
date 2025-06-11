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
            background-color: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            padding: 40px 20px;
            text-align: center;
            margin-bottom: 0;
        }

        .profile-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            max-width: 800px;
            margin: 0 auto;
        }

        .profile-img {
            border-radius: 50%;
            width: 120px;
            height: 120px;
            object-fit: cover;
            border: 4px solid rgba(255,255,255,0.2);
        }

        .profile-content h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .profile-content p {
            font-size: 1.2em;
            opacity: 0.9;
        }

        /* Tab Navigation */
        .tab-navigation {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 0;
        }

        .tab-nav {
            display: flex;
            max-width: 1200px;
            margin: 0 auto;
        }

        .tab-button {
            flex: 1;
            padding: 20px;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 1.1em;
            font-weight: 600;
            color: #666;
            border-bottom: 3px solid transparent;
            transition: all 0.3s ease;
        }

        .tab-button:hover {
            background-color: #f8f9fa;
            color: #2c3e50;
        }

        .tab-button.active {
            color: #3498db;
            border-bottom-color: #3498db;
            background-color: #fff;
        }

        /* Tab Content */
        .tab-content {
            background: white;
            min-height: 600px;
        }

        .tab-pane {
            display: none;
            padding: 40px;
            animation: fadeIn 0.3s ease-in;
        }

        .tab-pane.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Welcome Tab Styles */
        .welcome-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .competencies {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            text-align: left;
        }

        .competencies h3 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-size: 1.3em;
        }

        .competencies ul {
            list-style: none;
            padding: 0;
        }

        .competencies li {
            padding: 10px 0;
            border-bottom: 1px solid #ddd;
        }

        .competencies li:last-child {
            border-bottom: none;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 40px 0;
        }

        .skill-category {
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            border-top: 4px solid #3498db;
        }

        .skill-category h3 {
            color: #2c3e50;
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .skill-category ul {
            list-style: none;
            padding: 0;
        }

        .skill-category li {
            padding: 8px 0;
            color: #555;
        }

        /* Project Tab Styles */
        .project {
            background: #fff;
            padding: 30px;
            margin: 30px 0;
            border-radius: 15px;
            border-left: 5px solid #3498db;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .project h2 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-size: 1.5em;
        }

        .project h3 {
            color: #34495e;
            margin: 20px 0 10px 0;
        }

        .highlight-box {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            padding: 25px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #2196f3;
        }

        .stats-table {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            margin: 20px 0;
        }

        .stats-table table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            border-radius: 8px;
            overflow: hidden;
        }

        .stats-table th,
        .stats-table td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        .stats-table th {
            background-color: #3498db;
            color: white;
            font-weight: 600;
        }

        /* Slideshow Styles */
        .slideshow-container {
            position: relative;
            width: 100%;
            max-width: 900px;
            margin: 25px auto;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
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

        /* Experience Tab Styles */
        .experience-item {
            background: white;
            padding: 30px;
            margin: 25px 0;
            border-radius: 15px;
            border-left: 5px solid #27ae60;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .experience-item h3 {
            color: #2c3e50;
            font-size: 1.3em;
            margin-bottom: 5px;
        }

        .company-info {
            color: #7f8c8d;
            font-style: italic;
            margin-bottom: 15px;
            font-size: 1em;
        }

        .experience-item ul {
            list-style: none;
            padding: 0;
        }

        .experience-item li {
            padding: 8px 0;
            padding-left: 20px;
            position: relative;
            color: #555;
        }

        .experience-item li:before {
            content: "→";
            position: absolute;
            left: 0;
            color: #3498db;
            font-weight: bold;
        }

        /* Education Section */
        .education-section {
            background: linear-gradient(135deg, #f39c12, #e67e22);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
        }

        .education-section h2 {
            margin-bottom: 20px;
        }

        .education-item {
            background: rgba(255,255,255,0.1);
            padding: 20px;
            border-radius: 10px;
            margin: 15px 0;
        }

        /* Contact Section */
        .contact-section {
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            padding: 40px;
            border-radius: 15px;
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
            background: rgba(255,255,255,0.1);
            border-radius: 10px;
        }

        .contact-section a {
            color: #3498db;
            text-decoration: none;
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

            .tab-nav {
                flex-direction: column;
            }

            .tab-button {
                border-bottom: 1px solid #eee;
                border-right: none;
            }

            .tab-pane {
                padding: 20px;
            }

            .slideshow-container img {
                height: 300px;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .contact-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <div class="header">
        <div class="profile-container">
            <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
            <div class="profile-content">
                <h1>Nicholas Lawson</h1>
                <p>🗺️ GIS Analyst & Spatial Data Scientist</p>
            </div>
        </div>
    </div>

    <!-- Tab Navigation -->
    <div class="tab-navigation">
        <div class="tab-nav">
            <button class="tab-button active" onclick="openTab(event, 'welcome')">
                🏠 About Me
            </button>
            <button class="tab-button" onclick="openTab(event, 'projects')">
                📊 Projects
            </button>
            <button class="tab-button" onclick="openTab(event, 'experience')">
                💼 Experience
            </button>
        </div>
    </div>

    <!-- Tab Content -->
    <div class="tab-content">
        <!-- Welcome Tab -->
        <div id="welcome" class="tab-pane active">
            <div class="welcome-content">
                <h2>Welcome to My Portfolio</h2>
                <p style="font-size: 1.1em; margin: 20px 0;">I am <strong>Nicholas Lawson</strong>, an aspiring professional with a strong foundation in geospatial data analysis, research, and project coordination. I have experience using tools such as ArcGIS Pro, QGIS and spatial analysis techniques to support data-driven decision-making. With a diverse background in education, business development, and client engagement, I bring a well-rounded perspective to geospatial projects. I am eager to apply my growing expertise in GIS to solve complex problems and contribute meaningfully to your organization's spatial initiatives.</p>
                
                <div class="competencies">
                    <h3>🎯 Core Competencies</h3>
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
                            <li><strong>GIS:</strong> ArcGIS Pro, ArcGIS Online, QGIS</li>
                            <li><strong>Advanced Analysis:</strong> Network Analyst, Spatial Analyst, 3D Analyst, Geostatistical Analyst</li>
                            <li><strong>Statistical Methods:</strong> Geographically Weighted Regression, Hotspot Analysis, Spatial Autocorrelation</li>
                            <li><strong>Remote Sensing:</strong> LiDAR processing, Image classification, Change detection</li>
                        </ul>
                    </div>

                    <div class="skill-category">
                        <h3>💻 Programming & Data Management</h3>
                        <ul>
                            <li><strong>Python GIS:</strong> ArcPy, GeoPandas</li>
                            <li><strong>Database Management:</strong> SQL Server, File Geodatabase</li>
                            <li><strong>Statistical Software:</strong> R (spatial packages), SPSS, SAS</li>
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

                <div class="education-section">
                    <h2>🎓 Education & Certifications</h2>
                    
                    <div class="education-item">
                        <h3>Master of Science in Geography</h3>
                        <p><em>University of North Texas, 2025</em><br>
                        <em>Concentration: Geographic Information Systems & Health and Medical Geography</em></p>
                    </div>

                    <div class="education-item">
                        <h3>Bachelor of Art in Geography and Resource Development</h3>
                        <p><em>University of Ghana, 2018</em><br>
                        <em>Concentration: Geographic Information Systems, Cities and Urbanisation, Transportation</em></p>
                    </div>

                    <h3>Relevant Coursework</h3>
                    <ul style="list-style: none; padding: 0; margin-top: 15px;">
                        <li>• Advanced GIS Analysis</li>
                        <li>• Health Geography</li>
                        <li>• Urban Planning</li>
                        <li>• Spatial Statistics</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Projects Tab -->
        <div id="projects" class="tab-pane">
            <div class="project">
                <h2>🍎 Project 1: Multi-Criteria Food Access Analysis - Dallas-Fort Worth Metroplex</h2>
                
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
                        <li><strong>Policy Impact:</strong> Results shared with the City of Dallas at the 2025 North Texas Climate Symposium</li>
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

            <div class="project">
                <h2>🍎 Project 2: Geographically Weighted Regression Analysis - Chronic Disease & Food Environment</h2>
                
                <p><strong>Business Problem:</strong> Public health agencies needs to understand the spatial relationship between food environment and chronic disease prevalence to optimize intervention strategies and resource deployment across diverse Dallas-Fort Worth communities.</p>

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

                <div class="slideshow-container" id="slider2">
                    <img src="./GWR and Obesity.jpg" alt="Geographically Weighted Regression - Obesity Analysis" class="active">
                    <img src="./GWR and Diabtes.jpg" alt="Geographically Weighted Regression - Diabetes Analysis">
                    <img src="./Obesity and Food Deserts.jpg" alt="Obesity and Food Deserts Correlation">
                    <img src="./Diabetes and Food deserts.jpg" alt="Diabetes and Food Deserts Correlation">
                </div>

                <p><strong>Strategic Impact:</strong> This spatial analysis framework will enable public health agencies to shift from food-access-only interventions to comprehensive social determinants approaches, improving resource allocation efficiency and community health outcomes measurement.</p>
            </div>

            <div class="project">
                <h2>🏥 Project 3: Spatiotemporal Mortality Analysis - Texas Liver Disease Surveillance</h2>
                
                <p><strong>Business Problem:</strong> State health departments requires comprehensive mortality surveillance system to identify emerging geographic clusters of liver disease and allocate prevention resources across Texas's 254 counties over a 20-year period.</p>

                <p><strong>GIS Solution:</strong> Developed automated spatiotemporal analysis workflow combining CDC WONDER mortality data with County Health Rankings to identify persistent disease hotspots and quantify risk factor relationships using advanced spatial statistics.</p>

                <div class="highlight-box">
                    <h3>Quantifiable Results:</h3>
                    <ul>
                        <li><strong>12 persistent hotspot counties</strong> identified in South and West Texas regions</li>
                        <li><strong>87% prediction accuracy</strong> for high-mortality areas using integrated risk model</li>
                        <li><strong>4 distinct geographic clusters</strong> identified with different risk factor profiles</li>
                        <li><strong>Policy Impact:</strong> Analysis directly supported Texas Department of State Health Services regional resource allocation for liver disease prevention programs</li>
                    </ul>
                </div>

                <div class="slideshow-container" id="slider3">
                    <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Mortality Hotspot Analysis" class="active">
                    <img src="./AADR 2001-2007.jpg" alt="Age-Adjusted Death Rates 2001-2007">
                    <img src="./AADR 2008-2014.jpg" alt="Age-Adjusted Death Rates 2008-2014">
                    <img src="./AADR 2015-2020.jpg" alt="Age-Adjusted Death Rates 2015-2020">
                    <img src="./Rate Change 1.jpg" alt="Mortality Rate Change Analysis 1">
                    <img src="./Rate change 2.jpg" alt="Mortality Rate Change Analysis 2">
                </div>
            </div>

            <div class="project">
                <h2>🏗️ Project 4: Automated Population Estimation Using LiDAR Remote Sensing</h2>
                
                <p><strong>Business Problem:</strong> Municipal planning departments needs cost-effective method for small-area population estimation without expensive field surveys. Traditional census data becomes outdated quickly, creating gaps in infrastructure planning and emergency response preparation.</p>

                <p><strong>GIS Solution:</strong> Developed automated workflow using high-resolution LiDAR data to extract building metrics and create statistical models for population estimation. This remote sensing approach provides near real-time population estimates at census block level.</p>

                <div class="highlight-box">
                    <h3>Model Performance & Validation:</h3>
                    <p><strong>Study Area:</strong> 125 census blocks in Waco, TX (pop. 140,000) representing mixed urban-suburban-rural environments</p>
                    <ul>
                        <li><strong>Data Processing:</strong> Successfully extracted 3,247 building footprints from 1m resolution LiDAR</li>
                        <li><strong>Model Accuracy:</strong> Building count model achieved 99.99% accuracy (error: +0.0001%)</li>
                        <li><strong>Validation Method:</strong> Cross-validated against official 2020 Census block populations</li>
                        <li><strong>Processing Efficiency:</strong> Automated workflow reduced analysis time from weeks to 6 hours</li>
                    </ul>
                </div>

                <div class="stats-table">
                    <h3>Comparative Model Results:</h3>
                    <table>
                        <thead>
                            <tr>
                                <th>Model Type</th>
                                <th>LiDAR Metric</th>
                                <th>R² Value</th>
                                <th>Population Estimate</th>
                                <th>Accuracy Rate</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr style="background-color: #e8f5e8;">
                                <td><strong>Optimal Model</strong></td>
                                <td>Building Count</td>
                                <td>0.6259</td>
                                <td>5,713.01</td>
                                <td><strong>99.99%</strong></td>
                            </tr>
                            <tr>
                                <td>Secondary Model</td>
                                <td>Building Area (m²)</td>
                                <td>0.5815</td>
                                <td>5,709.54</td>
                                <td>99.94%</td>
                            </tr>
                            <tr>
                                <td>Alternative Model</td>
                                <td>Building Volume (m³)</td>
                                <td>0.1635</td>
                                <td>5,656.80</td>
                                <td>99.02%</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>

        <!-- Experience Tab -->
        <div id="experience" class="tab-pane">
            <h2 style="text-align: center; margin-bottom: 40px; color: #2c3e50;">Professional Experience</h2>
            
            <div class="experience-item">
                <h3>Teaching Assistant</h3>
                <div class="company-info">University of North Texas, Denton, TX | Aug 2023 – May 2025</div>
                <ul>
                    <li>Used ArcGIS tools in instructional labs to support spatial learning outcomes</li>
                    <li>Assisted in spatial data review, quality checks, and database updates for research activities</li>
                    <li>Managed student submissions and resolved technical issues in GIS software</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>Business Development Officer</h3>
                <div class="company-info">Sambus Geospatial Ltd., Accra, Ghana | Nov 2021 – Jul 2023</div>
                <ul>
                    <li>Delivered custom GIS solutions using ArcGIS, resulting in 30% growth in client accounts</li>
                    <li>Led training sessions and technical support for clients, improving GIS application rates</li>
                    <li>Advised on spatial data accuracy and usage across industries, ensuring high-quality output</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>Field Supervisor – 2021 Ghana Population and Housing Census</h3>
                <div class="company-info">Ghana Statistical Service | May 2021 – Aug 2021</div>
                <ul>
                    <li>Supervised enumeration teams for the national census, achieving 98% accuracy in data reporting</li>
                    <li>Managed and organized paper-based and digital work packets for archiving</li>
                    <li>Resolved logistical issues and coordinated stakeholder engagement to ensure full area coverage</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>Customer Service Executive</h3>
                <div class="company-info">Sporty Group, Accra, Ghana | Dec 2020 – Nov 2021</div>
                <ul>
                    <li>Provided technical support and monitored ticket resolutions to maintain service quality</li>
                    <li>Implemented QA measures to assess service call performance and user satisfaction</li>
                    <li>Achieved 95% customer satisfaction through consistent issue tracking and resolution</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>Communication/Administrative Assistant</h3>
                <div class="company-info">University of Ghana – Public Affairs Directorate | 2018 – 2019</div>
                <ul>
                    <li>Produced internal communications and maintained department files with QA oversight</li>
                    <li>Audited event documentation and reports for accuracy before release</li>
                    <li>Streamlined administrative records, contributing to improved process efficiency</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>GIS & Transportation Intern</h3>
                <div class="company-info">Greater Accra Passenger Transport Executive (GAPTE) | Jun 2017 – Aug 2017</div>
                <ul>
                    <li>Analyzed driver route data and submitted summary reports on system performance</li>
                    <li>Assisted with QA of GIS transit data and supported documentation for regulatory compliance</li>
                </ul>
            </div>

            <div class="experience-item">
                <h3>
