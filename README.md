# djangocms-rosetta

A little helper module for translating text.

Adds a menu in the Django CMS Toolbar that links to the admin of the
translations module [django-rosetta by Marco Bonetti](https://github.com/mbi/django-rosetta).

Code hosted [on github](https://github.com/philippze/djangocms-rosetta).


## Requirements

- Django>=1.7
- django-cms>=3.1
- django-rosetta>=0.7

It might also work with elder versions, but I havn't tested this (yet).


## Installation

This module requires a working `django-cms` installation.

To install it two things are necessary:

1. Install with pip:  
   `pip install djangocms-rosetta`
2. Add `djancocms_rosetta` and `rosetta` to your `INSTALLED_APPS`.
3. Include the required urls in your urlconf:  
   `url(r'^rosetta/', include('rosetta.urls'))`
4. Create translation files for *all* languages used in your project:  
   `python manage.py makemessages -l en`  
   ...


## Configuration and more info

The [django-rosetta docs](http://django-rosetta.readthedocs.org)
provide some more information about possible configurations and what
rosetta does.


## Questions

This module is tiny and new and published hoping it might be useful for anyone.

If it doesn't work as you expect, please create an issue on github.


## Author

Philipp Zedler  
[philipp@neue-musik.com](mailto:philipp@neue-musik.com)  
[www.zedler.it](http://www.zedler.it)
