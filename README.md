# Python-Django
#### You I will Explain all the steps one-on-one from scratch on how to create the simple addition operation with Django on the webpage at port http://127.0.0.1:8000/ - default Django port

#### Open the Command prompt
###### 1. Check whether your machine is installed with the Python version
###### C:\Windows\System32>python --version
###### Python 3.10.5 if not, cmd: pip install python
###### 2. Next, I need to create my virtual environment to install Django, because I don't want my entire machine to install on it.
###### 3. cmd: mkvirtualenv test after you created your environment you can go to your directory and check whether it is created or not under your Cdrive:
<img width="859" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/a6e596b4-d3c0-41c9-b939-3bf4e119de81">

<img width="856" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/8135f03e-be83-4ca7-98d0-7fe2e010535a">

###### 4. Here, I'm giving my virtual environment name as a test
###### 5. If you have already created the virtual environment before you can simply type cmd: C:\Users\lenovo>workon test
###### 6. So, from onwards it uses a test virtual environment to run all your commands. Now, install Django in your virtualenv test cmd: pip install django
###### 7. now I need to create my webpage so that I need to create a projects file cmd: mkdir projects
###### 8. cmd: django-admin startproject sidtronic -- Here I'm giving my project name as sidtronic, go to your dir and check for your project file created or not.
<img width="855" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/3e92f2ee-1935-457d-829b-d9c3c8c1d744">

###### Inside your project file there will be manage.py file where your main server runs on this. and also there are other files: 
###### 1. urls.py 2. settings.py -- I will explain this later on.
<img width="857" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/7ddcfae3-6e7d-480a-a044-fac776d8fc59">

###### To run my project in cmd prompt type: 
###### 9. (test) C:\Users\lenovo>cd projects
###### 10. (test) C:\Users\lenovo\projects>cd sidtronic
###### Now check with dir the files inside your project:
###### 11. (test) C:\Users\lenovo\projects\sidtronic>dir
<img width="381" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/6da4b583-76b5-4498-ab8a-4ea718bf34af">

###### 12. Now open Visual Studio code, If not install please refer: https://code.visualstudio.com/download -- for both windows & linux
###### 13. Now, click on open folder and import your project directory created on your CDrive.
<img width="188" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/a4f5f6b2-b239-4292-93b0-abc261b44f4a">

###### 14. Now I'm creating the app name called demoapp -- Note: It's an app, not the project, app we will use for to combine all the modules as the framework under the project. 
###### 15. To create demoapp run the command in a command prompt -- python manage.py startapp demoapp -- Note: It should run on test environment otherwise it occurs error. after creating you can check in your visual studio code of folder with name -demoapp
<img width="189" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/9fd5a31b-4538-44ce-a6be-7d1ae4f35d2d">

#### 1. views.py 
###### -- here views.py file will be there from demoapp, but not from your project file -- If you want you can create by create file -- views.py
###### Under this views.py we create or Implement the logic.

#### 2. urls.py
###### -- It's very important beacuse the web server with runs from this as it works like the admin, whatever logic you implemented on views.py the urls path should be added to this. # Note you should create additional paths on the main project file, not in the demoapp -- if you create url in demoapp the server will show you as default.

#### 3. Settings.py
###### This we will have DTL (Dashboard template language) -- where you can see different installed apps, and settings configurations for the web application.
<img width="960" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/566fbca4-0109-4c9d-87f8-1c95bdad68f0">

###### Here in settings I need to change few things, 
###### 1. I need to add demo app into my installed apps in settings.py
<img width="678" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/067fb8ea-4c0e-4d5c-a858-b93bcde8dbe8">

###### 2. I need to add my template folder where I do my HTML code workings -- for that I need to create folder with name templates in vs code. after that type command in settings.py -- under TEMPLATES [ 
###### 'DIRS': [os.path.join(BASE_DIR,'templates')] ]
<img width="698" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/e0cbcf8f-c9d1-4520-b503-bf5c646f7836">

###### 3. If you want you can change the time also - to Indian time by 'Asia/Kolkata'
<img width="656" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/a89f87f3-fdff-48c0-b15b-dd5d90b97203">

### Now, Let's implement the simple addition web page. 
#### 1. Firstly, I need to create home.html for my front end - view operations that view by the user.
#### 2. base.html where we add background color as bgcolor. -- Here to work jinja, add extension.

###### NOTE: GET is used to fetch the data, POST is used to submit the data.
###### I'm attaching the image format of the inputs you can Understand Easily.

# Inputs:
### 1. templates -> home.html
<img width="700" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/8b1adc1b-00d4-4e41-a2ac-2552a16c7a94">

###### Here under home.html we extend the base.html with jinja {% extends 'base.html' %} -- as in base.html we will have our docHTML frontend view operation.

### 2. base.html
<img width="690" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/1aefb52b-6947-4a5c-abc9-7a7a117fbc00">

### 3. views.py
<img width="691" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/48d9f009-7ad6-4ea8-a376-ca481d9ca89e">

### 4. result.html
<img width="696" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/9fee83d3-d700-4def-8f82-098628d31934">

### 5. urls.py
<img width="695" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/0b4f851f-a86a-4992-a92d-abfe51315722">

# OUTPUT:
###### To run the server of your web application go to command prompt and type cmd: 
###### python manage.py runserver
<img width="486" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/29572bfa-b7a7-4966-84e0-d54dc8e45e32">

<img width="960" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/cc6c87b1-e00b-446a-a4f3-85effba83f7b">

<img width="960" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/3d8b6eea-183b-4b3e-ad37-2259cb58a6ad">

<img width="960" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/306b0ae1-3339-48ee-8ec2-012c886f4b48">

## For Any Queries you can Contact Email Id: vigneswarsiddu07@gmail.com




















