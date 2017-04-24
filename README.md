# ImportantPoints

      Uninstall django 

sudo apt-get purge django*
sudo pip uninstall django
sudo rm -rf /usr/lib/python2.7/dist-packages/django


      install django

sudo apt-get install python-django  			//django 1.6.1
sudo pip --upgrade django								//django 1.10.2		

install mysql -> phpmyadmin -> php7.0-mbstring -> 	libapache2-mod-php7.0 -> gettext -> restart apache

NLToolkit,  textrazor,  regex
Getting a list of processes, represented in the Launcher, using the window list : wmctrl -lp 

To Kill process on specific port :
 
This fuser 8080/tcp will print you PID of process bound on that port.
And this fuser -k 8080/tcp will kill that process.
Works on Linux only. More universal is use of lsof -i4 (or 6 for IPv6).
lsof -i TCP:8800

let's say that you had problems with migration 0003 and 0002 but migration 0001 was ok... so to go back to migration 0001 do

python manage.py migrate my_app 0001 --fake
		
		import pdb
        pdb.set_trace()
        
        
       django objects.raw important ponts
 1. raw query must include primary key:  use primary key column as it is in db table(case sensitive)
 2. use any model to run raw method.
 3. for dict type queryset: use dictfetchall(cursor)
