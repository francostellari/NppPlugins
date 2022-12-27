# Run Me plugin (*a.k.a.* RunMe)
RunMe allows to execute the currently open file, based on its shell association. The plugin allows also to open an explorer or command shell at the file location. Options are available to same the current file (or all the files) before execution. The executed file can be run in foreground,background, or hidden mode. Context menu entries and tool bar icons are available.

## v1.61 (2022-12-27)
* Fix a problem with saving settings to INI file.

## v1.60 (2022-10-18)
* Added: menu icons for "Run with arguments" and "Run as administrator"
* Added: Toolbar entries for "Run with arguments" and "Run as administrator"
* Added: Tab context menu entries for "Run with arguments" and "Run as administrator"
* Added: Run me with a custom *verb*
* Fix: Cancelling a "Run me w/ arguments" would not stop the run
* Fix: Remove the tab flickering for save all unamed buffers before running

## v1.50
Added: run as administrator feature (accessible via menu)

## v1.40 (2016-10-11)
Added 64-bit version

Added the capability of running scripts with parameters

## v1.36 (2015-03-30)
Add plugin and tab menu icons. Improve tab menu detection.

## v1.35 (2014-02-06)
Added the possibility of running a different external program to explore a file folder.

Fixed a couple of issues that did not allow the plugin to run on WinXP.

This is the last version running on WinXP.

## v1.34 (2013-11-22)
Added date/time variables in path expansion.

This version drops ASCII support.

## v1.33 (2013-05-15)
Fix a regression in recent versions of NPP where the tab context menu entries did not work

## v1.32 (2012-12-22)
Fixed a problem with saving buffers in multiple views

## v1.31 (2010-07-150
fixes a problem with NPP v5.7

## v1.301 (2009-09-26)
fixes the context menu feature that was broken in Notepad++ v5.5.

## v1.30 (2009-09-03)
Adds customizable entries in the file tab context menu.

## v1.20 (2009-03-30)
New features have been added:
+ now it is possible to have toolbar icons for the three main functions of the plugin: run/explore/shell displaying the icons can be enabled/disabled (individually) from the newly designed options dialog box
+ now it is possible to take some actions after executing the current file from the newly designed options dialog box : one can decide to minimize NPP, keep the focus to NPP, or give the focus to the executed process

## v1.11 (2009-01-25)
Fix bug related to saving the file(s) before running the script.

## v1.10 (2008-11-21)
This version adds several new features and reorganizes all the options into a new options dialog box instead of the plugin sub-menu:
+ you can set the folder where the current file will be executed (requested by Michael): current process directory, file directory, you can enter it each time, or you can set one based on replacement variables
+ you can open an explorer window at the file location
+ you can open a shell (of your choice) at the file location
Additionally:
+ more options for saving the script before executing
+ more checks on file and folder existence
+ code clean up and minor bug fixes.

## v1.03 (2008-10-21)
added Unicode version compatible with NPP v5.1.

## v1.02 (2007-11-04)
Fixes a bug that caused files running in console to be hidden. This version also adds 3 new options to run the current file hidden, maximized, or minimized. When no option is checked, the file is run in normal mode.

## v1.01 (2007-05-08)
 has minor code cleanup, no end user differences

## v1.00 (2007-05-07)
 first release