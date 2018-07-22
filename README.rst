PEP: 9999
Title: Measurement Abbreviations in Numeric Literals
Author: Artyom Gavrichenkov <ximaera@gmail.com>,
        Dmitry Nazarov <mail@nazarov.tech>
Status: Draft
Type: Standards Track
Content-Type: text/x-rst
Created: 22-Jul-2018
Python-Version: 3.8
Post-History: 30-Aug-2002


Abstract
========

TODO


Rationale
=========

TODO


Syntax and semantics
====================

Instead of writing this

    MINUTES = 60
    timeout = 20 * MINUTES

or this

    timeout = 20 * 60  # 20 minutes  

we will write this

    >>> timeout = 20min
    >>> print(timeout)
    1200

This will also work nicely in terms of different units:

    >>> timeout = 5h + 20min
    >>> print(timeout)
    19200

TODO: more measurement abbreviations
TODO: how this will work within string formatting


References
==========

TODO


Copyright
=========

Copyright (c) 2018 by Artyom Gavrichenkov <ximaera@gmail.com>,
Dmitry Nazarov <mail@nazarov.tech>.

This material may be distributed only subject to the terms and conditions
set forth in the Open Publication License, v1.0 or later
(the latest version is presently available
at http://www.opencontent.org/openpub/).


..
   Local Variables:
   mode: indented-text
   indent-tabs-mode: nil
   sentence-end-double-space: t
   fill-column: 70
   coding: utf-8
   End: