### JimStim Pattern File Library

This repository is for storing [JimStim][j] jsw pattern files in and tracking
updates to the default set of patterns as provided by [jbperf.com][p]. The
[jbperf.com][p] file is in a directory called OtherPatternFiles and will be
updated as new ones are released.

The other file in here is the first of a series of pattern files that have been
independently verified by me as being accurate and correct, or with notes as to
the flaws that they contain. I hope to expand this library as I expand the
decoder library of [FreeEMS][f]!

At the moment [JimStim][j] is mainly used for testing of MegaSquirt units, that
run variants of [MSExtra][m] firmware such as MS1Extra and MS2Extra, while they
are being built, however, increasingly they are being used in the testing and
development of [FreeEMS][f] systems too.

Please check the ERRATA.md file in the OtherPatternFiles directory before using
any patterns from the jsw file within.

It is not recommended to load only one pattern at a time, or to load more than
about 3500 lines of pattern total. Thus, due to what seems like a bug in the
2.0.3 JimStim firmware, I recommend selecting the patterns you want and catting
them repeatedly into a .jsw file until it has around 3500 lines, then load. In
this way you are much more likely to be able to use one of each of the patterns
that you want to test with.

Note, I have no idea what license these are shared under, and it doesn't really
matter much as they are just data files for a tool anyway. I will choose a
suitable license for the ones that I created from scratch at a later date.

I hope someone, other than me, finds this repository useful.

### Links

 - [jbperf.com][j]
 - [JimStim][j]
 - [FreeEMS][f]
 - [MSExtra][m]

[f]: http://freeems.org/  (FreeEMS)
[p]: http://jbperf.com/ (jbperf.com)
[j]: http://jbperf.com/JimStim/ (JimStim)
[m]: http://msextra.com (MSExtra)

