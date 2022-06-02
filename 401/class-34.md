# API Deployment

### Django Settings Best Practices

#### Best practices:
- Use environment variables (exclude them from VCSs)
- Write default values for production configuration (ex env variables)

A deployed project typically sees different environments, e.g. dev, staging, and production, each of which require different settings.

Some key considerations to manage these settings include:
- Sensitive data, e.g. SECRET_KEY
- Sharing between team members, e.g. a way to eliminate human error working with settings

There are different approaches to managing settings, each with its pros and cons, for example:

- settings_local.py (ignored by VCSs)
- settings folder with settings files, one for each environment
- environment variables (for sensitive data)

#### Environment variables
Using environment variables seems to be the preferred approach.  To this end, the following libraries help:
- os.environ
- django-environ
- python-decouple
- python-dotenv

For Django, it seems sensible to use django-environ.

### What is SSH?

> SSH, or Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet.

Using encryption, it provides facilitates authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

#### How to use SSH?

Directly form the terminat, use the SSH command:
`ssh {user}@{host}` -'user' is the account you want to access and 'host' is the url.

#### Encryption

Typically, SSH uses a Public Key to authenticate the host.  Then, the two parties use a Key Exchange algorithm to create a symmetrical key.


### WhiteNoise

> Radically simplified static file serving for Python web apps.  A couple of lines of config WhiteNoise allows your web app to serve its own static files; making it a self-contained unit that can be deployed anywhere without relying on nginx, Amazon S3 or any other external service. (Especially useful on Heroku, OpenShift and other PaaS providers.)

---

### Resources

- [Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)
- [SSH Tutorial](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)
- [WhiteNoise](http://whitenoise.evans.io/en/stable/)
- [IaaS](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)
- [PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service)
- [CORS](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)

---

[Back to table of contents](../README.md)
