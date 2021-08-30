#  Reading 21: Django Models: 

Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms.

The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings.

Model definition
Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

Fields
A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables.

        my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')

Metadata
You can declare model-level metadata for your Model by declaring class Meta:

        class Meta:
        ordering = ['-my_field_name']

# Django Admin

## Creating a superuser: build a site area that you can use to create, view, update, and delete records. 

        python3 manage.py createsuperuser
        python3 manage.py runserver     

## Logging in and using the site: 
- via  /admin URL (e.g. http://127.0.0.1:8000/admin) its possible to login to the site
- You can also directly click the Add link next to each model to start creating a record of that type
- Press SAVE, Save and add another, or Save and continue editing to save the record.