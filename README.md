# Ex02 Django ORM Web Application
# Date:05.11.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-07 154822](https://github.com/user-attachments/assets/cf390f9a-1b32-4f5e-bd28-a6f534acc395)


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
## models. py
```
from django.db import models
from django.contrib import admin

# Create your models here.
class Bank_Loan(models.Model):
    loan_id = models.CharField(max_length=20,primary_key=True)
    loan_type = models.CharField(max_length=30)
    loan_amd = models.FloatField()
    cust_acno = models.IntegerField()
    cust_name = models.CharField(max_length=50)
```
## admin.py 
 from django.contrib import admin
from.models import Bank_Loan, Bank_LoanAdmin

# Register your models here.
admin.site.register( Bank_Loan,Bank_LoanAdmin)
# OUTPUT
![Screenshot 2024-12-07 154917](https://github.com/user-attachments/assets/f1534cef-7621-45c3-90e3-bbfec2b21550)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
