=======
WoPPack
=======

`World of Padman <http://worldofpadman.net/>`_ gamepack for
`NetRadiant <http://dev.xonotic.org/projects/3/wiki/Netradiant>`_.

This is based upon the original gamepack which can be found in
``wop-1.5.x-to-1.6-patch-unified.zip`` /
``XTRAS/editing files/WoP radiant files.zip``.

The gamepack is compatible with World of Padman v1.5+ and any version of NetRadiant.
It should work with the GtkRadiant 1.5.0 series as well.

Installation
------------

Extract ``WoPPack`` into your NetRadiant installation.

.. sourcecode:: sh

    $ # find NetRadiant directory
    $ ls ~/netradiant/
    RADIANT_MAJOR    gl            plugins       q3data.x86_64  radiant.x86_64
    RADIANT_MINOR    global.xlink  q1.game       q3map2         warsow.game
    bitmaps          heretic2      q2map         q3map2.x86_64  xonotic.game
    darkplaces.game  modules       q2map.x86_64  qdata3
    docs             nexuiz.game   q3data        qdata3.x86_64
    games            osirion.game  q3data.qdt    radiant

    $ # download WoPPack
    $ wget --output-document=WoPPack-master.zip https://github.com/robo9k/WoPPack/archive/master.zip

    $ # extract WoPPack and copy into NetRadiant directory
    $ unzip WoPPack-master.zip && cp --recursive WoPPack-master/* ~/netradiant/

When starting NetRadiant, select "World of Padman" as the game, then check
and confirm that the engine path is correct.

As a last step, you need to copy the file ``custinfoparms.txt`` into the
right place for ``q3map2``.

.. sourcecode:: sh

    $ mkdir --parents ~/.padman/wop/scripts/
    $ cp WoPPack-master/wop.game/wop/scripts/custinfoparms.txt ~/.padman/wop/scripts/
