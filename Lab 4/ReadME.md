## Lab 4 - Django and Flask

## Requirnments 
This lab comes with a few installation requirnments.

1) You must install Django and Django REST framework on Raspberry Pi. You can do this with the following command sets

                  $ pip3 -V
                  $ pip3 list
                  $ sudo pip3 install -U setuptools
                  $ sudo pip3 install -U django
                  $ sudo pip3 install -U djangorestframework
                  $ sudo pip3 install -U django-filter
                  $ sudo pip3 install -U markdown
                  $ sudo pip3 install -U requests
                  
 2) You must install psutil in mycpu step 11 using
    
                ~/mycpu $ sudo pip install -U psutil
                        
                                 
## Notes 
 
 1) When running the install commands, sudo is not supported in Msys2, and can be preformed without the sudo prefix.
 2) A raspberry pi was need for me to complete this lab. 
 
 ## My Cpu Setup
 1) Start the Django Rest project 
      $ django-admin startproject mycpu
      $ cd mycpu
    
 2) Start the Django Rest App
      $ python manage.py startapp myapp
      $ ls
 
 3) Edit the setting of Django project 
      ~/mycpu $ cd mycpu
      ~/mycpu/mycpu $ ls
      ~/mycpu/mycpu $ nano settings.py

 4) Copy the urls 
      ~/mycpu/mycpu $ cp ~/iot/lesson4/mycpu/urls.py .
      ~/mycpu/mycpu $ cd ..
 
 5) The copy admin.py, models.py, views.y, and serializers.py to the path ~/mycpu/myapp  
      ~/mycpu $ cd myapp
      ~/mycpu/myapp $ ls
      admin.py  apps.py  __init__.py  migrations  models.py  tests.py  views.py
      ~/mycpu/myapp $ cp ~/iot/lesson4/mycpu/admin.py .
      ~/mycpu/myapp $ cp ~/iot/lesson4/mycpu/models.py .
      ~/mycpu/myapp $ cp ~/iot/lesson4/mycpu/views.py .
      ~/mycpu/myapp $ cp ~/iot/lesson4/mycpu/serializers.py .

6) Change the password using the nano text editor
      ~/mycpu/myapp $ nano views.py
 
7) Copy the index file in hdml
      ~/mycpu/myapp $ mkdir static templates
      ~/mycpu/myapp $ cd templates
      ~/mycpu/myapp/templates $ mkdir myapp
      ~/mycpu/myapp/templates $ cd myapp
      ~/mycpu/myapp/templates/myapp $ cp ~/iot/lesson4/mycpu/index.html 
      
8) Copy the static file
      ~/mycpu/myapp/templates/myapp $ cd ~/mycpu/myapp/static
      ~/mycpu/myapp/static $ cp ~/iot/lesson4/static/favicon.ico .
      ~/mycpu/myapp/static $ mkdir myapp
      ~/mycpu/myapp/static $ cd myapp
      ~/mycpu/myapp/static/myapp $ cp ~/iot/lesson4/static/*css .
      ~/mycpu/myapp/static/myapp $ cp ~/iot/lesson4/static/*js .
      ~/mycpu/myapp/static/myapp $ cd ~/mycpu
 
 9) Copy the controller.py to the file path ~/mycpu
      ~/mycpu $ ls
      ~/mycpu $ cp ~/iot/lesson4/mycpu/controller.py .
 
 10) Change the default admin password
      ~/mycpu $ nano controller.py
 
 11) If you encounter no changes use the following commands
    ~/mycpu $ python manage.py makemigrations myapp
    ~/mycpu $ python manage.py migrate
    ~/mycpu $ python manage.py createsuperuser

12) Run the django server
 
      ~/mycpu $ python manage.py runserver
 
 
 ## Steps Stevens Setup
 After completing the installation enter the following steps.
 
 1) Start the project - This creates the project
    $ django-admin startproject stevens
    
    $ cd stevens
    
    $ ls
    
2) Create an Sql Database if you used MAriaDB
        
        $ sudo mysql -u root -p
        
        Enter password: PASSWORD
        
        MariaDB [(none)]> use mysql
        
        MariaDB [mysql]> select user, host from mysql.user;
        
        MariaDB [mysql]> create user pi@localhost identified by 'PASSWORD';
        
        MariaDB [mysql]> show databases;
        
        MariaDB [mysql]> create database stevens;
        
        MariaDB [mysql]> grant all privileges on stevens.* to pi@localhost;
        
        MariaDB [mysql]> quit
 
 3) If you want to edit settings use the following
 
        pi@raspberrypi:~/stevens $ cd stevens
        
        pi@raspberrypi:~/stevens/stevens $ ls
        
        pi@raspberrypi:~/stevens/stevens $ nano settings.py
        
        This will open nano to allow you to adjust and change settings 
        
 4) Copy the urls to stevens
 
      pi@raspberrypi:~/stevens $ cd myapp

      pi@raspberrypi:~/stevens/myapp $ ls

      admin.py  apps.py  __init__.py  migrations  models.py  tests.py  views.py

      pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/admin.py .

      pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/models.py .

      pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/views.py .
 
 5) Copy the index 
      
      pi@raspberrypi:~/stevens/myapp $ mkdir static templates
      
      pi@raspberrypi:~/stevens/myapp $ cd templates
      
      pi@raspberrypi:~/stevens/myapp/templates $ mkdir myapp
      
      pi@raspberrypi:~/stevens/myapp/templates $ cd myapp
      
      pi@raspberrypi:~/stevens/myapp/templates/myapp $ cp ~/iot/lesson4/stevens/index.html .


## Viewing 

After completing the setup, go to this address in a web browser " http://127.0.0.1:8000/admin ". 
Input the location data and add one of the following two locations 
      1) Location Stevens, Latitude 40.7451, Longitude -74.0255
      
      2) Location Xidian, Latitude 34.12250, Longitude 108.84029
      
Then save your changes. 


I ran mine locally using the following command

      python manage.py runserver 0.0.0.0:8000.
      
This will give you access to the admin page of the website you have set up previously. Here you can enter your username and password and view the temperature data.


Similarly with the mycpu you follow the same procedure and log into the account you set up using the password and username previosuly set. You can then view the cpu usage and memory available. 




 
        
        
