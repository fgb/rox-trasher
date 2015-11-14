#### ROX-Trasher

Trashcan application for the ROX Filer and Desktop

by Gabriel Rojas & Fernando Garcia Bermudez


##### BRIEF

A modified version of the trashcan application written for Puppy Linux by Dan Van Wormer. It was adapted to be non-distribution and non-user specific and updated to the latest version of [ROX-Filer](http://rox.sourceforge.net/desktop/).

It is undergoing substantial development in order to make it adhere to the [freedesktop.org Desktop Trash Can Specification](https://wiki.freedesktop.org/www/Specifications/trash-spec/) and related specifications.

Apart from the common requirements of this specification, we are working on an undo function to ease the recovery of mistakingly trashed items and towards a better integration into ROX filer and its desktop (hopefully, getting it included into the ROX trunk in the near future).


##### NEWS FOR THIS VERSION

[ChangeLog](Changes)


##### LICENSE

[GNU GPL v2](COPYING)


##### REQUERIMENTS

zenity >= 2.12.1


##### INSTALLATION

Simply extract "ROX-Trasher-xx.tar.bz2".


##### OPERATIONS

When you first click on the trash icon it will create (if it does not already exist) the $XDG_CONFIG_HOME/ROX-Trasher  directory.

Clicking on the desktop icon will open up the  $XDG_CONFIG_HOME/ROX-Trasher directory.

Once the Trash is open you can right click on a "Trashed" item and select "Restore". This will copy the original file or directory back to its original location. If another item with the same name is in that location it will prompt you before it over-writes it. Also, you can choose delete the item, but USE THE CONTEXTUAL MENU OF THE APP, NOT THE DELETE OPERATION OF ROX-FILER!!!.

Dragging and dropping a file or directory into the Trash desktop icon will move that file or directory into $XDG_CONFIG_HOME/ROX-Trasher

Files and directories will have a unique number appended to the end of their names. This prevents new trashed items with the same names form over writing the old files.

Right-clicking on a file or directory and selecting "Send To - Trash" will have the same effect as dragging and dropping the file on the desktop icon.

To restore all items, right click on the desktop icon and select "Restore all". The trashcan will restore all items stored in the trash directory and shows a info dialog with the names of the restored items. If the item have a pinboard or panel shortcut it will be restored too.

To empty the trash right click on the desktop icon and select "Empty Trashcan". Emptying the Trash will display all the files and directories in the trash and ask for confirmation.

You will get a prompt if you send a symbolic link to the Trash. This is just to let you know that you are not sending the original item to the Trash.


##### TRANSLATIONS HOW-TO

Check the "TRANSLATIONS" section in the AppRund and item-template files, redefine the variable strings, and add in the case loop the generic $LANG code (for example, for es_ES: es* ). You can also have to translate the AppInfo.xml file in the $APPDIR directory, check the Chapter 17 in the ROX-Filer manual.
If you add some translations for your own, please send us with the proper $LANG code and the translated AppInfo file to add to the next version of the app.


##### FUTURE

- The posibility to add in Rox-Filer to be oficial part of the program.
- If the up item is posible, a item menu in Rox-Filer: "Send to Trash".


##### CONDITIONS

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA


##### CONTACT

Help? Bugs? Suggestions? Opinions? ----------> achaw.ar@gmail.com


##### TESTERS

David Arthur (dave@kouya.ne)
