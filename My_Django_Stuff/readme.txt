Activate and Deactivate Django Env:
  source activate myDjangoEnv
  source deactivate myDjangoEnv

Create Project:
  django-admin startproject first_project

Start/Run Project:
  cd first_project
  python manage.py runserver

Create Application within Django Project:
  python manage.py startapp first_app

File/Dir Path from import os:
  print(__file__)
  print(os.path.dirname(__file__))
