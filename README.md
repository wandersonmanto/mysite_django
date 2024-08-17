# mysite_django

1 - Criando ambiente virtual 
python -m venv env

2 - Ativar o ambiente virtual
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
.\env\Scripts\Activate.ps1

3 - Adicionando nova branch
git checkout -b "projeto-setup"

4 - intall Django
pip install django

5 - iniciando o projeto Django
django-admin startproject mysite

6 - Iniciando um Django Application
python manage.py startapp blog

7 - Add o projeto ao settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'blog'
]

8 - migrations default
python manage.py migrate

9 - executando o servidor de desenvolvimento integrado do Django.
python manage.py runserver

10 - Adicionando nova branch
git checkout -b "SETUP"