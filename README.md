# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

Entity Relationship Diagram:

##![ERdiagram](https://github.com/Raakesh007/django-orm-app/assets/138850267/1b0dcdee-ef80-4e74-a9fa-1b41463aebfa)
 

## DESIGN STEPS

### STEP 1:
creating a table using required details in Django-ORM
### STEP 2:
uplode the python code.
### STEP 3:
push the code to github.

## PROGRAM

### models.py:
from django.db import models
from django.contrib import admin

class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    mobile=models.IntegerField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','mobile') 

### admin.py:
from django.contrib import admin
from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)

## OUTPUT

### student list:
![studentlist](https://github.com/Raakesh007/django-orm-app/assets/138850267/50a1a83f-2935-42ec-a159-f3e66c66fc63)


### student error:
![studenterror](https://github.com/Raakesh007/django-orm-app/assets/138850267/094203a5-a163-4a25-9596-fa98acbb9c16)



## RESULT:
The Program is Executed successfully.
