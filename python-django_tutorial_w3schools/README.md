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
9. Migrate changes and tell Django an update has ocurred. / Updates database schema. Manages both apps with migrations and those without.
    python manage.py migrate
10. Create the model (table) in the database. / Creates new migration(s) for apps.
    python manage.py makemigrations members
11. View the executed SQL command during migration. / Prints the SQL statements for the named migration.
    python manage.py sqlmigrate members 0001
12. Add records to the (now empty) table
    1. Open a Python shell
        python manage.py shell
    2. Import the model
        from members.models import Member
    3. Check model table
        Member.objects.all()
        Member.objects.all().values()
    4. Aggregate a member
        member = Member(firstname='Emil', lastname='Refsnes')
        member.save()
13. Update a record
    1. Get an item
        x = Member.objects.all()[4]
    2. Update and save the item
        x.firstname = "Stalikken"
        x.save()
14. Delete a record
    x.delete()
