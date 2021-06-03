# About

This playbook installs the very latest version of [Crystal](https://crystal-lang.org/) on Debian. It automates the installation instructions described [here](https://crystal-lang.org/install/on_debian/) under "Manual setup".


# Setup

`ansible` has to be installed.

Select the Debian branch of your installation by setting the variable `repository` in the playbook to the appropriate value.

Run the following command to install `crystal` and recommended packages on localhost:

	ansible-playbook -K install-crystal-apt.yaml

Then confirm that `crystal` has been installed successfully by entering:

	crystal version


