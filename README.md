#Data visualization with ggplot2

http://www.datacarpentry.org/R-ecology-lesson/04-visualization-ggplot2.html


Useful resources for plotting using Rstudio
https://cran.r-project.org/web/packages/gridExtra/vignettes/arrangeGrob.html


#! /bin/bash
##Find, ls, etc

#Find all the files with an extension of fastq in a directory or sub-directories and move to a new folder within that directory
find . -name "*.fastq" -print0 | xargs -0 -I {} mv {} fastqfiles/

#Tree-like output using ls
#by — by clitips on April 26, 2013, 1:37 p.m @ http://www.bashoneliners.com/oneliners/oneliner/157/

ls -R | grep ":$" | sed -e 's/:$//' -e 's/[^-][^\/]*\//--/g' -e 's/^/   /' -e 's/-/|/'

#This one-liner initially does a recursive listing of the current directory: ls -R.
#Any output other that the directory names, identified by ":" at the very end of each line (hence ":$"), is filtered out: grep ":$".
#Finally there's a little of "sed" magic replacing any hierarchy level ("/") with dashes ("-"): sed ....
#Works for me with Bash under Linux, Mac OS X, Solaris.


