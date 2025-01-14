===================
django-adminfilters
===================

Collection of extra filters for the Django admin site


.. image:: https://travis-ci.org/saxix/django-adminfilters.svg?branch=develop
    :target: https://travis-ci.org/saxix/django-adminfilters

.. image:: https://codecov.io/github/saxix/django-adminfilters/coverage.svg?branch=develop
    :target: https://codecov.io/github/saxix/django-adminfilters?branch=develop

.. image:: https://badges.gitter.im/saxix/django-adminfilters.svg
    :target: https://gitter.im/saxix/django-adminfilters?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge


Filters
=======

* AutocompleteFilter
* AllValuesComboFilter
* AllValuesRadioFilter
* RelatedFieldComboFilter
* RelatedFieldRadioFilter
* RelatedFieldCheckBoxFilter
* StartWithFilter
* PermissionPrefixFilter
* MultipleSelectFieldListFilter
* IntersectionFieldListFilter
* UnionFieldListFilter
* ForeignKeyFieldFilter


Usage examples
==============

.. code-block:: python

    class UserAdmin(ModelAdmin):
        list_filter = (TextFieldFilter.factory('name__istartswith'),)



Run demo app
============

.. code-block:: bash

    $ git checkout https://github.com/saxix/django-adminfilters.git
    $ cd django-adminfilters
    $ make develop
    $ make demo


Project links
-------------

* Project home page: https://github.com/saxix/django-adminfilters
* Download: http://pypi.python.org/pypi/django-adminfilters/
