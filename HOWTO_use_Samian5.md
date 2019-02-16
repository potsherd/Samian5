
How to use the Samian5 font
===========================

The Samian5 font is intended to display the terra sigillata stamp readings.
The surrounding 'normal' text of the catalogue should be in some standard font,
such as 'Times New Roman' or 'Helvetica'.  This is how the published volumes of
the Index are formatted and that is how it is intended to be used.

To format a reading to use the Samian5 font, highlight the reading in the text
and switch the font to Samian5 in one of the boxes in the tool bar.  If Samian5
does not appear as an option in the list of available fonts then it is not
installed (or not installed correctly) on the computer.

The Index project uses the program BabelMap to build up strings of characters
for stamp readings.  In BabelMap, set Samian5 as the 'Single Font' in the box
near the bottom of the screen.   The special characters start at code point
F500 (use 'Go to Code Point').  Sequences of characters built up in the Edit
buffer can be copied and pasted into a word processor, where the readings have
to be set as Samian5 (as above) to display the glyphs correctly.

BabelMap can be downloaded from:
<http://www.babelstone.co.uk/Software/BabelMap.html>

Passing on word processor files using Samian5 to other users
============================================================

If you pass on a PDF version of your report, the fonts (including Samian5) are
embedded in the pdf file and should display correctly on any printer or in any
viewer - or in a browser with the standard plugins.

If you send out a word processor file, like a Word .doc file, you also have to
send a copy of the original font (preferably in the original installation 
file) and the font has to be installed on any machine that is used to edit or
view the .doc file, otherwise it the Samian5 characters will not display.  This
is because unlike .pdf files, which carry their own fonts around with them,
.doc files rely on the fonts installed on the host system.  If Samian5 is not
installed, the Samian5 glyphs in a .doc file will display as black (or empty)
boxes, or in an Asian script (depending on what fonts are installed on the
system).

Using Samian5 in LaTeX
=================================

The following commands define a macro to display text in the Samian5
font using XeLaTeX.

~~~
% load and define samian font
\newfontfamily{\samian}{Samian5} % Use Samian5 font in sigillata section
\newcommand\sam[1]{{\samian #1}} % set text in Samian5 font
% examples of usage
\sam{OF.CALVI} % plain text
\sam{\symbol{"F5C3}ER\symbol{"F609}[NI]} % syntax for non-standard glyphs
~~~

The development of the Samian5 font
===================================

The characters in the Samian5 font reflect the state of development of the
Index, and continued to develop up until the publication of Volume 9 in 2012. 

P A Tyers\
\today
<!--    $Id: HOWTO_use_Samian5.md,v 1.3 2014/03/06 09:42:17 paul Exp paul $ -->

