blob_utils
==========

File management utils for the curator core project.

Quick start
===========

1. Add "blob_utils" to your INSTALLED_APPS setting
--------------------------------------------------

.. code:: python

    INSTALLED_APPS = [
        ...
        'blob_utils',
    ]

Tests
=====

This set of test is particular since GridFS cannot be mocked and has to be run on a live database. The following steps
guide you through the process:

* Start MongoDb
* Set MONGODB_URI in tests/test_settings.py
* Run the tests with :code:`python runtests.py`