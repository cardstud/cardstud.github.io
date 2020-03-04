---
title: Framingham Cardiovascular study
subtitle: Predicting Heart Disease risk
image: /img/th.jpg
---

Coronary Heart Disease kills over 12 million people a year across the globe, according to WHO. In the United States alone, over 600,000 Americans die each year from Heart Disease, which equates to 1 in every 4 deaths. 

Consider these facts from the CDC  (https://cdc.gov/heartdisease/facts.htm):

    •	Heart disease is the leading cause of death for men and women in the U.S. from most racial and ethnic groups
    •	About 365,00 Americans die from Coronary Artery Disease each year, the most common type of heart disease
    •	Every 37 seconds, someone in the U.S. succumbs to the heart disease
    •	Every 40 seconds, someone has a heart attack in the US.
    •	Heart Disease costs the U.S. upwards of over 220 billion each year from 2014 to 2015

A 10-year cardiovascular study is being performed in Framingham, Massachusetts with the dual objective of trying to predict which risk factors will contribute the most to a person developing heart disease, as well as to determine what the overall risk of developing heart disease is for an individual.

By identifying which factors are high risks to developing cardiovascular disease, doctors and patients can work together to either eliminate, reduce or manage the overall risk of developing this deadly disease.
The study includes over 4,000 records with 15 attributes (risk factors), which are composed of demographic (such as sex and age), behavioral (such as current smoker, # of cigs per day), and medical (such as cholesterol, blood pressure) risk factors.

The 15 risk factors in this study are:
    •	male (sex): 		male = 1, female = 0
    •	age: 			age at time of the exam
    •	education: 		1 - Some HS, 2- HS or GED, 3-Some College or vocational school, 4- College
    •	currentSmoker: 	0 = nonsmoker, 1 = smoker
    •	cigsPerDay: 		# of cigarettes smoked per day (estimate)
    •	BPMeds:	 	0 = not on BP meds, 1 = on BP meds
    •	prevalentStroke: 	whether individual had a stroke prior
    •	prevalentHyp:		whether individual was hypertensive or not
    •	diabetes:		 0 = No, 1 = Yes
    •	totChol: 		total cholesterol level (mg/dL) 
    •	sysBP: 			systolic blood pressure (mmHg)
    •	diaBP: 			diastolic blood pressure (mmHg)
    •	BMI: 			Body Mass Index: Weight (kg) / Height (m2)
    •	heartrate: 		heart rate (ventricul
    ar beats/min)
    •	glucose: 		glucose level (mg/dL)
Predicting: TenYearCHD:  0 = No, 1 = Yes (Binary classification problem)

After doing exploratory analysis of the data, the following attributes were dropped mostly due to these factors having low correlation with the output variable. (Heat map and distributions below)
    •	currentSmoker (low correlation with output variable)
    •	education (low correlation with output variable)
    •	heartrate (low correlation with output variable)
    •	prevalentStroke ( 4215 cases = 0, 25 patients = 1)
    •	diabetes (4131 = 0, 109 = 1)
    •	BPMeds (4063 cases = 0, 124 = 1, 53 = missing values)
