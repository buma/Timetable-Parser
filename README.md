Readme
=============

Application for parsing [FERI Timetable](http://www.feri.uni-mb.si/urniki/groups.asp) and exporting the data as txt, pdf or iCal. 
Original Author is [Tomaž Muraus](http://www.tomaz-muraus.info) I just fixed some encoding and time issues.


Requirements
-----------

* Windows / Linux / Mac
* Python >= 2.6 (< 3.0)
* Python cURL interface - [pycURL](http://pycurl.sourceforge.net/)
* Reportlab PDF library - [reportlab](http://www.reportlab.org/oss/rl-toolkit/download/)
* Python iCalendar library - [VObject](http://vobject.skyhouseconsulting.com/)


Usage
-----

    Usage: python timetable_parser.py [OPTIONS]
    
    Options:
    --programs -> lists available programs
    --branches <program_id> <year> -> lists available branches for specified year and program
    --timetable <txt|pdf|ical> <date> <program_id> <year> <branch_id> -> generates and saves a timetable in specified format for specified year, program and branch

Examples
-------

    python timetable_parser.py --programs
    python timetable_parser.py --branches 21 2 //year is always 2
    python timetable_parser.py --timetable txt 03.10.2012 21 2 127


Bugs
----

PDF output is weird.

