# Nicholas Lawson | GIS Analyst Portfolio

<img src="./profile.jpg.jfif" style="float: right; border-radius: 50%; width: 120px; margin-left: 20px;" />

## 👋 About Me

I am **Nicholas Lawson**, a recent Geography graduate with expertise in GIS, spatial analysis, and health geography. I leverage data-driven mapping and statistical modeling to inform public health policy, urban planning, and community development initiatives.

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

**Objective:**  
Estimate small-area population using LiDAR-derived building metrics (count, area, volume) across 125 census blocks in Waco, Texas.

**Study Area:**  
Waco, a mid-sized city with 140,000 residents, offers a mix of urban, suburban, and semi-rural environments—ideal for testing population estimation models in transitional landscapes.

**Approach:**  
High-resolution LiDAR data (TNRIS) and 2020 Census block data were integrated using ArcGIS Pro. The methodology included:
- Generation of DSM, DTM, and DHM
- Building extraction (threshold > 2.2m)
- Binary mask filtering and footprint vectorization
- Calculation of count, area, and volume metrics
- Population estimation using OLS regression models

**Model Results:**

| Model | Metric Used       | R²      | Pop. Estimate | Error (%)     |
|-------|-------------------|---------|---------------|----------------|
| 1     | Building Count    | 0.6259  | 5,713.01      | +0.0001%       |
| 2     | Building Area     | 0.5815  | 5,709.54      | −0.06%         |
| 3     | Building Volume   | 0.1635  | 5,656.80      | −0.98%         |

**Key Takeaways:**
- **Building count** was the most accurate and interpretable metric for population estimation in Waco’s mixed-density environment.
- **Volume** was the weakest predictor due to the influence of non-residential or tall commercial buildings.
- Results align with literature emphasizing building count and area as effective proxies in semi-urban contexts.

**Implications:**
- Supports scalable LiDAR methods for urban planning, emergency response, and infrastructure management.
- Future work should incorporate land-use data, socio-demographic context, or machine learning for improved precision.


## 📈 Technical Skills

**GIS & Spatial Analysis**
- Advanced cartography and spatial modeling
- Network analysis and service area optimization  
- Regression, clustering, and spatial statistics
- Remote sensing and classification

**Programming & Data**
- Python (ArcPy, Pandas, GeoPandas)
- SQL for spatial databases
- SPSS
- Web mapping: ArcGIS Pro, ArcGIS Online

**Professional Experience**
- Project design, research, and execution
- Data visualization and report writing
- Public presentations and stakeholder engagement

---

## 🎓 Education & Certifications

**Master of Science in Geography**  
_University of North Texas, 2025_  
_Concentration: Geographic Information Systems & Health and Medical Geography_

**Bachelor of Art in Geography and Resource Development**  
_University of Ghana, 2018_  
_Concentration: Geographic Information Systems,  Cities and Urbanisation, Transportation_

**Relevant Coursework**
- Advanced GIS Analysis
- Health Geography  
- Urban Planning
- Spatial Statistics
 

---

## 📞 Let's Connect

I'm actively seeking opportunities in GIS analysis, urban planning, and public health research. Let's discuss how spatial analysis can drive better decision-making in your organization.

📧 **Email:** nickklas96@gmail.com  
💼 **LinkedIn:** (https://www.linkedin.com/in/nicholas-lawson-a3b861b6/) 
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

