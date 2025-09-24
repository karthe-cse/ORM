# Ex02 Django ORM Web Application
# Date:24-09-25
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
from django.db import models
from django.contrib import admin
class Car(models.Model):
	car_id = models.AutoField(primary_key=True)   
	brand = models.CharField(max_length=50)
	model = models.CharField(max_length=50)
	year = models.IntegerField()
	price = models.DecimalField(max_digits=10, decimal_places=2)
	fuel_type = models.CharField(max_length=20)

	
class CarAdmin(admin.ModelAdmin):
    list_display = ('car_id', 'brand', 'model', 'year', 'price','fuel_type')

models.py
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)UT
Include the screenshot of your admin page.
```
# Ouput
<img width="1471" height="779" alt="Screenshot 2025-09-24 090632" src="https://github.com/user-attachments/assets/73fd9a9d-2d0d-48e0-9c1b-a28c7a2c8efc" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
