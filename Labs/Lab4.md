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


