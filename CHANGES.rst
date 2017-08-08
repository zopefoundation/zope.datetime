=========
 CHANGES
=========

4.2.0 (unreleased)
==================

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
