=========
 CHANGES
=========

6.0 (2025-09-12)
================

- Replace ``pkg_resources`` namespace with PEP 420 native namespace.


5.1 (2025-02-14)
================

- Add support for Python 3.12, 3.13.

- Drop support for Python 3.7, 3.8.


5.0.0 (2023-04-25)
==================

- Drop support for Python 2.7, 3.5, 3.6.

- Add support for Python 3.10, 3.11.


4.3.0 (2021-02-26)
==================

- Drop support for Python 3.4.

- Add support for Python 3.7, 3.8 and 3.9.

- Prevent a ``DeprecationWarning`` in Python 3.8+ when using a parameter for
  ``iso8601_date``, ``rfc850_date``, or ``rfc1123_date`` which has to be
  converted via its ``__int__`` method.


4.2.0 (2017-08-14)
==================

- Remove support for guessing the timezone name when a timestamp
  exceeds the value supported by Python's ``localtime`` function. On
  platforms with a 32-bit ``time_t``, this would involve parsed values
  that do not specify a timezone and are past the year 2038. Now the
  underlying exception will be propagated. Previously an undocumented
  heuristic was used. This is not expected to be a common issue;
  Windows, as one example, always uses a 64-bit ``time_t``, even on
  32-bit platforms. See
  https://github.com/zopefoundation/zope.datetime/issues/4

- Use true division on Python 2 to match Python 3, in case certain
  parameters turn out to be integers instead of floating point values.
  This is not expected to be user-visible, but it can arise in
  artificial tests of internal functions.

- Add support for Python 3.5 and 3.6.

- Drop support for Python 2.6, 3.2 and 3.3.


4.1.0 (2014-12-26)
==================

- Add support for PyPy and PyPy3.

- Add support for Python 3.4.

- Add support for testing on Travis.


4.0.0 (2013-02-19)
==================

- Add support for Python 3.2 and 3.3.

- Drop support for Python 2.4 and 2.5.


3.4.1 (2011-11-29)
==================

- Add test cases from LP #139360 (all passed without modification to
  the ``parse`` function).

- Remove unneeded ``zope.testing`` dependency.


3.4.0 (2007-07-20)
==================

- Initial release as a separate project.
