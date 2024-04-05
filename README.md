# Machine-Learning-Project-with-mlflow

## Workflow
1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity 
5. Update the configuration manager in the src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Upadata the app.py

# How to run the project

### Steps:

Clone the repository
~~~bash
https://github.com/Subash7Lingden/Machine-Learning-Project-with-mlflow
~~~

### Step 01 - Create a conda environement after opening the repository
~~~bash
conda create -n mlproj python=3.8 -y
~~~

~~~bash
conda activate mlproj
~~~

### step 02 - Install the requiements
~~~bash
pip install -r requirements.txt
~~~

~~~bash
# Finally run tht following command
python app.py
~~~
Now,
~~~ bash
open up your local host and port
~~~

## MLflow
[Documentation](https://mlflow.org/docs/latest/index.html)

### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/Subash7Lingden/Machine-Learning-Project-with-mlflow.mlflow \
MLFLOW_TRACKING_USERNAME=Subash7Lingden \
MLFLOW_TRACKING_PASSWORD=e47cb2181458071797d31f2e25e11e1defd6bd99 \
python script.py

Run this to export as env variables:

~~~bash
set MLFLOW_TRACKING_URI = https://dagshub.com/Subash7Lingden/Machine-Learning-Project-with-mlflow.mlflow

set MLFLOW_TRACKING_USERNAME = Subash7Lingden

set MLFLOW_TRACKING_PASSWORD = e47cb2181458071797d31f2e25e11e1defd6bd99

~~~
