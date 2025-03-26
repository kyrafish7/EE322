# Lab 4
#  Django and Flask

## Installing Django and REST framework
### The following commands were executed in my terminal to install Django and Django REST framework:
#### `pip3 install -U setuptools`, `pip3 install -U django`, `pip3 install -U djangorestframework`, `pip3 install -U django-filter`, `pip3 install -U markdown`, `pip3 install -U requests`
![image](Images/Lab4downloads.png)
![image](Images/Lab4downloads2.png)


### `django-admin startproject stevens` 
#### This started a Django project named "stevens" 
![image](Images/Lab4stevens.png)

![image](Images/Lab4stevens2.png)

### `python3 manage.py startapp myapp`
#### This started a Django app named "myapp" 
![image](Images/Lab4startapp.png)

![image](Images/Lab4startapp2.png)

### `python3 manage.py migrate`
#### I started the app and then this allowed me to mirgrate the database and ensure SQLite was set up 
![image](Images/Lab4migrate.png)

### `nano settings.py`
#### This allowed me to edit settings.py in ~/stevens/stevens to add an asterisk to ALLOWED_HOSTS and 'myapp' to INSTALLED_APPS
![image](Images/Lab4settings.png)

### `cp ~/iot/lesson4/stevens/urls.py .`
#### This copied urls.py to ~/stevens/stevens
![image](Images/Lab4copyurlstostevens.png)

### `cp ~/iot/lesson4/stevens/admin.py .`, `cp ~/iot/lesson4/stevens/models.py .`, `cp ~/iot/lesson4/stevens/views.py .`
#### This copied admin.py, models.py and views.py to ~/stevens/myapp
![image](Images/Lab4copytomyapp.png)

### `mkdir static templates`, `cd templates`, `mkdir myapp`, `cd myapp`, `cp ~/iot/lesson4/stevens/index.html .`
#### This copied index.html
![image](Images/Lab4copyindex.png)

### `nano index.html`
#### This this allowed me to replaced "YOUR_API_KEY" in index.html with the API key which enabled google maps API. To do this, I obtained an API key from the google cloud console. 
![image](Images/Lab4indexhtml.png)

### `cp ~/iot/lesson4/static/favicon.ico .`, `mkdir myapp`, `cd myapp`, `cp ~/iot/lesson4/static/*css .`, `cp ~/iot/lesson4/static/*js .`
#### This allowed me to copy static files from the GitHub repository. I was having errors when running these commands but it should have allowed me to copy these files
![image](Images/Lab4issueswithstaticfiles.png)

### `python3 manage.py makemigrations myapp`, `python3 manage.py migrate` 
#### This allowed me to update the database before running the server

### `python3 manage.py runserver`
![image](Images/Lab4runserver.png)

#### I went to http://127.0.0.1:8000/admin and signed in. I added in  date/time, temperature, longitude, and latitude and saved. Then I went to the Django app by going to http://127.0.0.1:8000. I was getting errors when trying to run this but this was the results I should have gotten.

### The app is shown below:
![image](Images/Lab4results.png)

## Django REST project
### To start this part of the lab I started a Django project titled stevens by executing
#### `django-admin startproject stevens` and `python3 manage.py startapp myapp`
![image](Images/Lab4_1.png)
![image](Images/Lab4_2.png)

### Then I edited settings.py in /mycpu/myapp to the following :
![image](Images/Lab4Settings1.png)

![image](Images/Lab4Settings2.png)

### Then I copied urls.py, admin.py, models.py, views.py and serializers.py to /mycpu/mycpu
### by running the following commands : 
#### - `cp ~/iot/lesson4/mycpu/admin.py .`
#### - `cp ~/iot/lesson4/mycpu/models.py .`
#### - `cp ~/iot/lesson4/mycpu/views.py .`
#### - `cp ~/iot/lesson4/mycpu/serializers.py .`

### Once those were copied I changed my passord in views.py by running `nano views.py` 

### Then I created a few new files and copied index.html by running `cp ~/iot/lesson4/mycpu/index.html .`
![image](Images/Lab4_3.png)

### Next I copied the static files by executing 1cp ~/iot/lesson4/static/*css .` and `cp ~/iot/lesson4/static/*js .`
![image](Images/Lab4_4.png)

### Then I changed switched back to mycpu and copied controller.py by running `cp ~/iot/lesson4/mycpu/controller.py`. Then changed the password by using `nano controller.py.`. Additionally I also installed psutil by running `pip3 install -U psutil`. 
![image](Images/Lab4_5.png)

### Then I ran `python3 manage.py makemigrations myapp`, `python3 manage.py migrate` and `python3 manage.py createsuperuser`. This was giving me some issues I wasn't able to open the actual app but this is what it should have looked like.
![image](Images/Lab4_6.png)
![image](Images/Lab4_7.png)
![image](Images/Lab4_10.png)

## Running Flask Server
### I had previously installed Flask therefore all I had to run was `cd ~/iot/lesson4` and `python3 hello_world.py`
![image](Images/Lab4_8.png)
### Once running I went to the server at http://127.0.0.1:5000/.
![image](Images/Lab4_9.png)

