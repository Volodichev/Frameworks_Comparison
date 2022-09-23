# Frameworks_Comparison
FastAPI, Django and Flask comparison



<table>
   <thead>
      <tr>
         <th></th>
         <th><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-plain.svg" alt="django" width="15" height="15"/> Django</th>
         <th><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-plain.svg" alt="fastapi" width="15" height="15"/> FastAPI</th>
         <th><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/flask/flask-original.svg" alt="flask" width="15" height="15"/> Flask</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Release</td>
         <td>2005</td>
         <td>2018</td>
         <td>2010</td>
      </tr>
      <tr>
         <td>License</td>
         <td>3-clause license</td>
         <td>MIT License</td>
         <td>BSD 3-Clause</td>
      </tr>
      <tr>
         <td>url</td>
         <td>djangoproject.com</td>
         <td>fastapi.tiangolo.com</td>
         <td>flask.palletsprojects.com</td>
      </tr>
      <tr>
         <td></td>
         <td></td>
         <td></td>
         <td></td>
      </tr>
   </tbody>
</table>


## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-plain.svg" alt="django" width="35" height="35"/> Django

### Installation

```console
pip install Django
django-admin startproject todoapp
```

### Start

```console
python manage.py migrate
python manage.py runserver
python manage.py startapp todolist
```

- add 'todolist' to INSTALLED_APPS

### Add views
- implement todolist.views.py and create todolist.urls.py
- add urls to todoapp.urls.py

### Add templates
- add templates folder and file
- add "templates" to DIR in settings.py
- modify view: return render...

### Add models
- implement todolist.models.py

### Put together
```console
manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```

- Adding models to the administration site:
    - todolist.admin.py: admin.site.register(Todo)
- login to admin

### add template
- add {% csrf_token %} to template

### CRUD
- implement views




## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-plain.svg" alt="fastapi" width="35" height="35"/> FastAPI

```console
pip install fastapi
pip install "uvicorn[standard]"
pip install python-multipart sqlalchemy jinja2

uvicorn app:app --reload
```


## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/flask/flask-original.svg" alt="flask" width="35" height="35"/> Flask

```console
python3 -m venv venv
. venv/bin/activate

pip install Flask
pip install Flask-SQLAlchemy

export FLASK_APP=app.py
export FLASK_ENV=development
flask run
```
