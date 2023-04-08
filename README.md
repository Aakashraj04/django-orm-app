# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![table](https://user-images.githubusercontent.com/121117266/230702799-27357c23-a3fd-4bcb-a73f-aaeb4d634adc.png)



Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Fork and clone the repositary in to your IDE.

### STEP 2:
Create a django project and an app and a superuser account and run the server.

### STEP 3:
Modify changes in settings and write ur code on models and admin and run the server.

### STEP 4:
Login in to admin using your superuser account and populate the records.

## PROGRAM
```python
from django.db import models
from django.contrib import admin

class Employee (models.Model):
   emp_id=models.CharField(primary_key=True,max_length=4,help_text='Employee ID')
   ename=models.CharField(max_length=50)
   post=models.CharField(max_length=20)
   phonenumber=models.IntegerField()
   salary=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','phonenumber','salary')
```

## OUTPUT

![output2](https://user-images.githubusercontent.com/121117266/230702810-bf0fec3d-5a6c-4bbf-a292-568210d41718.png)

## Verifying Primary-Key

![Screenshot 2023-04-06 090423](https://user-images.githubusercontent.com/121117266/230702977-9bf9097e-3e65-4394-8f90-ac0bf82845db.png)



## RESULT
Thus we developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
