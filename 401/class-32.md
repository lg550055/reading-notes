# Django Permissions

## Permissions
Permissions provide the actual authorization to an authenticated user to access a resource.

> Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

> When a permission check fails, either a "403 Forbidden" or a "401 Unauthorized" response will be returned (and the main body of the view will not run).

### Django Rest Frameworw (DRF) Permissions

The DRF allows object-level permissions, but they come with significant limitations; especially when using generic views.

The DRF also allows per-view permission using the APIView class.

### DRF Permissions Policy Implementation

Permissions can be defined in the project's settings.py file, on a class or view function or at the object level, with its notable limitations.

### DRF Generic Views

Developed as a shortcut for common usage patterns, they allow you to quickly buid API views that map closely to your database models.  Examples:

- CreateAPIView -create-only endpoints
- ListAPIView -read-only endpoints to represent a collection of model instances
- RetrieveAPIView -read-only endpoints to represent a single model instance
- DestroyAPIView -delete-only endpoints for a single model instance
- UpdateAPIView -update-only endpoints for a single model instance
- ListCreateAPIView -read-write endpoints to represent a collection of model instances
. . .
- RetrieveUpdateDestroyAPIView -read-write-delete endpoints to represent a single model instance

---

### Resources

- [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
- [Classy Django REST](https://www.cdrf.co/)
- [DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)

---

[Back to table of contents](../README.md)
