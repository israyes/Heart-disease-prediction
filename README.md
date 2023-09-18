[heart](https://github.com/abayomi-hayes/Heart-disease-prediction/assets/119630129/39ce7361-f885-49b3-9639-4b3eac0d223f)
# Heart-disease-prediction
Predicting heart disease from three different dataset
a deep learning model was applied to one of the dataset, binarization, one hot encoding when needed

he inception phase of this heart disease prediction endeavor entailed the strategic procurement of pertinent datasets. A triad of datasets was judiciously selected, each proffering indispensable insights conducive for heart disease prognostication: 

Dataset 1: Cleveland Heart Disease Dataset 

Sourced from the esteemed UCI Machine Learning Repository, this dataset encapsulates medical records curated by the Cleveland Clinic Foundation. It encompasses salient clinical variables, such as age, gender, the typology of chest discomfort, and angiographic data. The multifaceted nature of these parameters renders it a high-dimensional dataset, rendering it indispensable for the predictive modeling process. 

Dataset 2: 2020 annual CDC Survey Data Of 400k Adults Related To Their Health Status 

This dataset, for the temporal frame of 2020, collates information pertinent to the health status of an estimated 400,000 American adults. It is an integral segment of the Behavioral Risk Factor Surveillance System (BRFSS), an initiative pioneered by the CDC. Annually, BRFSS orchestrates telephone-based surveys, meticulously accumulating cardinal health-centric data from the American populace. Over its operational timeline, its outreach has burgeoned, now encapsulating all 50 states, the District of Columbia, and three U.S. territories, culminating in a staggering 400,000 interviews every annum. Structurally, the dataset boasts 319,795 entries and 18 attributes, encompassing variables like alcohol intake, stroke incidence, physiological and psychological health parameters, diabetes prevalence, ethnic categorization, and tobacco consumption metrics, among others. 

Dataset 3: HeartDisease1988 A Multi-National Heart Disease Dataset  

Hailing from the year 1988, this comprehensive dataset amalgamates data from four distinct geographical locales: Cleveland, Hungary, Switzerland, and Long Beach V. It houses a grand total of 76 attributes, inclusive of the prognostic variable. Notably, canonical research exploits have predominantly been fixated on a select subset comprising 14 of these attributes. The 'target' attribute, pivotal to this research, demarcates the presence or absence of heart disease in patients, represented by binary integer values: 0 (indicative of no disease) and 1 (signifying disease presence). 

Data Preprocessing:  

Dataset 1: 

Cleveland Heart Disease Dataset 

In the preliminary phase, a meticulous examination of the data structure was undertaken via descriptive statistical measures to glean an intricate understanding of the dataset's intrinsic attributes. By invoking functions such as "describe" and "info," an in-depth comprehension of the dataset's attributes and their associated characteristics was established. Subsequent to this, a rigorous scan for missing values was done, which fortuitously confirmed the absence of null entries within the dataset. 

 

 

Dataset 2:	 

2020 annual CDC Survey Data Of 400k Adults Related to Their Health Status 

The preprocessing phase for this dataset necessitated the identification of both categorical and numerical variables inherent to the dataset. The successful differentiation between categorical and numerical variables is paramount, as it steers the subsequent analytical methodologies, preprocessing strategies, and the eventual selection of predictive models. This endeavor underpins the assurance of achieving accurate and insightful analytical outcomes. 

 

Dataset 3: 

Heart Disease1988 A Multi-National Heart Disease Dataset 

The first step in this preprocessing process is a rigorous inspection of the data structure. Features such as "describe" and "info" were employed to obtain a granular overview of the dataset's composition. In tandem, an assessment for potential "nan" values was executed, corroborating the dataset's integrity by highlighting the absence of null entries. Following this, a focused exploration was directed towards ascertaining the categorical and numerical attributes embedded within the data. 

 

Categorical and numerical Variables  

The categorical variables found are 'anaemia',, ‘diabetes’, ‘high_blood_pressure’, ‘sex’, ‘ smoking’, and ‘DEATH_EVENT’ while the numerical variables 'age', 'creatinine_phosphokinase', 'ejection_fraction', 'platelets', 'serum_creatinine', 'serum_sodium','time'.   

 

 

Data Cleaning 

Dataset 1, 2 and 3 

The initiation of the data cleansing phase necessitated a comprehensive assessment for "nan" values. Identified gaps were subsequently filled leveraging the modal values of the respective attributes, thereby maintaining data integrity and consistency. It was observed that the datasets’ architecture predominantly employs a binary nomenclature, characterized by dichotomous "yes" and "no" responses. Given that such categorical representations can impede the efficacy of prediction in machine learning algorithms, a transition was imperative. Thus, binary encoding techniques were harnessed, facilitating the conversion of "yes" and "no" responses to '1' and '0' respectively. This transformation not only enhances the data's congruence with machine learning protocols but also augments the model's proficiency in discerning intricate patterns and correlations. 

 

Feature Selection 

 

Dataset 1 and 3	 

For the task of predicting the pivotal target variable, "Death event", a curated subset of 14 attributes was leveraged. Owing to their intrinsic even distribution, there was a strategic omission of any requisite binarization for these columns, preserving their authentic representation. 

Dataset 2: 

An astute selection of features was undertaken to judiciously prune the dataset, thus attenuating dimensionality and bolstering model efficacy. Distinct columns, namely ["Race","GenHealth","AgeCategory"], were subjected to one-hot encoding, a transformative process pivotal for converting categorical variables into their corresponding binary vector representations. This discerning process of feature selection was orchestrated with the dual guidance of domain expertise and an in-depth data analysis. 

 

 

 

Data Scaling 

Dataset 1,2, and 3 

For the triumvirate of datasets under examination, the continuous attributes underwent a scaling process. The objective was to that they have similar ranges, thereby effectuating a congruous contribution from each feature in subsequent analytical processes. Numerical features were transmuted either through standardisation, yielding a resultant mean of 0 and a standard deviation of 1, or by constraining them within a predefined range. This scaling process makes sure all features have an equal say in the machine learning models, preventing any single feature with a larger range from having an outsized impact. 

 

 

 

 

 
