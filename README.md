# Final_Project

### Analyzing motor vehicle accident data in Austin.
- Using a variety of tools, we will look at how different factors may contribute to the severity of a car crash.

## Reason for Selecting Topic
- We want to build a model that will predict the severity of crash depending on different factors. 
- This information can be used by car insurance companies and by consumers who are trying to shop for cars keeping safety in mind.

## Description of the Source Data
TxDot Crash Query System -- This database uses a multitude of factors to input details on a car accident including but not limited to:
- Weather, longitutde, latitutde, severity, time and date of accident over the course of many years. 
- For the sake of our analysis, we will only use data from 2018-2020.
Additionally, we used NHTSA WebAPIs - https://one.nhtsa.gov/webapi/Default.aspx?SafetyRatings/API/5
- This webAPI gives access to the New Car Assessment Program - 5 Star Safety Rating of the US Department Of Transportation, to retrieve overall safety ratings of the cars involved in the crashes.

## Questions we hope to answer with the data
- How do different cars perform in terms of frequency and severity of car accidents?
- How do different weather types affect the frequency of car accidents?
- How demographics affect frequency of car accidents?
- Where do most accidents occur in Austin?

## Communication Protocols
- In order to keep updated on the status of each of our parts of the project, we message each other regularly through Slack. Any other questions or concerns that arise outside of our daily check-ins, we tackle during (or after) class, our group Zoom meetings, or even during weekly TA sessions.

## Tools
- Creating Database
    - PostgreSQL
    - Amazon Web Services (AWS)
- Connecting to Database
    - Psycopg2
- Analyzing Data
    - Pandas
- Machine Learning
    - Imbalanced-learn
    - Tensorflow
- Dashboard
    - Javascript
    - Flask
    - CSS
