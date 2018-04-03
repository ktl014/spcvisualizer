# spcvisualizer
Real-time viewer for SPCBench Camera system data collection

### Background: 
After a year of collecting image data with the SPCBench camera system by ECE undergraduates of the SVCL, several issues with the imaging procedure have become apparent: dirty or smudged cuvettes, improperly set up sensor region, and multiple organisms per sample all contribute to poor dataset quality. These problems need to be resolved in order to run machine learning experiments on properly quality controlled datasets. Minimizing the number of garbage images is the top priority of this project. 

### Goal: 
Design and implement a modular, real-time visualizer for the SPCBench camera system to improve our data collection methodology. Viewing real-time images will reduce the number of garbage images. Modular code will allow for flexibility when adding functional components in the future.

### Objectives: 
1. Write script that downloads images from the camera in real time
2. Modify spconvert.py to run dynamically as new images are coming in
3. Display color-converted images over web browser through websockets, such as Flask.

### Resources:
The following python scripts to help with this project can be found here. A brief description is provided with each script.
spconvert.py - converts raw images into color, saves them to a directory, and builds a static HTML page for ROI browsing. Currently runs on a file folder containing archived images.
spcpull_spcdata.py - downloads images from the camera system.

### Next Steps:
Add in the following functionalities:
Machine classification
Machine pose prediction
Computing pose variability
