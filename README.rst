Using this repo as a place to put code for a blog series on learning Salt
Stack. Using Django (since that is what I use it for) project. 

Initially starting out deploying Two Scoops of Django's project layout.
https://github.com/twoscoops/django-twoscoops-project

Will then add support for Postgresql, Memcache, Nginx, and uWSGI.

The block below is a tree output as of 2013/03/12


.. code-block:: shell

    .
    ├── django
    │   ├── init.sls
    │   └── requirements.txt
    ├── minion.conf
    ├── README.rst
    ├── requirements
    │   └── init.sls
    ├── top.sls
    └── Vagrantfile



tree output on 2013/04/17 blog post:
http://www.barrymorrison.com/2013/Apr/21/deploying-django-with-salt-now-with-postgresql/

.. code-block:: shell

    .
    ├── django
    │   ├── base.py
    │   ├── init.sls
    │   └── requirements.txt
    ├── minion.conf
    ├── pillar
    │   ├── settings.sls
    │   └── top.sls
    ├── postgresql
    │   ├── init.sls
    │   └── pg_hba.conf
    ├── README.rst
    ├── requirements
    │   └── init.sls
    ├── top.sls
    └── Vagrantfile

