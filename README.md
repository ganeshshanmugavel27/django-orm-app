# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github.

### STEP 2:
Create a new app.

### STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Create django app and add student details.

## PROGRAM
## models.py 
```
from django.db import models
from django.contrib import admin


class Student(models.Model):
    referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## Admin.py
```
from django.contrib import admin
from myapp.models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```

## OUTPUT
![dj2](https://user-images.githubusercontent.com/122046208/236866978-05f0f7c9-0d1e-4188-a8f4-51eae92ffe81.png)
![d j](https://user-images.githubusercontent.com/122046208/236867212-45c31df4-8a39-4b05-a6db-75dae336e7f4.png)

## RESULT
Program executed successfully.
