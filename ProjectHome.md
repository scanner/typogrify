## Note ##

Typogrify 1.0! Bug fixes, support for Django's autoescaping, and a new titlecase filter.

**important note** about Typogrify's handling of autoecaping: All typogrify filters (except for the new titlecase) mark their output as "safe". This means you should only use them on input you trust or have cleaned somehow. if you'd like to use them on user content like comments please run them through |force\_escape or |markdown:"safe" on them first.

Please use [version 0.2](http://typogrify.googlecode.com/files/typogrify-0.2.tar.gz) if you're still on Django 0.96.

## About Typogrify ##

Typogrify is a collection of Django template filters that help prettify your web typography by preventing ugly quotes and widows and providing CSS hooks to style some special cases.

A [demonstration of everything it does](http://static.mintchaos.com/projects/typogrify/) explains better than I do.

But here's the quick list of the included filters:

  * Widon't
  * SmartyPants
  * Initial quotes wrapped in class='dquo' or class='quo' depending on if they are single or double
  * Ampersands wrapped in class='amp'
  * Multiple adjacent capital letters wrapped in class='caps'
  * A lazy crazy filter to do all of them
  * A titlecase filter that uses Stuart Colville's port of John Gruber's titlecase.pl

You can checkout the SVN:
`svn checkout http://typogrify.googlecode.com/svn/trunk/ typogrify`

Or grab the [latest release](http://code.google.com/p/typogrify/downloads/list).