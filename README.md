<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-timedelta.svg?maxAge=3600)](https://pypi.org/project/django-timedelta/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-timedelta.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-timedelta.py/actions)

### Installation
```bash
$ [sudo] pip install django-timedelta
```

##### `settings.py`
```python
INSTALLED_APPS+=['django_timedelta']
```

#### Examples
```html
{% load timedelta %}

{% if started_at and completed_at %}
    {% timedelta completed_at started_at %}
    {% timedelta completed_at started_at 3 %}
{% endif %}
```

```
0:00:42.123456
```

```html
{% timedelta completed_at started_at 3 %}
```
```
0:00:42.123
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>
