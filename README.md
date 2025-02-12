### AIRCRAFT RISK ANALYSIS PROJECT
## Introduction

# Business Problem
Company XYZ is looking to venture into new enterprises as it expands its portfolio. They have a keen interest in the aviation industry but would like further research done as they are not knowledgeable <brk> with the industry. Specifically, they are interested in knowing the potential risks in aircraft before they embark on this new business venture. The company's stakeholders recognize the importance of making data-driven decisions.

In the quest to answer the Company's questions on the potential risks in aircraft, an explorative data analysis on current data about aircraft incidences was done. Data from the National Transportation Safety Board (NTSB) includes all aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters. The files are **AviationData.csv** and **USState_Codes.csv**

The questions we sought to answer to establish the low-risk aircraft that the head of aviation at Company XYZ will use to make a decision when purchasing aircraft.
1. Which aircraft are most common in accidents?   
2. Which aircraft have been involved in the fewest accidents?  
3. What is the trend in accidents/incidents cases over the years in the industry?
## Loading the data
**load the libraries**
```import os 
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns```

**load the file**
```data_df = pd.read_csv("AviationData.csv", encoding="ISO-8859-1", low_memory=False)
data_df.head()```

**checking the data type**
```data_df.dtypes```

**checking the structure**
```data_df.info()```

**check for missing values**
```data_df.isnull().sum()```

**check for the percentage of missing data rounded off to 2 decimal places**
```percentage_missing = np.round(((data_df.isnull().sum() / len(data_df)) * 100), 2)
percentage_missing.sort_values(ascending=False)```

**Check for duplicated data**
```data_df.duplicated().any```

From the above, there is no duplicated data but there are columns that are highly missing data and some of these columns are crucial for our analysis. 
We now have an idea of what the data looks like and established that there are missing values in majority of the columns. Though, it is worth noting that the categorical columns have few data missing.
Lets now answer our three questions.

**1. Which air crafts are most commonly involved in accidents from the data frame data_df?**
![image](https://github.com/user-attachments/assets/636d4e3f-4659-4d32-8881-6e1925617973)
![image](https://github.com/user-attachments/assets/b82ea832-a991-4507-825b-33051fc6952d)
**2. The makes and models of air crafts that have been involved in the fewest accidents?**
![image](https://github.com/user-attachments/assets/dbfdef3f-ebde-417e-9cde-13c56fa5e7d1)
**3. To wind up with our analysis, check what the accident trend has been over the years.**
![image](https://github.com/user-attachments/assets/450a31a5-eebc-4f90-8f50-a6fab03fcf21)

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


   


 
