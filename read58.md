#  Reading 23: Django Custum User Model:

- A built-in User model for authentication
## Setup steps:
AbstractUser vs AbstractBaseUser:
Two modern ways to create a custom user model in Django: 
1-AbstractUser 
2-AbstractBaseUser.
In both you can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. 

# Custom User Model: 
Creating our initial custom user model requires four steps:

Update config/settings.py
Create a new CustomUser model
Create new UserCreation and UserChangeForm
Update the admin


In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call our custom user model CustomUser.

Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.

        INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'accounts', # new   
        ]

Now update accounts/models.py with a new User model which we'll call CustomUser.

        AUTH_USER_MODEL = 'accounts.CustomUser' # new


        # accounts/models.py
        from django.contrib.auth.models import AbstractUser
        from django.db import models

        class CustomUser(AbstractUser):
        pass
        # add additional fields in here

        def __str__(self):
                return self.username