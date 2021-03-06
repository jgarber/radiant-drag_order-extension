# DragOrder for Radiant 0.9.2+

Created by Bright 4, February 2009. Inspired by and based on Sean Cribbs' Reorder extension.

## Notes

Only designers and admins have the ability to re-order pages

Is now only compatible with Radiant above 0.9.1 (especially as a gem)

## Installation

    git clone git://github.com/gerrit/radiant-drag-order.git vendor/extensions/drag_order
    
    rake radiant:extensions:drag_order:migrate
    rake radiant:extensions:drag_order:update

## Version History

### v0.4.2 - 2010-11-27

* Made compatible with edge, otherwise we can't override views
* Tidied up a lot of internal javascript
* Overrode some helpers
* Rewrote more of sitemap.js

### v0.3.7 - 2010-11-22

* Turned into a gem
* Went back to radiant-drag_order-extension instead of radiant-drag-extension

### v0.3.6 - 2010-08-31

* updated for Radiant 0.9 edge. Use tag radiant-0.9.1 with released gem version

### v0.3.5 - 2010-07-09

* renamed back to DragOrder
* SQL Injection fixes
* code cleanup

### v0.3.4 - 29-03-2010

* Moved assets to extension/drag directory
* Updated instructions

### v0.3.3 - 09-02-2010

* Made compatible with Radiant 0.9.0

### v0.3.2 - 18-11-2009

* Made compatible with Radiant 0.8.1. This extension should now be compatible with at least version >= 0.6.9

### v0.3.1 - 25-05-2009

* FIX: if the move request takes some time to finish, the dragline now stays put when dropped instead of still being 
dragged along with the mouse.
* Changed color of the row that is being dragged to fit better with default Radiant colors.
* Small robustness-fix for cases when the rake migrate is forgotten.
* Modified install instructions in README.

### v0.3 - 16-03-2009

* Incorporated copy functionality. When pressing Ctrl or Command, you can copy the item.
* Fixed errors which occurred when trying to place two pages with the same slugs. Now, the second one is seen as a copy.
* Fixed some JS errors.

### v0.2.3 - 16-03-2009

* v0.2.2. was not really compatible with Radiant > 0.6.9... This one should be compatible with versions both before and after 0.7.

### v0.2.2 - 12-03-2009

* Made compatible with Radiant > 0.6.9

### v0.2.1 - 23-02-2009

* Fixed JS bug that did not allow dragging of child pages which were loaded using AJAX after expanding a page.

### v0.2 - 21-02-2009

* Initial commit