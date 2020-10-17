# README for project: comparing_filters

## Author details: 
Name: Sam Huguet  
E-mail: samhuguet1@gmail.com

## Description:   
- This purpose of this package is to allow a user to compare the effect of different filters which tend to smooth/blur images. 
- The user selects an image, and the code outputs a montage displaying the effect of each individual filter (listed blow), alongside the segmentation output (with a threshold determined by the Otsu method). 
  - [A gaussian filter](https://en.wikipedia.org/wiki/Gaussian_filter#:~:text=In%20electronics%20and%20signal%20processing,as%20it%20has%20infinite%20support) (smooths/blurs image). 
  - [A median filter](https://en.wikipedia.org/wiki/Median_filter#:~:text=The%20median%20filter%20is%20a,edge%20detection%20on%20an%20image) (smooths/blurs image). 
  - [A maximum filter](https://reference.wolfram.com/language/ref/MaxFilter.html) (does not smooth/blur image, but yields similar effect).  
  - [A minimum filter](https://reference.wolfram.com/language/ref/MinFilter.html) (does not smooth/blur image, but yields similar effect). 
- For each ```.py``` file provided, there is an accompanying ```.ipynb``` file for those who use JupiterLab.

## How to use the code: 

# First, open the RUNME.py file. 

(1) Within the ```RUNME.py``` file, first load in the module functions with the following code: 
```
# Import functions from the module file. 
from comparing_filters_functions import *
```

(2) Then, with the following function...
```
# Function input args: None. 
# Function returns: The file path corresponding to the image selected by the user. 
file_path = file_selection_dialog()
```
... a GUI will appear (see the image below), within which, the user should select the image they which to filter and segment.

<img src="https://github.com/SamHSoftware/Image-Analysis/blob/main/comparing-filters/img/File%20selection.PNG?raw=true" alt="file selection GUI" width="500"/>
