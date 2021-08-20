# Flood risk of the Helsinki road network
_A network analysis determining travel time increases due to flooding in Helsinki_

## This repository
This repository contains all the data to support the research paper. It is split in the following directories:
 - [data-processing](data-processing): Contains the Python script to download and combine all the XYZ-coordinates for the Digital Elevation Model (DEM).
 - [data](data): Contains the input and intermediate data to reproduce the results.
   - The TomTom traffic data (TomTom-data-ext.csv and TomTom-data-int.csv).
   - The flooding data from the stormwater model linked to each road segment (edges-rain.csv).
   - The OD traffic regions linked to each node in the graph (node-regions.csv).
   - A GeoJSON file with the borders of each OD traffic region (region-polygons.json).
   - The road graph in GeoPackage format (road-graph-def.gpkg) and GraphML format (road-graph-def.graphml).
 - [graphs](graphs): The figures/graphs plotted (in SVG and PNG formats).
 - [images](images): The figures and images not belonging to another category (including the flood maps).
 - [model-images](model-images): Images of the sub-models in the stormwater model.
 - [results](results): The results gathered. CSVs are raw data, XLSX spreadsheets (starting with proc) are processed data.
 - [road-graph](road-graph): The Jupyter notebooks with all the Python code used in the road graph [compilation](road-graph/OSMnx_road_graph_compilation_BEP.ipynb) and [analysis](road-graph/OSMnx_road_graph_analysis_BEP.ipynb). Both are also viewable in Google Colab.
 - [segment-images](segment-images): Images of interesting road segments referred to in the paper.
 - [stormwater-depth](stormwater-depth): Contains the [RainDepthProduction.tbx](stormwater-depth/RainDepthProduction.tbx) toolbox, with all the tooling developed for the stormwater model in ArcGIS Pro.

