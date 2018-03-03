=======
jinjafy
=======
Render a Jinja2 template from the commandline, writing it to stdout.

Install
-------
Run ``pip install jinjafy`` to install the ``jinjafy`` command line tool.


Usage
--------
::

    $ jinjafy --help
    usage: jinjafy [-h] [-v] filepath [key=value [key=value ...]]
    ...
    $ cat ru.j2
    Ben De La {{creme}}
    $ jinjafy ru.j2 creme=Christ
    Ben De La Christ
    $ jinjafy ru.j2 creme="Christ, Series Winner" # Quote spaces to include them in values
    Ben De La Christ, Series Winner

Development
-----------
This project uses [`Pipenv`](docs.pipenv.org) to isolate development environments. To test::

    $ pipenv shell
    pytest


License
-------
`MIT <LICENSE>`_
