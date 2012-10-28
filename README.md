DJANGO APPENGINE EMPTY TEMPLATE
===============================


About
----

This is an empty template project for quickly creating a new application based on [django-nonrel][1] and [djangoappengine][2]

**REQUIREMENTS**

	+ [Python ver. 2.7](http://www.python.org/download/releases/2.7/)
	+ [Git](https://github.com/)
	+ [Mercurial](http://mercurial.selenic.com)


Installation and usage
----------------------

Create a directory for your project:

' % mkdir my-project '
' % cd my-project '

Clone the repository:

' % git clone git://github.com/samuele-mattiuzzo/django-appengine-template-app.git '

Now we need to download all the required libraries.
There's a script provided inside *srv* folder:

' % cd srv '
' % python align_libs.py '

This script downloads for you (either with git or hg): 

	+ [django-nonrel][1] 
	+ [djangoappengine][2] 
	+ [django-toolbox][3] 
	+ [django-autoload][4] 
	+ [django-dbindexer][5]

then copies the modules inside your project root folder.

**NOTE**: make sure you have python, git and mercurial installed before running this script.


What to do next?
----------------

After the setup is complete, go back to your project folder and create a new app:

' % python manage.py startapp appname '

You also have to edit *app.yaml* file, and change the application name accordingly to your needs.

*THERE YOU GO!* you can now develop your djangoappengine-based app as you prefer. There's no need to use the *dev_appserver.py* command, you can run your webserver
with django's classic *manage.py*

' % python manage.py runserver '

If everything went fine, open a browser and head over to *http://localhost:8000/* to see your first **It Works!** screen.
On newly generated page, you'll find useful links about django-nonrel and appengine.

[1]: https://github.com/django-nonrel/	"Django-nonrel"
[2]: https://github.com/djangoappengine/	"Djangoappengine"
[3]: https://github.com/django-nonrel/djangotoolbox/	"Django-toolbox"
[4]: http://bitbucket.org/twanschik/django-autoload/	"Django-autoload"
[4]: https://github.com/django-nonrel/django-dbindexer/	"Django-dbindexer"
