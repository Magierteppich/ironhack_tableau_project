# ironhack_tableau_project
Applying knowledge on using Tableau to visualize data. 

## Animal Control and Rescue Center (ACRC) in Baton Rouge

Banton Roupge is the capital city of the US State Louisiana. As part of the open source project, the city of Banton Rouge made the animal incidents records of the Animal Control and Rescue Center available (https://data.brla.gov/Public-Safety/Animal-Control-Incidents/qmns-hw3s). 

The Dataset containts records of all filed cases of ACRC starting from 2012. 

## Approach

## Step 1: 

After reading and understanding the structure of the data, I used Python to clean the data. The detailed steps can be read in the workbook: https://github.com/Magierteppich/ironhack_tableau_project/blob/master/workbook/01_data_review_data_cleaning.ipynb

My key learnings from this step is: 
- Understand your data first before cleaning
- Deduplicate first! 
- Have a goal in mind first helps to be focused while cleaning 
- Key challenge: select the relevant columns to use and understand the NaN values

## Step 2: 

When first plotting the data in Tableau, one can observe: 1) for year 2016-2018, the number of cases are as doubled compared to the preious years and 2019. 2) for year 2016-2018, almost half of the records didn't contain complete information, especially for SERVICE CODE, location, species, breed etc. 

Therefore, I developed hypothesis based on my understanding of the data and validated my hypothesis by using panda again. Details can be read in workbook 2: https://github.com/Magierteppich/ironhack_tableau_project/blob/master/workbook/02.%20deep_dive_missing_data.ipynb

The key challenge was to discover the pattern in the data and from there draw hypothesis without domain knowledge. 

Key learnings:
- It helps to get a sample and open it in Excel, as one can see the data in a bigger picture. I could identify the data pattern by using this method. 

## Step 3: 

I had a clear story in my mind. So I wrote the story down and produced the plots as needed. During this step, no bigger challenges encountered. 

Lessons learned: Formatting in Tableau takes up as much time as plotting data. 

## Step 4: 

I had the idea to convert the adress into geocodes in order to plot them on a map as well. I used geocoder to access the opencage API and was able to operate the conversion. However, the unpaid version is limited to 250 entries per day and my dataset hat more than 30.000 adresses. I have also started using the Bing Map API to do the job. But due to time constraints, I decided to leave it out for this project. However, the results I have done so far can be read in workbook 3: https://github.com/Magierteppich/ironhack_tableau_project/blob/master/workbook/03.%20Geocoding.ipynb

Lessons learnd: I need to review the API lecture. :D 

## LINKS:

Tableau public: https://public.tableau.com/profile/tian4529#!/vizhome/BatonRougeAnimalControlanRescueCener/Story1?publish=yes
