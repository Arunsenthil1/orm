# Ex02 Django ORM Web Application
## Date: 19/11/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![er diagram](https://github.com/user-attachments/assets/a351899c-6900-4b64-a8f2-a221007a3ab4)


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
'''
admin.py 

from django.contrib import admin
from .models import loan,loanadmin
admin.site.register(loan,loanadmin)

models.py

from django.db import models
from django.contrib import admin
class loan (models.Model):
    loan_id=models.IntegerField(primary_key=True)
    loan_type =models.CharField(max_length=30)
    loan_amnt =models.FloatField()
    cust_acntno =models.IntegerField()
    cust_name=models.CharField(max_length=50)
 
class loanadmin(admin.ModelAdmin):
    list_display=('loan_id','loan_type','loan_amnt','cust_acntno','cust_name')
'''
## OUTPUT

![e9384cd0-d12a-4f8c-8263-f572a337c40a](https://github.com/user-attachments/assets/0b6231a1-7540-4730-a7db-1fd7088d8066)
![5c257433-a8c5-4fd6-baf8-661d2eae9eae](https://github.com/user-attachments/assets/4154cf98-8144-45ad-8f62-063bcb07c47c)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
