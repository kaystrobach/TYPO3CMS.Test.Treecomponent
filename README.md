TYPO3CMS.Test.Treecomponent
===========================

Testing infrastructure for a generic tree component for TYPO3 CMS.

This repository should serve as a R&D matrix to evaluate different **Javascript Tree Components** for future use within TYPO3 CMS.

Currently implemented:
======================
* jsTree (jstree.com)

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

Add a folder beneath "Web" and give it a name according to the library you are using.
Add all the files however you see fit, but keep an index.html that sets links to all scenarios you supply.
When you are finished, add to this file in order to make easily visible what you tested.

How to set it up
================

We supply a database dump of a fictional pages table.
This used to be a real world table that we stripped of fields we deem not necessary and scrambled the data.
Apart from that we kept the original uid/pid relations in order to supply an as-close-to-reality scenario as possible.
The pagetree is roughly 9000 pages in size.
We chose this example because we needed a rather huge sample in order to do the benchmarks right.

Just set up a database and import the data.
Change the credentials in config.php to reflect the user/password of your mysql database.

Call "Web/doesItWork.php" in your browser to make sure you get some data.
Be patient because the deliver more than 9000 pages.