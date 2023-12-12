# Bike Sharing System 
> BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. Model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic.
- They want to understand the factors affecting the demand for these shared bikes in the American market.
- The company wants to know: 1) Which variables are significant in predicting the demand for shared bikes. 2)How well those variables describe the bike demands
- The demand model has developed throught multilinear regression methods.
- day.csv dataset used to find the factors affecting the demand. This dataset contains bike registration count, humudity, temperature, windspeed, date, season, weather condition, weekday, working day and holidays.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Impact of categorical features. 
    -Bike demand in 2019 is higher than 2018.
    -Bike demand is high on fall season
    -Bike demand high between the month from April to October
    -Almost constant demand on weekdays
    -Demand is slightly high on working day
    -Demand is high on Clear, Few clouds, Partly cloudy, Partly cloudy weather condition

- Below are the features impacting the demand model, considering with 10 features including constant.
    temp, light snow&rain(weathersit:3), year, windspeed, winter,september,summer, mist&cloudy(weathersit:2) and August
    Best fit line:  cnt=0.5211*temp-0.2786*weathersit:3+0.2328*yr-0.1516*windspeed+0.1374*winter+0.1133*september+0.1016*summer-0.0809*weathersit:2+0.0557*August+0.1264
- r2_score(y_test, y_pred) = 0.782


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy                         1.24.3
- pandas                        1.5.3
- seaborn                       0.12.2
- matplotlib                    3.7.1
- scikit-learn                  1.2.2
- statsmodels                   0.13.5


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project is an assignment for machine learning module as part of upgrad curriculam.
- Refered all online contents of Upgrad and live sessions and tutors.
- This project was based on https://learn.upgrad.com/course/4705/segment/43555/258687/790246/3970578


## Contact
Created by [@sgragupathi] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->