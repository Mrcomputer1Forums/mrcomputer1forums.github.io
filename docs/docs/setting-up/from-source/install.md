**Setting Up -> From source code**

# Install

In the folder you created in [Setup Django Server](#page=setting-up/from-source/setting-up-django-server)

Download the latest release of Mrcomputer1 Forums from [this](/)

Put the downloaded folder called Forum in your folder

In (projects name)/settings.py find 
```python
INSTALLED_APPS = (
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
)
```
and add
```python
	'Forum',
```
before the )

After STATIC_URL add
```python

STATICFILES_DIRS = (
    os.path.join(BASE_DIR, "static"),
)
```

In (project name)/urls.py change urlpatterns so it looks like this
```python
urlpatterns = [
    url(r'^admin/', include(admin.site.urls)),
    url(r'^$', include('Forum.urls')),
    url(r'^', include('Forum.urls')),
]
```

Then open a command window in the main folder with manage.py and run
```batch
python manage.py migrate
```