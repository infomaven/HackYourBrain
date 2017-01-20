# HackYourBrain
An app that uses pictures of food to train your brain to have negative associations with junk food. 
For the We Code Hackathon 2016

## Installation
Install Python 2.7
* clone the project
* cd into the project directory

```
pip install virtualenv
```
```
virtualenv env
```
### On Mac:
```
source env/bin/activate
```
### On Windows:
```
source env\Scripts\activate 
```

Make sure there is a little (env) in front of your prompt before running this> 
```
pip install django && pip install pillow
```

Change to braintrainer directory and run the following: 

```
python manage.py makemigrations trainer && python manage.py migrate
```

```
python manage.py ls
```

If you get an error like this:
    __import__(name)
ImportError: No module named PIL
Verify  you are running pip version of at least 8.x. Then  run the following:

```
pip install image
```

### Create an admin:
```
python manage.py createsuperuser
```
ex.
username: admin,
email: admin@example.com (optional),
password: 12.345678Jj

### Command to START app server
```
python manage.py runserver
```

### Command to STOP app server
```
CTRL-C
```

### Command to stop VIRTUALENV
```
deactivate
```



## Usage 
Browse to [http://localhost:8000/admin/](http://localhost:8000/admin/) and login 

#### First time only
Use the admin page to upload images from your local machine. Also load models.

Then go to [http://localhost:8000/](http://localhost:8000/)
