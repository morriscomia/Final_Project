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
-  Any other questions or concerns that arise outside of my daily check-ins, I tackle during (or after) class, our group Zoom meetings, or even during weekly TA sessions.

## Tools
- Creating Database
    - PostgreSQL
    - Amazon Web Services (AWS)

- Analyzing Data
    - Pandas
- Machine Learning
    - Imbalanced-learn
    - Tensorflow
- Dashboard
    - Javascript
    - Flask
    - CSS

## Provisional Database

## Machine Learning Model
- The preliminary data includes columns that describe the environment for each crash that took place in Austin, TX. These features include the weather condition, crash severity, day of the week, vehicle make and model, etc.
- An ERD showcasing the inter-relationships between each of the features from the different datasets can be found [here](https://app.quickdatabasediagrams.com/#/d/C8XBSf
). 
- After connecting to the database, I printed out the header for each column to see all of the features available. From that list, I chose the features that I believed would have the highest correlation with crash severity.
- The data was split into training and test data using the train_test_split function. We used the default 75% to 25% split.
- After careful analyzing, it was determined that the linear models only yielded about 50% correlation. Altering the parameters, such as increasing max iterations and n_jobs,  to these did not increase the accuracy. Neural network model was then used to see if it would have a higher accuracy rate. After adding 8 layers (using Relu, Swish and Sigmoid), the accuracy rate was still at 54%, with 69% loss. This means our model could only accurately predict the outcome of the severity of a crash about 50% of the time. 
- I decided to use the decision tree model for our machine learning model. I grouped our crash severity data into two categories, 0 - no injury, and 1 - injury. The benefit of this model is that it can be used to predict our binary outcome. The downside of this model is that if we choose to group our crash severity data differently (the data is grouped into 5 classifications: no injury, possible injury, non-incapacitating injury, severe injury, and fatal injury), we will not be able to use the decision tree model.

## Presentation
- My presentation can be found here [Google Slide Presentation](https://docs.google.com/presentation/d/1L4druVSpZPPmJu9Y5_xuQHMjc9uxpaxPkGMytEVdTJE/edit?usp=sharing)
