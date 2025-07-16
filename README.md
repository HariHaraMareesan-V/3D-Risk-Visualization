# 3D-Risk-Visualization
This project visualizes district-wise risk levels in a 3D elevation map using Python, Matplotlib, and GeoPandas. Each district is represented as a 3D polygon whose height corresponds to its risk level.

#Key Features

3D Risk Elevation Map: Each district is extruded vertically based on its risk level.
Color-Coded Risk Levels:
5 → Dark Blue (Very High Risk)
4 → Light Sky Blue (High Risk)
3 → Grey (Moderate Risk)
2 → Wheat (Sandal) (Low Risk)
1 → Maroon (Very Low Risk)
No Overlap View: Adds slight horizontal spacing between districts to prevent visual overlap.
Custom Legend: Shows risk level colors for easy interpretation.
Interactive 3D Camera View: Rotatable & zoomable for better visualization.


#How It Works

Load GeoData
Merges shapefile (district boundaries) with risk-level data.
Process Geometry
Extracts polygons (or multipolygons) for each district.
3D Extrusion
Creates top surfaces & vertical walls for each district polygon based on risk height.
Color Mapping
Uses a predefined color dictionary for each risk level.
Legend & Camera
Adds a custom legend and sets a camera view for a clear district layout.

#Tech Stack

Python
GeoPandas – for spatial data handling
Matplotlib (mplot3d) – for 3D plotting
Shapely – for polygon geometry

#Install dependencies:

pip install geopandas shapely matplotlib

#Run the script:

python 3d_risk_map.py

#Output:

A 3D interactive plot showing district boundaries with elevated risk levels.


