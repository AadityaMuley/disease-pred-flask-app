# Symptoms Based Disease Prediction  - Flask App
Random Forest Classifier to predict disease based on different symptoms deployed on a Flask web-app.

## Steps to run this app (**WARNING: Don't directly clone the repo**):
- Create a separate folder for your project wherever you want and ensure you are in that working directory on your terminal (my folder name is ***disease_det_flask*** so change it according to your folder name):
    ```
    mkdir disease_det_flask
    cd disease_det_flask
    ```
- We need to create a virtual enviromnet in this folder to run our app. So install venv first if you haven't already. If you have skip the first command:
    ```
    sudo apt install python3-venv
    python3 -m venv venv
    ```
- Now that our virtual env is setup we will activate it and install our flask app dependancies in this venv:
    ```
    source venv/bin/activate
    pip install Flask
    python -m flask --version
    pip install sklearn
    ```
- Now clone this repo into you folder (disease_det_flask for me - do not clone inside venv folder)
- The ml_proj_disease_detection.ipynb has many different models tested out on the data. ***Random Forest Classifier*** gave me the best accuracy results so I created its pickle dump file. You need not run this again since I have already included the model.pkl file in the repo.
- Execute these commands to run the Flask App:
    ```
    export FLASK_APP=app.py
    flask run
    ```
  This will display an URL on the terminal. Open that url and the web app will open up!
  
  ## Preview:
  ### Input:
  ![alt text](https://github.com/AadityaMuley/disease-pred-flask-app/blob/main/screenshots/ss-1.png?raw=true) 
  ### Output:
  ![alt text](https://github.com/AadityaMuley/disease-pred-flask-app/blob/main/screenshots/ss-2.png?raw=true)
