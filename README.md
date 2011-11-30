Pretty Vim Python
=================

This is my attemp to make the python syntax highlighting in Vim look like Textmate's.

Important
---------

In the syntax folder is the **python.vim** which does the syntax highlighting for Python. Just replace yours with mine
but remember to backup beforehand.

Next I had to add another color definition to the **molokai.vim** stylesheet. This is probably not a very good idea
because the new color definition will not be available for a different color theme. So in your colors folder
add this molokai.vim and remember to select it as your default colorscheme.

The changes made in the files are highlighted with comments and begins with **NOTE: @pfdevilliers added this**.


General
-------

The additions are still very much a hack job and must be improved upon. I think there are still two issues to 
sort out to duplicate the functionality of the Textmate highlighting, but I guess it is usable.
