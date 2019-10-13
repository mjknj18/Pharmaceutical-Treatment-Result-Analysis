# Pharmaceutical-Treatment-Result-Analysis

The goal of this project was to calculate and display various performance metrics for four phareceutical cancer treatments (Capomulin, Infubinol, Ketapril, Placebo) on test mice over a 45 day treatment period. Since the baseline data was provided in CSV format, Python with Pandas, Numpy, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as calculate the desired outputs.

## Questions

1. For each treatment, what was the tumor volume change in the test mice over the length of the treatment period?
2. For each treatment, what was the metastatic site change in the test mice over the length of the treatment period?
3. For each treatment, what was the survival rate of the test mice over the length of the treatment period?
4. For each treatment, what the percentage change in tumor volume in the test mice over the length of the treatment period?

## Datasets

1. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical%20Treatment%20Data/clinicaltrial_data.csv
2. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical%20Treatment%20Data/mouse_drug_data.csv

## Tasks

### Tumor Response to Treatment

1. Import the mouse data and clinical data CSV files as individual Pandas data frames.
2. Merge individual data frames into combined data frame based on Mouse ID.
3. Split the combined data frame into groups by treatment and time index.
4. Calculate the average mean tumor volume for each treatment at each time index.
5. Calculate the tumor volume standard error for each treatment at each time index.
6. Create individual data frames for average volume and standard error data.
7. Plot the average volume data versus time with error bars defined by standard error data.

### Metstatic Spread During Treatment

1. Split the combined data frame into groups by treatment and time index.
2. Calculate the average number of metastatic sites for each treatment at each time index.
3. Calculate the metastatic site standard error for each treatment at each time index.
4. Create individual data frames for average metastatic site and standard error data.
5. Plot the average metastatic site data versus time with error bars defined by standard error data.

### Survival During Treatment

1. Split the combined data frame into groups by treatment and time index.
2. Calculate the number of surviving mice for each treatment at each time index.
3. Create a data frames for survivng mice data.
4. Plot the survivng mice data versus time.

### Tumor Change Over 45 Day Treatment

1. Calculate percent change in average tumor volume data over the full length of treatment period.
2. Plot the percent change data for each treatment.

## Results

1. https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Pharmaceutical_Treatment_Results_Main.ipynb

### Tumor Response to Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Tumor_Response_to_Treatment.jpg>

### Metstatic Spread During Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Metastatic_Spread_During_Treatment.jpg>

### Survival During Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Survival_During_Treatment.jpg>

### Tumor Change Over 45 Day Treatment

<img src = https://github.com/mjknj18/Pharmaceutical-Treatment-Result-Analysis/blob/master/Images/Tumor_Change_Over_45_Day_Treatment.jpg>

## Observations

Looking at the tumor volume change over time for each treatment, it is clear that Capomulin had the greatest positive effect on shrinking cancer cells. Total tumor volume in the mice receiving Capomulin dropped by just under 10 mm3 on average over the forty-five day test period. In contrast, total tumor volume in the mice receiving Infubinol, Placebo, or Ketapril increased by 20, 22.5, and 25 mm3 respectively throughout the study. This data, additionally supported by the tumor volume percent change data, clearly shows that Capomulin is the drug of choice for shrinking these cancerous tumor cells.

Picking the most effective drug of the group is slightly more challenging when it comes to the data comparing metastatic sites versus time. All four of the treatments in question showed metastatic site increases, but two stood out in particular as being better. Capomulin did have the lowest increase at 1.5 sites, while Infubinol wasn't far behind at 2. They were followed by Ketapril and Placebo both around 3.25, which clearly weren't as effective. Therefore, none of the treatments were able to prevent metastatic site increases.

Similar to the tumor volume change data, the mice survival rate data shows Capomulin had a clear advantage over the other three treatments. Over the length of the study, more mice treated with Capomulin survived and this effect was becoming evident even after the first ten days. At the end of the forty-five day period, over 80 percent of the mice on Capomulin survived compared to under 50 percent for Infubinol, Ketapril, and Placebo. Therefore, it was once again proven that Capomulin is the best choice for reducing the spread of these cancer cells and increasing the survival rate.

## Disclaimer

The baseline data used for this analysis was provided by a third party source and its accuracy in relation to actual cancer pharmaceutical drug testing data is unknown.