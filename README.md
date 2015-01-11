Magento 2.0 Sample Module
====================

Last tested on beta2.


<img src="http://i.imgur.com/Ma6v2gs.jpg" alt="Magento 2 Sample Module" />

What I got so far:
----------

This extension contains the admin and frontend sections for a single entity (Author) store view related.  
The frontend and other types of entities listed in **the purpose** will follow.  
Don't put many hopes in this. Based on the comments on the magento 2 repo the grid system will be changed...A LOT.  

The purpose 
----------

....of this repository is to hold a sample CRUD module for Magento 2.0.  
This module should contain the following: 

 * 4 Entities. 
  * 1 Flat - with a store selector. Similar to CMS pages
  * 1 Flat but behaving as a tree - with a store selector. Similar to categories but non EAV
  * 1 EAV - similar to products
  * 1 EAV but behaving as tree - Similar to categories.
 * Backend files for managing the entities mentioned above
 * Frontend files for list and view each of the entities mentioned above
 * RSS feeds for each entity mentioned above
 * SOAP & REST API files for the entities mentioned above
 * URL rewrites filed for frontend for the entities above
 * Files needed for a many to many relation between the entities above and products
 * Files needed for a many to many relation between the entities above and categories
 * Files needed for a many to many relation between the entities above (among themselves)
 * Each entity must support different attribute types:
  * Text
  * Textarea (with and without WYSIWYG editor)
  * Date
  * Boolean
  * Dropdown (with different source models)
  * Multi-select (with different source models)
  * File
  * Image
  * Decimal
  * Integer
 * Each entity should have fronend links to the list page in one of the menu/link areas provided by the default theme
 * Each entity must have SEO attributes (meta-title, meta-description, meta-keywords)
 * Would be nice to have unit tests for every class in the code - but that's low priority.
 * Each entity type must have widgets for frontend (link, short view).
 * Each entity must support customer comments.
 * Each EAV entity must have a section for managing attributes (similar to product attribtues).
 
After this is complete (or almost) it will become the base source for the Ultimate Module Creator 2.0 which will be a version for Magento 2.0 of the <a href="https://github.com/tzyganu/UMC1.9">Ultimate Module Creator for Magento 1.7+</a>. 

Any other ideas and pieces of code are welcomed even encouraged.

Install
-----

To install this module copy the code from this repo to `app/code` folder of your Magento 2 instance,  
If you do this after installing Magento 2 you will have to edit `app/etc/config.php` and add this line in the  `$modules` array at the end:

    'Sample_News' => 1, 
	
then run from the console `php setup/index.php update`.
 