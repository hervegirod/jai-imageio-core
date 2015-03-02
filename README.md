jai-imageio-core (standalone)
=============================

[![Build Status](https://travis-ci.org/jai-imageio/jai-imageio-core.svg)](https://travis-ci.org/jai-imageio/jai-imageio-core)

NOTE: This is a fork of
[jai-imageio-core](https://java.net/projects/jai-imageio-core/) 
which is no longer maintained upstream. 

This 'standalone' version has removed has removed 
dependencies to jai-core packages (`javax.media.jai`) and JPEG 2000 (`jj2000`).
This version also does excludes the C
implementations from libJIIO, meaning that this version is platform independent
and fully redistributable under the 3-clause BSD license in
[LICENSE.txt](LICENSE.txt) (and thus is Apache and GPL compatible).

JPEG 2000 support is available as an additional module 
[jai-imageio-jpeg2000](https://github.com/jai-imageio/jai-imageio-jpeg2000)
with a different (non-GPL compatible) license.


If you are not concerned about GPL compatibility or source code
availability, you might instead want to use
https://github.com/geosolutions-it/imageio-ext/ which is actively
maintained and extends the original imageio with many useful features,
but depends on the [binary distribution of jai\_core](
http://download.osgeo.org/webdav/geotools/javax/media/jai_core/1.1.3/).


Contribute
----------

There is **NO ACTIVE DEVELOPMENT** in this repository; any commits here are
mainly to keep the build working with recent versions of Maven/Java - the date
in the version number indicates the time of such modifications and should not
have any effect on functionality.

You are however encouraged to raise a 
[Github Pull Request](https://github.com/jai-imageio/jai-imageio-core/pulls)
with any suggested improvements.

You can also look at and raise an
[issue](https://github.com/jai-imageio/jai-imageio-core/issues) - your stacktrace
might still be of use to someone else.


Usage
-----

To build this project, use Apache Maven 2.2.1 or newer and run:

    mvn clean install

To use jai-imageio-corefrom a Maven project, add:

    <dependency>
        <groupId>com.github.jai-imageio</groupId>
        <artifactId>jai-imageio-core</artifactId>
        <version>1.3.0</version>
    </dependency>

(see the latest `<version>` within [pom.xml](pom.xml#L10).


Download
--------

To download the binary JAR, see the 
[Downloads at BinTray](https://bintray.com/jai-imageio/maven/jai-imageio-core-standalone/view).


Javadoc
-------

Standalone [Javadoc for jai-imageio-core](http://jai-imageio.github.io/jai-imageio-core/javadoc/) is also
provided.



Copyright and licenses
----------------------

* Copyright © 2005 Sun Microsystems
* Copyright © 2010-2014 University of Manchester
* Copyright © 2010-2015 Stian Soiland-Reyes
* Copyright © 2015 Peter Hull

The source code for the jai-imageio-core project is copyrighted code that
is licensed to individuals or companies who download or otherwise
access the code.

The complete copyright notice for this project is in
[COPYRIGHT.txt](COPYRIGHT.txt)

The source code license for this project is **BSD 3-clause**, see
[LICENSE.txt](LICENSE.txt)


Changelog
---------

* 1.3.0 - Java package changed to com.github.jaiimageio
* 1.2.1 - Version 1.2.1 released. Pushing to Maven Central and BinTray. 
      Workaround for OpenJDK8 libjpeg bug (issue #6).
      groupId changed from net.java.dev.jai-imageio to com.github.jai-imageio.
      Fix for PNM ASCII write (issue #7).
* 1.2-pre-dr-b04-2014-09-13 - Removed last jpeg2000 plugin. Javadoc now includes overview.      
* 1.2-pre-dr-b04-2014-09-12 - Separated out [JPEG 2000](https://github.com/jai-imageio/jai-imageio-core/issues/4)
      support from [jai-imageio-core](http://github.com/jai-imageio/jai-imageio-core)
      for [licensing reasons](https://github.com/jai-imageio/jai-imageio-core/issues/4).
      Re-enabled junit test (issue #5).
* 1.2-pre-dr-b04-2013-04-23 - Updated README and pom, newer maven plugins, removed
  broken links to dev.java.net. Javadocs included and published at
  http://jai-imageio.github.com/jai-imageio-core/
* 1.2-pre-dr-b04-2011-07-04 - Avoid Maven many build warnings. Fixed character set.
* 1.2-pre-dr-b04-2010-04-30 - Initial Maven version, based on CVS checkout from
  dev.java.net, but with Maven pom.xml and only code covered
  by open source license.



More info
---------

* https://github.com/jai-imageio/jai-imageio-core
* http://jai-imageio.github.io/jai-imageio-core/javadoc/
* https://java.net/projects/jai-imageio-core/
* http://www.oracle.com/technetwork/java/current-142188.html
* http://download.java.net/media/jai/builds/release/1_1_3/

