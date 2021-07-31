# Compare two versions of `st_segments()`

The R-package `nngeo` includes the function [`st_segments`](https://michaeldorman.github.io/nngeo/reference/st_segments.html),
which splits lines or polygons into separate segments. A
[forked version of `nngeo`](https://github.com/a-benini/nngeo/tree/st_segments_efficient)
modifies `st_segments()`with the objective of processing large numbers of
geometries efficiently. 

* [This modification](https://github.com/a-benini/nngeo/commit/34a33274b28f31b99b3cbd9c5d239a7c395482f4) and
* the original version of `st_segments` (`nngeo`, version 0.4.3)

are compared in __*st_segments_version_comparison.Rmd*__.
<span style="color:red">__Warning__</span>: The run time of the code included
in this __*.Rmd*__ is quite longsome. So you may want to examine the
[documented outcome](https://a-benini.github.io/st_segments_version_comparison/st_segments_version_comparison.html)
, especially the printed out time difference for running the code chunk with
`microbenchmark()`, before compiling this __*.Rmd*__  to a __*.html*__ yourself.
