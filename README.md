# Catalogs Table - an app for RDMO
This app can be installed next to the rdmo-app and adds a page `/catalogs-table` with an interactive overview of the catalogs in the instance.



## Installation

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
