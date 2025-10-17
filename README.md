# Week-5-6-Data-Preprocessing-HW

## `內容說明`

在此份報告中，利用NHANES data, 2021–2023資料集中下述3份檔案：
I.	DEMO_L.xpt (Demographics Data: Demographic Variables and Sample Weights)
-	Coding book: https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm
II.	BMX_L.xpt (Examination Data: Body Measures)
-	Coding book: https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/BMX_L.htm 
III.BPXO_L.xpt (Examination Data: Blood Pressure - Oscillometric Measurements)
-	Coding book: https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/BPXO_L.htm

NHANES 2021–2023 是一項全美代表性調查，結合了問卷訪談與身體檢查，收集美
國人口的健康狀況、營養攝取、疾病盛行率、生理與生化測量資料。這些資料常用
於公共衛生研究，例如慢性病（如糖尿病、肥胖、高血壓）之流行趨勢分析與營養
政策制定。 
基於此資料集進行分析並回答下列問題。 

Q1. Among adults aged ≥20 years in the 2021–2023 NHANES, observe the 
association between BMI and mean systolic blood pressure (SBP) and does the 
association vary between sex ? 
Q2. Among all the subjects in 2021-2023 NHANES dataset, observe the distribution 
of BMI in different races and education levels 
I. 
What is the distribution of educational attainment (EDU) and ethnicity (Race) 
in your data? (Please calculate the number and proportion of each EDU and 
Race, and output the table) 
(a) For Education levels, please refer to the variable “dmdeduc2” 
(b) For Race categories, please refer to the variable “ridreth3” 
II. Please use boxplots to visualize the BMI distribution in different races and 
education levels (2 outputs: BMI as X variable and filled by education and 
vice versa) 
III. Please state your brief conclusion about the plots (Do not need the 
statistical testsyou’re your inference) 
Q2. Among all the subjects in 2021-2023 NHANES dataset, BPX is the data including 
three times of examination of blood pressure (SBP & DBP). The values were 
recorded in different columns (bpxosy1-3; bpxodi1-3) (Reminder: please use the 
“cleaned” BP data). 
I. 
Currently the dataset is stored in a wide format, meaning that each 
measurement is placed in a separate column. Please reshape the dataset 
into a long format, so that each row represents a single measurement, and 
include the following variables: 
(a) seqn: Participant ID 
(b) measure (new defined): Measurement type (SBP or DBP) 
(c) trial (new defined): Trial number (1, 2, or 3) 
(d) value (from each BP value): The recorded blood pressure value 
II. After reshaping the dataset, create a boxplot to compare the distribution of 
SBP and DBP across the three trials and facet by the measurement type. 
III. Now, suppose we are only interested in the two trials that show the largest 
difference for each subject. Please complete the tasks aboved. 
IV. Please infer whether these blood pressure values were measured at long 
intervals or on the same day to avoid errors.

## `文件說明`

#### `Week 5-6 Data Preprocessing HW`
使用R markdown製作的報告檔案，包含程式碼以及相關圖表與闡述。

#### `Week 5-6 Data Preprocessing HW`
報告的pdf檔。

#### `data raw`
內含此次資料分析所需使用的資料：
1.DEMO_L.xpt
2.BMX_L.xpt
3.BPXO_L.xpt

