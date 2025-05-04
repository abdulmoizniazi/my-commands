``` bash
python -m venv .venv
which python
source .venv/scripts/activate
pip install django
python -m django --version
mkdir newfolder
django-admin startproject myprojectname newfolder
py manage.py startapp myapplicationname
py manage.py makemigrations myapplicationname
py manage.py sqlmigrate myapplicationname 0001 #sql query executed
py manage.py migrate
py manage.py shell #testing and checking 
py manage.py createsuperuser
py manage.py runserver

```
