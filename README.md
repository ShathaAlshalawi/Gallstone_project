# Gallstone Classification Project   

 

## Project Description   



This project uses the **Gallstone-1 dataset** to study patterns in patient health data and to build predictive models that can help identify 
whether a person is at risk of developing gallstones.


Gallstones are a widespread health issue that can cause severe abdominal pain and other complications if not detected early. By analyzing medical attributes such as age, weight, cholesterol, and lifestyle factors, **our goal is to**:


- **Support Early Detection**: Provide insights that could assist doctors in recognizing patients at higher risk.  
- **Reduce Complications**: Early predictions can help patients take preventive measures before gallstones become severe.  
- **Promote Healthcare Awareness**: Show how data analysis can contribute to real-world medical challenges and improve quality of life.  


In addition to prediction, we also explore **clustering methods** to see if patients naturally group into patterns that may not be immediately visible to medical staff.
This could provide additional knowledge for research and public health.


 
--- 



## Motivation   

Gallstones are one of the most common digestive diseases. Early diagnosis can reduce pain, 
improve treatment decisions, and help patients avoid serious complications.   


We chose this dataset because it represents a real medical challenge and allows us to 
practice both **classification and clustering** methods in a way that is socially impactful.   

 


--- 

 



## Dataset Information   

- **Dataset Name:** Gallstone-1   

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/1150/gallstone-1)   

- **Number of Instances:** 319   

- **Number of Features:** 16 medical and lifestyle attributes   

- **Class Label:** Gallstone Status (0 = Present, 1 = Absent)


--- 
## Data Processing: Cleaning and Preparing the Data 

To ensure our models are accurate, the raw data was cleaned and standardized in four steps:

1.  **Converting Data Types:** We translated categorical data into a **numerical format** that the computer can process, expanding the dataset from 16 to **37 features**.
2.  **Removing Outliers:** We identified and removed **73 extreme patient records** (outliers) that could mislead the analysis. The final dataset includes **246 patient records**.
3.  **Standardizing Scales:** We rescaled all numerical features to a consistent range (0 to 1). This prevents features with naturally larger values from unfairly dominating the analysis.
4.  **Result:** The cleaned and processed data is saved as `Preprocessed_dataset.csv`.

---

## Data Visualizations

We created three types of visualizations to understand the dataset:

1. **Scatter Plot (Age vs BMI):**  
   Shows the relationship between a patient’s age and BMI. Points are colored by Gallstone Status, helping us see if certain ages or BMI values are more likely to have gallstones.

2. **Histograms (Numeric Attributes):**  
   Show the distribution of numeric data like Age, BMI, Cholesterol, and Glucose. These plots help identify which ranges of values are most common among patients.

3. **Bar Plots (Nominal Attributes):**  
   Show counts for categories such as Gender, Comorbidity, and Gallstone Status. This makes it easy to compare groups and check for patterns, like whether more males or females have gallstones.

---
## Data Analysis and Feature Insights 

Our analysis of the prepared data revealed three main insights:

* **Feature Relationships:** Charts like **Age vs. BMI** showed patterns and clusters among high-risk patients. We also found a strong link between specific **pre-existing conditions (Comorbidities)** and gallstone presence, identifying key risk factors.
* **Data Preparation Check:** We reviewed the spread of variables to confirm the need for standardization, ensuring no single factor dominates the model.
* **Class Balance:** The dataset was confirmed to be **well-balanced** (nearly equal patients with and without gallstones), meaning our models will not be biased toward one outcome.

---

### Class Distribution   




| Class | Meaning              | Instances |
|-------|----------------------|-----------|
| 0     | Gallstones Present   | 161       |
| 1     | Gallstones Absent    | 158       |
| **Total** |                      | **319**   |


 

--- 


 

## Students   

- Dana Alattas
- Shatha Alharthi
- Mai Alghamdi
- Lina Alsaaran   

## Project Supervisor  
Dr.Lama Alsudais

