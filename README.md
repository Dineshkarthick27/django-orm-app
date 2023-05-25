# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/Dineshkarthick27/django-orm-app/assets/120552008/4370c337-5bf1-4263-91f3-920239d02329)


## DESIGN STEPS

### STEP 1:
clone the repository from github.

### STEP 2:
create an admin interface for django

### STEP 3:
create an app and edit settings.py

### STEP 4:
make migrations and migrate the changes.

### STEP 5:
create admin user and write python code for admin and models.

### STEP 6:
make all the migrations to 'myapp'.

### STEP 7:
create an student database with 10 fields using runserver command.

## PROGRAM

### admin.py:
```python
from django.contrib import admin
from.models import student,studentAdmin
admin.site.register(student,studentAdmin)
```
### models.py:
```python
from django.db import models
from django.contrib import admin
class student(models.Model):
    sid=models.CharField(max_length=200)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','salary','age','email')
```
## OUTPUT
## server output:

## client output:


## RESULT
The program for creating an student database using ORM is executed sucessfully.
