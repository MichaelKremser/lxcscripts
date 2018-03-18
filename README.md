# lxcscripts

This repository contains various scripts related to LXC.

## list-lxc

Simply calls "lxc-ls" with some commonly used parameters.

## restart-lxc

Restarts a container, in fact just calls lxc-stop and lxc-start.

## create_container_*

Scripts to automatically create containers with (almost) ready-to-use software.

### fdroidserver

Container featuring fdroidserver and nginx. nginx is configured to use self-signed certificates for SSL. In production use, those should be replaced by certificates accepted by clients.
