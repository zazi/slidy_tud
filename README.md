Slidy TUD
=========

About
-----

* <b>author</b>: Bo Ferri
* <b>year</b>: 2011

This is an extension of the [Slidy](http://www.w3.org/Talks/Tools/Slidy/help.html) presentation template that was originally created by [Dave Raggett](http://www.w3.org/People/Raggett/). It enables to design a
presentation in HTML markup.

Enhancements/Usage
------------------

* configurable metadata area on the top right side with (meta identifiers in brackets):
   * short title of the presentation (short_title)
   * author name (author_name)
   * presentation type (presentation type) - to be able to express the kind of a presentation, e.g., thesis defense   
* configurable navigation menu near the bottom:
   * can divide the presentation into up to 5 parts
   * the titles of the parts can be set via meta identifiers (frag_1 - frag_5)
   * single slides can be annotated with a specific part identifier via a class name (s_frag_1 - s_frag_5)
   * this toolbar can be toggled via the key 'M'   
* tabulator simulation:
   * tabulator can be simulated with the help of the classes 'tab' and 'normal' or restrictive 'tab2' and 'normal2'  
* restart page:
   * an URL of a restart page can be defined via the meta identifier 'restart_page'   
* source references:
   * source can be hyperlinked referenced with the help of the class 'source_ref' on an 'A' element
   * application:
      * don't set the 'href' attribute, this will be set automatically via a JavaScript function
      * only set the class 'source_ref' on an 'A' element whose body only includes the number of the source (the source identifier), e.g., '1'
      * attach the class 'sources' to sources slides
      * set the id 's_[source identifier]' for every source reference on a sources slide, e.g., 's_1'
* set total slides number:
   * you can choose between "total slides number with appendix" or "total slides number without appendix" (i.e. it counts only slides up to last fragment identifier(that is used for the menu))
   * this behavior can be set with the help of the meta identifier 'total_slides_with_appendix': 
      * value 'true' == "total slides number with appendix"
      * value 'false' == "total slides number without appendix"           
   
Changes/Usage
-------------

* slide headlines should be a DIV of the class 'headline'
* slide bodies should be a DIV of the class 'slide_body'  
 
Example
-------

* see [blank.html](https://github.com/zazi/slidy_tud/blob/master/blank.html) for an example of the new functionalities
* see [here](http://zazi.smiy.org/slides/pmkb-defence/pmkb.html) for Slidy TUD in practise (best view with Firefox 4.x+, full-screen mode on, and Univers font family installed)
