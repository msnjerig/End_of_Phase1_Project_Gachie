###AIRCRAFT RISK ANALYSIS PROJECT
## Introduction

# Business Problem
Company XYZ is looking to venture into new enterprises as it expands its portfolio. They have a keen interest in the aviation industry but would like further research done as they are not knowledgeable <brk> with the industry. Specifically, they are interested in knowing the potential risks in aircraft before they embark on this new business venture. The company's stakeholders recognize the importance of making data-driven decisions.

In the quest to answer the Company's questions on the potential risks in aircraft, an explorative data analysis on current data about aircraft incidences was done. Data from the National Transportation Safety Board (NTSB) includes all aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters. The files are **AviationData.csv** and **USState_Codes.csv**

The questions we sought to answer to establish the low-risk aircraft that the head of aviation at Company XYZ will use to make a decision when purchasing aircraft.
1. Which aircraft are most common in accidents?   
2. Which aircraft have been involved in the fewest accidents?  
3. What is the trend in accidents/incidents cases over the years in the industry?
## Loading the data
# load the libraries
import os
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns


## Findings & Recommendations
From the analysis, the following was deduced:
1. The safest aircraft, make and model combined are;
   - Zlin model Z143,Z-42M and Savage
   - Zivkko Aeronautics Inc. mode Edde 540-T
   - a. le Francois model RANS S-7
   - A. H. Gettings model GLASSAIR
   - A pair of jacks model RV-6A
From the above findings, the company should invest in the above makes amd models as they have been involved in the fewest accidents.

2. The air craft makes with the highest accidents are as follows:
    1. Cessna
    2. Piper
    3. Beech
    4. Boeing
    5. Bell
The above air craft makes are the ones that have been prone to accidents and incidents over the years. If the company feels that they would want to invest in any of the makes, then they should conduct further research.

3. The accident trend of aircraft has gradually declined over the years from 1982 to date. The year 2020 recorded the lowest number of accidents but because it was the year with minimal air traffic due to the COVID-19 pandemic. The decline in accidents signifies that the industry has put in place and worked on mitigating factors that lessen accidents and incidents.


   


 
