
#The Flask Mega-Tutorial, Part I: Hello, World!

#https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world

#Flask
Flask is a microframework for Python based on Werkzeug, Jinja 2 and good intentions. And before you ask: It's BSD licensed!
http://flask.pocoo.org/

#Installing Flask
Okay, let's get started!

If you haven't yet, go ahead and install Python.

Now we have to install Flask and several extensions that we will be using. My preferred way to do this is to create a virtual environment where everything gets installed, so that your main Python installation is not affected. As an added benefit, you won't need root access to do the installation in this way.

So, open up a terminal window, choose a location where you want your application to live and create a new folder there to contain it. Let's call the application folder microblog.

If you are using Python 3, then cd into the microblog folder and then create a virtual environment with the following command:

$ python -m venv flask
Note that in some operating systems you may need to use python3 instead of python. The above command creates a private version of your Python interpreter inside a folder named flask.

If you are using any other version of Python older than 3.4, then you need to download and install virtualenv.py before you can create a virtual environment. If you are on Mac OS X, then you can install it with the following command:

$ sudo easy_install virtualenv
On Linux you likely have a package for your distribution. For example, if you use Ubuntu:

$ sudo apt-get install python-virtualenv
Windows users have the most difficulty in installing virtualenv, so if you want to avoid the trouble then install Python 3. If you want to install virtualenv on Windows then the easiest way is by installing pip first, as explaned in this page. Once pip is installed, the following command installsvirtualenv`:

$ pip install virtualenv
We've seen above how to create a virtual environment in Python 3. For older versions of Python that have been expanded with virtualenv, the command that creates a virtual environment is the following:

$ virtualenv flask
Regardless of the method you use to create the virtual environment, you will end up with a folder named flask that contains a complete Python environment ready to be used for this project.

Virtual environments can be activated and deactivated, if desired. An activated environment adds the location of its bin folder to the system path, so that for example, when you type python you get the environment's version and not the system's one. But activating a virtual environment is not necessary, it is equally effective to invoke the interpreter by specifying its pathname.

If you are on Linux, OS X or Cygwin, install flask and extensions by entering the following commands, one after another:

$ flask/bin/pip install flask
$ flask/bin/pip install flask-login
$ flask/bin/pip install flask-openid
$ flask/bin/pip install flask-mail
$ flask/bin/pip install flask-sqlalchemy
$ flask/bin/pip install sqlalchemy-migrate
$ flask/bin/pip install flask-whooshalchemy
$ flask/bin/pip install flask-wtf
$ flask/bin/pip install flask-babel
$ flask/bin/pip install guess_language
$ flask/bin/pip install flipflop
$ flask/bin/pip install coverage
