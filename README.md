# Landing-Page
A simple Django Landing Page for Department of Information Technology.

# Running the site locally

## Requirments

* [Python 3.6.3](https://python.org)
* [Django 2.0.1](https://www.djangoproject.com/)
* [virtualenv](https://virtualenv.pypa.io/en/stable/) or [Virtualenvwrapper](https://virtualenvwrapper.readthedocs.io)

## Installation on Ubuntu

* [Follow the guide here](https://help.github.com/articles/fork-a-repo) on how to clone or fork a repo
* [Follow the guide here](http://simononsoftware.com/virtualenv-tutorial/) on how to create virtualenv

* To create a normal virtualenv (example _myvenv_) and activate it (see Code below).

  ```
  sudo apt-get install python-virtualenv
  
  virtualenv --python=python3.6.3 myvenv
  
  source myvenv/bin/activate

  (myvenv) $ pip install -r django

  (myvenv) $ python manage.py makemigrations

  (myvenv) $ python manage.py migrate

  (myvenv) $ python manage.py runserver
  ```
* Copy the IP address provided once your server has completed building the site. (It will say something like >> Serving at 127.0.0.1....).
* Open the address in the browser
* Don't forget to Change ALLOWED_HOSTS = ['127.0.0.1'] in settings.py
* `Note`: It is important that when you create your virtualenv, do not create it in the same folder as the code you downloaded.

