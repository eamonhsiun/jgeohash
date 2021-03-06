## jgeohash

<a href="http://flattr.com/thing/4067696/astrapi69jgeohash-on-GitHub" target="_blank"><img src="http://api.flattr.com/button/flattr-badge-large.png" alt="Flattr this" title="Flattr this" border="0" /></a>

[![Build Status](https://travis-ci.org/astrapi69/jgeohash.svg?branch=master)](https://travis-ci.org/astrapi69/jgeohash)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/de.alpharogroup/jgeohash-core/badge.svg)](https://maven-badges.herokuapp.com/maven-central/de.alpharogroup/jgeohash-core)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/de.alpharogroup/jgeohash-geoip/badge.svg)](https://maven-badges.herokuapp.com/maven-central/de.alpharogroup/jgeohash-geoip)

## Key features:

1. Very small size (<30Kb)
2. Can get the adjacent geohash area from the given direction
3. Can get the geohash from an ip address
4. Can calculate distance between two geohash values in various measuring units like miles, km, meters
5. Can get the geohash cells around from the first, second or thrird ring from a given geohash cell

An easy-to-implement library that can assist Java developers in using the GeoHash algorithm in order to create geocodes based on custom latitude and longitude values.

With the help of jGeohash, Java developers will be able to quickly and easily generate a geohash code using user-defined latitude and longitude values. By using the GeoHash algorithm, the space can be divided into multiple grid shapes.

This library is a basic implementation from the GeoHash algorithm written in the java and can be applied to generate from the latitude and longitude a geohash code and reverse.

The library is kept simple and have no dependencies to other libraries.

## License

The source code comes under the liberal Apache License V2.0, making jgeohash great for all types of applications.

## Maven dependency

Maven dependency is now on sonatype.
Check out [sonatype repository](https://oss.sonatype.org/index.html#nexus-search;quick~jgeohash) for latest snapshots and releases.

Add the following maven dependency to your project `pom.xml` if you want to import the core functionality of jgeohash:

Than you can add the dependency to your dependencies:

		<!-- GEOHASH LOCATION version -->
		<jgeohash.version>2.3.0</jgeohash.version>
		<jgeohash-core.version>${jgeohash.version}</jgeohash-core.version>
		<jgeohash-geoip.version>${jgeohash.version}</jgeohash-geoip.version>

		<dependencies>
			...
			<dependency>
				<groupId>de.alpharogroup</groupId>
				<artifactId>jgeohash-core</artifactId>
				<version>${jgeohash-core.version}</version>
			</dependency>
		</dependencies>

Add the following maven dependency to your project `pom.xml` if you want to import the geoip functionality of jgeohash:

Than you can add the dependency to your dependencies:

		<dependencies>
			...
			<dependency>
				<groupId>de.alpharogroup</groupId>
				<artifactId>jgeohash-geoip</artifactId>
				<version>${jgeohash-geoip.version}</version>
			</dependency>
		</dependencies>


## Want to Help and improve it? ###

The source code for jGeohash are on GitHub. Please feel free to fork and send pull requests!

Create your own fork of [astrapi69/jgeohash/fork](https://github.com/astrapi69/jgeohash/fork)

To share your changes, [submit a pull request](https://github.com/astrapi69/jgeohash/pull/new/master).

Don't forget to add new units tests on your changes.

## Contacting the Developer

Do not hesitate to contact the jgeohash developers with your questions, concerns, comments, bug reports, or feature requests.
- Feature requests, questions and bug reports can be reported at the [issues page](https://github.com/astrapi69/jgeohash/issues).

## Examples

  * [SpatialDataQueries][SpatialDataQueries]
  * [Simple-example][Simple-example]
  * [Hibernate-example][Hibernate-example]

   [SpatialDataQueries]: https://github.com/astrapi69/jgeohash/wiki/Adding-spatial-data-queries-to-Phoenix-on-HBase "Adding spatial data queries to Phoenix on HBase"
   [Simple-example]: https://github.com/astrapi69/jgeohash/wiki/Simple-example "Simple-example"
   [Hibernate-example]: https://github.com/astrapi69/jgeohash/wiki/Hibernate-example "Hibernate-example"



Last changes
----------------------

Version 2.3.0
-------------
- Created new module projects. jgeohash-core and jgeohash-geoip

Version 2.0.0
-------------
- JDK version upgraded to version 8.

Version 1.4.6
-------------
- Added project to sonatype repository.
- Added project to continous integration: https://travis-ci.org/astrapi69/jgeohash
- Added project to flattr.com: https://flattr.com/thing/4067696/astrapi69jgeohash-on-GitHub

Version 1.4.5
-------------
Gets the geohash from the given ip address
added dependency for geoip-api

Version 1.4.3
-------------
Extend functionality to calculate distance from two Points, Positions, coordinate values(latitude, longitude) or two geohash values in meters.
Created a new class for keeping data of the neighbors cells from the given geohash to cardinal directions for the first and second ring region.


Version 1.4.2
-------------
Added new interface Position for the class Point.

Created new class that calculates distance from two Points or two geohash values in km or miles.


Version 1.4.1
-------------

Added method to get getAdjacent from multiply directions.

Added functionality for get first and second ring neighbors from a geohash cell.


