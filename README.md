# Ex02 Django ORM Web Application
# Date:25/03/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-04 144713](https://github.com/user-attachments/assets/72ecffd9-9d9b-4f19-8756-af8c6a320e35)

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

admin.py
~~~
from django.contrib import admin
from .models import book,bookadmin
admin.site.register(book,bookadmin)
~~~

models.py
~~~
from django.db import models
from django.contrib import admin
class book(models.Model):
    Book_name=models.CharField(max_length=100)
    Author=models.CharField(max_length=100)
    Co_author=models.CharField(max_length=100)
    Book_code=models.IntegerField()
    Publisher=models.CharField(max_length=100)
    MRP=models.IntegerField()
class bookadmin(admin.ModelAdmin):
    list_display=("Book_name","Author","Co_author","Book_code","Publisher","MRP")
~~~

# OUTPUT
![image](https://github.com/user-attachments/assets/e4cd64d0-4102-402e-a355-fc27992200b4)

![Screenshot (62)](https://github.com/user-attachments/assets/fe550d54-8c83-4e14-931e-b450c1b9ba26)

![Screenshot (60)](https://github.com/user-attachments/assets/d66affd9-b148-4c38-8a94-7b32b756cb99)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
