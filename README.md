=================================================================
QUnit-server
=================================================================

This is slightly modified version of QUnit that can be used along
with JSUnit server to use QUnit with continuous integration 
software like Hudson or Continuum.

If you run your QUnit tests with a querystring argument 
"submitresults=true" then the modified QUnit.js will dynamically 
create and populate a form in the format that is expected by 
JSUnit server and then submit that form to JSUnit server.

Since it is hard to hook into the QUnit.done etc functions I had 
to just bung the changes into the QUnit.js file, which I don't 
really like but it might be helpful for some of you out there.

QUint: http://docs.jquery.com/QUnit

JSUnit: http://www.jsunit.net/


===============================================
License
===============================================

Copyright (c) 2009 Dave Johnson
Licensed under the MIT (MIT-LICENSE.txt)