# Numbergame with FastAPI
A simple FastAPI for number classification  with a backend API hosted on AWS Lambda, serving request via Api-Gateway and a simple frontend on S3

This project collects user input and returns output on the number classification with funfacts integration from http://numbersapi.com/.

## API Endpoints
/test
/api/funfact
/api/classify-number


## How to Run this Locally
- [x] Clone this repo - `git clone `
- [x] cd to the repo  `cd  number-classification-with-python`
- [x] Ensure Python is installed `python --version`
- [x] Create a virtual env  `python -m venv venv`
- [x] Activate VENV  `.\venv\Scripts\activate`
- [x] Install requirements.txt `pip install -r requirements.txt`
- [x] Run the App `uvicorn backend.main:app --reload`



## API Endpoints

#### GET /static
This gets the input and forwards it  to the backend using `/api/classify-number?number=${number}` 
Frontend is built with HTML, CSS, and JavaScript

![alt text](https://github.com/ChisomJude/number-classification-with-python/blob/master/image.png)

####  GET /api/classify-number 
The backend API can be accessed directly using the same request

```
http://localhost:8000/api/classify-number?number=56

```
Output:

![image-1.png](https://github.com/ChisomJude/number-classification-with-python/blob/master/image-1.png)


## How to Run this Locally
- [x] Clone this repo - `git clone `
- [x] cd to the repo  `cd  number-classification-with-python`
- [x] Ensure Python is installed `python --version`
- [x] Create a virtual env  `python -m venv venv`
- [x] Activate VENV  `.\venv\Scripts\activate`
- [x] Install requirements.txt `pip install -r requirements.txt`
- [x] Run the App `uvicorn backend.main:app --reload`


## Deploying to AWS Lamda and APIGateWay

- [x] Package your deployment file for AWS using the command

```powershell
mkdir awslamdapackage
pip install -r requirements.txt -t awslamdapackage
cp -r backend awslamdapackage
cp -r frontend awslamdapackage
cd  awslamdapackage
Compress-Archive -Path .\* -DestinationPath ..\awslamdapackage -Force

```


![alt text](https://github.com/ChisomJude/number-classification-with-python/blob/master/image-2.png)

Connect to API Gateway
Choose HTTP API
Add Name 
