django-custuser
===============

## Description

This is a simple and basic Custom User Django App.

The email field is used for the username. Other fields are required for
the built-in admin or registration process.

You can add your custom fields by following the instructions bellow.

Read the code and understand what it does. Help me to make it better!
But remember, this must stay simple and basic.

Thank you!

Fields list:
-------------------
    - email (username)
    - password
    - date_joined
    - last_login
    - is_active
    - is_admin

## Requirements

    - Python 3.4
    - Django 1.6

## How to install it

Copy the app folder into your project.

Add 'custuser' to INSTALLED_APPS in your settings.py.
Don't forget the ',' at the end!

Add AUTH_USER_MODEL = 'custuser.CustUser' to your settings.py

## How to use it

Run the following command in your django project folder:
python manage.py syncdb

That's it! You now have custom user in your project.

## How to add fields

models.py
    - Add your custom fields at line #42
    - Add your required fields at line #59
    - Add your required fields to the create functions at line #11, #18, #24 and #28

forms.py
    - Add your required fields and desired fields to line #17 and #45

admin.py
    - Add your custom fields to line #21 and #30

*** WORK IN PROGRESS ***