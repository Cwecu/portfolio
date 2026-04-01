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

        .project {
            background: #f8f9fa;
            padding: 25px;
            margin: 30px 0;
            border-radius: 15px;
            border-left: 5px solid #3498db;
        }

        .highlight-box {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            padding: 15px;
            border-radius: 10px;
            margin: 15px 0;
            border-left: 4px solid #2196f3;
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
            <p>I am a GIS Analyst with a specialized focus on **Health Geography** and Geospatial Data Analysis. With a background as a Registered Nurse, I bring a unique clinical perspective to spatial problems, utilizing ArcGIS Pro, Python, and advanced spatial statistics to drive data-informed decision-making in public health and infrastructure.</p>
        </div>
    </div>

    <div class="project">
        <h2>📊 Project 1: Youth Substance Exposure Dashboard & Story Map</h2>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Public health advocates in Texas lacked a centralized tool to visualize the density of alcohol and hemp retailers near schools and youth centers.</p>
            <p><strong>Tools Used:</strong> ArcGIS Online, ArcGIS Dashboards, <strong>Experience Builder</strong>, and Story Maps.</p>
            <p><strong>Results:</strong> Developed a multi-layered interface that allows for real-time filtering of outlet types across the state.</p>
            <p><strong>Strategic Impact:</strong> This tool is actively used for evidence-based policy advocacy to reduce youth exposure to substance retailers.</p>
        </div>
    </div>

    <div class="project">
        <h2>🏥 Project 2: Spatiotemporal Analysis of Liver Disease Mortality</h2>
        <div class="slideshow-container" id="slider-liver">
            <img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Hotspot" class="active">
            <img src="./AADR 2001-2007.jpg" alt="AADR 2001-2007">
            <img src="./AADR 2008-2014.jpg" alt="AADR 2008-2014">
            <img src="./AADR 2015-2020.jpg" alt="AADR 2015-2020">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Identifying long-term geographic clusters of liver disease across Texas's 254 counties to optimize resource allocation.</p>
            <p><strong>Tools Used:</strong> ArcGIS Pro, CDC WONDER Data, Getis-Ord Gi* Statistics.</p>
            <p><strong>Results:</strong> Identified 12 persistent hotspot counties with a 23% mortality increase, significantly higher than the state average.</p>
            <p><strong>Strategic Impact:</strong> Provided the Texas Department of State Health Services with a predictive model boasting 87% accuracy for future high-mortality areas.</p>
        </div>
    </div>

    <div class="project">
        <h2>🍎 Project 3: Multi-Criteria Food Access Analysis - DFW Metroplex</h2>
        <div class="slideshow-container" id="slider-food">
            <img src="./food_desert_map_sample.png.jpg" alt="Food Desert Map" class="active">
            <img src="./Food Deserts hotspot.jpg" alt="Food Desert Hotspot">
            <img src="./Food Access.jpg" alt="Food Access Map">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Standard USDA food desert models often miss culturally-relevant retailers, leading to inaccurate public health planning.</p>
            <p><strong>Tools Used:</strong> ArcGIS Network Analyst, Python (ArcPy), custom-geocoded retailer datasets.</p>
            <p><strong>Results:</strong> Reduced food desert classification errors by 16% and identified 268 unmapped food sources.</p>
            <p><strong>Strategic Impact:</strong> Findings were shared with the City of Dallas to improve resource allocation in diverse urban communities.</p>
        </div>
    </div>

    <div class="project">
        <h2>📈 Project 4: GWR Analysis of Chronic Disease & Food Environment</h2>
        <div class="slideshow-container" id="slider-gwr">
            <img src="./GWR and Obesity.jpg" alt="Obesity GWR" class="active">
            <img src="./GWR and Diabtes.jpg" alt="Diabetes GWR">
            <img src="./Obesity and Food Deserts.jpg" alt="Correlation Analysis">
        </div>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Public health agencies needed to understand if "food deserts" were the primary driver of obesity and diabetes in North Texas.</p>
            <p><strong>Tools Used:</strong> Geographically Weighted Regression (GWR), ArcGIS Pro, CDC PLACES Health Data.</p>
            <p><strong>Results:</strong> Discovered that social determinants like age and poverty (R²=0.89) were stronger predictors than food access alone.</p>
            <p><strong>Strategic Impact:</strong> Guided the Dallas County Health Department to prioritize social determinants in their intervention strategies.</p>
        </div>
    </div>

    <div class="project">
        <h2>🏗️ Project 5: Automated Population Estimation via LiDAR</h2>
        <div class="highlight-box">
            <h3>Case Study:</h3>
            <p><strong>Problem:</strong> Decennial census data becomes outdated quickly, hindering effective emergency response and infrastructure planning.</p>
            <p><strong>Tools Used:</strong> LiDAR Remote Sensing, 3D Analyst, ArcGIS Pro Spatial Analyst.</p>
            <p><strong>Results:</strong> Achieved a 99.99% accuracy rate in building count extraction and population estimation across a 125-block study area.</p>
            <p><strong>Strategic Impact:</strong> Provided a scalable, cost-effective method (90% cost reduction) for annual population updates.</p>
        </div>
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
