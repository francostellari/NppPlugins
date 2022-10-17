# Language Help plugin (*a.k.a.* LanguageHelp)
LanguageHelp allows to load a language specific help file (CHM, HLP, PDF) and search for the keyword under the cursor. The latest version allows also to show the help files as menu entries or in the context menu.

## 1v72 (2017-02-14)
Improve detection of context menu.

## 1v71 (2017-02-08)
Fix a bug related to the Edit menu getting corrupted in recent version of NPP

## 1v70 (2016-10-11)
Added 64-bit version

## 1v61 (2015-03-30)
Improve context menu detection and adds capability to enable/disable the menu icons introduced in the last version

## 1v60 (2015-03-05)
Bug fix and added menu icons (NOTE: menu icons do not display correctly in WinXP)

## 1v52 (2014-02-06)
Fixed a couple of issues that did not allow the plugin to run on WinXP

## 1v51 (2013-11-22)
Fixed a problem with the context menu not displaying in recent versions of Notepad++.
Added date/time variables in path expansion.
This version drops ASCII support.

## 1v50 (2013-01-19)
A new extension/file matching algorithm has been implemented that allows to use command line file search patterns.

Note that the old format for extension matching should be automatically updated to the new format... but if it does not work, you may need to do so manually.

Please note that this version may be incompatible with WinXP system because it requires shlwapi.dll v7... thanks to Diamanti.

## 1v40 (2010-08-12)
Fix a problem with winhelp32 not displaying the context menu... thanks to Tom Williams

## 1v33 (2010-07-15)
Fix problems with Notepad++ v5.7

## v1.321 (2009-09-26)
Fix the context menu feature that was broken in Notepad++ v5.5.

## 1v32 (2009-09-05)
Add several options/features that were requested by users:
- the context menu entry can be displayed either at the top or bottom (see new options dialog box )
- if no Acrobat program is found in the registry the PDF file is shell executed so that you preferred read is started (note that in this way no keyword search is possible)
- the *Test* button in the language edit dialog box has been renamed to a more appropriated *Expand*. A new *Test* button has been added to test the help file in the same way as calling the *Help*"* from the menu.

## 1v311 (2009-09-03)
Fix a bug introduced in 1v31 that disabled several previous features. This version also fixes a mysterious bug were the Help menu entries would be shown in the file tab popup menu if it was double right clicked with the mouse.

## 1v31 (2009-09-02)
Add several options:
- a toolbar button for calling the help on the currently selected word (enable in options dialog box)
- the possibility of showing the help command on the context menu
- the possibility of searching for the currently selected word even when using the menu entries

## 1v301 (2009-08-26)
Adds support for ms-help collections (thanks to Wintruder) and removes the requirement of lowercasing of path that are shell executed (as requested by Diamanti
Ms-Help collection may be accessed in two ways by specifying a path that starts with `"ms-help://"` in the extended file path control box in the options dialog box. One can just specify the collection: `"ms-help://<collection>"` (such as `"ms-help://ms.vscc "`), in this case the current work will be automatically appended to be searched. Alternatively, a complete search string can be specified using any of the special variable available: `"ms-help://<collection>?word=$word$&filter=<filter>"` (such as `"ms-help://ms.vscc?word=$word$&filter=Visual C++"`).

## 1v20 (2008-11-12)
Adds environment and special variables to the help path as well as the capability of calling HTML files and do internet searches:

The help file path may point to a local CHM or PDF files for keyword search.
Alternatively, the field may point to a command/file that will be shell executed.
This include HTML file both on the local machine and on the internet.

The help file path edit box may contain special substitution strings:
`$fullpath$` = full path of the currently active file
`$dir$` = directory of the currently active file
`$name$` = file name without extension of the currently active file
`$ext$` = extension of the currently active file
`$word$` = currently selected word
`$nppdir$` = directory of notepad.exe
`$pdir$` = plugin directory
`$cdir$` = config directory

Additionally enviroment variables are accepted in the form `%envvar%`.
For example: `%programfiles%` will be replaced by `"c:\program files\"`
For example: `http://www.google.com/search?q=$word$` will search for the current word on Google

Use the test button to see the expanded path based on current settings.

## 1v14 (2008-11-11)
Fixes two bugs:
- PDF help was not working anymore since the Unicode version was introduced;
- The CHM help window was sending messages to the main window (thanks eRIC & Michael).
Some additional error checking and messages have been added.

## 1v13 (2008-10-21)
added Unicode version compatible with NPP v5.1.

## 1v12 (2008-07-14)
This version fixes a bug preventing the plugin to save the correct menu display choice upon closing Notepad++, when the help file where shown in the main Notepad++ help menu (thanks Bertrou).

## v1.11 (2008-07-02)
This version fixes a small bug and try to work around the Acrobat Reader incapability to execute a DDE DocFind command request (thanks to Mauro for pointing it out). The search is implemented through the command line argument "/A search=". Unfortunately this solution does not allow to search for additional words once the PDF file is open... so in order to search new words one has to close the PDF file first. When I have time I will look into a OLE implementation that may be able to fix this issue.

## v1.10 (2008-06-27)
Adds two main functionality to the previous version: PDF help file search and capability to show the help files as menu entries either in the plugin menu or in the main Notepad++ help menu. If one specify a PDF file as an help file in the option dialog box, the plugin automatically recognize it and call Acrobat to show it (NOTE that this implementation is based on the Acrobat DDE and therfore require at least the Acrobat Reader). Check box have been added and enabled in the main Option dialog box and in the language help edit box to enable showing the help file as a menu entry.

## v1.00 (2007-11-29)
Does not offer new functionality but implements an options dialog box to add/remove/edit language specific help files. The dialog box is accessible through an option menu entry .

## v0.10 (2007-10-03)
It is the very first version of the plugin so there is no fancy GUI to setup the list of language specific help files. At the moment you have to manually edit the LanguageHelp.ini file that will be created in you plugin/config directory. Please note that the file path do not need to be in SNF as in the example below.

    [Options]
    StayOnTop=0

If StayOnTop=1, the window will stay on top of Notepad++, otherwise clicking on Notepad++ main window will put the help in bkgnd. The default value is 0.

Here are some example of setting for help file:

    [AutoIt]
    Extension=au3
    File=C:\Progra~1\AutoIt3\AutoIt.chm

    [JPSoft]
    Extension=bat btm cmd
    File=C:\Progra~1\JPSoft\4NT7\jphelp.chm

For each language you specfy a short name for the section: [MyLanguage]
Then you define two entries to list the extensions without the "." and separated by space.
They you define the path to the help file to use for that extension.

Error handling is not very advanced at the moment!!!