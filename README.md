# Canopy System Phenotyping with PlantCV

The canopy phenotyping pipelines from the paper "Scion and rootstock genotypes drive root system dynamics in modern apple orchards."

## Description 
This code is designed to phenotype apple canopy images.  

## Basic Usage
Language: Python 

Environment: This code was written in a conda environment, the dependencies can be found in the environment.yml file

This code was written using Jupyter Notebook, so it is suggested to use environments compatible with the .ipynb filetype (i.e. JupyterNotebook, VSCode, etc.)

## Image Capture 
Image the canopy from a known distance or with an object of a known size with a white background (we used a large sheet)

If you cannot capture only the white sheet in the background, preprocess the images in ImageJ (Fiji) to remove the background using the following protocol: 
1. Import images into ImageJ
2. Remove background objects using a combination of the clear outside and fill shape tools

## Scale: 
This code does not account for a scale marker. You can convert the pixel output to actual units after using either an included scale marker (this can be done with ImageJ) or if you know the distance the camera was from the canopy. 
 
## Main pipeline: 
1. Download canopy analysis final.ipynb file and sample data (canopy input)
2. Run the first piece of code to import all libraries and functions 
3. Run the second and third piece of code to create the  necessary functions
4. Change the folder paths and the name of the output data set (outputs as a .csv). The output folder should not be in the input folder. 
- folder_path (string) = "full path to folder containing images"
- data_name_out (string) = "name of output file (.csv)"
- output_folder_path(string) = "full path path to folder for output dataset and processed images"
5. Run the final function canopy_analysis(folder_path, data_name_out, output_folder_path) 

Other information: 
-
This code was written in MacOS 
