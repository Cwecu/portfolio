
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nicholas Lawson | GIS Analyst Portfolio</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
        }

        .profile-container {
            display: flex;
            align-items: flex-start;
            gap: 30px;
            margin-bottom: 30px;
        }

        .profile-img {
            border-radius: 50%;
            width: 120px;
            height: 120px;
            object-fit: cover;
            flex-shrink: 0;
            border: 3px solid #e9ecef;
        }

        .profile-content {
            flex: 1;
        }

        h1 {
            color: #2c3e50;
            margin-bottom: 10px;
            font-size: 2.5em;
        }

        h2 {
            color: #34495e;
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
            margin-top: 40px;
        }

        h3 {
            color: #2c3e50;
            margin-top: 25px;
        }

        .competencies {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
        }

        .competencies ul {
            margin: 0;
            padding-left: 20px;
        }

        /* Slideshow Styles */
        .slideshow-container {
            position: relative;
            width: 100%;
            max-width: 1000px;
            margin: 20px auto;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
            background: #f8f9fa;
        }

        .slideshow-container img {
            width: 100%;
            height: 600px;
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

        /* Project sections */
        .project {
            background: #f8f9fa;
            padding: 25px;
            margin: 30px 0;
            border-radius: 15px;
            border-left: 5px solid #3498db;
        }

        .project h2 {
            border-bottom: none;
            color: #2c3e50;
            margin-top: 0;
        }

        .stats-table {
            background: white;
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .stats-table table {
            width: 100%;
            border-collapse: collapse;
        }

        .stats-table th,
        .stats-table td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        .stats-table th {
            background-color: #3498db;
            color: white;
        }

        .highlight-box {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            padding: 20px;
            border-radius: 10px;
            margin: 15px 0;
            border-left: 4px solid #2196f3;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .skill-category {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            border-top: 4px solid #3498db;
        }

        .contact-section {
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            margin-top: 40px;
        }

        .contact-section h2 {
            color: white;
            border-bottom: 3px solid #3498db;
        }

        .contact-section a {
            color: #3498db;
            text-decoration: none;
        }

        .contact-section a:hover {
            color: #5dade2;
        }

        @media (max-width: 768px) {
            .profile-container {
                flex-direction: column;
                text-align: center;
            }

            .slideshow-container img {
                height: 400px;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
        <div class="profile-content">
            <h1>Nicholas Lawson</h1>
            <h2>🗺️ GIS Analyst Portfolio</h2>
            
            <p>I am <strong>Nicholas Lawson</strong>, an aspiring professional with a strong foundation in geospatial data analysis, research, and project coordination. I have experience using tools such as ArcGIS Pro, and spatial analysis techniques to support data-driven decision-making. With a diverse background in education, business development, and client engagement, I bring a well-rounded perspective to geospatial projects. I am eager to apply my growing expertise in GIS to solve complex problems and contribute meaningfully to your organization's spatial initiatives.</p>
            
            <div class="competencies">
                <h3>Core Competencies</h3>
                <ul>
                    <li><strong>GIS Software:</strong> ArcGIS Pro, ArcGIS Online, QGIS, Python (ArcPy, GeoPandas)</li>
                    <li><strong>Spatial Analysis:</strong> Geographically Weighted Regression, Network Analysis, Hotspot Analysis, Service Area Modeling</li>
                    <li><strong>Data Management:</strong> SQL, PostgreSQL/PostGIS, Feature Class Design, Geodatabase Management</li>
                    <li><strong>Remote Sensing:</strong> LiDAR Processing, Image Classification, Digital Elevation Models</li>
                </ul>
            </div>
        </div>
    </div>

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

    <div class="project">
        <h2>🏥 Project 3: Spatiotemporal Mortality Analysis - Texas Liver Disease Surveillance</h2>
        
        <p><strong>Business Problem:</strong> State health departments requires comprehensive mortality surveillance system to identify emerging geographic clusters of liver disease and allocate prevention resources across Texas's 254 counties over a 20-year period.</p>

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
            <img src="./Rate change 2.jpg" alt="Mortality Rate Change Analysis 2">
        </div>

        <p><strong>Strategic Impact:</strong> This comprehensive surveillance system will enable state health officials to implement region-specific prevention strategies, resulting in 15% improvement in early detection programs and more efficient deployment of limited public health resources across high-risk geographic areas.</p>
    </div>

    <div class="project">
        <h2>🏗️ Project 4: Automated Population Estimation Using LiDAR Remote Sensing</h2>
        
        <p><strong>Business Problem:</strong> Municipal planning departments needs cost-effective method for small-area population estimation without expensive field surveys. Traditional census data becomes outdated quickly, creating gaps in infrastructure planning and emergency response preparation.</p>

        <p><strong>GIS Solution:</strong> Developed automated workflow using high-resolution LiDAR data to extract building metrics and create statistical models for population estimation. This remote sensing approach provides near real-time population estimates at census block level.</p>

        <p><strong>Technical Implementation:</strong>
        <br>• <strong>LiDAR Processing:</strong> Generated Digital Surface Model (DSM), Digital Terrain Model (DTM), and normalized Digital Height Model using ArcGIS Pro Spatial Analyst
        <br>• <strong>Feature Extraction:</strong> Applied 2.2m height threshold for building classification with morphological filtering to remove noise
        <br>• <strong>Geometric Analysis:</strong> Calculated building count, footprint area, and volume using 3D Analyst tools
        <br>• <strong>Statistical Modeling:</strong> Developed OLS regression models comparing LiDAR metrics against 2020 Census block data</p>

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

        <div class="highlight-box">
            <h3>Business Value & Applications:</h3>
            <ul>
                <li><strong>Cost Reduction:</strong> 90% reduction in survey costs compared to traditional field enumeration methods</li>
                <li><strong>Scalability:</strong> Methodology successfully transferable to other Texas municipalities with available LiDAR data</li>
                <li><strong>Real-Time Updates:</strong> Population estimates can be updated annually with new LiDAR acquisitions</li>
                <li><strong>Multi-Purpose Applications:</strong> Building inventory supports emergency response planning, utility infrastructure sizing, and zoning analysis</li>
            </ul>
        </div>

        <p><strong>Strategic Impact:</strong> This automated population estimation system will enable municipalities to make data-driven infrastructure and service delivery decisions without waiting for decennial census updates, supporting rapid response to urban growth and development patterns.</p>
    </div>

    <div class="skills-grid">
        <div class="skill-category">
            <h3>🗺️ GIS & Spatial Analysis</h3>
            <ul>
                <li><strong>e GIS:</strong> ArcGIS Pro, ArcGIS Online</li>
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

    <div class="project">
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

    <div class="contact-section">
        <h2>📞 Let's Connect</h2>
        <p>I'm actively seeking GIS Analyst opportunities where I can apply advanced spatial analysis and statistical modeling to solve complex business problems. My expertise in geospatial technology, combined with strong analytical skills, enables organizations to make data-driven decisions and optimize operations.</p>
        
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin-top: 20px;">
            <div>📧 <strong>Email:</strong><br><a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a></div>
            <div>💼 <strong>LinkedIn:</strong><br><a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank">Nicholas Lawson</a></div>
            <div>💻 <strong>GitHub:</strong><br><a href="https://github.com/cwecu" target="_blank">cwecu</a></div>
            <div>📍 <strong>Location:</strong><br>Dallas-Fort Worth, Texas</div>
        </div>
        
        <p style="margin-top: 30px; font-style: italic;">Portfolio last updated: June 2025</p>
    </div>

    <script>
        // Slideshow functionality
        class Slideshow {
            constructor(containerId, interval = 4000) {
                this.container = document.getElementById(containerId);
                this.images = this.container.querySelectorAll('img');
                this.currentSlide = 0;
                this.interval = interval;
                this.startSlideshow();
            }

            showSlide(index) {
                // Remove active class from all images
                this.images.forEach(img => img.classList.remove('active'));
                
                // Add active class to current image
                this.images[index].classList.add('active');
            }

            nextSlide() {
                this.currentSlide = (this.currentSlide + 1) % this.images.length;
                this.showSlide(this.currentSlide);
            }

            startSlideshow() {
                setInterval(() => {
                    this.nextSlide();
                }, this.interval);
            }
        }

        // Initialize slideshows when page loads
        document.addEventListener('DOMContentLoaded', function() {
            new Slideshow('slider1', 5000); // 5 second intervals
            new Slideshow('slider2', 6000); // 6 second intervals
            new Slideshow('slider3', 4000); // 4 second intervals
        });

        // Add smooth scrolling for any internal links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
