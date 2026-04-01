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

        .experience-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 5px solid #2c3e50;
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

        .contact-section a { color: #3498db; text-decoration: none; }

        @media (max-width: 768px) {
            .profile-container { flex-direction: column; text-align: center; }
            .slideshow-container img { height: 400px; }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <img src="./profile.jpg.jfif" alt="Nicholas Lawson" class="profile-img" />
        <div class="profile-content">
            <h1>Nicholas Lawson</h1>
            <div class="current-titles">GIS Analyst | Emergency Communications & Public Works</div>
            
            <p>I am a GIS Analyst with a strong foundation in geospatial data analysis, health geography, and public infrastructure. Currently serving <strong>Sedgwick County</strong>, I specialize in operationalizing spatial data for emergency response and public works. My expertise bridges technical GIS implementation—using ArcGIS Pro, QGIS, and Python—with strategic research in health disparities and community safety.</p>
        </div>
    </div>

    <h2>💼 Professional Experience</h2>
    
    <div class="experience-card">
        <h3>GIS Analyst - Emergency Communications & Public Works</h3>
        <p><strong>Sedgwick County | Wichita, KS | Present</strong></p>
        <ul>
            <li>Support Emergency Communications operations through advanced spatial analysis and mapping solutions.</li>
            <li>Developed optimized snow route maps for Public Works to improve winter weather response efficiency.</li>
            <li>Collaborate with multiple county departments to deliver timely GIS products for operational needs.</li>
        </ul>
    </div>

    <div class="experience-card">
        <h3>GIS Consultant / Analyst</h3>
        <p><strong>Texans for Safe and Drug-Free Youth | Present</strong></p>
        <ul>
            <li>Designed and developed interactive ArcGIS Online dashboards tracking youth exposure to alcohol and hemp outlets across Texas.</li>
            <li>Created comprehensive story maps to communicate spatial patterns of substance outlet density.</li>
        </ul>
    </div>

    <h2>🚀 Projects & Portfolio</h2>

    <div class="project">
        <h2>📊 Project: Youth Substance Exposure Dashboard - Texas Analysis</h2>
        <p><strong>Purpose:</strong> Create data-driven visualization tools for public health advocacy.</p>
        <p><strong>Impact:</strong> Actively used by advocacy organizations for evidence-based policy recommendations.</p>
        <div class="highlight-box">
            <p>Technology: ArcGIS Online, Dashboards, Story Maps, Spatial Analysis</p>
        </div>
    </div>

    <div class="project">
        <h2>🍎 Project 1: Multi-Criteria Food Access Analysis - DFW Metroplex</h2>
        <p><strong>GIS Solution:</strong> Developed a comprehensive spatial analysis framework integrating Network Analyst with expanded retailer datasets.</p>
        
        <div class="slideshow-container" id="slider1">
            <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map Analysis" class="active">
            <img src="./Food Deserts hotspot.jpg" alt="Food Desert Hotspot Analysis">
            <img src="./Food Access.jpg" alt="Food Access Comprehensive Map">
        </div>

        <div class="highlight-box">
            <h3>Quantifiable Results:</h3>
            <ul>
                <li><strong>16% reduction</strong> in low-income food desert classification (385 → 325 tracts)</li>
                <li><strong>10% improvement</strong> in overall food access mapping accuracy</li>
            </ul>
        </div>
    </div>

    <div class="project">
        <h2>📈 Project 2: GWR Analysis - Chronic Disease & Food Environment</h2>
        <p><strong>Analytical Approach:</strong> Applied advanced spatial statistics using Geographically Weighted Regression (GWR) to model local variations in obesity and diabetes rates.</p>

        <div class="slideshow-container" id="slider2">
            <img src="./GWR and Obesity.jpg" alt="GWR Obesity Analysis" class="active">
            <img src="./GWR and Diabtes.jpg" alt="GWR Diabetes Analysis">
            <img src="./Obesity and Food Deserts.jpg" alt="Obesity/Food Deserts Correlation">
        </div>
    </div>

    <div class="contact-section">
        <h2>📞 Let's Connect</h2>
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin-top: 20px;">
            <div>📧 <strong>Email:</strong><br><a href="mailto:nickklas96@gmail.com">nickklas96@gmail.com</a></div>
            <div>💼 <strong>LinkedIn:</strong><br><a href="https://www.linkedin.com/in/nicholas-lawson-a3b861b6/" target="_blank">Nicholas Lawson</a></div>
            <div>📍 <strong>Location:</strong><br>Wichita, Kansas</div>
        </div>
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
            startSlideshow() {
                setInterval(() => this.nextSlide(), this.interval);
            }
        }

        document.addEventListener('DOMContentLoaded', function() {
            new Slideshow('slider1', 5000);
            new Slideshow('slider2', 6000);
        });
    </script>
</body>
</html>
