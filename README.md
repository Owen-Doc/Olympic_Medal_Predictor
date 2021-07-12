# Olympic_Medal_Predictor

## INTRODUCTION


Full of blood, passion and extraordinary feats of athletic endeavour, the Olympic Games were the sporting, social and cultural highlight of the Ancient Greek calendar for almost 12 centuries. The modern Olympic Games or Olympics are leading international sporting events featuring summer and winter sports competitions in which thousands of athletes from around the world participate in a variety of competitions. The Olympic Games are considered the world's foremost sports competition with more than 200 nations participating. The Olympic Games are normally held every four years, alternating between the Summer and Winter Olympics every two years in the four-year period.


![image](https://user-images.githubusercontent.com/78067427/125239768-2609c880-e2b7-11eb-95e8-08cd3dfa7ced.png)


However, during the early 20th century, many Olympic athletes discovered ways to improve their athletic abilities by boosting testosterone. As their methods became more extreme, it became increasingly evident that the use of performance-enhancing drugs was not only a threat to the integrity of sport but could also have potentially fatal side effects on the athlete.


![image](https://user-images.githubusercontent.com/78067427/125240046-8dc01380-e2b7-11eb-9a4a-d78bf209be8c.png)


## GOAL

The essence for this final project is to improvise on data wrangling, ETL, relational databases and statistical visualization to:
  - Create a supervised machine learning model to predict the 2021 Olympic medal counts for competing countries. 
  - Examine supplementary doping/disqualification data to quantify its correlation to the performance of the data metrics and athlete categorical metadata.

## Communication Protocols

  - Slack (group chats)
  - Text messaging
  - GoogleDrive (presentation sharing)
  - GitHub (code sharing)
  - Zoom (web meetings)

## ETL Process

#### Main dataset 

https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results athlete_events.csv.zip using data here to update the dataset for the 2022 olympics https://github.com/rgriff23/Olympic_history

Ineligible athletes list from https://www.athleticsintegrity.org/disciplinary-process/global-list-of-ineligible-persons tool to convert PDF to excel https://simplypdf.com/Excel toMay-2021-Sanctions-List-Full.xlsx

#### Data collection and preprocessing

Python/Jupyter Notebook/BeautifulSoup for scraping, Pandas for ETL

#### Data Storage

PostgreSQL server

#### Analytic tools

Sci-kit learn for ML model - RandomForestClassifier
R for statistical analysis and correlation visualizations when building ML model

#### Columns created
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

#### Target Features 
Medal (None, Gold, Silver, Bronze)

## Machine Learning

The data was split into testing and training sets and scaled. The Random Forest Classifer model was created, fitted and used to predict for an accurate score

![image](https://user-images.githubusercontent.com/78067427/125244463-5f453700-e2bd-11eb-9114-40392ae6b6c7.png)

The model was repeated, this time to show the importance of features in the random forest model

![image](https://user-images.githubusercontent.com/78067427/125245032-0de97780-e2be-11eb-973e-80ecfe9ff56b.png)

## Conclusion

The optimization goal for 75% or above was meet. The analysis reveals an accuracy of 0.93 weighted average for the first run of the Random Forest classifier model and 0.90 weighted average for the 2nd run this time showing the importance of using the relevant features to predict a favorable accuracy level.


