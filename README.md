# Ex02 Django ORM Web Application
## Register Number: 212221040044
## Date: 26-09-2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

### Models.py

```
from django.db import models
from django.contrib import admin
class Player (models.Model):
    pid=models.CharField(max_length=20,help_text="Player ID")
    name=models.CharField(max_length=100)
    goals=models.IntegerField()
    trophies=models.IntegerField()
    

class PlayerAdmin(admin.ModelAdmin):
    list_display=('pid','name','goals','trophies')
```

### Admin.py

```
from django.contrib import admin
from .models import Player,PlayerAdmin
admin.site.register(Player,PlayerAdmin)
```


## OUTPUT

![Alt text](<Screenshot 2023-11-15 141638.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
