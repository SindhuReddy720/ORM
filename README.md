# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![alt text](505150514-6a96f356-bc03-4c5a-a155-c9e960ec7933.png)

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
## Admin.py
```py
from django.contrib import admin
from . models import Car


admin.site.register(Car)

class CarAdmin(admin.ModelAdmin):
    list_display = ('id','brand','model','year','price')
```

## Models.py
```py
from django.db import models

class Car(models.Model):
    id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models.CharField(max_length=30)
    year = models.DateField()
    price = models.IntegerField()
```




## OUTPUT

![alt text](<Screenshot 2025-11-10 221647.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
