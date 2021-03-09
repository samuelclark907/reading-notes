## Django Best Practices: Custom User Model

- There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work.

### Setup

- To start, create a new Django project from the command line. We need to do several things:

1. create and navigate into a dedicated directory called accounts for our code
2. install Django
3. make a new Django project called config
4. make a new app accounts
5. start the local web server

### Custom User Model

- Creating our initial custom user model requires four steps:

1. update config/settings.py
2. create a new CustomUser model
3. create new UserCreation and UserChangeForm
4. update the admin