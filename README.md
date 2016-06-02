# Log4d-for-Delphi

This project contains files from the Log4D project with fixes to support newer Delphi versions and Free Pascal.

Log4D is a port of the well known log4j logging framework. You can find the original Log4D project at http://sourceforge.net/projects/log4d/

## What's New ##

### Parameterized Logging ###

It supports now an advanced feature called 'parameterized logging', which can 
significantly boost logging performance for disabled logging statement. If the 
current log level is lower than the global log level, log message will not be 
concatenated.                                                 

 * Using original Log4D: <code>LOG.Debug(Format('Invalid value %s' [Value]));</code>
 * Now: <code>LOG.Debug('Invalid value %s', [Value]);</code>
