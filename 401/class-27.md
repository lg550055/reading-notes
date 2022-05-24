# Django Models
> Django web applications access and manage data through Python objects referred to as models.

Models define the structure of stored data, independently of the underlying database.

Once a database is chosen and the model structure and functionality is defined, Django handles communicating with the database.

### Model design
Models are usually defined in the models.py file.  They are implemented as a subclass of `django.db.models.Model`.

- Separate model for each object group
- Use models to represent selection options, which may change over time
- Each field represents a column of data and has a name, type and optionally: size, default value, selection options, help text, label, etc
- Relationships
  - One to one  (OneToOneField)
  - One to many  (ForeignKey)
  - Many to many  (ManyToManyField)
- Models can have methods including `__str__()`, which returns an easy to read string representation of each record, or `get_absolute_url()`, which returns a url for the an idividual record
- Metadata, declared as `class Meta`, is commonly used to control the *ordering* of records returned from a query


### Model management
Create, read, update, or delete records.

- > To create a record you can define an instance of the model and then call save().
- > Search records matching a criteria using the `objects` attribute
- Refine a search with the `filter` method of the `objects` attribute
- To modify or delete records, access them with dot syntax

### Register models with admin

Register each model with the admin module.  Among other things, accessing models via the admin module saves time during development.

##### Create superuser

Create a superuser to manage the admin app and access and manipulate models:  `python3 manage.py createsuperuser`



---

### Resources

- [Django Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- [Django Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)
- [Beginner’s Guide to Django - Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)
- [Beginner’s Guide to Django - Part 2]()

---

[Back to table of contents](../README.md)