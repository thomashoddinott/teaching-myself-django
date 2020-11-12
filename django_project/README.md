https://www.youtube.com/watch?v=UmljXZIypDc

n.b. on powershell install django `pip install django` from elevated shell

---

**lessons 1 - 2**

`python manage.py startapp blog`

`python manage.py runserver`

`django-admin startproject django_project`

---

**lesson 3** 

- you should create templates for html
- add apps to `INSTALLED_APPS` in settings.py
- CSS goes into a `static` dir

---

**lesson 4**

- Django comes with admin functionality. Saves work on the backend.

- Before adding a superuser to admin, we need to run `python manage.py makemigrations` followed by `python .\manage.py migrate`

- Now `python .\manage.py createsuperuser` will work. Follow the instructions to create a superuser.

  





