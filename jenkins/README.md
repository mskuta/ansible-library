# About

This playbook installs the stable version of [Jenkins](https://www.jenkins.io/) on Debian or derivatives of it. It automates the installation instructions described [here](https://pkg.jenkins.io/debian-stable/).


# Setup

`ansible` has to be installed.

Run the following command to install `jenkins` and a Java runtime on localhost:

	ansible-playbook -K install-jenkins-apt.yaml

Then confirm that `jenkins` has been installed successfully and is up and running by entering:

	ps -C java -f | fgrep jenkins

or:

	wget --output-document=/dev/null --quiet --server-response localhost:8080 2>&1 | fgrep X-Jenkins:


