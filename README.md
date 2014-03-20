BRIEF
distributed todo list. creates `TODO' files in current directory or appends to existing ones.

AUTHOR
rn grapenthin

DATE
version 2014-03-19

DETAILS
This is a distributed TODO list. dido depends on environment variable $DIDO which should
point to a file that can hold a list of paths/filenames.

If invoked with no argument, dido will list the content of all files listed in $DIDO with
a little bit of formatting. If invoked with an argument, dido will either create a file
'TODO' in the local directory, add this file to the database held in $DIDO and add the
arguments to the file 'TODO.' If 'TODO' exists, the argument will just be appended.

For the listing of the contents it's useful to know, that dido will ignore all lines
in the TODO files that begin with `#' which allows commenting these items for archival
purposes, but they won't show up in the listing of all the tasks.

USAGE:

       dido 	   # shows all distributed TODO lists
       dido [task] # adds task to TODO list in current directory,
                   # creates TODO file if non-existant, adds todo file to global TODO db held in $DIDO env var

CHANGELOG
2014-03-xx, rngrp: First version.
2011-03-19, rngrp: added documentation 
