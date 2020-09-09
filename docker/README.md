# About

These playbooks install the very latest versions of Docker Engine and Docker Compose on Debian or any distribution using the Debian repositories. They automate the installation instructions described [here](https://docs.docker.com/engine/install/debian/ "Install Docker Engine on Debian"), [here](https://docs.docker.com/engine/install/linux-postinstall/ "Post-installation steps for Linux") and [here](https://docs.docker.com/compose/install/ "Install Docker Compose") in the official Docker Documentation.

`install-engine-apt.yaml` first sets up the Docker apt repository. The packages are then installed from this repository. If the apt configuration should remain untouched, `install-engine-deb.yaml` can be used instead. It downloads the packages as .deb files from a Docker file server and then installs them. To update the packages later on, run the originally used playbook again.

# Setup

`ansible` has to be installed.

Run the following command to install Docker Engine on localhost:

	ansible-playbook -K install-engine-apt.yaml

Run the following command to install Docker Compose on localhost:

	ansible-playbook -K install-compose.yaml


