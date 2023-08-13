# Python-Django
#### You I will Explain all the steps one-on-one from scratch on how to create the simple addition operation with Django on the webpage at port http://127.0.0.1:8000/ - default Django port

#### Open the Command prompt
###### 1. Check whether your machine is installed with the Python version
###### C:\Windows\System32>python --version
###### Python 3.10.5 if not, cmd: pip install python
###### 2. Next, I need to create my virtual environment to install Django, because I don't want my entire machine to install on it.
#### 3. cmd: mkvirtualenv test after you created your environment you can go to your directory and check whether it is created or not under your Cdrive:
<img width="859" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/a6e596b4-d3c0-41c9-b939-3bf4e119de81">
<img width="856" alt="image" src="https://github.com/Vigneswarsiddu/python-django/assets/93468524/8135f03e-be83-4ca7-98d0-7fe2e010535a">


###### 4. Here, I'm giving my virtual environment name as a test
###### 5. If you have already created the virtual environment before you can simply type cmd: C:\Users\lenovo>workon test
###### 6. So, from onwards it uses a test virtual environment to run all your commands. Now, install Django in your virtualenv test cmd: pip install django
  
8.   (test) C:\Users\lenovo>cd projects

(test) C:\Users\lenovo\projects>cd sidtronic

(test) C:\Users\lenovo\projects\sidtronic>dir
 Volume in drive C is Windows
 Volume Serial Number is E473-B7A3

 Directory of C:\Users\lenovo\projects\sidtronic

08/13/2023  01:54 AM    <DIR>          .
08/12/2023  10:55 PM    <DIR>          ..
08/12/2023  11:29 PM           131,072 db.sqlite3
08/13/2023  02:08 AM    <DIR>          demoapp
08/12/2023  10:55 PM               687 manage.py
08/13/2023  01:52 AM    <DIR>          sidtronic
               2 File(s)        131,759 bytes
               4 Dir(s)  61,753,499,648 bytes free
