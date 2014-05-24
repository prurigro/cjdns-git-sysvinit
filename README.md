# CJDNS System V Initscript #

## About ##

A legacy system v initscript (rc.d/init.d) for cjdns that should work on most platforms.

## Setup ##

* **cjdns**: Copy to _'/etc/default/cjdns'_ and change any values needed to match your system configuration.
* **cjdns.rc.d**: Copy to your OS' system v initscript location (usually _'/etc/rc.d'_ or _'/etc/init.d'_) with the name _'cjdns'_ (ie: _'/etc/rc.d/cjdns'_) and make it executable.
* **cjdns.sh**: Copy to $PATH and make it executable.

## Usage ##

You can now run the cjdns sysvinit script with the following commands (assuming sysvinit directory _'/etc/rc.d'_):

* /etc/rc.d/cjdns: Outputs the following information "usage: /etc/rc.d/cjdns {start|stop|restart|status}".
* /etc/rc.d/cjdns **start**: Start cjdroute using the values given in _'/etc/default/cjdns'_.
* /etc/rc.d/cjdns **stop**: Stop cjdroute.
* /etc/rc.d/cjdns **restart**: Stop cjdroute, then start it again using the values given in _'/etc/default/cjdns'_.
* /etc/rc.d/cjdns **status**: Displays whether or not cjdroute is currently running.

## Credits ##

* Written by prurigro: [GitHub Projects](https://github.com/prurigro) | [Arch Linux AUR Packages](https://aur.archlinux.org/packages/?SeB=m&K=prurigro)
* Some parts of the _'cjdns.rc.d'_ script were taken from the initscripts functions script that used to be included in Archlinux.
* The _'cjdns.sh'_ script was taken from the [cjdns repository](https://github.com/cjdelisle/cjdns), and was written by numerous authors including myself.
