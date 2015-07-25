flake8
======

.. image:: https://badges.gitter.im/Join%20Chat.svg
   :alt: Join the chat at https://gitter.im/AlpacaDB/docker_flake8
   :target: https://gitter.im/AlpacaDB/docker_flake8?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

python syntax checker


How to use
----------

By default, the docker image will run **flake8** on the `src/` directory (in
the container `/project/src/`).::

    $ docker run -ti -v $(pwd):/project alpacadb/flake8

Pass any arguments that you would like after flake8::

    $ docker run -ti -v $(pwd):/project alpacadb/flake8 --max-complexity 12 coolproject
