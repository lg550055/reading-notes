# Django REST Framework & Docker


### Beginner’s Guide to Docker

Docker is a way to isolate and run applications using Linux containers, a.k.a. containerization.

Linux containers are a form of virtualization.

Containerization is lighter weight than traditional virtualization, which virutalizes the whole machine and requires a copy of the operating system.  In contrast, containerization shares the operating system.

##### No need for a virtual environment
Docker eliminates the need for virtual environments. It allows reproducing a production environment locally.

#### Side note
> Virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

#### Images and containers

- An image is a snapshot in time of what a project contains
- A container is a running instance of the image.

> There are a large number of official images available on Docker Hub for common software like programming languages.

But typically we will create custom images using a `Dockerfile`. And use docker-compose.yml files to run the container.

> `Dockerfile` is a list of instructions for creating an image

##### Image layers

An image is made up of one or more image layers.  For example, the first layer might be a Linux version and the second a version of a programming language...

Each image layer is immutable.  Which helps collaboration and performance.

Order matters in a Dockerfile.  Thus, put code that won’t change often at the top and code that will change at the end.

### Django for APIs

> Django REST Framework works alongside the Django web framework (i.e. regular Django) to create web APIs. We cannot build a web API with only Django Rest Framework. It always must be added to a project after Django itself has been installed and configured.

The Django REST Framework creates web APIs which are a collection of URL endpoints that return JSON and HTTP verbs.

> Many professional Django developers include API logic in the related app and put URLs under an /api/ prefix.

##### Django REST views

> Django REST Framework views are similar to regular Django views except the end result is serialized data in JSON format.  Django REST Framework views rely on a model, a URL, and a serializer.

> There are generic Django REST Framework views for common use cases, e.g. ListAPIView.

##### Serializer

A serializer translates data like querysets and model instances into a format that is easy to consume over the internet, typically JSON.

> The real beauty of Django REST Framework lies in its serializers which abstracts away most of the complexity for us.

#### Testing

> Django comes with a test client that we can use to simulate GET or POST requests and other functionality.

> Django REST Framework provides several additional helper classes that extend Django’s existing test framework. One of these is APIClient, which can be used to test retrieving API data from the database.

---

### Resources

- [Beginner’s Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)
- [Django for APIs](https://djangoforapis.com/library-website-and-api/)
- [Beginner’s Guide to Django REST Framework](https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners)

---

[Back to table of contents](../README.md)
