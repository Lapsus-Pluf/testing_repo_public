Tutorial URL: https://www.w3schools.com/django/index.php
1. Install Python
2. Install Pip
3. Create virtual environment
    python -m venv venv
4. Activate virtual environment
    Unix/MacOS
        source venv/bin/activate
    Windows
        venv\Scripts\activate
5. Install Django (inside venv)
    python -m pip install Django
6. Create project
    django-admin startproject my_tennis_club
7. Run the Django project
    cd my_tennis_club
    python manage.py runserver
8. Create an app
    python manage.py startapp members
9. Migrate changes
    python manage.py migrate
10. Create the model (table) in the database. / Creates new migration(s) for apps.
    python manage.py makemigrations members
11. View the executed SQL command during migration. / Prints the SQL statements for the named migration.
    python manage.py sqlmigrate members 0001
