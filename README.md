
# contactform

#helplink : http://sayhelloworld.co/how-to-deploy-django-project-to-heroku/
this is a simple django project that sends mail to EMAIL_HOST_USER. besides that we have some files changed or added through adding this project to heroku.
these files are runtime.txt which consist the verion of python that you use, requirements.txt that has been made by pip freeze , Procfile which is neccessary to heroku and the spaces are important in this file , .gitignore states that which files should not added to heroku, the last file is settings.py and heroku settings are defined at the end of this file . another thing is ALLOWED_HOSTS vaiable in this file and we should add some hosts.
then we need to add a midleware "whitenoise" and its place is right after security middleware . at the end after creating app on heroku go to the settings and add a python buildpack in the bulidpack components.static files are needed when you want to deploy on heroku.
