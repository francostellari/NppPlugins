# Menu Icons plugin (*a.k.a.* MenuIcons)

*Menu Icons* is a Notepad++ plugin designed to make the menus and tab more beautiful by adding:
* icons to stabdard menu items
* file shell icons to the *Recent file* and *Window* menus
* file shell icons to the *Tabs* in both tab bars

Icons for the standard menu items can be provided as *icon* files in a folder, where the sub-folder names indicate sub-menu names, and icon file names indicate menu items.

MenuIcons allows to add icons to both main and context menu. Several options are available to load the icons from a folder. 
More than provide a full set of icons, it's design to enable people to create their own set of icon themes. 

Note: the plugin does not work correctly on WinXP. 

Alternative icon sets: 
* [English by Yaron](http://www.google.com/url?q=http%3A%2F%2Fsourceforge.net%2Fp%2Fnotepad-plus%2Fdiscussion%2F482781%2Fthread%2Fdb6db280%2F8b56%2Fattachment%2FMenuIcons%2520English.zip&sa=D&sntz=1&usg=AOvVaw3xhFVfsCSP2rdTMNRqupdM)
* [Hebrew by Yaron](http://www.google.com/url?q=http%3A%2F%2Fsourceforge.net%2Fp%2Fnotepad-plus%2Fdiscussion%2F482781%2Fthread%2Fdb6db280%2F8b56%2Fattachment%2FMenuIcons%2520Hebrew.zip&sa=D&sntz=1&usg=AOvVaw0-R0qReB6hjvo1rAJigmsw)
* [Russian by vodek3](https://github.com/francostellari/NppPlugins/files/10197405/MenuIcons.Russian.zip)
* [Universal Command ID by HeIIoW0RLD](https://github.com/francostellari/NppPlugins/files/10427908/ALL_2.zip)

Just download them and replace the MenuIcon folder or save them somewhere else and set the new folder in the Menu Icons plugin options.

## v2.03 (2023-05-26)

* Fix a problem with menu items containing some special characters: < > " '

## v2.02 (2023-01-14)

* Fix problem with using menu id ([Issue #38](https://github.com/francostellari/NppPlugins/issues/38))

## v2.01 (2022-12-27)

* Fix tab icon problem when renaming the file
* Increase the tab symbol to 8 characters and unicode support. To use unicode simbols, make sure to save the MenuIcon.ini as UTF-16.

## v2.00 (2022-10-17)

Significant refactoring of the code to improve icon management and thus enable fixing some long outstanding issues with the menu icons disappearing in some circumstances.

Fixes:
* Menu icons do not diappear anymore when opening recent files
* File shell icons do not diappear anymore when opening recent files

Enhancements:
* Added file shell icons to the tabs
* Added a *symbol* to the tab text to indicate when its buffer becomes dirty and needs saving

Releases:
* [MenuIcons v2.00 x64](MenuIcons_dll_2v00_x64.zip)
* [MenuIcons v2.00 x32](MenuIcons_dll_2v00_x32.zip)


## v1.22 (2017-02-14)

Improve detection of context menu.


## v1.21 (2017-02-09)

This version fix a bug that did not display the file icons in the Window sub menu in recent versions of NPP.
Speed improvement in generating the recent file icons when network files are listed


## v1.20 (2016-10-11)

Added 64-bit version


## v1.10 (2015-04-17)

Adds shell icons for recent files and open windows menus


## v1.04 (2015-03-30)

Better context and tab menu recognition


## v1.03 (2015-03-25)

Fix icon placement problem in Win7 Classic Theme.
Free icon memory allocation after Tab and Context menu are destroyed.


## v1.02 (2015-03-19)

This version adds icons to the tab popup menu. More icons are included from both open icon library (http://sourceforge.net/projects/openiconlibrary/) and famfamfam.com.


## v1.00 (2015-03-06)

First release
