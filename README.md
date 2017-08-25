# Code Louisville 2017 Python/Django Cohort
Basic Django Project for the Fall 2017 Python Cohort serving the site from FEWD and extending functionality. LouiePizza contains the full Django project.

For the original FEWD project see https://github.com/CodeLouisville/May2017-FEWD-Class-Project

#Setup Python:
https://www.python.org/downloads/
For Linux/MacOS you can use apt/yum or brew to install also.

I would highly recommend using virtual environments for your python projects. To make that easy you can:
    pip install pipenv
The first time you do a pip install in your project directory pipenv will check for a virtualenv and create one of it is absent. To activate the virtual environment in your console enter:
    pipenv shell
And you will be in a shell in your virtual environment for that project.

#Setup project
The official Django documentation can be found here:
https://docs.djangoproject.com/en/1.11/

The official Django intro tutorial can be found here, but our project is a little different:
https://docs.djangoproject.com/en/1.11/intro/tutorial01/

In your terminal activate your virtual environment and install Django:
    pip install django 

If you want to check if django is installed from the terminal:
    python -m django --version

Once you have Django installed navigate to your project directory in the command line/terminal and once you are in your project directory start your Django project by entering the command:
    django-admin startproject LouiePizza

In your python project directory you should now see a django project directory called LouiePizza and a manage.py file. Your LouiePizza project folder should have a subfolder named LouiePizza as well as some key Python files:

*__init__.py
*settings.py
*urls.py
*wsgi.py

Finally lets start the built in Django web server and make sure you can access your site locally.
    python manage.py runserver

##Additional information and project updates will occur as the Fall Python Cohort progresses.

#Running the project
If you just want to run the project (assuming Python is on your system and pipenv) in your terminal:

    git clone https://github.com/AlexHagerman/code_louisville_django.git
    cd code_louisville_django\LouiePizza
    python manage.py migrate
    python manage.py runserver

And navigate to 127.0.0.1:8000 in your browser
