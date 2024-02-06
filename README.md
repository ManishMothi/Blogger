## Blogger Web Application

Create a virtualenv and activate it::

    $ python3 -m venv .venv
    $ . .venv/bin/activate

Or on Windows cmd::

    $ py -3 -m venv .venv
    $ .venv\Scripts\activate.bat

## Run

.. code-block:: text

    $ blogger --app blogger init-db
    $ blogger --app blogger run --debug

Open http://127.0.0.1:5000 in a browser.

## Test

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser
