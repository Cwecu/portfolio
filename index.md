<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nicholas Lawson
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
            
            <p>I am <strong>Nicholas Lawson</strong>, a recent Geography graduate with expertise in GIS, spatial analysis, and health geography. I leverage data-driven mapping and statistical modeling to inform public health policy, urban planning, and community development initiatives.</p>
            
            <div class="competencies">
                <h3>Core Competencies</h3>
                <ul>
                    <li><strong>Software:</strong> ArcGIS Pro, QGIS, Python for GIS</li>
                    <li><strong>Analysis:</strong> Geographically Weighted Regression (GWR), Network Analysis, Hotspot Analysis</li>
                    <li><strong>Specializations:</strong> Health Geography, Urban Planning, LiDAR Processing</li>
                </ul>
            </div>
        </div>
    </div>

    <div class="project">
        <h2>🍎 Project 1: 🌆 Urbanization, Food Security & Spatial Access in DFW</h2>
        
        <p><strong>Challenge:</strong> Despite being part of a major metropolitan region, the urban cores of Dallas and Fort Worth continue to exhibit widespread food insecurity. Paradoxically, areas with high population density and infrastructure are home to some of the region's most persistent food deserts. Traditional definitions—based solely on proximity to supermarkets—fail to capture the lived realities of these communities, where cultural preferences, mobility limitations, and overlooked food retailers reshape access. This study addresses the spatial mismatch between where people live and where healthy food is truly available.</p>

        <p><strong>Approach:</strong> Comprehensive mapping that includes farmers' markets and ethnic grocery stores alongside traditional supermarkets to provide a more nuanced view of food access.</p>

        <p><strong>Tools Used:</strong> ArcGIS Pro, Network Analyst, USDA SNAP Retailer Locator, CDC PLACES, American Community Survey, Transport Network</p>

        <div class="highlight-box">
            <h3>Spatial Analysis:</h3>
            <ul>
                <li>Used Network Analyst to generate 1-mile service areas from food retailers.</li>
                <li>Expanded retailer dataset with ethnic stores and farmers' markets.</li>
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
        <h2>🍎 Project 2: Food Deserts and Chronic Disease in DFW: Association vs. Causality</h2>
        
        <p><strong>Objective:</strong> Examine the spatial relationship between food desert classification and the prevalence of obesity and diabetes using regression models.</p>

        <p><strong>Approach:</strong> Used Geographically Weighted Regression (GWR) to test local associations between food access and chronic disease rates across Dallas-Fort Worth census tracts.</p>

        <div class="highlight-box">
            <h3>Statistical Highlights:</h3>
            <ul>
                <li><strong>Obesity:</strong> R² = 0.52 (significant, p = 0.008)</li>
                <li><strong>Diabetes:</strong> R² = 0.40 (not significant, p = 0.12)</li>
                <li>Highest coefficients in southern Dallas and western Tarrant Counties</li>
            </ul>
        </div>

        <div class="stats-table">
            <h3>Key Findings:</h3>
            <ul>
                <li>Food deserts alone were <strong>not causal predictors</strong> of disease (p > 0.27)</li>
                <li><strong>Stronger predictors included:</strong>
                    <ul>
                        <li>Age 65+</li>
                        <li>Education level</li>
                        <li>Race/ethnicity (Black and Hispanic)</li>
                        <li>Poverty</li>
                    </ul>
                </li>
                <li><strong>Integrated Model Performance:</strong>
                    <ul>
                        <li>Obesity model R² = <strong>0.89</strong></li>
                        <li>Diabetes model R² = <strong>0.82</strong></li>
                    </ul>
                </li>
            </ul>
        </div>

        <div class="slideshow-container" id="slider2">
            <img src="./GWR and Obesity.jpg" alt="Geographically Weighted Regression - Obesity Analysis" class="active">
            <img src="./GWR and Diabtes.jpg" alt="Geographically Weighted Regression - Diabetes Analysis">
            <img src="./Obesity and Food Deserts.jpg" alt="Obesity and Food Deserts Correlation">
            <img src="./Diabetes and Food deserts.jpg" alt="Diabetes and Food Deserts Correlation">
        </div>

        <p><strong>Interpretation:</strong> Food access is <strong>associated</strong> with poor health outcomes in specific areas, but <strong>causality</strong> is best explained through a broader social determinants framework. Spatial modeling helps identify where food environments align with health risks, guiding targeted interventions.</p>
    </div>

    <div class="project">
        <h2>🏥 Project 3: Liver Disease Mortality Patterns in Texas</h2>
        
        <p><strong>Challenge:</strong> Understanding the geographic distribution and temporal trends of liver disease mortality to identify at-risk communities.</p>

        <p><strong>Approach:</strong> 20-year spatiotemporal analysis combining mortality data with socioeconomic and health indicators to identify hotspots and risk factors.</p>

        <p><strong>Tools Used:</strong> ArcGIS Pro, CDC WONDER, County Health Rankings, Geographically Weighted Regression (GWR)</p>

        <div class="highlight-box">
            <h3>Spatial Analysis:</h3>
            <ul>
                <li>Hotspot analysis identified persistent high mortality clusters.</li>
                <li>GWR analyzed local relationships between mortality and health/socioeconomic variables.</li>
            </ul>
        </div>

        <div class="stats-table">
            <h3>Summary Statistics:</h3>
            <ul>
                <li>Counties analyzed: 207</li>
                <li>Significant hotspots: 12 counties in south and west Texas</li>
                <li><strong>Strongest variable correlations:</strong>
                    <ul>
                        <li>Diabetes (R² = 0.43)</li>
                        <li>Hispanic population (R² = 0.32)</li>
                        <li>Obesity (R² = 0.30)</li>
                        <li>Income (R² = 0.25)</li>
                    </ul>
                </li>
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

        <p><strong>Interpretation:</strong> Public health risks are spatially clustered and vary regionally. Policy focus should be tailored for regions like South Texas where multiple risk factors converge.</p>
    </div>

    <div class="project">
        <h2>🏗️ Project 4: LiDAR Building Extraction in Waco, TX</h2>
        
        <p><strong>Challenge:</strong> Accurate building inventory and volume estimation for urban planning without costly field surveys.</p>

        <p><strong>Objective:</strong> Estimate small-area population using LiDAR-derived building metrics (count, area, volume) across 125 census blocks in Waco, Texas.</p>

        <p><strong>Study Area:</strong> Waco, a mid-sized city with 140,000 residents, offers a mix of urban, suburban, and semi-rural environments—ideal for testing population estimation models in transitional landscapes.</p>

        <div class="highlight-box">
            <h3>Approach:</h3>
            <p>High-resolution LiDAR data (TNRIS) and 2020 Census block data were integrated using ArcGIS Pro. The methodology included:</p>
            <ul>
                <li>Generation of DSM, DTM, and DHM</li>
                <li>Building extraction (threshold > 2.2m)</li>
                <li>Binary mask filtering and footprint vectorization</li>
                <li>Calculation of count, area, and volume metrics</li>
                <li>Population estimation using OLS regression models</li>
            </ul>
        </div>

        <div class="stats-table">
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
        </div>

        <div class="highlight-box">
            <h3>Key Takeaways:</h3>
            <ul>
                <li><strong>Building count</strong> was the most accurate and interpretable metric for population estimation in Waco's mixed-density environment.</li>
                <li><strong>Volume</strong> was the weakest predictor due to the influence of non-residential or tall commercial buildings.</li>
                <li>Results align with literature emphasizing building count and area as effective proxies in semi-urban contexts.</li>
            </ul>
        </div>

        <p><strong>Implications:</strong> Supports scalable LiDAR methods for urban planning, emergency response, and infrastructure management. Future work should incorporate land-use data, socio-demographic context, or machine learning for improved precision.</p>
    </div>

    <div class="skills-grid">
        <div class="skill-category">
            <h3>📈 GIS & Spatial Analysis</h3>
            <ul>
                <li>Advanced cartography and spatial modeling</li>
                <li>Network analysis and service area optimization</li>
                <li>Regression, clustering, and spatial statistics</li>
                <li>Remote sensing and classification</li>
            </ul>
        </div>

        <div class="skill-category">
            <h3>💻 Programming & Data</h3>
            <ul>
                <li>Python (ArcPy, Pandas, GeoPandas)</li>
                <li>SQL for spatial databases</li>
                <li>SPSS</li>
                <li>Web mapping: ArcGIS Pro, ArcGIS Online</li>
            </ul>
        </div>

        <div class="skill-category">
            <h3>🏢 Professional Experience</h3>
            <ul>
                <li>Project design, research, and execution</li>
                <li>Data visualization and report writing</li>
                <li>Public presentations and stakeholder engagement</li>
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
        <p>I'm actively seeking opportunities in GIS analysis, urban planning, and public health research. Let's discuss how spatial analysis can drive better decision-making in your organization.</p>
        
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
