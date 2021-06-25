# About

This playbook creates a packet filtering rule that prevents programs, that are forced to run under a specific group account, from establishing any outgoing network connection.


# Setup

`ansible` has to be installed.

Run the following command to have all necessary installation steps performed automatically on localhost:

	ansible-playbook -K install.yaml


# Usage

There are two possible ways.

Either execute _command_ as group `nonet`:

	sg nonet command

Or let the convenience script `nonet` execute _command_:

	nonet command

## Example

```
$ command='nslookup github.com 1.1.1.1'
$ $command
Server:		1.1.1.1
Address:	1.1.1.1#53

Non-authoritative answer:
Name:	github.com
Address: 140.82.118.4

$ nonet $command
;; connection timed out; no servers could be reached

```


