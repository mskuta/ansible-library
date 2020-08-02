# About

These playbooks install the very latest versions of Docker Engine and Docker Compoase on Debian or any distribution using the Debian repositories. They automate the installation instructions described [here](https://docs.docker.com/engine/install/debian/ "Install Docker Engine on Debian"), [here](https://docs.docker.com/engine/install/linux-postinstall/ "Post-installation steps for Linux") and [here](https://docs.docker.com/compose/install/ "Install Docker Compose") in the official Docker Documentation.


# Setup

`ansible` has to be installed.

Run the following command to install Docker Engine on localhost:

	ansible-playbook -K install-engine.yaml

Run the following command to install Docker Compose on localhost:

	ansible-playbook -K install-compose.yaml


