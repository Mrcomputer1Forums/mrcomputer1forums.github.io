**Setting Up -> Heroku**

# Extra stuff

## Changing the config file

Create a empty folder and do the following commands

**Requires heroku and git command**

```batch
git init
heroku git:remote --app=(app name)
git pull heroku master
```

Change the config file (see [this](#page=setting-up/from-source/config) for more)

Then do this

```batch
git commit -am "Commit"
git push heroku master
```