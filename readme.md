# Deploy FastAPI dengan menggunakan App Engine
Deploy FastAPI Machine Learning model dengan menggunakan CloudRun


## Kebutuhan
* Pyenv (optional)
* Virtualenv (optional)
* Python 3.9
* Google Cloud Platform Account
* Google Cloud Platform - API Cloud Build


## Jalankan secara lokal
```
$ virtualenv -p python3.8.2 .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
$ uvicorn main:app --reload
```

## Cara deploy ke cloud-run
```
$ gcloud app create
$ gcloud builds submit --tag gcr.io/astute-acolyte-381310/fastapi-model-deployment
$ gcloud app browser
```
