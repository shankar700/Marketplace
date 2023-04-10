# Work Tracker
>To *Track* each and every step and its significance


## Step 1: Setting Up

1. Create a Virtual Enviroment
>`python3 -m venv django_env` django_env is the name of the environment

2. Activate the Virtual Env
>`source django_env/bin/activate`

3. Install Django
>`pip3 install Django`

4. Initialize a *new* Django project
>`django-admin startproject marketplace` - cmd to intialize a new Django project

## Step 2: Creating an App

1. Initialize an App through cmd line
>`python manage.py startapp core` - It will initialize an app named **core**

2. After the app is initialized add it to the ***Installed Apps*** list in *marketplace /marketplace/settings.py*

3. Create Index View in the views.py file in core app folder
```
def index(request):
    return render(request, 'core/index.html')
```

4. Create the corresponding view template core/index.html
    - create a folder called ***templates*** , this is the folder Django looks for to render templates
    - inside it create a folder ***core***
    - inside that folder create the ***index.html*** 
