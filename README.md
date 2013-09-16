cjdns-git-sysvinit
========

About: A sysvinit (rc.d/init.d) startup script for cjdns that should work with most unix-like operating systems

Requirements:
    1. The 'cjdns.sh' script from the cjdns scripts folder to be executable and located in $PATH
    2. The 'cjdns' config file from the cjdns scripts folder to be configured and located @ /etc/default/cjdns
    *The cjdns scripts folder is located in the cjdns repo, which can be cloned from: https://github.com/cjdelisle/cjdns

Usage:
    1. Copy cjdns.rc.d to the sysvinit script location for your OS (usually /etc/rc.d or /etc/init.d)
    2. You can now run the cjdns sysvinit script with the following usage: /etc/rc.d/cjdns {start|stop|restart|status}
