# HR_Employee File Management System
A Employee file management site to take care of employee's salaries, deductions, bonuses and leave management.
## Installation Steps:
* Create a virtual Environment
* Install Django using:
  * ```
    pip install django
    ```
* Install mysqlclient using:
  * ```
     pip install mysqlclinet
    ```
* clone this project.
* Go to settings.py by payroll_management_sys -> settings.py
  Change the database user credentials, this block of code:
  ```
  DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'payrolldb',
        'HOST': '127.0.0.1',
        'PORT': '3306',
        'USER': 'root',
        'PASSWORD': 'password',
      }
  }
  ```
* create database : payrolldb
* run these commands in cmd in payroll_management_system folder:
  ```
  python manage.py makemigrations
  python manage.py migrate
  python populate_user.py 
  ```
* run populate_table.sql -> SQL script in mysql
* Finally on cmd run,
```
python manage.py runserver
```
* If successful , the site will be running on [localhost:8000/](localhost:8000)
## Admin credentials:
|   Admin Id    |   Password    |
| ------------- | ------------- |
|       0       |   password    |

## employee credentials:
|  employee Id  |   Password    |
| ------------- | ------------- |
|       1       |   password    |
|       2       |   password    |
|       3       |   password    |
|       4       |   password    |
|       5       |   password    |
|       6       |   password    |
|       7       |   password    |
|       8       |   password    |
|       9       |   password    |
|       10      |   password    |
|       11      |   password    |
