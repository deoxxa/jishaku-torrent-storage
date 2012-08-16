Jishaku Torrent Storage
=======================

Everyone needs somewhere to put their loot!

Overview
--------

This application allows users to upload and download torrent files, nothing less
and nothing more. There's a little bit of validation and sanity checking on the
input data, but that's all. There's no way to list, browse or search.

Requirements
------------

1) A running [seaport](https://github.com/substack/seaport) server.
2) A [MongoDB](http://www.mongodb.org/) database

Installation
------------

```
$ npm install jishaku-torrent-storage -g
```

OR

```
$ git clone git://github.com/deoxxa/jishaku-torrent-storage.git
```

Usage
-----

```
$ jishaku-torrent-storage [--config:option=value ...] [config_file_to_load.json ...]
```

Configuration
-------------

* seaport (object)
  * host (string) host or ip of seaport server
  * port (number) port of seaport server
* mongo (object)
  * host (string) host and port of mongodb server
  * db (string) database name for mongodb
* winston (object)
  * console (object/null) if null, don't log to console
    * colorize (boolean) show colourful logs
    * timestamp (boolean) show timestamp in logs
  * loggly (object/null) if null, don't log to loggly
    * all config options found [here](https://github.com/indexzero/winston-loggly)

License
-------

3-clause BSD. A copy is included with the source.

Contact
-------

* GitHub ([deoxxa](http://github.com/deoxxa))
* Twitter ([@deoxxa](http://twitter.com/deoxxa))
* Email ([deoxxa@fknsrs.biz](mailto:deoxxa@fknsrs.biz))
