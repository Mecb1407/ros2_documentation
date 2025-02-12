:orphan:

.. redirect-from::

    RQt-Source-Install-MacOS
    Guides/RQt-Source-Install-MacOS

<<<<<<< HEAD:source/How-To-Guides/RQt-Source-Install-MacOS.rst
Building RQt from source on macOS
=================================

This page provides specific information to building RQt from source on macOS.
Follow these instructions before proceeding with :doc:`RQt Source Install <RQt-Source-Install>` page.

System Requirements
-------------------

RQt is supported on macOS 10.12, but 10.13 also seems to work.

Dependencies
------------

The primary dependencies of the RQt package are sip and PyQt5.
PySide2 may be supported in the future.

Install dependencies
^^^^^^^^^^^^^^^^^^^^

.. code-block:: bash

     $ brew install sip pyqt5
     $ brew install graphviz
     $ python3 -m pip install pygraphviz pydot
     $ brew link --force qt

This is the quickest solution but may cause issues when upgrading Qt or if other packages are expecting Qt 4.
Another option is to update your ``PATH`` and ``CMAKE_PREFIX_PATH`` to include the Qt install location:

  .. code-block:: bash

     $ export PATH="$(brew --prefix qt)/bin:$PATH"
     $ export CMAKE_PREFIX_PATH="$(brew --prefix qt):$CMAKE_PREFIX_PATH"

Install RQt by source
---------------------

Continue with the :doc:`RQt source install page <RQt-Source-Install>`.
=======
The files on this branch are no longer used.  See the 'rolling' branch instead.
>>>>>>> 5884b736042684e34db58d74fabbabd321bdfafa:source/Tutorials/RQt-Source-Install-MacOS.rst
