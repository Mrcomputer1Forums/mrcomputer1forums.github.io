**Setting Up -> From source code**

# Setting up Django Server

Make sure you have [Django](http://djangoproject.com) installed and [Python 3](http://python.org)

Then create an empty folder and type

```batch
django-admin startproject (a name - no spaces) .
```

**Files and folders created**
Note: Some files not included
```
name              <FILE/DIR> file format (file info)

aname             <DIR>      Folder      (Django project folder)
aname/settings.py <FILE>     Python File (Django project settings)
aname/urls.py     <FILE>     Python File (Django project URLs)

manage.py         <FILE>     Python File (Django project command file)

1 Directory
3 Files - 1 in current directory, 2 in "aname" directory
```

**Controls**
Start server with
```batch
python manage.py runserver
```