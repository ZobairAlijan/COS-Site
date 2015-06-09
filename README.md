# COS-Site

This repository holds the rework of centerforopenscience.org into the Django and Mezzanine frameworks.

# Install Instructions
- Clone or Download repo
- Run $ pip install -r requirements.txt
- Run $ python manage.py runserver
- Visit http://127.0.0.1:8000/

#Admin Interface
- http://127.0.0.1:8000/admin
- Admin username: zobair
- Admin password: cos

#FAQ

<b>My server won't start</b>

If the server doesn't run, check the reqirements.txt folder. Sometimes, pip doesn't install all of the requirements properly, and the server will tell you which ones aren't installed. These must be installed manually

$ pip install [packagename]

<b> My server was working but is now broken</b>

If you made changes to the ViewModels, you'll likely need to update the database tables

$ python manage.py makemigrations
$ python manage.py migrate
If your database is completely broken, to create a new database:

$ rm /mysite/dev.db
$ python manage.py createdb
Note: some tables won't be repopulated (Team, News, Ambassadors, Jobs). These can be repopulated with

$python manage.py csvimport [options]
- Replace '[options]' with --help for help.
- TODO: script for ^
