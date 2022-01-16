# Django-initial-setup

1/ Creation of  local environment

py -m venv venv

2/ Activate virtual environment

venv\Scripts\activate

3/ Upgrade pip and check version

py -m pip install --upgrade pip
py -m pip --version

4/ Installl django framework

pip install django

5/ Creation of first project

django-admin startproject mysite .

NB : adding a "dot", project will be under projectfolder/mysite/ otherwise projectfolder/mysite/mysite/

documentation django :
"mettre du code Python dans le répertoire racine de votre serveur Web, parce que cela crée le risque que l’on puisse voir votre code sur le Web, ce qui n’est pas bon pour la sécurité."

6/ Creation of a new app

py manage.py startapp polls

7/ Others useful commands

py manage.py makemigrations --dry-run --verbosity 3
py manage.py runserver
py manage.py createsuperuser 
pip install coverage
coverage run --omit='*/venv/*' manage.py test
coverage html
pip install djangorestframework
python -m pip freeze > requirements.txt