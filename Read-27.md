## Django Models
- Django web applications access and manage data through Python objects referred to as models. 
- Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc. 
- Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata
- A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables
    - CharField is used to define short-to-mid sized fixed-length strings. 
    - TextField is used for large arbitrary-length strings. You may specify a max_length for the field, but this is used only when the field is displayed in forms (it is not enforced at the database level).
    - IntegerField is a field for storing integer (whole number) values, and for validating entered values as integers in forms.
    - DateField and DateTimeField are used for storing/representing dates and date/time information (as Python datetime.date in and datetime.datetime objects, respectively). These fields can additionally declare the (mutually exclusive) parameters auto_now=True (to set the field to the current date every time the model is saved), auto_now_add (to only set the date when the model is first created) , and default (to set a default date that can be overridden by the user).
    - EmailField is used to store and validate email addresses.
    - FileField and ImageField are used to upload files and images respectively (the ImageField simply adds additional validation that the uploaded file is an image). These have parameters to define how and where the uploaded files are stored.
    - AutoField is a special type of IntegerField that automatically increments. A primary key of this type is automatically added to your model if you don’t explicitly specify one.
    - ForeignKey is used to specify a one-to-many relationship to another database model (e.g. a car has one manufacturer, but a manufacturer can make many cars). The "one" side of the relationship is the model that contains the "key" (models containing a "foreign key" referring to that "key", are on the "many" side of such a relationship).
    - ManyToManyField is used to specify a many-to-many relationship (e.g. a book can have several genres, and each genre can contain several books).

- A model can also have methods.

## Django Admin
- The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. 
- You can create a "superuser" account that has full access to the site and all needed permissions using manage.py.
- To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) and enter your new superuser userid and password credentials 