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

Installation
---------------
