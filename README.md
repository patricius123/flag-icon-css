gae-init-pro
========
**gae-init-pro** is a stripped version of [gae-init][gaeinitbit] with a fluid
design. If you're not familiar with [gae-init][gaeinitbit] then it's recommened
to fork that version instead.

Demo Page
---------

The latest version is always accessible from:
[http://pro.gae-init.appspot.com][gaeinitpro]

Getting the code and running the application
--------------------------------------------

    $ hg clone https://bitbucket.org/lipis/gae-init-pro project-name
    $ dev_appserver.py /path/to/project-name/main

To test it visit `http://localhost:8080/` in your browser.

Running the build.py script (first time)
----------------------------------------

    $ cd /path/to/project-name/main
    $ npm install
    $ ./build.py -c
    $ dev_appserver.py .

To test it visit `http://localhost:8080/` in your browser.

Running the Development Environment
-----------------------------------

To watch for changes of your `*.less` and `*.coffee` files and compile them
automatically to `*.css` and `*.js` respectively:

    $ cd /path/to/project-name/main
    $ ./build.py -wc

To run the actual server (in another bash):

    $ dev_appserver.py /path/to/project-name/main

To test it visit `http://localhost:8080/` in your browser.

Deploying on Google App Engine
------------------------------

Before deploying make sure that the `app.yaml` and `config.py` are up to date.

    $ cd /path/to/project/main
    $ ./build.py
    $ appcfg.py update .

Tech Stack
----------

  - [Google App Engine][gae]
  - [Python 2.7][gaepython]
  - [NDB][]
  - [Jinja2][]
  - [Flask][]
  - [CoffeeScript][]
  - [LessCSS][]
  - [Twitter Bootstrap][bootstrap]
  - [PubNub][]

Requirements
------------

  - [Google App Engine SDK for Python][gaesdk]
  - [node.js][nodejs]
  - [OSX][] or [Linux][]
  - [Mercurial][]
  - [Sublime][] (If you are a developer, you need that)

Examples
--------

  - [Remby][]
  - [The Smallest Creature][thesmallestcreature]

Contributions and Ideas
-----------------------

  - [tzador][]
  - [chris][]
  - [ksymeon][]
  - [gmist][]

Author
------

[![Lipis flair on stackoverflow.com][lipisflair]][lipis]

[gaeinit]: http://gae-init.appspot.com
[gaeinitpro]: http://pro.gae-init.appspot.com
[gaeinitbit]: https://bitbucket.org/Lipis/gae-init
[gae]: https://developers.google.com/appengine/
[gaepython]: https://developers.google.com/appengine/docs/python/python27/using27
[ndb]: https://developers.google.com/appengine/docs/python/ndb/
[jinja2]: http://jinja.pocoo.org/docs/
[flask]: http://flask.pocoo.org/
[coffeescript]: http://coffeescript.org/
[lesscss]: http://lesscss.org/
[bootstrap]: http://twitter.github.com/bootstrap/
[pubnub]: http://www.pubnub.com

[gaesdk]: https://developers.google.com/appengine/downloads
[nodejs]: http://nodejs.org/
[osx]: http://www.apple.com/osx/
[linux]: http://www.ubuntu.com
[mercurial]: http://mercurial.selenic.com/
[sublime]: http://www.sublimetext.com/2

[remby]: http://www.remby.com
[thesmallestcreature]: http://www.thesmallestcreature.com/

[tzador]: http://stackoverflow.com/users/165697/tzador
[chris]: http://stackoverflow.com/users/226394/chris-top
[ksymeon]: https://plus.google.com/102598378133436784997
[gmist]: https://github.com/gmist

[lipisflair]: http://stackexchange.com/users/flair/5282.png
[lipis]: http://stackoverflow.com/users/8418/lipis
