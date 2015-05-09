Fakku-Verse 2.0
============

[![Build Status](https://travis-ci.org/browserquest/BrowserQuest.png)](https://travis-ci.org/browserquest/BrowserQuest) [![Dependency Status](https://gemnasium.com/browserquest/BrowserQuest.png)](https://gemnasium.com/browserquest/BrowserQuest)

[BrowserQuest](http://browserquest-teambq.rhcloud.com:8000) is a HTML5/JavaScript multiplayer game experiment.

It has three major parts:

* the server side, which runs using Node.js
* the client side, which runs using javascript in your browser
* the database side, which runs using Redis

Browser Support
---------------

* Firefox - Works well.
* Chrome - Works well.
* Chromium - Works well.
* Opera 15.x - Works well.
* Opera 12.16 - Background music doesn't play.  Everything else works (Very slow though).
* Safari 6.x - Background music doesn't play.  Everything else works well.
* IE 10.x - Doesn't work.  Other versions untested.

How to get it going
-------------------

Getting the server up and running is pretty easy. You need to have the following installed:

* Node.js ← Versions 0.8.x-0.10.x work.  **Do not use 0.6.x, it [does not work](https://github.com/senchalabs/connect/issues/858).**
* Winamp server ← needed to run the bloody thing
* jQuerry ← java nodes
* socket.io ← needed to run the server connection

Ubuntu ← not working (yet)
------


Mac OS X ← F*ck apple
--------
^


Node.js, Memcached, and Redis for Fedora 16+ and RHEL/CentOS/SL 6.x ← Might work, we aint sure.
-------------------------------------------------------------------

On Fedora 16+ and RHEL/CentOS/SL 6.x, you can install Redis (required) and Memcached (optional) using
yum.

For just RHEL/CentOS/SL 6.x, you need to add the EPEL repo first.  Not needed for Fedora:

    $ sudo rpm -Uvh http://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm

Then install Node.js and everything else needed:

    $ sudo yum install zlib-devel gcc gcc-c++ autoconf automake make redis nodejs npm memcached
    $ sudo chkconfig redis on
    $ sudo chkconfig memcached on

Start Redis and Memcached by running:

    $ sudo service redis start
    $ sudo service memcached start

Now continue on with the normal steps to clone the BrowserQuest git repo, and start up BrowserQuest:

    $ git clone git://github.com/harleyknd1/Fakku-Verse.git
    $ cd Fakku-Verse
    $ npm install -d
    $ node server/js/main.js

Windows
-------
0. download and un-pack the project folder
1. download node.js and install it https://nodejs.org/
2. download and install WAMPSERVER (make sure the icon is green)
3. download and install socket.io http://socket.io/
4. copy or move the project files into the www folder of wamp (or a sub folder under the www folder)
5. install socket.io into the program folder


Documentation
-------------

I'll re-write it when i feel like it.

Mailing List
------------

N/A

IRC Channel
-----------

\#FakkuVerse2 on irc.rizon.net

License
-------

Code is licensed under The MIT License (MIT) Content is licensed under The MIT License (MIT)
See the LICENSE file for details.

Credits
-------
Originally created by [Aneko-Chan] (https://www.fakku.net/users/aneko-chan-5618558 & https://github.com/harleyknd1):

