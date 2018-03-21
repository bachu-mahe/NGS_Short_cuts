**Useful Short Cuts**
##########################################################################################
1. **Arranging plots properly**
http://www.sthda.com/english/articles/24-ggpubr-publication-ready-plots/81-ggplot2-easy-way-to-mix-multiple-graphs-on-the-same-page/

2. **Very good resource for ggplot from r-statistics.co by Selva Prabhakaran**
http://r-statistics.co/R-Tutorial.html
http://tutorials.iq.harvard.edu/R/Rgraphics/Rgraphics.html
http://www.cookbook-r.com/Graphs/Axes_(ggplot2)/

3. **Data visualization with ggplot2**
http://www.datacarpentry.org/R-ecology-lesson/04-visualization-ggplot2.html

4. **Useful resources for plotting using Rstudio**
https://cran.r-project.org/web/packages/gridExtra/vignettes/arrangeGrob.html

5. **Find all the files with an extension of fastq in a directory or sub-directories and move to a new folder within that directory**
```find . -name "*.fastq" -print0 | xargs -0 -I {} mv {} fastqfiles/```

6. **Tree-like output using ls** _by — by clitips on April 26, 2013, 1:37 p.m @ http://www.bashoneliners.com/oneliners/oneliner/157/_
```ls -R | grep ":$" | sed -e 's/:$//' -e 's/[^-][^\/]*\//--/g' -e 's/^/   /' -e 's/-/|/'```
 >This one-liner initially does a recursive listing of the current directory: ls -R.
 #Any output other that the directory names, identified by ":" at the very end of each line (hence ":$"), is filtered out: grep ":$".
 #Finally there's a little of "sed" magic replacing any hierarchy level ("/") with dashes ("-"): sed ....
 #Works for me with Bash under Linux, Mac OS X, Solaris

7. **See the contents of .tar.gz file without opening**
```tar -tf filename.tar.gz```
8. **Find all files recursively with specified string in the filename and output any lines found containing a different string.**
```find . -name *conf* -exec grep -Hni 'matching_text' {} \; > matching_text.conf.list```
