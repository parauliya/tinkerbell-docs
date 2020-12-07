---
title: Index
date: 2020-08-31
---

# Index

When a Worker first starts in a Tinkerbell environment, it network boots and contacts the Provisioner where [Boots](/docs/services/boots) handles its DHCP settings and provides iPXE support. As part of this process Tinkerbell sets up the Worker with an in-memory operating system called OSIE and is based on [Alpine](https://alpinelinux.org).

OSIE is downloaded to the Worker via iPXE. Usually, this will happen when a Worker network boots and an operating system is not installed, otherwise the bootloader will boot from the disk which contains your operating system.

OSIE can built, run, and tested outside of the Tinkerbell stack. Take a look at the code in its GitHub repository: [tinkerbell/osie](https://github.com/tinkerbell/osie).