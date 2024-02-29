# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Alt text](<WhatsApp Image 2024-02-29 at 08.46.55_80727506.jpg>)

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
class BooK(models.Model):
   bookno=models.IntegerField(primary_key=True);=models.CharField(max_length=20);
   bookprice=models.IntegerField(help_text="Enter the price of book");
   quantity=models.IntegerField();
   authorname=models.CharField(max_length=50);
class BookAdmin(admin.ModelAdmin):
   list_display=("bookno","bookname","bookprice","quantity","authorname");


admin.py

from django.contrib import admin
from.models import BooK,BookAdmin

admin.site.register(BooK,BookAdmin) 

```


## OUTPUT

![Alt text](<Screenshot 2024-02-29 084455.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
