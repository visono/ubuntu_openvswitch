# ubuntu_openvswitch
## Provides openvswitch 2.3.2 debian packages build on Ubuntu 14.04 for installation on the docker host.

### The following command will copy the debian packages of openvswitch into ~/openvswitch on the docker host:

    $ docker run --rm -v ~/openvswitch:/openvswitch-2.3.2-build visono/ubuntu_openvswitch

### To install openvswitch on the docker host execute the following commands with sudo or as root inside the ~/openvswitch folder:

    $ apt-get install bridge-utils
    $ dpkg -i openvswitch-common_2.3.2-1_amd64.deb openvswitch-switch_2.3.2-1_amd64.deb

### Very handy for docker multi host networking as described [here](http://wiredcraft.com/blog/multi-host-docker-network/)!!!
