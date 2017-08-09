=====
 API
=====

.. currentmodule:: zope.datetime

Parsing Strings
===============

This module defines three functions for parsing strings.

.. autofunction:: parse(string, local=True) -> tuple
.. autofunction:: parseDatetimetz
.. autofunction:: time(string) -> float

The functions :func:`parse` and :func:`time` are both methods of an
instance of the :class:`DateTimeParser` class. This is an immutable,
stateless class.

.. autoclass:: DateTimeParser
   :exclude-members: parse, time

   .. function:: parse(self, string, local=True)

      The same as :func:`parse`.

   .. function:: time(self, string)

      The same as :func:`time`.

Formatting Strings
==================

This module defines a few convenience functions for producing
formatted date strings.

.. autofunction:: iso8601_date
.. autofunction:: rfc850_date
.. autofunction:: rfc1123_date


Exceptions
==========

This module defines an exception tree that it uses to report errors.

.. autoclass:: DateTimeError
.. autoclass:: DateError
.. autoclass:: TimeError
.. autoclass:: SyntaxError
