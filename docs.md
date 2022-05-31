# Code used

## Environment setup

Run initial compose with:

```console
sudo docker-compose run web django-admin startproject TicTacToeRemake .
```

(Only on Linux) Change owner for files created with Django:

```console
sudo chown -R $USER:$USER TicTacToeRemake manage.py
```

Compose up to run the app:

```console
sudo docker-compose up
```

Get the SECRET_KEY and paste it in the .env file:

```console
python -c "import secrets; print(secrets.token_urlsafe())"
```

After any changes to the project requirements rebuild the service:

```console
user@host:~$ sudo docker-compose build --no-cache [SERVICE...]
```

## New app in project

```console
sudo docker-compose run web python manage.py startapp [app-name]
```

After adding a new app change owner:

```console
sudo chown -R $USER:$USER [app-name]
```

## Add new view and URL to app and project

Add a new view:

```python
def index(request):
    return something
```

*Note* View always needs to return something!

Add the path to app [app]/urls.py:

```python
from . import views

urlpatterns = [
    path('[path]', views.[view-name], name='[view-name]'),
]
```

Add app URL path to [project]/urls.py:

```python
from django.urls import include

urlpatterns = [
    path('[path]', include('[app-name].urls')),
]
```
