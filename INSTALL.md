
NOTES ON THE INSTALLATION OF SAMIAN5 FONT
=========================================


The Microsoft typography page at 
<http://www.microsoft.com/typography/TrueTypeInstall.mspx>
describes the process of installing on various version of Windows.


Windows XP
----------

It seems to be preferable to de-install any existing copies of the Samian5
font before installing a new one.

1. Open Font management window (Start->Control Panel->Fonts)

2. Delete the Samian5 font if it is already installed (right click on icon,
then Delete).  If the font icon is greyed out or cannot be deleted, this
suggests that the font is already in use by an application on the system.
Identify the application, stop it and then try to delete the font again.

3. Unzip the Samian5-2.XX.zip file into a temporary directory. Locate the .ttf
file, which will be named Samian5-2.XX.ttf, where XX is the version number.

4. Drag-and-drop the .ttf file into the Font management window opened at 1).  A
popup window confirms the installation.

5. To verify installation right click on the font icon, then Properties.   The
filename should match the installed .ttf name.


Linux, using fontconfig system
------------------------------

Tested on Mandriva 2009.1, 2010.0 and later

1. Run 'unzip Samian5-2.XX.zip' in a temporary directory.  Locate the .ttf file.

2. Delete existing copies of Samian5-*.ttf from ~/.fonts directory or move them
out of the way.

3. Copy .ttf file from .zip file into ~/.fonts.  Name will be Samian5-2.XX.ttf
where XX is version number.

4. Run 'fc-cache' to rebuild font cache

5. Run 'fc-list Samian5' to confirm installation


P A Tyers

    $Id: INSTALL,v 1.8 2012/11/08 11:14:34 paul Exp paul $

