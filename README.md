# Bike Sharing Assignment
> #### Problem Statement:
A US bike-sharing provider aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 
They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
<!--* [Acknowledgements](#acknowledgements)-->

<!-- You can include any other section that is pertinent to your problem -->

## General Information
**The company wants to know:**
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

**Our objecties:**
- Create a linear model that describes the effect of various factors on the demand for these shared bikes
- The model should be interpretable so that the management understands it
- Dataset being used for this case study


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

**Final Observations from our model:**
- We got r2 score of 0.835 on training data and 0.802 on test data with 10 predictor variables
- Below are the predictor variables used in our final model after RFE and manual feature elimination based on p-values & VIF values
    - `yr`, `workingday`, `temp`, `hum`, `windspeed`, `season_summer`, `season_winter`, `mnth_Sep`, `weathersit_LightSnowRain`, `weathersit_Mist`
- Equation of best fitted line based on the final summary we have

$ cnt = 0.2286 \times   yr   + 0.0232 \times workingday + 0.5730 \times temp + (-0.1743 \times hum) + (-0.1859 * windspeed) + 0.09 \times seasonsummer + 0.140 \times seasonwinter + 0.103 \times mnthSep + (-0.2349 \times weathersitLightSnowRain) + (-0.051 \times weathersitMist)$
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Pandas
- Matplotlib
- Seaborn
- sklearn
- statsmodels

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

<!--
## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).
-->

## Contact
Created by [@naga-shanmukha]
