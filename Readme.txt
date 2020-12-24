================== English =================================================

Entware developers are happy to announce Entware-ng and Entware-3x merge. The new project is called Entware.
Entware will have all package repositories from Entware-3x (armv5, armv7, aarch64, mips, mipsel, x64) and
a repo for armv7 (Linux kernel 2.6.36) from Entware-ng. All other repositories will be available for installation but will not be
updated.

We have updated the toolchain in Entware. We use GCC 8.4.0 to build binaries and glibc 2.27 as a system library
(glibc 2.23 is used for kernel 2.6.36 - it is glibс limitation).

Current armv7 architecture users running Entware-ng, or any user currently running Entware-3x, can switch to Entware by running
`opkg update; opkg upgrade` twice.
The first upgrade changes repo URL in opkg.conf file, the second run updates the packages.

Entware standard installation is similar to Entware-ng. It does not install Entware version of busybox.
There is also alternative installer in Entware that is similar to Entware-3x installer.
It installs Entware version of busybox. For this installation Entware users are independent from firmware users.
Entware has root user with 12345 password. Other users can be added permanently to Entware in this case
to run services that require such users.

Currently different Entware versions are widely used in routers, NASes, 
Android devices and other hardware that uses Linux kernel.

Entware team is ready to add other repositories for different embedded devices running Linux kernel higher or equal
than 2.6.36. Please give us your device name, output of `uname -a` command and other useful information.
