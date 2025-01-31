# Ex02 Django ORM Web Application
## Date: 04.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-18 131715](https://github.com/Kavi45-msk/ORM/assets/147457752/f99b0381-d43e-4da3-9752-01a68971cd2b)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
from django.db import models
from django.contrib import admin
class Book_dbs(models.Model):
     serialno=models.IntegerField(primary_key="serialno");
     bookname=models.CharField(max_length=20);
     publisher=models.CharField(max_length=20);
     Dop=models.DateField();
     totalpg=models.IntegerField();
class Book_dbsAdmin(admin.ModelAdmin):
     list_display=("serialno","bookname","publisher","Dop","totalpg");

from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```

## OUTPUt
![alt text](screenshot-1.png)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
