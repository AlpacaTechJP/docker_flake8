flake8
======

python syntax checker


How to use
----------

By default, the docker image will run **flake8** on the `src/` directory (in
the container `/project/src/`).::

    $ docker run -ti -v $(PWD):/project alpacadb/flake8

Pass any arguments that you would like after flake8::

    $ docker run -ti -v $(PWD):/project alpacadb/flake8 --max-complexity 12 coolproject
