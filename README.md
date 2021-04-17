# matplotlib-challenge

This repository reads in a dataset containing a tumor volume study in mice for different drug treatments and uses pandas, matplotlib, and jupyter notebooks to create various summary graphics/calculations. Two files are read in and merged together to perform the analysis. The first file, **study_results.csv**, is of the following format:

  ```csv
Mouse ID,Timepoint,Tumor Volume (mm3),Metastatic Sites
b128,0,45,0
f932,0,45,0
g107,0,45,0
a457,0,45,0
  ```
  
  The second file, **mouse_metadata.csv**, is structured as follows:
 
 ```csv 
"Mouse ID","Drug Regimen","Sex","Age_months","Weight (g)"
"k403","Ramicane","Male",21,16
"s185","Capomulin","Female",3,17
"x401","Capomulin","Female",16,15
"m601","Capomulin","Male",22,17
  ```
  
  After merging these 2 datasets together, the following outputs are created:
  
  1. Bar chart containing the number of measurements taken for each treatment regimen (outputs created using both matplotlib and pandas plot functionality)
  2. Pie chart showing the distribution of male vs. female mice in the study (outputs created using both matplotlib and pandas plot functionality)
  3. Quartile and outlier analysis of 4 specific treatments in the study, along with corresponding box and whisker plots
  4. Line plot of tumor volume over time for specific selected mouse ID
  5. Scatter plot of tumor volume versus weight of specific treatment regimen 
  6. Calculated correlation coefficient and linear regression line/equation for scatter plot generated in # 5
