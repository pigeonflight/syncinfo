The syncinfo tools are simple shell scripts to be used with two node clusters. The assumption that the nodes in the cluster have identical configurations and users provided with the shadow password system (/etc/passwd, /etc/group etc..)

The tools also assume that shared keys have been setup to allow rsync between the nodes without passwords.

These tools are very primitive and should be considered to be in a "work's for me" state. They are known to work on Red Hat 5 and 6, but I can't make promises about other systems.
In other words, if you don't know what you're doing then you probably want to stay away.

The included tools are:

* /usr/local/bin/syncpass
* /usr/local/bin/synchome
* /usr/local/bin/syncprint
* /usr/local/bin/synchttp

Normally I place them in the /usr/local/bin directory

Preparation
------------
Make sure you have two nodes which both have passwordless ssh access.
There's a good article on this here: http://www.thegeekstuff.com/2008/11/3-steps-to-perform-ssh-login-without-password-using-ssh-keygen-ssh-copy-id/

Installation
---------------
1. Clone the repository

::

    git clone https://github.com/pigeonflight/syncinfo.git
    cd syncinfo
    sh ./install.sh

2. On both nodes edit the `/etc/syncinfo` and add the name (or ip address) of the opposite node

