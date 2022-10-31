### Catalogs table - an app for rdmo

This app adds a page with the an overview of the catalogs in an instance.
An extra dependency is `django-tables2` for rendering the html table. 
The front-end interactive elements are made with `htmx`.

``` python
# add these apps to the rdmo-app INSTALLED_APPS in settings
INSTALLED_APPS += ['django_tables2']
INSTALLED_APPS += ['catalogs_table']
```


An app for RDMO - Research Data Management Organiser
=========================================

RDMO is a tool to support the systematic planning, organisation and implementation of the data management throughout the course of a research project. RDMO is funded by the Deutsche Forschungsgemeinschaft (DFG).

<dl>
  <dt>Home Page</dt>
  <dd><a href="https://rdmorganiser.github.io">https://rdmorganiser.github.io</a></dd>
  <dt>Source code</dt>
  <dd><a href="https://github.com/rdmorganiser/rdmo">https://github.com/rdmorganiser/rdmo</a></dd>
  <dt>Documentation</dt>
  <dd><a href="http://rdmo.readthedocs.io">http://rdmo.readthedocs.io</a></dd>
  <dt>Demo</dt>
  <dd><a href="https://rdmo.aip.de">https://rdmo.aip.de</a></dd>
</dl>

This repository contains the `rdmo-app`, to be forked and used together with `rdmo`.
