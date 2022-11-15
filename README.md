# Catalogs Table - an app for RDMO

An app for the [RDMO - Research Data Management Organiser](https://rdmorganiser.github.io) Django project.

Made for the Issue (https://github.com/rdmorganiser/rdmo/issues/448) and developed in PR (https://github.com/rdmorganiser/rdmo/pull/482).

This app can be installed in the folder of the [rdmo-app](https://github.com/rdmorganiser/rdmo-app) and adds a page `/catalogs-table` with an interactive overview of the catalogs in the instance.


<details>
  <summary>Screenshot</summary>
  
  ![Catalog-Table](https://user-images.githubusercontent.com/13996213/201897504-6483dde5-b0f6-46f0-b4ae-8bfde7f5e9e1.PNG)
  
</details>

## Installation

Suggested installation from the `<git-repo-url>` as a git `submodule`.

```
cd rdmo-app
git submodule add <git-repo-url> catalogs_table_app
```

The only external requirement is `django_tables2`.

```bash
# in the python env
python3 -m pip install -r catalogs_table_app/requirements.txt
```
Add to the `settings.py`
```py
INSTALLED_APPS += ['django_tables2', 'catalogs_table_app']
```
Add to the `config/urls.py`
```py
urlpatterns = [
    ...
    path('catalogs-table/', include('catalogs_table_app.urls')),
]
```
