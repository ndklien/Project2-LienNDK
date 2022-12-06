# Disaster Response Pipeline Project

### Overview

- In this course, I learnt some data engineering skills, which could widen my potential to become a data scientist. To improve those skills, I will utilize these skills in this project to analyze Disaster data from Appen and build a model for an API that classifies disaster messages.

- This project includes people interaction where users could submit a new message into the project's web application and then it will categorize the message using a built-in classification model. Moreover, some visualizations will be included.

### Project structure
- app
	- template
    - master.html  # main page of web app
    - go.html  # classification result page of web app
- run.py  # Flask file that runs app

- data
	- disaster_categories.csv  # data to process 
	- disaster_messages.csv  # data to process
	- process_data.py
	- Udacity-LienNDK.db   # database to save clean data to

- models
	- train_classifier.py
    - classifier.pkl  # saved model 
- README.md

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/Udacity-LienNDK.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run your web app: `python run.py`

4. Go to http://0.0.0.0:3000/
