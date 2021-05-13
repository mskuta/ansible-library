# About

This playbook installs the very latest version of [Lynis](https://cisofy.com/lynis/) on Debian or derivatives of it. It automates the installation instructions described [here](https://packages.cisofy.com/community/#debian-ubuntu).


# Setup

`ansible` has to be installed.

Run the following command to install `lynis` on localhost:

	ansible-playbook -K install-lynis-apt.yaml

Then confirm that `lynis` has been installed successfully by entering:

	lynis show version


