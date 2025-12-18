## Chennai – A Tale of Urbanization, Land Transformation, and Flood Risk  
*When land forgets its water, water remembers its land*

---

### Overview
This repository contains a GIS-based spatial analysis project examining the causes of flooding in Chennai, India, with a focus on urbanization, land use–land cover (LULC) transformation, elevation dynamics, and the loss of historical water bodies. The project was developed as a semester-long final project for a GIS and Spatial Analysis course using ArcGIS Pro 3.

The study integrates historical maps, satellite imagery, elevation data, and rainfall observations to qualitatively assess how urban expansion into low-lying areas and former tanks/reservoirs has increased flood vulnerability, particularly evident during the December 2023 flood event.

---

### Results
![img](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Maps/floodriskchennai.png)
- Most of Chennai lies within the 0–3 m elevation range, making it highly susceptible to flooding.  
- LULC change analysis shows substantial urban expansion between 1985 and 2023, particularly over former water bodies.  
- Several historically significant tanks and reservoirs have been fully encroached upon by urban development.  
- The flood risk map reveals a strong spatial overlap between low elevation, dense urbanization, and high flood susceptibility.

---

### Abstract
Chennai, the capital of Tamil Nadu, is situated along the Bay of Bengal on India’s southeast coast and plays a significant role in India’s urban and coastal dynamics. Rapid urbanization has profoundly altered the city’s landscape, disrupting long-standing relationships between land, water, and elevation. This project investigates how changes in land use, loss of historical water bodies, and elevation characteristics have contributed to increasing flood risk. Using GIS-based analyses and historical context, the study highlights how development patterns have intensified vulnerability to flooding. The theme “When land forgets its water, water remembers its land” encapsulates the core finding: urban transformation has come at the cost of hydrological resilience.

---

### Purpose and Motivation
Historically, Chennai benefited from carefully planned water management systems, particularly during the Pallava period, where tanks and reservoirs were strategically placed based on topography and monsoon behavior. This project is motivated by firsthand experience during the December 2023 floods and aims to contrast historical planning practices with present-day urban realities. The goal is to qualitatively analyze how modern urbanization has disrupted natural drainage and water storage systems, leading to recurrent flooding.

---

### Study Area
- **Location:** Chennai, Tamil Nadu, India  
- **Geographic context:** Coastal city along the Bay of Bengal  
- **Focus:** Municipal boundaries of Chennai and surrounding low-lying regions  

---

### Data Sources
The project integrates raster and vector datasets from multiple authoritative sources:
![img](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/datafloechart.png?raw=true)
- **Land Use / Land Cover (1985):** ORNL DAAC  
- **Land Use / Land Cover (2023):** Esri, Microsoft, Impact Observatory  
- **Rainfall Data (December 2023):** CHRS Data Portal (PERSIANN-CCS, 0.04° × 0.04°, 3-hourly)  
- **Digital Elevation Model (DEM):** USGS Earth Explorer  
- **Satellite Imagery:** Landsat 8–9 surface reflectance (USGS Earth Explorer)  
- **Administrative Boundaries:** Municipal and regional shapefiles for Chennai  
- **Historical Map:** Georeferenced old Madras map (Wikipedia source)

All data sources can be found [here](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Data)

---

### Methodology
![img](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/methodologyflowchart.png)
1. **Elevation Analysis:**  
   DEM data was classified to identify low-lying areas prone to flooding.

2. **Historical Map Georeferencing:**  
   An old Madras map was georeferenced using Ground Control Points (GCPs) and regression fitting.

3. **Extraction of Lost Water Bodies:**  
   Tanks and reservoirs were digitized as polygons and polylines using ArcGIS Pro’s Create Features tool.

4. **LULC Classification and Change Detection:**  
   LULC maps for 1985 and 2023 were classified and compared to identify urban expansion and loss of water bodies.

5. **Flood Risk Mapping:**  
   Elevation, slope, proximity to streams, LULC, and rainfall layers were reclassified, weighted, and combined using raster-based analysis to produce a flood risk map.

---

### Workflow Summary
![img](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/workflowflowchart1.png) ![img](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/workflowflowchart2.png)
- DEM reclassification  
- Historical map georeferencing (GCP-based)  
- Digitization of lost tanks and reservoirs  
- LULC classification (1985 vs. 2023)  
- Change detection analysis  
- Hydrological processing (Fill, Flow Direction, Flow Accumulation, Stream Extraction)  
- Raster combination and flood risk visualization
- A detailed workflow diagram is included in the [reports folder](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Reports).
---

### Discussion
The analysis demonstrates a clear qualitative link between urban encroachment and increased flood risk. While historical water management systems prioritized both flood mitigation and water storage, modern development has largely ignored these principles. This project serves as a preliminary assessment and highlights the need for more quantitative hydrological and urban planning studies to support sustainable development and disaster mitigation in Chennai.

---

### Repository Structure
- **[ArcGISFiles](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/ArcGISFiles)/** – ArcGIS Pro project files and toolboxes  
- **[Data](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Data)/** – Raster and vector datasets used in the analysis  
- **[Maps](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Maps)/** – Exported maps (PDFs and images)  
- **[Reports](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Reports)/** – Final report, presentation slides, and supporting figures  

---

### Key Outputs
- LULC maps (1985 and 2023)  
- LULC change detection [map](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Maps/Change_LULC.pdf)  
- Elevation and slope [maps](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Maps/Elevation_Chennai.pdf)  
- Flood risk [map](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Maps/FLOODRISKMAPPED.pdf) for Chennai 
- Final project [report](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/GIS_Nandhika_FinalProject_Report.pdf) and [presentation](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/blob/main/Reports/FW5550_FinalProject.pptx)

---

### Links
- Final Report: [Link to PDF](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Reports) 
- Key Maps and Figures:[Link to maps folder](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Maps)
- Data Sources: [Links to datasets](https://github.com/nandhika03/Chennai-analyzing-flood-causes-ArcGISPro3/tree/main/Data)

---

### Future Work
- Incorporating higher-resolution DEM and rainfall datasets  
- Quantitative flood modeling and validation  
- Integration with urban planning and policy analysis  
- Scenario-based simulations for future urban growth  

---

### Citation
Please cite this project appropriately if you use or reference any part of this work. Formal citations for datasets and tools are provided in the final report.

---
