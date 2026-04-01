<!DOCTYPE html>
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
            border: 3px solid #3498db;
        }

        .profile-content {
            flex: 1;
        }

        h1 {
            color: #2c3e50;
            margin-bottom: 5px;
            font-size: 2.5em;
        }

        .current-titles {
            color: #3498db;
            font-weight: 600;
            margin-bottom: 15px;
            font-size: 1.1em;
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

        .experience-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 5px solid #2c3e50;
        }

        .competencies {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
        }

        .project {
            background: #f8f9fa;
            padding: 25px;
            margin: 30px 0;
            border-radius: 15px;
            border-left: 5px solid #3498db;
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

        .contact-section a {
            color: #3498db;
            text-decoration: none;
        }

        .tag {
            display: inline-block;
            background: #3498db;
            color: white;
            padding: 2px 10px;
            border-radius: 15px;
            font-size: 0.85em;
            margin-right: 5px;
        }

        @media (max-width: 768px) {
            .profile-container {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
        <div class="profile-content">
            <h1>Nicholas Lawson</h1>
            <div class="current-titles">GIS Analyst | Emergency Communications & Public Works</div>
            
            <p>I am a GIS Analyst with a strong foundation in geospatial data analysis, health geography, and public infrastructure. Currently serving <strong>Sedgwick County</strong>, I specialize in operationalizing spatial data for emergency response and public works. My expertise bridges technical GIS implementation—using ArcGIS Pro, QGIS, and Python—with strategic research in health disparities and community safety. I am passionate about leveraging spatial intelligence to drive evidence-based policy and operational efficiency.</p>
            
            <div class="competencies">
                <h3>Core Competencies</h3>
                <ul>
                    <li><strong>GIS Software:</strong> ArcGIS Pro, ArcGIS Online (Dashboards/StoryMaps), QGIS, Python (ArcPy)</li>
                    <li><strong>Spatial Analysis:</strong> Network Analysis, Hotspot Analysis (Getis-Ord Gi*), GWR, Service Area Modeling</li>
                    <li><strong>Data Management:</strong> SQL, Geodatabase Management, LiDAR Processing, Feature Class Design</li>
                    <li><strong>Public Operations:</strong> Emergency Response Mapping, Infrastructure Planning, Public Health Surveillance</li>
                </ul>
            </div>
        </div>
    </div>

    <h2>💼 Professional Experience</h2>
    
    <div class="experience-card">
        <h3>GIS Analyst - Emergency Communications & Public Works</h3>
        <p><strong>Sedgwick County | Wichita, KS | Present</strong></p>
        <ul>
            <li>Support Emergency Communications operations through advanced spatial analysis and mapping solutions.</li>
            <li>Developed optimized snow route maps for Public Works to enhance winter weather response efficiency.</li>
            <li>Create construction project maps to support infrastructure planning and cross-departmental decision-making.</li>
            <li>Maintain and update critical infrastructure datasets essential for real-time emergency response coordination.</li>
        </ul>
    </div>

    <div class="experience-card">
        <h3>GIS Consultant / Analyst</h3>
        <p><strong>Texans for Safe and Drug-Free Youth | Present</strong></p>
        <ul>
            <li>Designed interactive ArcGIS Online dashboards tracking youth exposure to alcohol and hemp outlets across Texas.</li>
            <li>Developed comprehensive Story Maps to communicate patterns of substance outlet density and accessibility.</li>
            <li>Identify high-risk areas via spatial analysis to support policy advocacy and community intervention strategies.</li>
            <li>Deliver web-based tools that enable non-technical stakeholders to explore complex statewide datasets.</li>
        </ul>
    </div>

    <h2>🚀 Featured Projects</h2>

    <div class="project">
        <div style="display: flex; justify-content: space-between; align-items: flex-start;">
            <h2>📊 Youth Substance Exposure Dashboard - Texas Statewide Analysis</h2>
            <span class="tag">ArcGIS Online</span>
        </div>
        <p><strong>Purpose:</strong> To provide data-driven visualization tools for public health advocacy regarding youth accessibility to harmful substances.</p>
        <p><strong>Technical Implementation:</strong> 
            Leveraged <strong>ArcGIS Dashboards</strong> for real-time filtering of retail outlets and <strong>ArcGIS Story Maps</strong> for narrative-driven spatial analysis. Applied spatial density modeling to identify correlations between outlet clusters and youth-populated zones.</p>
        <div class="highlight-box">
            <h3>Impact:</h3>
            <ul>
                <li>Actively used by advocacy organizations for evidence-based policy recommendations in Texas.</li>
                <li>Transformed complex regulatory data into intuitive, actionable web-GIS tools.</li>
            </ul>
        </div>
    </div>

    <div class="project">
        <h2>🍎 Multi-Criteria Food Access Analysis - DFW Metroplex</h2>
        <p><strong>Business Problem:</strong> Traditional mapping underestimates food accessibility by excluding culturally-relevant retailers.</p>
        <p><strong>Solution:</strong> Developed a spatial framework integrating Network Analyst to incorporate ethnic grocers and farmers' markets.</p>
        <div class="highlight-box">
            <h3>Results:</h3>
            <ul>
                <li>16% reduction in low-income food desert classification accuracy gaps.</li>
                <li>10% improvement in overall mapping accuracy across 1,536 census tracts.</li>
            </ul>
        </div>
    </div>

    <div class="project">
        <h2>🏗️ Automated Population Estimation Using LiDAR Remote Sensing</h2>
        <p><strong>Business Problem:</strong> Municipalities need cost-effective population updates between census cycles.</p>
        <p><strong>Solution:</strong> Automated workflow using high-resolution LiDAR to extract building metrics for statistical modeling.</p>
        <div class="highlight-box">
            <h3>Performance:</h3>
            <ul>
                <li>Building count model achieved <strong>99.99% accuracy</strong> in study area.</li>
                <li>Reduced analysis time from weeks to 6 hours through automated 3D Analyst workflows.</li>
            </ul>
        </div>
    </div>

    <div class="skills-grid">
        <div class="skill-category">
            <h3>🗺️ GIS & Spatial Analysis</h3>
            <ul>
                <li>ArcGIS Pro & Online</li>
                <li>Network & Spatial Analyst</li>
                <li>Remote Sensing (LiDAR)</li>
                <li>Hotspot Analysis</li>
            </ul>
        </div>
        <div class="skill-category">
            <h3>💻 Data & Programming</h3>
            <ul>
                <li>Python (ArcPy, GeoPandas)</li>
                <li>SQL / PostGIS</li>
                <li>ArcGIS Dashboards</li>
                <li>Statistical Modeling (R, SPSS)</li>
            </ul>
        </div>
        <div class="skill-category">
            <h3>📊 Communication</h3>
            <ul>
                <li>Policy Advocacy Tools</li>
                <li>Executive Reporting</li>
                <li>Story Map Production</li>
                <li>Cross-Departmental Liaison</li>
            </ul>
        </div>
    </div>

    <div class="contact-section">
        <h2>📞 Let's Connect</h2>
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin-top: 20px;">
            <div>📧 <strong>Email:</strong><br><a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a></div>
            <div>💼 <strong>LinkedIn:</strong><br><a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank">Nicholas Lawson</a></div>
            <div>💻 <strong>GitHub:</strong><br><a href="https://github.com/cwecu" target="_blank">cwecu</a></div>
            <div>📍 <strong>Location:</strong><br>Wichita, Kansas</div>
        </div>
        <p style="margin-top: 30px; font-style: italic; font-size: 0.8em; opacity: 0.8;">Portfolio last updated: April 2026</p>
    </div>
</body>
</html>
