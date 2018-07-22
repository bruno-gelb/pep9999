| PEP: 9999  
| Title: Measurement Abbreviations in Numeric Literals  
| Author: Artyom Gavrichenkov <ximaera@gmail.com>,  
| Dmitry Nazarov <mail@nazarov.tech>  
| Status: Draft  
| Type: Standards Track  
| Content-Type: text/x-rst  
| Created: 22-Jul-2018  
| Python-Version: 3.8  
| Post-History: 30-Aug-2002  


Abstract  
========  

TODO  


Rationale  
=========  

TODO  


Syntax and semantics  
====================  

Instead of writing this::  

    MINUTES = 60  
    timeout = 20 * MINUTES  

or this::  

    timeout = 20 * 60  # 20 minutes  

we will write this:: 

    >>> timeout = 20 min  
    >>> print(timeout)  
    1200  

This will also work nicely in terms of different units::  

    >>> timeout = 5 h + 20 min  
    >>> print(timeout)  
    19200  


More examples::  

    connect(buffer = 4K, ..)  #  4096  
    sleep(1 min)              #    60  
    TOKEN_TTL = 8h            # 28800  
    MAX_WEIGHT = 7.5 kg       #  7500  


| TODO: more real world examples
| TODO: how this will work within string formatting  


References  
==========  

.. [1] Proof of concept implementation  
   (https://github.com/nazarov-tech/cpython/tree/measurement-abbreviations)  


Copyright  
=========  

| Copyright (c) 2018 by Artyom Gavrichenkov <ximaera@gmail.com>,  
| Dmitry Nazarov <mail@nazarov.tech>.  

| This material may be distributed only subject to the terms and conditions  
| set forth in the Open Publication License, v1.0 or later  
| (the latest version is presently available  
| at http://www.opencontent.org/openpub/).  


..
   Local Variables:  
   mode: indented-text  
   indent-tabs-mode: nil  
   sentence-end-double-space: t  
   fill-column: 70  
   coding: utf-8  
   End:  