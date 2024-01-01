# Django ORM Web Application.
DEVELOPED.BY:V.THAANESH
REG.NO:212223230228

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Create a django project with the name “myfoodblog"
### STEP 2: 
Initiate a database & create data tables for existing models of the generated project in the database

### STEP 3:
Open a new windows cli and move to the project workspace. Run the following command to start up a local host

### STEP 4: 
Creating a superuser and refresh http://127.0.0.1:8000/admin/ in your browser & sign in

### STEP 5:
Create an application in the myfoodblog project with the name “cuisine"
### STEP 6:
Define a cuisine model to handle posts by the owner / users of the blog , edit settings.py:
### STEP 7: 
Add your cuisine model to the administration site. Customizing the way models (eg. Cuisine)
are displayed in the admin app and customize the admin model some more.

## PROGRAM

### SETTINGS.PY
``````
Django settings for MyFoodBlog project.
Generated by ‘django-admin startproject’ using Django 4.2.6.
For more information on this file, see
https://docs.djangoproject.com/en/4.2/topics/settings/
For the full list of settings and their values, see
https://docs.djangoproject.com/en/4.2/ref/settings/
“””
import os
from pathlib import Path
# Build paths inside the project like this: BASE_DIR / ‘subdir’.
BASE_DIR = Path(__file__).resolve().parent.parent
# Quick-start development settings – unsuitable for production
# See https://docs.djangoproject.com/en/4.2/howto/deployment/checklist/
# SECURITY WARNING: keep the secret key used in production secret!
SECRET_KEY = ‘django-insecure-
@)&cuctn6pqlkpd&a$i7j#3_qy53#@o8%pte)^_nz!uq21&s0z’
# SECURITY WARNING: don’t run with debug turned on in production!
DEBUG = True
ALLOWED_HOSTS = []
# Application definition
INSTALLED_APPS = [
‘django.contrib.admin’,
‘django.contrib.auth’,
‘django.contrib.contenttypes’,
‘django.contrib.sessions’,
‘django.contrib.messages’,
‘django.contrib.staticfiles’,
‘cuisine’
]
MIDDLEWARE = [
‘django.middleware.security.SecurityMiddleware’,
‘django.contrib.sessions.middleware.SessionMiddleware’,
‘django.middleware.common.CommonMiddleware’,
‘django.middleware.csrf.CsrfViewMiddleware’,
‘django.contrib.auth.middleware.AuthenticationMiddleware’,
‘django.contrib.messages.middleware.MessageMiddleware’,
‘django.middleware.clickjacking.XframeOptionsMiddleware’,
]
ROOT_URLCONF = ‘MyFoodBlog.urls’
TEMPLATES = [
{
‘BACKEND’: ‘django.template.backends.django.DjangoTemplates’,
‘DIRS’: [],
‘APP_DIRS’: True,
‘OPTIONS’: {
‘context_processors’: [
‘django.template.context_processors.debug’,
‘django.template.context_processors.request’,
‘django.contrib.auth.context_processors.auth’,
‘django.contrib.messages.context_processors.messages’,
],
},
},
]
WSGI_APPLICATION = ‘MyFoodBlog.wsgi.application’
# Database
# https://docs.djangoproject.com/en/4.2/ref/settings/#databases
DATABASES = {
‘default’: {
‘ENGINE’: ‘django.db.backends.sqlite3’,
‘NAME’: BASE_DIR / ‘db.sqlite3’,
}
}
# Password validation
# https://docs.djangoproject.com/en/4.2/ref/settings/#auth-password-validators
AUTH_PASSWORD_VALIDATORS = [
{
‘NAME’: ‘django.contrib.auth.password_validation.UserAttributeSimilarityValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.MinimumLengthValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.CommonPasswordValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.NumericPasswordValidator’,
},
]
# Internationalization
# https://docs.djangoproject.com/en/4.2/topics/i18n/
LANGUAGE_CODE = ‘en-us’
TIME_ZONE = ‘UTC’
USE_I18N = True
USE_TZ = True
# Static files (CSS, JavaScript, Images)
# https://docs.djangoproject.com/en/4.2/howto/static-files/
STATIC_URL = ‘static/’
MEDIA_URL = ‘/pics/’
MEDIA_ROOT= os.path.join(BASE_DIR, ‘cuisine/pics’)
# Default primary key field type
# https://docs.djangoproject.com/en/4.2/ref/settings/#default-auto-field
DEFAULT_AUTO_FIELD = ‘django.db.models.BigAutoField’
``````

### MODEL.PY
``````
},
]
WSGI_APPLICATION = ‘MyFoodBlog.wsgi.application’
# Database
# https://docs.djangoproject.com/en/4.2/ref/settings/#databases
DATABASES = {
‘default’: {
‘ENGINE’: ‘django.db.backends.sqlite3’,
‘NAME’: BASE_DIR / ‘db.sqlite3’,
}
}
# Password validation
# https://docs.djangoproject.com/en/4.2/ref/settings/#auth-password-validators
AUTH_PASSWORD_VALIDATORS = [
{
‘NAME’: ‘django.contrib.auth.password_validation.UserAttributeSimilarityValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.MinimumLengthValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.CommonPasswordValidator’,
},
{
‘NAME’: ‘django.contrib.auth.password_validation.NumericPasswordValidator’,
},
]
# Internationalization
# https://docs.djangoproject.com/en/4.2/topics/i18n/
LANGUAGE_CODE = ‘en-us’
TIME_ZONE = ‘UTC’
USE_I18N = True
USE_TZ = True
# Static files (CSS, JavaScript, Images)
# https://docs.djangoproject.com/en/4.2/howto/static-files/
STATIC_URL = ‘static/’
MEDIA_URL = ‘/pics/’
MEDIA_ROOT= os.path.join(BASE_DIR, ‘cuisine/pics’)
# Default primary key field type
# https://docs.djangoproject.com/en/4.2/ref/settings/#default-auto-field
DEFAULT_AUTO_FIELD = ‘django.db.models.BigAutoField’
``````
## OUTPUT
![Screenshot 2024-01-01 131323](https://github.com/vthaanesh22/django-orm-app/assets/139373686/76daeb67-3a28-4ab3-926f-baef0ca70331)
![Screenshot 2024-01-01 131426](https://github.com/vthaanesh22/django-orm-app/assets/139373686/2c7ce2a1-611a-4499-890f-ce04a9badedc)

## RESULT
Thus the program for creating database using ORM has been created successfully
