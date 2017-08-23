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

![Django Start](https://github.com/AlexHagerman/code_louisville_django/challenge_docs/project_screenshots/challenge_1.1.png)

In your python project directory you should now see a django project directory called LouiePizza and a manage.py file. Your LouiePizza project folder should have a subfolder named LouiePizza as well as some key Python files:

*__init__.py
*settings.py
*urls.py
*wsgi.py

Finally lets start the built in Django web server and make sure you can access your site locally.

![Django Hello](https://github.com/AlexHagerman/code_louisville_django/challenge_docs/project_screenshots/challenge_1.2.png)
