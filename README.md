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

### mediawiki

Creates a container with MediaWiki based on Debian 9 (stretch). Should not be used for new deployments!

### ubu1804_mw1.31.3

Creates a container with MediaWiki 1.31.3 based on Ubuntu 18.04. The MediaWiki installation archive (mediawiki-1.31.3.tar.gz) will be automatically downloaded to /root/Downloads if necessary.

## vmnet

Creates a bridge with the name "vmnet" that can be used if lxcbr0 cannot be used or has issues.
