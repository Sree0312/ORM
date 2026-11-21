# Ex02 Django ORM Web Application
# Date:
19/11/2026
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
admin.py
from django.contrib import admin
from .models import Car

admin.site.register(Car)

apps.py
from django.apps import AppConfig


class CarsConfig(AppConfig):
    name = 'cars'

models.py
from django.db import models
class Car(models.Model):
    company = models.CharField(max_length=100)
    name = models.CharField(max_length=100)
    year = models.IntegerField()
    price = models.IntegerField()

    def __str__(self):
        return self.name


# OUTPUT
<img width="1917" height="1078" alt="EX02_Output" src="https://github.com/user-attachments/assets/89cce325-3595-4272-af2e-16bc1718410b" />
<img width="1917" height="1078" alt="image" src="https://github.com/user-attachments/assets/76a92573-112a-4ca7-823b-6bcec680abd5" />


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
