# Olympic_Medal_Predictor

The goal for this final project is to utilize our skills in data wrathing, ETL, relational databases and statistical visualization to eventually build out a machine learning model (supervised) that will predict the 2021 Olympic model counts for competing countries. Using historical Olympic data dating back to as early as 1900, in addition to supplemental doping/disqualification data, we will analyze performance data metrics and athlete categorical metadata. 

Questions to consider that can conflate the data:
- Merging doping data with previous performance data--as atheletes are found guilty, they are removed from medal data (what type of merge is most appropriate? Are there ways to concatenate data or build off of both resources to maintain integrity of true historical performance?
- Are we isolating Summer vs Winter Olympics?
- Disproprotional, imbalanced nature of the competitng athletes and respective countries (with respect to population, total athletes competing, having model weigh those values more than performance metrics)
- Home field advantage question? - Correlation between medal counts per country and host country of specific Olympic games?
- Team vs individual sport?
- Subjective nature of judging certain sports? Rules changing over time? 


## Data Features and Resources:

Main dataset: https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results  [athlete_events.csv.zip](https://github.com/Owen-Doc/Olympic_Medal_Predictor/tree/main/Resources/athlete_events.csv.zip) 
using data here to update the dataset for the 2022 olympics https://github.com/rgriff23/Olympic_history

Ineligible athletes list from https://www.athleticsintegrity.org/disciplinary-process/global-list-of-ineligible-persons
tool to convert PDF to excel https://simplypdf.com/Excel to[May-2021-Sanctions-List-Full.xlsx](https://github.com/Owen-Doc/Olympic_Medal_Predictor/tree/main/Resources/May-2021-Sanctions-List-Full.xlsx) 

- Tools

1. Python/Jupyter Notebook for data scraping, ETL process- with BeautifulSoup for scraping from sites
2. Tableau for Heat maps weigh medal winners/counts vs home field advantage?
3. R for statistical analysis and correlation visualizations prior to machine learning model?
4. HTML/javascript for presentation of findings (viewer friendly stats and user friendly inputs with output predictions?)
5. Flask App for web instance
6. Google Maps API for visualization of geographical correlates in relation to medal placement/ density of competing athletes per contry?

   
