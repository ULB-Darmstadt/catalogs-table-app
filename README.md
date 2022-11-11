# Catalogs Table - an app for RDMO

An app for the RDMO - Research Data Management Organiser Django project:  
* Home Page
  * https://rdmorganiser.github.io


This app can be installed in the folder of the [rdmo-app](https://github.com/rdmorganiser/rdmo-app) and adds a page `/catalogs-table` with an interactive overview of the catalogs in the instance.


## Installation

Suggested installation from the `<git-repo>` as a git `submodule`.

```
cd rdmo-app
git submodule add catalogs-table <git-repo-url>
git submodule update --remote --init
```

The only external requirement is `django_tables2`.

```bash
# in the python env
python3 -m pip install -r catalogs_table/requirements.txt
```
Add to the `settings.py`
```py
INSTALLED_APPS += ['django_tables2', 'catalogs_table']
```
Add to the `config/urls.py`
```py
urlpatterns = [
    ...
    path('catalogs-table/', include('catalogs_table.urls')),
]
```
