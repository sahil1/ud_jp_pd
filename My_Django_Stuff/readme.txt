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

------------------------------------------
Django create models:
  python manage.py migrate
  python manage.py makemigrations first_app
  python manage.py migrate

Verify DB:
  python manage.py shell
>>> print('hello')
hello
>>> print(Topic.objects.all())
<QuerySet []>
>>> T = Topic(top_name="Social Network")
>>> T.save()
>>> print(Topic.objects.all())
<QuerySet [<Topic: Social Network>]>
>>> quit()

Create SuperUser:
  python manage.py createsuperuser (sahil, gmail, testpassword)
