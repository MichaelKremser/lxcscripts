# lxcscripts

This repository contains various scripts and files related to LXC.

## list-lxc

Simply calls "lxc-ls" with some commonly used parameters.

## restart-lxc

Restarts a container by calling lxc-stop and lxc-start and waits for the file "/run/dhclient.eth0.pid" to be created.

## create_container_*

Scripts to automatically create containers with (almost) ready-to-use software.

### fdroidserver

Container featuring fdroidserver and nginx. nginx is configured to use self-signed certificates for SSL. In production use, those should be replaced by certificates accepted by clients.
