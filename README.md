# Learning Django bit by bit.
# Create and activate a virtual environment

mkdir Dev
cd Dev
ls
mkdir trydjango
cd trydjango
virtualenv
pwd
ls
virtualenv -p python3 .             #the last part can be ignored if python3 already exists
source bin/activate
pip install django==2.0.7

cd Dev
ls
source bin/activate
.\scripts\activate                  #this command is for windows users
pip freeze
virtualenv venv -p python3
 rm -rf Dev                         #to remove directory
 
# Creating a new project
cd Dev
ls
cd trydjango
source bin/activate

mkdir src
cd src
ls
cd ./
ls
django-admin startproject trydjango
ls
python manage.py runserver              #get the url to open project in new window, from here just open project in new editor
python manage.py migrate                #sync database with project
python manage.py createsuperuser
