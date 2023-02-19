# Auto Save plugin (*a.k.a.* AutoSave)
AutoSave allows to automatically save the currently open files based on a timer schedule (default is 1 min) and/or upon the application losing focus. The plugin offers several options to save the current (or all the files), selecting only the named ones, accessible through an options dialog box.

## v2.00
Major code rework breaking previous features
- Removed: various file checking features to simplify the behavior
- Fix: tab flipping to save only named files
- Added: save on tab change feature
- Added: save on Notepad++ exit

## v1.60 (2017-02-08)
Added the capability of creating a time stamped copy of current file content.

## v1.50 (2016-10-11)
Added 64-bit version

## v1.40 (2012-12-11)
Fix bug involving multiple views

## v1.30 (2010-12-01)
Adds a requested functionality to ignore files larger than a specified size.

## v1.20 (2010-07-16)
Is designed for NPP >= v5.7
+ enable new features that allow to save unamed buffers as well as create autorecovery files
+ fixes a problem that disabled previous version under NPP v5.7
Old menu settings has been replaced with a new options dialog box

## v1.12 (2010-04-16)
Fixed the autosave at 0 time interval ==> disable timed autosave.

## v1.11 (2008-10-21)
Added Unicode version compatible with NPP v5.1.

## v1.10 (2007-05-24)
A new dialog box to set the interval of the timed autosave as well as the new NPPM_GETPLUGINSCONFIGDIR available since NotePad++ v4.1.0. This means that for users using %APPDATA% directory the profiles will be saved in %APPDATA%\Notepad++\Plugins\Config instead of %APPDATA%\Notepad++.

## v1.00 (2007-05-08)
First release using menu settings
