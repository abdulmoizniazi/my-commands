pip install dotenv
pip install djangorestframework
pip install djangorestframework-simplejwt
pip install django-cors-headers
pip install python-dotenv



//settings.py
from datetime import timedelta
from dotenv import load_dotenv
import os

load_dotenv()


ALLOWED_HOSTS = ["*"]

REST_FRAMEWORK = {
    "DEFAULT_AUTHENTICATION_CLASSES": (
        "rest_framework_simplejwt.authentication.JWTAuthentication",
    ),
    "DEFAULT_PERMISSION_CLASSES": [
        "rest_framework.permissions.IsAuthenticated",
    ],
}

SIMPLE_JWT = {
    "ACCESS_TOKEN_LIFETIME": timedelta(minutes=30),
    "REFRESH_TOKEN_LIFETIME": timedelta(days=1),
}


INSTALLED_APPS = [
    ...
    'rest_framework',
    'corsheaders',
]


MIDDLEWARE = [
    ...
    'corsheaders.middleware.CorsMiddleware',
]


CORS_ALLOW_ALL_ORIGINS = True
CORS_ALLOW_CREDENTIALS = True
/////////////////////////////////////////////////////


serializers.py
models.py
views.py
/////////////////////////////////////////////////////

npm create vite@latest frontend -- --template react
npm install axios react-router-dom jwt-decode

----------->>>> pages/ styles/ components/  .env
----------->>>> src/constants.js  src/api.js