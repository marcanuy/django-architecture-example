# django-architecture-example
Django Configuration and environment isolation example

Full explanation at
https://simpleit.rocks/python/django/custom-django-configurations-for-different-servers/


## Notes

To test this setup locally, put the development environment variables
at `myapp/_env` in a dot env file like: `myapp/.env`

In production they should be environment variables, never put them in
a settings file.
