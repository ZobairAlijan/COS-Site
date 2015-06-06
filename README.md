# COS-Site

This repository holds the rework of centerforopenscience.org into the Django and Mezzanine frameworks.


#Install Instructions

  - Clone or Download repo
  - Run $ pip install -r requirements.txt
  - In the folder, run $ python manage.py makemigrations
  - Then run $ python manage.py migrate
  - Lastly, run $ python manage.py runserver

If the server doesn't run, check the reqirements.txt folder. Sometimes, pip doesn't install all of the requirements properly, and the server will tell you which ones aren't installed. These must be installed manually ($ pip install {packagename})

Admin username: zobair

Admin password: cos
