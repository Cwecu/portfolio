# Full index.md content with updated Project 1 section included

full_index_md = """
# Nicholas Lawson | GIS Analyst Portfolio

<img src="./profile.jpg.jfif" style="float: right; border-radius: 50%; width: 120px; margin-left: 20px;" />

## 👋 About Me

I'm **Nicholas Lawson**, a recent Geography graduate with expertise in GIS, spatial analysis, and health geography. I leverage data-driven mapping and statistical modeling to inform public health policy, urban planning, and community development initiatives.

### Core Competencies
- **Software:** ArcGIS Pro, QGIS, Python for GIS
- **Analysis:** Geographically Weighted Regression (GWR), Network Analysis, Hotspot Analysis
- **Specializations:** Health Geography, Urban Planning, LiDAR Processing

---

## 🍎 Project 1: Redefining Food Deserts in North Texas

**Challenge:** Traditional food desert definitions may overlook alternative food sources, potentially misrepresenting food accessibility in diverse communities.

**Approach:** Comprehensive mapping that includes farmers' markets and ethnic grocery stores alongside traditional supermarkets to provide a more nuanced view of food access.

**Tools Used:** ArcGIS Pro, Network Analyst, USDA SNAP Retailer Locator, CDC PLACES, American Community Survey

**Spatial Analysis:**
- Used Network Analyst to generate 1-mile service areas from food retailers.
- Expanded retailer dataset with ethnic stores and farmers' markets.

**Summary Statistics:**
- Total food retailers: 1,023 (755 supermarkets, 241 small grocers, 27 farmers' markets)
- Census tracts analyzed: 1,536 (1,508 urban, 28 rural)
- Food desert tracts (traditional definition): 1,127
- Food desert tracts (expanded definition): 1,010 (10% reduction)
- Low-income food desert tracts dropped from 385 to 325 (16% reduction)

**Health & GWR Findings:**
- Food deserts explained 52% of obesity variation (p = 0.008) and 40% of diabetes variation (p = 0.12)
- Strongest associations found in southern Dallas and western Tarrant Counties

**Social Determinants Insight:**
- Food deserts were not strong predictors on their own (p > 0.27)
- Significant predictors included:
  - Age 65+ (strong for diabetes)
  - Race/ethnicity: Black (linked to obesity), Hispanic (linked to both)
  - Education (negative correlation with both outcomes)
  - Poverty (linked to obesity)
- Comprehensive model explained 89% of obesity and 82% of diabetes variation

**Interpretation:**
- The inclusion of smaller and culturally specific food sources reduced misclassification of access.
- Social and economic conditions more strongly predict chronic health outcomes than food deserts alone.

<img src="./food_desert_map_sample.png.jpg" alt="Food Desert Analysis" style="width: 100%; max-width: 600px;" />

---

## 🏥 Project 2: Liver Disease Mortality Patterns in Texas

**Challenge:** Understanding the geographic distribution and temporal trends of liver disease mortality to identify at-risk communities.

**Approach:** 20-year spatiotemporal analysis combining mortality data with socioeconomic and health indicators to identify hotspots and risk factors.

**Tools Used:** ArcGIS Pro, CDC WONDER, County Health Rankings, Geographically Weighted Regression (GWR)

**Spatial Analysis:**
- Hotspot analysis identified persistent high mortality clusters.
- GWR analyzed local relationships between mortality and health/socioeconomic variables.

**Summary Statistics:**
- Counties analyzed: 207
- Significant hotspots: 12 counties in south and west Texas
- Strongest variable correlations:
  - Diabetes (R² = 0.43)
  - Hispanic population (R² = 0.32)
  - Obesity (R² = 0.30)
  - Income (R² = 0.25)

**Interpretation:**
- Public health risks are spatially clustered and vary regionally.
- Policy focus should be tailored for regions like South Texas where multiple risk factors converge.

<img src="./liver_disease_hotspot_sample.png.jpg" alt="Liver Disease Hotspots" style="width: 100%; max-width: 600px;" />

---

## 🏗️ Project 3: LiDAR Building Extraction in Waco, TX

**Challenge:** Accurate building inventory and volume estimation for urban planning without costly field surveys.

**Approach:** Used LiDAR point clouds to classify buildings, estimate volumes, and convert raster data into usable building polygons.

**Tools Used:** ArcGIS Pro, LAS Dataset, Raster Calculations, Python

**Spatial Analysis:**
- Generated DSM, DTM, DHM from LAS data
- Isolated building masks and converted rasters to vector polygons

**Summary Statistics:**
- Buildings extracted: 15,847
- Mean building height: 7.4 meters
- Total estimated volume: ~1.6 million m³
- Classification accuracy: 94%

**Interpretation:**
- Enabled 3D building inventory with high spatial accuracy.
- Scalable approach for city planning, disaster preparedness, and zoning enforcement.

<img src="./lidar_buildings_sample.png.jpg" alt="LiDAR Building Extraction" style="width: 100%; max-width: 600px;" />

---

## 📈 Technical Skills

**GIS & Spatial Analysis**
- Advanced cartography and spatial modeling
- Network analysis and service area optimization  
- Regression, clustering, and spatial statistics
- Remote sensing and classification

**Programming & Data**
- Python (ArcPy, Pandas, GeoPandas)
- SQL for spatial databases
- R for statistical modeling
- Web mapping: Leaflet, ArcGIS Online

**Professional Experience**
- Project design, research, and execution
- Data visualization and report writing
- Public presentations and stakeholder engagement

---

## 🎓 Education & Certifications

**Bachelor of Science in Geography**  
_University of North Texas, 2024_  
_Concentration: Geographic Information Systems_

**Relevant Coursework**
- Advanced GIS Analysis
- Health Geography  
- Urban Planning
- Spatial Statistics

---

## 📞 Let's Connect

I'm actively seeking opportunities in GIS analysis, urban planning, and public health research. Let's discuss how spatial analysis can drive better decision-making in your organization.

📧 **Email:** nicholas.lawson@email.com  
💼 **LinkedIn:** [nicholas-lawson-gis](https://www.linkedin.com/in/your-profile)  
💻 **GitHub:** [cwecu](https://github.com/cwecu)  
📍 **Location:** Dallas-Fort Worth, Texas

---

*Portfolio last updated: June 2025*
"""

# Save the updated file
index_path = "/mnt/data/index.md"
with open(index_path, "w") as f:
    f.write(full_index_md)

index_path  # Return path to the user

