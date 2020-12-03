console-messenger
=================

| |Downloads|
| |Downloads/Week|
| |Downloads/Month|
| |MIT License|
| |Latest PyPI version|
| |Supported Python versions|

About
-----

This package displays success, warning and info messages and errors on
console with different colours using
`rich <https://pypi.org/project/rich/>`__ module. It also prints any
error type without passing it as a parameter.

Requirements
------------

.. code:: shell

     python>=3.0

Dependencies
------------

.. code:: shell

     rich>=9.0.0

Installation
------------

.. code:: shell

     pip install console-messenger

Usage
-----

.. code:: python

     >>> from ConsoleMessenger import ConsoleMessage
     >>> console = ConsoleMessage()

**Print an error**

.. code:: python

     try:
         a = 5/0
     except Exception as e:
         console.danger(e)

Output :-

|Broken Image|

**Display a custom error**

.. code:: python

     console.danger("this is a custom error", err_type="My Error")

Output :-

|Broken Image|

**Print a success message**

.. code:: python

     console.success("Success", "success method worked!")

Output :-

|Broken Image|

**Display a warning**

.. code:: python

     console.warning("Warning", "You are using pip version 20.2.4; however, version 20.3 is available.")

Output :-

|Broken Image|

**Display a info message**

.. code:: python

     console.info("INFO", "Hello User!")

Output :-

|Broken Image|

**Display a dark message**

.. code:: python

     console.dark("Dark", "This is a dark message!")

Output :-

|Broken Image|

.. |Downloads| image:: https://static.pepy.tech/personalized-badge/console-messenger?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads
   :target: https://pepy.tech/project/console-messenger
.. |Downloads/Week| image:: https://static.pepy.tech/personalized-badge/console-messenger?period=week&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week
   :target: https://pepy.tech/project/console-messenger
.. |Downloads/Month| image:: https://static.pepy.tech/personalized-badge/console-messenger?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/Month
   :target: https://pepy.tech/project/console-messenger
.. |MIT License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
   :target: https://opensource.org/licenses/MIT
.. |Latest PyPI version| image:: https://img.shields.io/pypi/v/console-messenger.svg
   :target: https://pypi.org/project/console-messenger
.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/console-messenger.svg
   :target: https://pypi.org/project/console-messenger
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img.png
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img1.png
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img2.png
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img3.png
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img4.png
.. |Broken Image| image:: https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img5.png
