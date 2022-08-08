<p><img src="https://upload.wikimedia.org/wikipedia/commons/3/33/Systemd-logo.svg" title="systemd" align="top" height=100 /></p>

*The Portable Service concept takes inspiration from classic chroot() environments as well as container management and brings a number of their features to more regular system service management - Lennart Poettering (0pointer.net)*

### General informations

This repository contains various files to build Portable Services images to be deployed using `systemd` and `systemd-portabled` tools.

**Images**

**Requirements**

- systemd >= 241
- mkosi >= 12

### How to build and use these images ?

Firstly, install `mkosi` from the package manager:

```shell
dnf install -y mkosi
```

### References

* Portable Services : https://systemd.io/PORTABLE_SERVICES/
* Walkthrough for Portable Services : https://0pointer.net/blog/walkthrough-for-portable-services.html
* mkosi : https://github.com/systemd/mkosi
