# Authentication & Production Server

Tokens allow to verify information without accessing a database.

## JSON Web Tokens
### Intro to JSON Web Tokens

JSON Web Token (JWT) is an open standard for securely transmitting information (including authorization) between parties as a JSON object.

> This information can be verified and trusted because it is digitally signed.  Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties.

> When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

A JSON Web Token has three parts separated by a dot ( . ):
`header.payload.signature`, each of which is a Base64-URL string.

### DRF JWT Authentication

The JWT, which should be included in all requests, is acquired by exchanging an username & password.  Actually, bot an access token and a refresh token are aquired.

The DRF recommends using the 'djangorestframework_simplejwt' library.

The code to implement this library is not too complicated.  Just needs to be included in all the right files, e.g. settings.py, urls.py, and views.py.


### Django Runserver Is Not Your Production Server

The docs emphatically ask to not use `runserver` for production because it may be slow and unreliable:

> DO NOT USE THIS SERVER IN A PRODUCTION SETTING. It has not gone through security audits or performance tests.

**Use a dedicated web server like Nginx in combination with an app server like Gunicorn.**

---

### Resources

- [JSON Web Tokens](https://jwt.io/introduction/)
- [DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)
- [JWT with DRF video](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)
- [Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)
- [Gunicorn](https://gunicorn.org/)
- [Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)

---

[Back to table of contents](../README.md)
