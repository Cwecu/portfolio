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

        h1 { color: #2c3e50; margin-bottom: 5px; font-size: 2.5em; }
        .current-titles { color: #3498db; font-weight: 600; margin-bottom: 15px; font-size: 1.2em; }
        h2 { color: #34495e; border-bottom: 3px solid #3498db; padding-bottom: 10px; margin-top: 40px; }
        
        .card {
            background: #f8f9fa;
            padding: 25px;
            margin: 30px 0;
            border-radius: 15px;
            border-left: 5px solid #3498db;
        }

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
            height: 550px;
            object-fit: contain;
            position: absolute;
            top: 0;
            left: 0;
            opacity: 0;
            transition: opacity 1s ease-in-out;
            background: white;
        }

        .slideshow-container img.active { opacity: 1; }
        .slideshow-container img:first-child { position: relative; }

        .highlight-box {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            padding: 15px;
            border-radius: 10px;
            margin: 15px 0;
            border-left: 4px solid #2196f3;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
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

        .contact-section a { color: #3498db; text-decoration: none; }

        @media (max-width: 768px) {
            .profile-container { flex-direction: column; text-align: center; }
            .slideshow-container img { height: 350px; }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
        <div class="profile-content">
            <h1>Nicholas Lawson</h1>
            <div class="current-titles">GIS Analyst</div>
            <p>I am <strong>Nicholas Lawson</strong>, a GIS Analyst with a strong foundation in geospatial data analysis, research, and project coordination. I have experience using tools such as ArcGIS Pro, QGIS and spatial analysis techniques to support data-driven decision-making. With a diverse background in education, business development, and client engagement, I bring a well-rounded perspective to geospatial projects. I am eager to apply my growing expertise in GIS to solve complex problems and contribute meaningfully to your organization's spatial initiatives.</p>
        </div>
    </div>

    <h2>💼 Professional Experience</h2>
    
    <div class="card">
        <h3>GIS Analyst</h3>
        <p><strong>Sedgwick County | Wichita, KS | Present</strong></p>
        <ul>
            <li>Support Emergency Communications operations through spatial analysis and mapping solutions.</li>
            <li>Developed optimized snow route maps for Public Works Department to improve winter weather response efficiency.</li>
            <li>Created construction project maps to support infrastructure planning and decision-making processes.</li>
            <li>Collaborate with multiple county departments to deliver timely GIS products for operational needs.</li>
            <li>Maintain and update critical infrastructure datasets for emergency response coordination.</li>
        </ul>
    </div>

    <div class="card">
        <h3>GIS Consultant / Analyst</h3>
        <p><strong>Texans for Safe and Drug-Free Youth | Present</strong></p>
        <ul>
            <li>Designed and developed interactive ArcGIS Online dashboard tracking youth exposure to alcohol and hemp outlets across Texas.</li>
            <li>Created comprehensive story map to communicate spatial patterns of substance outlet density and youth accessibility.</li>
            <li>Performed spatial analysis to identify high-risk areas with elevated youth exposure to alcohol and hemp retailers.</li>
            <li>Delivered web-based GIS tools including Experience Builder applications for non-technical users.</li>
        </ul>
    </div>

    <h2>🚀 Featured Projects</h2>

    <div class="card">
        <h2>📊 Project 1: Youth Substance Exposure Dashboard & Story Map</h2>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Public health advocates needed a spatial platform to visualize alcohol and hemp retailer density near schools and youth centers to support legislative changes.</p>
            <p><strong>Tools Used:</strong> ArcGIS Online, ArcGIS Dashboards, <strong>Experience Builder</strong>, and Story Maps.</p>
            <p><strong>Results:</strong> Developed a multi-layered interactive suite allowing real-time filtering of statewide outlet data and proximity analysis.</p>
            <p><strong>Impact:</strong> Actively used by advocacy organizations for evidence-based policy recommendations to Texas state legislators.</p>
        </div>
    </div>

    <div class="card">
        <h2>🏥 Project 2: Spatiotemporal Analysis of Texas Liver Disease</h2>
        <div class="slideshow-container" id="slider-liver">
            <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Hotspot" class="active">
            <img src="./AADR 2001-2007.jpg" alt="AADR 2001-2007">
            <img src="./AADR 2008-2014.jpg" alt="AADR 2008-2014">
            <img src="./AADR 2015-2020.jpg" alt="AADR 2015-2020">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Identifying long-term mortality clusters across 254 counties to optimize public health resource allocation.</p>
            <p><strong>Tools Used:</strong> ArcGIS Pro, Getis-Ord Gi* Statistics, CDC WONDER Mortality Data.</p>
            <p><strong>Results:</strong> Identified 12 persistent hotspots and achieved 87% prediction accuracy for future high-mortality areas.</p>
            <p><strong>Impact:</strong> Directed state health prevention resources to high-risk geographic areas, improving early detection efficiency.</p>
        </div>
    </div>

    <div class="card">
        <h2>🍎 Project 3: Food Access Analysis - DFW Metroplex</h2>
        <div class="slideshow-container" id="slider-food">
            <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Analysis" class="active">
            <img src="./Food Deserts hotspot.jpg" alt="Hotspot Analysis">
            <img src="./Food Access.jpg" alt="Food Access Map">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Traditional models underestimate food accessibility by ignoring culturally-relevant ethnic retailers and small grocers.</p>
            <p><strong>Tools Used:</strong> Network Analyst, Python (ArcPy), custom geocoding.</p>
            <p><strong>Results:</strong> Reduced low-income food desert classification errors by 16% and identified 268 previously unmapped food sources.</p>
            <p><strong>Impact:</strong> Shared with the City of Dallas at the 2025 North Texas Climate Symposium to guide urban development planning.</p>
        </div>
    </div>

    <div class="card">
        <h2>📈 Project 4: GWR Analysis - Chronic Disease & Food Environment</h2>
        <div class="slideshow-container" id="slider-gwr">
            <img src="./GWR and Obesity.jpg" alt="Obesity GWR" class="active">
            <img src="./GWR and Diabtes.jpg" alt="Diabetes GWR">
            <img src="./Obesity and Food Deserts.jpg" alt="Correlation Map">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Determine the spatial relationship between food environments and chronic disease prevalence to optimize interventions.</p>
            <p><strong>Tools Used:</strong> Geographically Weighted Regression (GWR), ArcGIS Pro, CDC PLACES Health Data.</p>
            <p><strong>Results:</strong> Proved that socio-economic determinants (poverty/age) were stronger predictors of disease than food access alone (R²=0.89).</p>
            <p><strong>Impact:</strong> Informed Dallas County Health Department strategies to prioritize social determinants over food access solutions alone.</p>
        </div>
    </div>

    <div class="card">
        <h2>🏗️ Project 5: Automated Population Estimation via LiDAR</h2>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Municipal departments need cost-effective population estimates between decennial census updates for infrastructure planning.</p>
            <p><strong>Tools Used:</strong> LiDAR Remote Sensing, 3D Analyst, Morphological Filtering.</p>
            <p><strong>Results:</strong> Achieved a 99.99% accuracy rate in building extraction and population estimation across a 125-block study area.</p>
            <p><strong>Impact:</strong> Enabled annual population metrics updates at 10% of the cost of traditional field surveys.</p>
        </div>
    </div>

    <h2>🛠️ Technical Skills</h2>
    <div class="skills-grid">
        <div class="skill-category">
            <h3>GIS & Spatial Analysis</h3>
            <ul>
                <li><strong>Software:</strong> ArcGIS Pro, ArcGIS Online, QGIS</li>
                <li><strong>Analysis:</strong> Network Analyst, Spatial Analyst, 3D Analyst</li>
                <li><strong>Statistics:</strong> GWR, Hotspot Analysis, Spatial Autocorrelation</li>
                <li><strong>Remote Sensing:</strong> LiDAR processing, Image classification</li>
            </ul>
        </div>
        <div class="skill-category">
            <h3>Web GIS & Development</h3>
            <ul>
                <li><strong>Platforms:</strong> Experience Builder, Dashboards, Story Maps</li>
                <li><strong>Programming:</strong> Python (ArcPy), SQL</li>
                <li><strong>Data Visualization:</strong> Cartographic Design, Executive Reporting</li>
            </ul>
        </div>
    </div>

    <h2>🎓 Education</h2>
    <div class="card">
        <h3>Master of Science in Geography</h3>
        <p><strong>University of North Texas | Denton, TX | 2025</strong></p>
        <p>Concentration: Medical Geography and GIS</p>
    </div>
    <div class="card">
        <h3>Graduate Certificate in Geographic Information System</h3>
        <p><strong>University of North Texas | Denton, TX | 2025</strong></p>
    </div>
    <div class="card">
        <h3>Bachelor of Arts in Geography</h3>
        <p><strong>University of Ghana | Legon, Accra | 2018</strong></p>
    </div>

    <div class="contact-section">
        <h2>📞 Let's Connect</h2>
        <p>📧 <a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a> | 💼 <a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank">LinkedIn</a></p>
        <p>📍 Wichita, Kansas</p>
    </div>

    <script>
        class Slideshow {
            constructor(containerId, interval = 4000) {
                this.container = document.getElementById(containerId);
                if(!this.container) return;
                this.images = this.container.querySelectorAll('img');
                this.currentSlide = 0;
                this.interval = interval;
                this.startSlideshow();
            }
            showSlide(index) {
                this.images.forEach(img => img.classList.remove('active'));
                this.images[index].classList.add('active');
            }
            nextSlide() {
                this.currentSlide = (this.currentSlide + 1) % this.images.length;
                this.showSlide(this.currentSlide);
            }
            startSlideshow() { setInterval(() => this.nextSlide(), this.interval); }
        }

        document.addEventListener('DOMContentLoaded', function() {
            new Slideshow('slider-liver', 4500);
            new Slideshow('slider-food', 5000);
            new Slideshow('slider-gwr', 5500);
        });
    </script>
</body>
</html>
