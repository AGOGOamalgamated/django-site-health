# django-health
Configurable health endpoint for applications hosted in ElasticBeanstalk.

## Installation

* Download this repo locally

* Run the install

```bash
python setup.py install
```

## Quick Start

* Add `django-health` to your `INSTALLED_APPS`

```python
INSTALLED_APPS = [
    ...
    'django_health',
]
```

* Include the `django-health` URLconf in your project urls.py

```python
    url(r'^health/', include('django_health.urls')),
```

* Test that you can access the `/health/` on the dev server
