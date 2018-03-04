======
Padova
======

.. image:: https://zenodo.org/badge/10943/jonathansick/padova.svg
    :target: http://dx.doi.org/10.5281/zenodo.16869
    :alt: Digital Object Identifier (DOI)

.. image:: https://img.shields.io/pypi/l/padova.svg
    :target: https://pypi.python.org/pypi/padova/
    :alt: License

.. image:: https://travis-ci.org/jonathansick/padova.svg?branch=master
    :target: https://travis-ci.org/jonathansick/padova

.. image:: https://img.shields.io/pypi/v/padova.svg?label=version
    :target: https://pypi.python.org/pypi/padova/
    :alt: Latest Version

.. image:: https://img.shields.io/pypi/status/padova.svg
    :target: https://pypi.python.org/pypi/padova/
    :alt: Development Status

.. image:: https://img.shields.io/pypi/pyversions/padova.svg
    :target: https://pypi.python.org/pypi/padova/
    :alt: Supported Python versions

.. image:: https://img.shields.io/pypi/format/padova.svg
    :target: https://pypi.python.org/pypi/padova/
    :alt: Download format

Padova is a small python package for working with the so-called `Padova evolutionary tracks <http://stev.oapd.inaf.it/cgi-bin/cmd>`_ produced by Girardi and collaborators.
Padova is compatible with the `Astropy`_ project.

Take a look at this `Jupyter notebook <http://nbviewer.ipython.org/github/jonathansick/padova/blob/master/notebooks/demo.ipynb>`_ to see what Padova can do.

Of course, please use this project *responsibly*.
Don't abuse the CMD servers.


Features
--------

- Simple interfaces to obtain either single isochrones or grids of isochrones.
- Validation of settings before requesting data from the CMD servers.
- Caching of requests so you don't hit the CMD servers when you ask for an isochrone set you already have.
- Isochrones are provided as `Astropy`_ tables with metadata.
- Isochrones can be exported for use with `StarFISH`_.


Installation
------------

    pip install padova


Dependencies
------------

- numpy
- `Astropy`_
- Requests
- pytoml
- setuptools


Tests
-----

Padova uses py.test and tox to run tests. Setup with:

    pip install tox

Then to run the test suite:

    tox


Credits
-------

- Padova provides data from the `CMD web site <http://stev.oapd.inaf.it/cgi-bin/cmd>`_, which is a product of Leo Girardi and collaborators.
- Padova takes inspiration and incorporates code from `ezpadova`_ by Morgan Fouesneau.


Info
----

Copyright 2013-2015 Jonathan Sick (@jonathansick).

Some parts are adapted from `ezpadova`_, Copyright 2015 Morgan Fouesneau.

Padova is MIT licensed.

.. _Astropy: http://www.astropy.org/
.. _ezpadova: https://github.com/mfouesneau/ezpadova
.. _StarFISH: http://www.noao.edu/staff/jharris/SFH/
