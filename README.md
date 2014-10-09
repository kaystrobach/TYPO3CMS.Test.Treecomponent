TYPO3CMS.Test.Treecomponent
===========================

Testing infrastructure for a generic tree component for TYPO3 CMS.

This repository should serve as a R&D matrix to evaluate different **Javascript Tree Components** for future use within TYPO3 CMS.

These are the specs:

Actions
-------
* **should** be able to filter nodes clientside
* **must** be able to filter nodes serverside
* **should** be able to support mountpoints
* **must** be able to display a context menu with 2 levels
* **must** be able to drag & drop nodes (configurable)
* **must** be able to add new nodes
* **must** be able to support a tree refresh, preferably on a regular basis without user interaction

Interactions
------------
* **must** be able to display different icons per node (record type awareness)
* **should** be able to display two icons next to each other
* **must** be able to use icon fonts
* **must** be usable on touch-devices
* **must** have a state indicator (where am i)
* **must** be able to select multiple nodes

Developer
---------
* **must** be useable and configurable as viewhelper / no js needed for integration in either frontend or backend
* **must** supply an extendable JS interface 
* **must** be usable in tceforms
* **must** be compatible / non- intrusive with jquery

Scalability
-----------
* **must** be able to get subnodes via ajax
* **must** should be usable with 10000 nodes visible at a time

How to contribute
=================

