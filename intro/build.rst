Building OCLint
===============

This page presents building OCLint in release mode.

System Requirements
-------------------

#. See `LLVM System Requirements`_
#. `Python`_
#. `Git`_
#. `Apache Subversion`_
#. `CMake`_
#. `OpenSSL`_ (only for analytics-enabled build)

Building OCLint
---------------

The whole build process can be done with the ``make`` script inside ``oclint-scripts`` folder.

#. ``cd oclint-scripts``
#. ``./make``
#. ``cd ..``

Verifying the Build
-------------------

By calling the binary

.. code-block:: bash

    ./build/oclint-<major>.<minor>.dev.<git-hash>/bin/oclint

The following error message is expected::

    oclint: Not enough positional command line arguments specified!
    Must specify at least 1 positional arguments: See: ./oclint -help

It's highly recommended to `add the bin directory into system PATH <installation.html>`_.

.. seealso:: If you are looking for compiling and testing OCLint in debug mode for development and testing purposes, please move onto `development <../devel/index.html>`_ section.

.. _LLVM System Requirements: http://llvm.org/docs/GettingStarted.html#requirements
.. _Apache Subversion: http://subversion.apache.org/
.. _CMake: http://www.cmake.org/
.. _Git: http://git-scm.org/
.. _Python: http://www.python.org/
.. _OpenSSL: https://www.openssl.org/
