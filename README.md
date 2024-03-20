# Ex02 Django ORM Web Application
## Date: 20/3/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/babavoss05/ORM/assets/103019882/064fe3c6-a632-411b-8956-0cbaced40861)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM:
``` python
admin.py

from django.contrib import admin
from.models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

model.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
    b_id = models.IntegerField(primary_key="b_id");
    b_name = models.CharField(max_length=100);
    b_author = models.CharField(max_length=100);
    b_edition = models.CharField(max_length=20);
    b_year = models.DateField();

class Book_DBAdmin(admin.ModelAdmin):
    list_display = ("b_id","b_name","b_author","b_edition","b_year");

```

## OUTPUT:

![image](https://github.com/babavoss05/ORM/assets/103019882/a1fce1ba-aeff-40e8-8464-0fcdea047880)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
