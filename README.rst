======
README
======
**This README is not updated, yet !**
**Todo: change python to python2.7**

This is a basic buildout for Plone 4.2.x

Installation
------------

Tested on Debian 6 [Squeeze], Debian 7 [Wheezy].

Make sure you have all dependencies you need/want, i prefer to install it into its own virtual environm
ent::
**TODO: change to python2.7**

        apt-get install build-essential python2.6-dev python-virtualenv


go to/create /path/where/you/want/to/install/it for example /home/$USER/plone and create your vritualen
v::
**TODO: change to python2.7**
        virtualenv --python=python2.6 --no-site-packages $MYPLONESITENAME

after the creation its done do::

        cd $MYPLONESITENAME
        source bin/activate

Plone is installed using the buildout system. Installation is as straight forward as possible::

        git clone git://github.com/svx/Plone-Buildout-Example.git buildout
        cd buildout

Now you have to create your buildout.cfg file, depending on what you want to run yo have to do::

        vim [<- choose the editor of your choise] buildout.cfg

        [buildout]
        extends = config/development.cfg


after that just do::

        python bootstrap.py
        bin/buildout



and start it with::

        bin/instance fg



Credits
-------

Plone - http://plone.org

Lennart Regebro - https://github.com/regebro

thet -> https://github.com/thet

natea -> https://github.com/natea
