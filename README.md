# STA141_Final
STA141 Final Project: Wildfire Visualization

The final HTML render is provided as STA141_Final_Project_JovanRadovic.html. 

The two additional datasets used in the creation of this project, ERA5 and PRISM, are too large to fit into the repository. Information on their retrieval is detailed below. 

## Files:
The rmd file final_project.rmd was knitted to produce the submitted html. The training of the models was done in a separate ipynb notebook, provided as training_colab.ipynb, in order to allow GPU access from colab. The ipynb notebook produced the model_results.rds file (stored in data/processed), which details the performance statistics of the models, across all validation years. If seeking to reproduce the render, first run the ipynb script, place the resulting rds in the appropriate directory, and then run the rmd file. 

## Datasets:
### PRISM: 
* Monthly data for the years 1992-2015 was downloaded from: https://prism.oregonstate.edu/data/. If seeking to recreate the file, include this in the "data/raw" directory. 

### ERA5: 
* Monthly data for the years 1992-2015 was downloaded from https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=download. All variables for the categories of 'temperature and pressure', 'evaporation and runoff', 'wind', and 'precipitation and rain' were donwloaded. The resulting file is extremely large (20+ GB), and should be placed in "data/raw" if seeking to recreate the project. 
