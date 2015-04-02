# ethercat_grant

This is a repo for the pr2-grant utility. It makes it possible to run the *ros_ethercat_loop* without requiring root privileges.

## Installation

If you installed this package from *apt-get* then you're good to go. (This is definitely the recommended way)

If you compiled this package from source, then you'll need to copy the resulting `ethercat_grant` executable to `/usr/local/bin` and add the sticky bit to it: `sudo chmod +s /usr/local/bin/ethercat_grant`.

## Use
Using ethercat_grant makes it possible to not use *sudo* anymore for running the ethercat main loop. Just use `launch-prefix="ethercat_grant"` in your launch files for the *ros_ethercat_loop*.
