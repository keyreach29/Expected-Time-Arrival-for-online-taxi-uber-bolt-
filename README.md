## Expected-Time-Arrival-for-online-taxi-uber-bolt-
Predict the estimated time of arrival at the dropoff point for a single Taxi journey
# Introduction
Ride-hailing apps like Uber and Bolt rely on real-time data and machine learning algorithms to automate their services. Accurately predicting the estimated time of arrival (ETA) for Uber trips will make Uber's services more reliable and attractive; this will have a direct and indirect impact on both customers and business partners. The solution would help the company save money and allocate more resources to other parts of the business.

The objective of this project is to predict the estimated time of arrival at the dropoff point for a single Uber journey.

Dataset
The dataset used for this case study is provided here.

The data contains details for 119,549 trips (train and test are split by date). Each row contains a start location and end location (reported as latitude and longitude to within approximately 100m) and the travel distance along the fastest route. Each trip also has a timestamp, which can be used to pull the weather for that day from Weather.csv file. The weather data includes temperature, rainfall and wind speed for the time period during which the trip data was collected.

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

Repository Structure
The repository is organized as follows:

data/: Contains the dataset files.
notebooks/: Contains Jupyter notebooks showcasing the step-by-step implementation of the case study, including EDA, feature engineering, model development, and evaluation.
dev/: Contains any source code or scripts used in the case study, such as data preprocessing or custom functions.
Feel free to explore the notebooks and source code to gain a deeper understanding.

Run FastAPI
To run the fastAPI, paste this code to your terminal:

uvicorn main:app — reload
When you run the script and start the web server using Uvicorn, your FastAPI application becomes accessible at

http://127.0.0.1:8000
To access the documentation of your API, you can simply add “/docs” to the URL:

http://127.0.0.1:8000/docs
Screenshots
ezgif com-optimize (1) ezgif com-crop

Resources
Here are some ressources you would read to have a good understanding of FastAPI :

Tutorial - User Guide
Video - Building a Machine Learning API in 15 Minutes
FastAPI for Machine Learning: Live coding an ML web application
Video - Deploy ML models with FastAPI, Docker, and Heroku
FastAPI Tutorial Series
Http status codes
👏 Support
If you found this article helpful, please give it a clap or a star on GitHub!

Author
Mike Kibet Kerich
Medium channel
 https://medium.com/@mkibekerich14
