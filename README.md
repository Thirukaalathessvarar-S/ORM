# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![entity diagramjjh](https://user-images.githubusercontent.com/121166390/230269600-81b3f57b-970c-4ce4-915d-8d158ebc6489.png)

## DESIGN STEPS

### STEP 1:
An Django application is created inside dataproject folder.

### STEP 2:
A python program is written to create a table to store and retrieve data.

### STEP 3:
The table is created with 6 fields in which the username field is made as PrimaryKey.

### STEP 4:
Then the project files migrated. A superuser is also created.Write your own steps

### STEP 5:
Now the server side program is executed .

### STEP 6:
The admin page of our website is accessed using username and password.

### STEP 7:
Records are added and saved in the table inside the database.

## PROGRAM
```
from django.db import models
from django.contrib import admin


# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## OUTPUT
![web_exp1(2)](https://user-images.githubusercontent.com/121166390/230269739-0129e48a-9329-4572-9712-1e3fe89b5698.png)

![2023-04-06 (10)](https://user-images.githubusercontent.com/121166390/230270177-f12a6c71-30aa-4c0e-9d82-2a323614b14c.png)

## RESULT
Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
