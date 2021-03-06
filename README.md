# Olympic_Medal_Predictor

## INTRODUCTION


<img width="812" alt="Olympic_symbol" src="https://user-images.githubusercontent.com/78067427/126909102-1fc7cf99-dae8-40bc-b1f2-d22367a20c4d.png">

Full of blood, passion and extraordinary feats of athletic endeavour, the Olympic Games were the sporting, social and cultural highlight of the Ancient Greek calendar for almost 12 centuries. The modern Olympic Games or Olympics are leading international sporting events featuring summer and winter sports competitions in which thousands of athletes from around the world participate in a variety of competitions. The Olympic Games are considered the world's foremost sports competition with more than 200 nations participating. The Olympic Games are normally held every four years, alternating between the Summer and Winter Olympics every two years in the four-year period.

This project will be focused on the relationship between participants, medal achievers and predictions for medals counts during a certain period of the event. The purpose is to determine if countries with certain features can influence achieving higher number of medals at incoming games.

The dataset comprises of athletes who have participated at the Olympics from 1896 – 2016, along ineligible athletes for doping. Relevant years from 1960 -2016 will be used to run the project

<img width="758" alt="Participation" src="https://user-images.githubusercontent.com/78067427/126909974-f00f710b-0043-441e-b9f5-6105ff003350.PNG">

## GOAL

The essence for this final project is to improvise on data wrangling, ETL, relational databases and statistical visualization to:
  - Create a supervised machine learning model to predict the 2021 Olympic medal counts for competing countries. 
  - Manipulate data to quantify its correlation to the performance of the data metrics and athlete categorical metadata.
  - Answer preliminary questions like:
    - Are we isolating Summer vs Winter Olympics?
    - Home field advantage question?
    - Correlation between medal counts per country and host country of specific Olympic games?
    - Team vs individual sport?
    - Subjective nature of judging certain sports?
    - Rules changing over time?

## Communication Protocols

  - Slack (group chats)
  - Text messaging
  - GoogleDrive (presentation sharing)
  - GitHub (code sharing)
  - Zoom (web meetings)

## ETL Process

#### Main dataset 
Primary CSV: https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results athlete_events.csv.zip 

Complete webpage that data can be scraped from
https://www.olympedia.org/athletes

Using data here to update the dataset for the 2022 olympics https://github.com/rgriff23/Olympic_history

Ineligible athletes list from https://www.athleticsintegrity.org/disciplinary-process/global-list-of-ineligible-persons 

Tool to convert PDF to excel 
https://simplypdf.com/Excel toMay-2021-Sanctions-List-Full.xlsx

#### Data collection and preprocessing

Python/Jupyter Notebook/BeautifulSoup for scraping, Pandas for ETL

#### Data Storage

PostgreSQL server

#### Analytic tools

Sci-kit learn for ML model - RandomForestClassifier
Correlation visualizations when building ML model

<img width="752" alt="Tools" src="https://user-images.githubusercontent.com/78067427/126913788-2461dfe2-13fb-4b7e-ae60-0fe7ede5f662.PNG">

#### Relevant Columns analyzed
  - Year
  - Season
  - Games
  - Host Country
  - NOC
  - Region
  - Athlete
  - Gender
  - Age
  - Height
  - Weight
  - Sport
  - Event
  - Medal
  - Medal Type
  - Population
  - GDP

#### Target Features 
Medal and No medal

<img width="752" alt="visualizing feature selection" src="https://user-images.githubusercontent.com/78067427/126914023-c87dda44-be54-4533-9ea8-92cdf65a4748.PNG">

<img width="784" alt="Body types" src="https://user-images.githubusercontent.com/78067427/126915041-00ca249d-325b-4cee-88eb-00dcd5926187.PNG">


## Machine Learning

The data was split into testing and training sets and scaled. The Random Forest Classifer model was created, fitted and used to predict for an accurate score. The model was repeated, this time to show the importance of features in the random forest model

<img width="775" alt="ML result" src="https://user-images.githubusercontent.com/78067427/126913817-c256c231-1dc8-43bc-acb8-bc237f15c795.PNG">

The first run of the model shows an accuracy of 0.77 weighted average, population and GDP being the major factors for countries winning medals. The second run of the Random Forest classifier model with added features of Sporting category and Events gave a 0.84 weighted average predicting to a favorable accuracy level.

## Conclusion

The optimization goal for 75% or above was meet. The model shows certain features indeed are influencial for countries to gain more medal counts. These major features are the country itself, its population, GDP, the sport category(s) and the event participated upon (winter or summer olympics). Below is an example of China's GDP growth in correlation to more medal achievements

<img width="681" alt="GDP" src="https://user-images.githubusercontent.com/78067427/126914624-6b4ba5a2-74e4-4370-948e-8b7300b5be9e.PNG">

#### The following are links for the required deliverables: 

[Machine learning codes](https://github.com/Owen-Doc/Olympic_Medal_Predictor/tree/Carly)

[Database connection strings and codes](https://github.com/Owen-Doc/Olympic_Medal_Predictor/tree/OwensBranch)

[Google Slides](https://docs.google.com/presentation/d/13BkwpaAfonPbkYUwHNgPaWav6qAYV6PfYI1Y0RyVfMI/edit#slide=id.gc6f73a04f_0_0)


