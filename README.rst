================
Config Templater
================


.. image:: https://img.shields.io/pypi/v/config_templater.svg
        :target: https://pypi.python.org/pypi/config_templater

.. image:: https://img.shields.io/travis/squ4rks/config_templater.svg
        :target: https://travis-ci.org/squ4rks/config_templater

.. image:: https://readthedocs.org/projects/config-templater/badge/?version=latest
        :target: https://config-templater.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status




Simple python module to generate configurations from templates


* Free software: MIT license

Usage
-----

You should run this script as a module. Executing in a directory will recursively parse the entire
directory for `.conftpl` files and replace the jinja2 variables included with the corresponding 
environment variables.

Example
-------

Given a configuration template file *test.yml.conftpl* like this: 

.. code-blcok:: 
        
        ---
        access_token: {{ API_ACCESS_TOKEN }}
        data_url: {{ DATA_URL }}


Credits
-------

This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
