# Week 3 Challenge Code Louisville 2017 Python/Django Cohort
Basic Django Project for the Fall 2017 Python Cohort serving the site from FEWD and extending functionality. LouiePizza contains the full Django project.

For the original FEWD project see https://github.com/CodeLouisville/May2017-FEWD-Class-Project

# Challenge
The Code Louisville Louies Pizza FEWD project served content on one page. Let's break the various pieces of content (Newsletter, Menu, Contact, Homepage) into separate pages that we can use to learn more about Django. Each page should take advantage of the Django templating engine and inherited layouts with block content. 

The Homepage should be a simple landing page with Louie Pizza's history and operational links to the other pages.

The Newsletter should be it's own page and use the javascript email validation from the FEWD project, but is not functional beyond that at this point.

The Menu should be populated via Django models and categories/menu items should be added and managed via the Django Admin console.

Finally the contact page will not be available and will be setup at a later time using Django Forms.

## Setup Python:
https://www.python.org/downloads/
For Linux/MacOS you can use apt/yum or brew to install also.

I would highly recommend using virtual environments for your python projects. To make that easy you can:

    pip install pipenv
The first time you do a pip install in your project directory pipenv will check for a virtualenv and create one of it is absent. To activate the virtual environment in your console enter:

    pipenv shell
And to exit the pipenv shell:

    exit
And you will be in a shell in your virtual environment for that project.

## Django project setup
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

 - \__init__.py
 - settings.py
 - urls.py
 - wsgi.py

Finally lets start the built in Django web server and make sure you can access your site locally.

    python manage.py runserver

You are now ready to take what you have learned from the Django Treehouse modules and convert the FEWD content to be served via the Django backend.

# Solution
In your parent Django Directory you should begin by creating two templates one for all pages to inherit from including the header and footer, and one for the homepage.

Next following the Django app model we can create a Menus and Newsletters app for us to handle Louie Pizza's menu and newsletter.

Within the Menus

Within the Newsletters

# Running the solution project
If you just want to run the project (assuming Python is on your system and pipenv) in your terminal:

    git clone https://github.com/AlexHagerman/code_louisville_django.git
    cd code_louisville_django
    pipenv install
    cd LouiePizza
    pipenv shell
    python manage.py migrate
    python manage.py runserver

And navigate to 127.0.0.1:8000 in your browser
When you are ready to shutdown the server and exit the environment:

    ctrl+c
    exit

