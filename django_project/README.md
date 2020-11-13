https://www.youtube.com/watch?v=UmljXZIypDc

n.b. on powershell install django `pip install django` from elevated shell

---

**lessons 1,2 - Getting Started**

`python manage.py startapp blog`

`python manage.py runserver`

`django-admin startproject django_project`

---

**lesson 3 - Templates** 

- you should create templates for html
- add apps to `INSTALLED_APPS` in settings.py
- CSS goes into a `static` dir

---

**lesson 4 - Admin**

- Django comes with admin functionality. Saves work on the backend.
- `localhost:8000/admin`
- Before adding a superuser to admin, we need to run `python manage.py makemigrations` followed by `python .\manage.py migrate`
- Now `python .\manage.py createsuperuser` will work. Follow the instructions to create a superuser.

---

**lesson 5 - Datebase and Migrations** 

Django has its own ORM

SQLite in dev, Postgres in prod ???

new tables (classes) go into `models.py`

We can do some queries from the interactive shell `python .\manage.py shell` — see video for detailed demo.

We can also open up a connection to Dbeaver with [./db.sqlite3](./db.sqlite3) and do stuff from there:

![dbeaver-django-connection](readme-img/dbeaver-django-connection.PNG)

If we add `admin.site.register(Post)` to `admin.py` we gain access to admin tools for managing Posts:

![django-admin-posts](readme-img/django-admin-posts.PNG)

---

**lesson 6 - User Registration Form**

create new `users` app `python .\manage.py startapp users`

add it to `INSTALLED_APPS` in settings.py

`form.save()` is all we need to add the user in our login. Django takes care of everything.

https://django-crispy-forms.readthedocs.io/en/latest/

*django-crispy-forms provides you with a `|crispy` filter and `{% crispy %}` tag that will let you control the rendering behavior of your [Django](http://djangoproject.com) forms in a very elegant and DRY way. Have full control without writing  custom form templates. All this without breaking the standard way of  doing things in [Django](http://djangoproject.com), so it plays nice with any other form application.*

needs to be added to `INSTALLED_APPS` in settings.py again

^ Bit annoying, `npm install` or `yarn add` automatically add to `package.json`

---







