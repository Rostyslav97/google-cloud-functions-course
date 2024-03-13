# Google Cloud Functions Course
## Starting a project
To start a new project in Google Cloudm we can go to the [Firebase Console](http://console.firebase.google.com) or create it from [Google Cloud Platform Console](http://console.cloud.google.com)
## Creating a virtual environment
First we have to install `python3-venv` with the following command:
```
sudo apt instll python3 -venv
```
Then we execute the following command:
```
python3 -m venv venv
```
To activate the virtual environment we do:
```
source venv/bin/activate
```
In order to add new packages to our new virtual environment we create a file called `requirements.txt` and execute the following command:
```
pip install -r requirements.txt
```

## Deploying function
First, we have to set our project ID with the follosing command:
```
gcloud config set project [YOUR PROJECT ID]
```
Then we deploy our function with this command:
```
gcloud functions deploy [FUNCTION NAME] --runtime python37 --trigger-http
```