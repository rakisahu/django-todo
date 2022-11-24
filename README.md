# django-todo
A simple todo app built with django

![todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoApp.png)
### Setup
To get this repository, run the following command inside your git enabled terminal
```bash
$ git clone https://github.com/shreys7/django-todo.git 
It would be best practice always, if we create a new enviornment before running the application. 
Before creating a new enviornment check python3 is installed or not and also pip module need to install.
follow the below steps for installing python3, pip module and creating a new environment.
install python 3.9 as per your linux distribution
install pip module (for python3.9)
install virtual enviornment (venv for RHEL & centos)"# pip3.9 install virtualenv"
create a virtual environment # python3 -m venv environmentnameasperyourchoice
                             # python3 -m venv appenv (in may case i created a virtual environment as "appenv")
activate your virtual environment : # source appenv/bin/activate   (virtual environment name as "appenv" followed by /bin/activate)
Now go to the directory django-todo where we need to perform all the tasks.
```
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Once you have downloaded django, go to the cloned repo directory and run the following command

```bash
$ python manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
$ python manage.py migrate
```

One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user
```bash
$ python manage.py createsuperuser
```

That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash
$ python manage.py runserver
```

Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Cheers and Happy Coding :)
