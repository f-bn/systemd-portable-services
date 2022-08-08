<p><img src="https://upload.wikimedia.org/wikipedia/commons/3/33/Systemd-logo.svg" title="systemd" align="top" height=100 /></p>

*The Portable Service concept takes inspiration from classic chroot() environments as well as container management and brings a number of their features to more regular system service management - Lennart Poettering (0pointer.net)*

### General informations

This repository contains various files to build Portable Services images to be deployed using `systemd` and `systemd-portabled` tools.

**Images**

There are 2 types of images in this repository :

  - **Runtime images** (`*-runtime`) : base images used to share runtime(s) between multiples Portables Services (OpenJDK, NodeJS, Python... or standalone userspace) much like a Docker base image
  - **Regular images** : the service application images, they can be monolithic (runtime + application embedded in a single image) or they can be a lightweight extension image (but they require a runtime base image in order to run)

**Requirements**

- systemd >= 241
- mkosi >= 12

### How to build and use these images ?

Firstly, install `mkosi` from the package manager :

```shell
dnf install -y mkosi
```

### References

* Portable Services : https://systemd.io/PORTABLE_SERVICES/
* Walkthrough for Portable Services : https://0pointer.net/blog/walkthrough-for-portable-services.html
* mkosi : https://github.com/systemd/mkosi
