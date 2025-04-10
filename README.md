# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![alt text](<Screenshot (231).png>)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 movies.

## PROGRAM
admin.py

'''
from django.contrib import admin
from .models import Movies,MoviesAdmin
admin.site.register(Movies,MoviesAdmin)
'''

models.py
'''
from django.db import models
from django.contrib import admin
class Movies(models.Model):
    User_ID = models.IntegerField(primary_key=True)
    User_Name = models.CharField(max_length=100)
    Email_ID = models.EmailField()
    Phone_Number = models.BigIntegerField()
    MovieName = models.CharField(max_length=150)
    Show_DateTime = models.DateTimeField()
    No_of_Seats = models.IntegerField()

class MoviesAdmin(admin.ModelAdmin):
    list_display=('User_ID','User_Name','Email_ID','Phone_Number','MovieName','Show_DateTime','No_of_Seats')
'''





## OUTPUT
![alt text](<Screenshot (229).png>)




## RESULT
Thus the program for creating a database using ORM has been executed successfully