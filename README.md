# Sepsis-Prediction-with-ML-and-FastAPI
Develop a Machine Learning API (Application Programming Interface) using FastAPI.
Introduction
We will explore a comprehensive machine learning project focused on predicting sepsis using classification techniques. By leveraging FastAPI, we were able to deploy the model as a user-friendly API, enabling real-time predictions. The combination of machine learning and web development has immense potential in healthcare and can significantly contribute to early sepsis detection and patient care.

Description
Importance of Project  
The dataset used contains a list of patients in a hospital and their attributes and whether the patient is positive for Sepssis or not.

Sepsis is a severe and potentially life-threatening condition that occurs when the body's response to an infection triggers widespread inflammation. It is often referred to as blood poisoning.

The aim of this project is to explore the various factors that can cause sepsis in order to predict the occurence of sepsis.

Predicting sepsis is important because early recognition and intervention can significantly improve patient outcomes. Sepsis can progress rapidly and become life-threatening within a short period. By identifying patients who are at risk of developing sepsis, healthcare providers can initiate timely treatment and interventions to prevent the condition from worsening.

Dataset Description -
The data for this project is in a csv format. The following describes the columns present in the data.

Column Name	Target	Description
ID	N/A	Unique number to represent patient ID
PRG	False	Plasma glucose
PL	False	Blood Work Result-1 (mu U/ml)
PR	False	Blood Pressure (mm Hg)
SK	False	Blood Work Result-2 (mm)
TS	False	Blood Work Result-3 (mu U/ml)
M11	False	Body mass index (weight in kg/(height in m)^2
BD2	False	Blood Work Result-4 (mu U/ml)
Age	False	patients age (years)
Insurance	N/A	If a patient holds a valid insurance card
Sepssis	True	Positive: if a patient in ICU will develop a sepsis , and Negative: otherwise
Setup
Install the required packages to be able to run the evaluation locally.

You need to have Python 3 on your system (a Python version lower than 3.10). Then you can clone this repo and being at the repo's root :: repository_name> ... follow the steps below:

Windows:
python -m venv venv; venv\Scripts\activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt
Linux & MacOs:
python3 -m venv venv; source venv/bin/activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt
The both long command-lines have a same structure, they pipe multiple commands using the symbol ; but you may manually execute them one after another.

Create the Python's virtual environment that isolates the required libraries of the project to avoid conflicts;
Activate the Python's virtual environment so that the Python kernel & libraries will be those of the isolated environment;
Upgrade Pip, the installed libraries/packages manager to have the up-to-date version that will work correctly;
Install the required libraries/packages listed in the requirements.txt file so that it will be allow to import them into the python's scripts and notebooks without any issue.
NB: For MacOs users, please install Xcode if you have an issue.

Run FastAPI
To run the fastAPI, paste this code to your terminal:

uvicorn main:app — reload
When you run the script and start the web server using Uvicorn, your FastAPI application becomes accessible at

http://127.0.0.1:8000
To access the documentation of your API, you can simply add “/docs” to the URL:

http://127.0.0.1:8000/docs
Screenshots
ezgif com-optimize (1) 


Resources
Here are some ressources you would read to have a good understanding of FastAPI :

Tutorial - User Guide
Video - Building a Machine Learning API in 15 Minutes
FastAPI for Machine Learning: Live coding an ML web application
Video - Deploy ML models with FastAPI, Docker, and Heroku
FastAPI Tutorial Series
Http status codes
👏 Support
If you found this article helpful, please give it applause or a star on GitHub!

Author
Ronald Shiundu
