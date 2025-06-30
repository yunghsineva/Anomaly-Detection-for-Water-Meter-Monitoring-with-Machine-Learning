## Anomaly-Detection-for-Water-Meter-Monitoring-with-Machine-Learning

## Project Overview

The research aim is to effectively identify and predict unusual household water usage patterns on a daily and weekly basis using machine learning algorithms.
Different from existing knowledge, the novelty of the hybrid model inthis paper is its ability to combine supervised and unsupervised learning methods. It improves both
accuracy and efficiency compared to solely unsupervised or supervised models.

### 🎯 Objectives

Building a hybrid model, which combines the advantages of supervised and unsupervised methods, using unsupervised learning to identify leakage features and building a supervised model to conduct prediction on time-series meter data.


## 🧠 Methodology

1. **DATA COLLECTION**  
- Extracted six months of 2016 was collected from HELIX (open-source)
- Sample included 10% of consumers (around 100 users).
- 361,712 readings of hourly household water consumption.

2. **1st Data preprocessing**  
   - Dropping missing and duplicate values
   - Changing data type
   - Feature engineering: separates time series into time durations (morning, afternoon, and night), and days of the week.
   - Standardization

3. **Unsupervised METHOD (DBSCAN)**  
   DBSCAN helps identify unusual patterns in water usage data by assign data to different clusters based on their similarity and find out the noise in the data.

4. **2nd Data preprocessing**  
- Identified outliers to distinguish between normal and anomalous behaviors within the same cluster. 
- Manually label the outliers and class = -1 (noise class classified by DBSCAN) as Anomaly =1 
- Split data into training (80%) and test (20%) sets, adjusting class weights for data imbalance.


---

## 🗂 Repository Structure
