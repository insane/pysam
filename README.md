### Description

This is an unofficial git port of [http://code.google.com/p/pysam/](http://code.google.com/p/pysam/).

Pysam is a python module for reading and manipulating Samfiles. It's a lightweight wrapper of the [samtools](http://samtools.sourceforge.net/) C-API. Pysam also includes an interface for [tabix](http://samtools.sourceforge.net/tabix.shtml).

The latest version is available on the 'Downloads' page. See the 'INSTALL' file for instructions.

The quick start guide is [here](http://www.cgat.org/~andreas/documentation/pysam/api.html). More detailed documentation is available [here](http://www.cgat.org/~andreas/documentation/pysam/contents.html).

Questions and comments are very welcome and should be send to the the pysam [user group](http://groups.google.com/group/pysam-user-group).

### Fixes
It contains fixes to make it work on MacOS X 10.7 with samtools 0.18.1. The original sources
were producing the following linker errors when ```import pysam``` was invoked:

```
ImportError: dlopen(/usr/local/Cellar/python/2.7.2/Frameworks/Python.framework/Versions/2.7/lib/python2.7/site-packages/csamtools.so, 2): Symbol not found: ___ks_insertsort_heap
  Referenced from: /usr/local/Cellar/python/2.7.2/Frameworks/Python.framework/Versions/2.7/lib/python2.7/site-packages/csamtools.so
  Expected in: dynamic lookup
```

The error occurred both when installed from source and homebrew.

### License

[MIT](http://www.opensource.org/licenses/mit-license.php)
