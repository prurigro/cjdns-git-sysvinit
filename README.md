cjdns-git-sysvinit
========

About: A sysvinit (rc.d/init.d) startup script for cjdns that should work with most unix-like operating systems

Requirements: This script requires cjdns.sh to be executable and in $PATH. It can be found in the cjdns repository (https://github.com/cjdelisle/cjdns) @ cjdns/scripts/cjdns.sh

Usage:
    1. Copy cjdns.rc.d to the sysvinit script location for your OS (usually /etc/rc.d or /etc/init.d)
    2. Copy cjdns.default to /etc/default/cjdns and configure the locations listed inside based on your system configuration
    3. You can now run the cjdns sysvinit script with the following usage: /etc/rc.d/cjdns {start|stop|restart|status}
