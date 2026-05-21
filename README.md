# Ex02 Django ORM Web Application
## Date:

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).


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
models.py

from django.db import models 
from django.contrib import admin
class Cars_DB (models.Model):
     Car_name=models.CharField(max_length=20)
     reg_no=models.IntegerField (primary_key=True)
     fuel_type=models.CharField(max_length=20)
     engine_model=models.CharField(max_length=20)
     insurance_no=models.IntegerField()
class Cars_DBAdmin(admin.ModelAdmin):
     list_display=["Car_name","reg_no","fuel_type","engine_model","insurance_no"]

admin.py

from django.contrib import admin
from .models import Cars_DB,Cars_DBAdmin
admin.site.register(Cars_DB,Cars_DBAdmin)
```


## OUTPUT


<img width="1013" height="543" alt="Screenshot 2026-05-21 131702" src="https://github.com/user-attachments/assets/27b4754c-c107-4f15-ab09-7d550c02434f" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
