# Bike-Sharing Demand Prediction Analysis  
## Table of Contents  
•⁠  ⁠[General Information](#general-information)  
•⁠  ⁠[Technologies Used](#technologies-used)  
•⁠  ⁠[Conclusions](#conclusions)  
•⁠  ⁠[Acknowledgements](#acknowledgements)  
•⁠  ⁠[Contact](#contact)  

---

## General Information  
*Objective*  
Build a multiple linear regression model to predict bike-sharing demand for BoomBikes, a US-based provider, and identify key factors influencing rentals post-COVID-19 lockdowns.  

*Business Context*  
BoomBikes aims to optimize its operations by understanding:  
1.⁠ ⁠Variables significantly impacting daily bike rentals.  
2.⁠ ⁠Quantitative influence of these variables on demand.  

*Dataset*  
•⁠  ⁠*Target Variable*: ⁠ cnt ⁠ (total rentals = ⁠ casual ⁠ + ⁠ registered ⁠).  
•⁠  ⁠*Features*: Weather (⁠ temp ⁠, ⁠ hum ⁠, ⁠ windspeed ⁠, ⁠ weathersit ⁠), temporal factors (⁠ yr ⁠, ⁠ mnth ⁠, ⁠ holiday ⁠, ⁠ weekday ⁠), and seasonal trends.  
•⁠  ⁠*Data Transformation*: Categorical variables like ⁠ season ⁠ and ⁠ weathersit ⁠ were converted from numeric to string labels to avoid ordinal misinterpretation.  

---

## Technologies Used  
•⁠  ⁠*Python* (Core programming language)  
•⁠  ⁠*Pandas* - Data manipulation and cleaning  
•⁠  ⁠*NumPy* - Numerical operations  
•⁠  ⁠*Scikit-learn* - Model building and evaluation  
•⁠  ⁠*Statsmodels* - Statistical analysis and VIF calculation  
•⁠  ⁠*Matplotlib* & *Seaborn* - Visualization  
•⁠  ⁠*Jupyter Notebook* - Interactive analysis  

---

## Conclusions  
*Significant Variables*:  
1.⁠ ⁠*Temporal Trends*:  
   - Year 2019 saw *~40% higher demand* than 2018.  
   - Peak demand in *summer months* (June–September); lowest in *winter* (January, December).  

2.⁠ ⁠*Weather Impact*:  
   - *Temperature* (⁠ temp ⁠) has the strongest positive correlation (coefficient: *0.55*).  
   - *Humidity* (⁠ hum ⁠) and *windspeed* reduce demand.  
   - *Light snow/rain* (⁠ weathersit=3 ⁠) decreases rentals by *~25%* vs. clear days.  

*Model Performance*:  
•⁠  ⁠*R² of 0.81* on test data, indicating strong explanatory power.  
•⁠  ⁠Key predictors: ⁠ yr ⁠, ⁠ temp ⁠, ⁠ hum ⁠, ⁠ weathersit ⁠, and specific months.  

*Strategic Recommendations*:  
1.⁠ ⁠Increase bike availability during *summer months* and *favorable weather days*.  
2.⁠ ⁠Launch promotions during *winter* and *holidays* to offset demand dips.  

Demand of bikes depend on 
    - year
    - Dec, Sep, March Months
    - temp
    - windspeed 
    - Light_snowrain
    - Misty
    - spring and winter.

---

## Acknowledgements  
•⁠  ⁠Dataset provided by *BoomBikes*.  

---

## Contact  
Created by [@sankalps08](https://github.com/sankalps08) - Reach out for collaborations or queries!
