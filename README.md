# Pharmaceutical-Treatment-Result-Analysis

The goal of this project was to calculate and display various performance metrics for four phareceutical cancer drugs (Capomulin, Infubinol, Ketapril, Placebo) on test mice over a 45 day treatment period. Since the baseline data was provided in CSV format, Python with Pandas, Numpy, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as calculate the desired outputs.

## Questions

1. For each cancer drug, what was the tumor volume change in the test mice over the length of the treatment period?
2. For each cancer drug, what was the metastatic site change in the test mice over the length of the treatment period?
3. For each cancer drug, what was the survival rate of the test mice over the length of the treatment period?
4. For each cancer drug, what the percentage change in tumor volume in the test mice over the length of the treatment period?

## Datasets

1. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical%20Treatment%20Data/clinicaltrial_data.csv
2. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical%20Treatment%20Data/mouse_drug_data.csv

## Tasks

### Tumor Response to Treatment

1. Import the mouse data and clinical data CSV files as individual Pandas data frames.
2. Merge individual data frames into combined data frame based on Mouse ID.
3. Split the combined data frame into groups by drug and time index.
4. Calculate the average mean tumor volume for each drug at each time index.
5. Calculate the tumor volume standard error for each drug at each time index.
6. Create individual data frames for average volume and standard error data.
7. Plot the average volume data versus time with error bars defined by standard error data.

### Metstatic Spread During Treatment

1. Split the combined data frame into groups by drug and time index.
2. Calculate the average number of metastatic sites for each drug at each time index.
3. Calculate the metastatic site standard error for each drug at each time index.
4. Create individual data frames for average metastatic site and standard error data.
5. Plot the average metastatic site data versus time with error bars defined by standard error data.

### Survival During Treatment

1. Split the combined data frame into groups by drug and time index.
2. Calculate the number of surviving mice for each drug at each time index.
3. Create a data frames for survivng mice data.
4. Plot the survivng mice data versus time.

### Tumor Change Over 45 Day Treatment

1. Calculate percent change in average tumor volume data over full length of study.
2. Plot percent change data for each drug.

## Results

1. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical_Treatment_Results_Main.ipynb

### Tumor Response to Treatement

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Tumor_Response_to_Treatment.jpg>

### Metstatic Spread During Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Metastatic_Spread_During_Treatment.jpg>

### Survival During Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Survival_During_Treatment.jpg>

### Tumor Change Over 45 Day Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Tumor_Change_Over_45_Day_Treatment.jpg>

## Observations

Looking at the tumor volume change over time for each treatment, it is clear that Capomulin had the greatest positive effect on eliminating cancer cells. Total tumor volume for mice recieving Capomulin dropped by just under 10 mm3 on average over the forty-five day test period. In contrast, total tumor volume for mice recieving Infubinol, Ketapril, or Placebo increased by 20, 25, and 30 mm3 respectively throughout the study. This data, along with the tumor volume percent change data, is a clear indication that Capomulin is the drug of choice for reducing cancer cell size.

Picking the best drug of the bunch is a little tougher when it comes to the data comparing metastatic sites versus time. All four of the drugs in question showed a metastatic site increases, and the overall change amounts over the forty-five day period were fairly close. Capomulin did have the lowest increase at 1.5 sites, but Infubinol wasn't far behind at 2. These were followed by Ketapril and Placebo both around 3.25. Therefore, no drug had a clear benefit when it came to mitigating the growth of metastatic sites.

Similar to the tumor volume change data, the mice survival rate data give Capomulin a clear advantage over the other three drugs of interest. Over all stages of the study, more mice treated with Capomulin survived cancer and this effect was more pronounced in the later stages of the study. At the end of the forty-five day period, over 80 percent of the mice on Capomulin survived compared to under 50 percent for Infubinol, Ketapril, and Placebo. Therefore, it was once again proven that Capomulin is the best choice fore reducing the spread of cancer and increasing survival rate.

## Disclaimer

The baseline data used for this analysis was provided by a third party source and its accuracy in relation to actual cancer pharmaceutical drug testing data is unknown.