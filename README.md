# django-architecture-example
Django Configuration and environment isolation example

Full explanation at
https://simpleit.rocks/python/django/custom-django-configurations-for-different-servers/

## Directory tree

~~~
.
├── _env
├── Makefile
├── manage.py
├── myapp
│   ├── __init__.py
│   ├── settings
│   │   ├── base.py
│   │   ├── __init__.py
│   │   ├── local.py
│   │   ├── production.py
│   │   ├── staging.py
│   │   └── testing.py
│   ├── urls.py
│   └── wsgi.py
├── requirements
│   ├── base.txt
│   ├── dev.txt
│   └── production.txt
└── requirements.txt
~~~

## Notes

To test this setup locally, put the development environment variables
at `myapp/_env` in a dot env file like: `myapp/.env`

In production they should be environment variables, never put them in
a settings file.
