# building-datasets
The repository contains code for importing and analyzing European building data.

0-[_functions]-0_methods.ipynb
The notebook contains common functions for loading raw data, loading data enriched with NUTS information using the dask_geopandas library, a function for spatial join executed in parallel to calculate the area of each building, the number of vertices, an aggregation function for the results obtained from the spatial join, and a function for drawing the map of provinces of each input country with respect to the degree of urbanization.

1-[data_processing]-0_mapping_buildings_to_nuts.ipynb: This notebook contains the code for processing raw data and mapping each building to the province (NUTS 3 LEVEL) in which it is located.

1-[data_processing]-1_compute_overlapping_area_among_datasets.ipynb: The code performs intersection between pairs of datasets to measure the degree of overlap of building geometries. Additionally, an intersection is performed across all datasets to measure the common area. Also, some images showing individual intersections between pairs of datasets are generated as output.

2-[data_analysis]-0_dataset_comparison.ipynb: This notebook contains the code used to compute statistics for comparing various datasets.
