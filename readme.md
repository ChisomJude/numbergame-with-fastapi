# numbergame with FastAPI
A simple FastAPI for number classification  with a backend API hosted on Lamda and a simple frontend on S3

This project collects input from user and return output on the number classification with funfacts integration from http://numbersapi.com/.

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