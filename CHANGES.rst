Changes
=======

Version {{UNREALEASED}}
-----------------------

-   Explicitly check if db_session is None in converter (`PR #1`_ from timheap_)
-   Check for ``sqlalchemy.`` prefix to avoid conflicts with modules that start
    with ``sqlalchemy`` (`PR #4`_ from msouth_)
-   Always return model_fields fields in the order requested (`PR #6`_ from
    timheap_)
-   Use SQLAlchemy's Column.doc for WTForm's Field.description (`PR #10`_ from
    timheap_)
-   Do not assume not-nullable means Required for Boolean columns (`PR #9`_ from
    timheap_)

.. _PR #1: https://github.com/mlenzen/wtforms-sqlalchemy/pull/1
.. _timheap: https://github.com/timheap
.. _PR #4: https://github.com/mlenzen/wtforms-sqlalchemy/pull/4
.. _msouth: https://github.com/msouth
.. _PR #6: https://github.com/mlenzen/wtforms-sqlalchemy/pull/6
.. _PR #9: https://github.com/mlenzen/wtforms-sqlalchemy/pull/9
.. _PR #10: https://github.com/mlenzen/wtforms-sqlalchemy/pull/10

Version 0.2
-----------

Released on October 16, 2019

-   Fork the irregularly maintained WTForms-SQLAlchemy
-   Auto-generated ``DecimalField`` does not limit places for ``Float``
    columns. (`#2`_)
-   Add an example of using this library with Flask-SQAlchemy. (`#3`_)
-   Generating a form from a model copies any lists of validators
    passed in ``field_args`` to prevent modifying a shared value across
    forms. (`#5`_)
-   Don't add a ``Length`` validator when the column's length is not an
    int. (`#6`_)
-   Add ``QueryRadioField``, like ``QuerySelectField`` except
    it renders a list of radio fields. Add ``QueryCheckboxField``, like
    ``QuerySelectMultipleField`` except it renders a list of checkbox
    fields. (`#8`_)
-   Fix a compatibility issue with SQLAlchemy 2.1 that caused
    ``QuerySelectField`` to fail with a ``ValueError``. (`#9`_, `#10`_,
    `#11`_)
-   ``QuerySelectField.query`` allows no results. (`#15`_)

.. _#2: https://github.com/wtforms/wtforms-sqlalchemy/pull/2
.. _#3: https://github.com/wtforms/wtforms-sqlalchemy/pull/3
.. _#5: https://github.com/wtforms/wtforms-sqlalchemy/pull/5
.. _#6: https://github.com/wtforms/wtforms-sqlalchemy/pull/6
.. _#8: https://github.com/wtforms/wtforms-sqlalchemy/pull/8
.. _#9: https://github.com/wtforms/wtforms-sqlalchemy/issues/9
.. _#10: https://github.com/wtforms/wtforms-sqlalchemy/pull/10
.. _#11: https://github.com/wtforms/wtforms-sqlalchemy/pull/11
.. _#15: https://github.com/wtforms/wtforms-sqlalchemy/pull/15


Version 0.1
-----------

Released on January 18th, 2015

-   Initial release, extracted from WTForms 2.1.
