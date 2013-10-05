<img style="float:right" src="http://www.digifail.com/images/misc/github/netgear_sc101.jpg" />
sc101-nbd
==============

sc101-nbd supplies the userland utility and daemon script to mount partitions
on the [Netgear Storage Central (SC101)](http://en.wikipedia.org/wiki/Netgear_SC101) SAN under Linux as a standard network block device (NBD). Partitions must
be managed with the Windows-only configuration program, this tool can only
mount existing partitions.

**WARNING:** There is no compatibility with Windows clients, partitions must
be formated before use, deleting all existing data.

Commands
==============

The included utility "ut" supports the following commands:

#### listall
Display a listing of all discovered Netgear SC101's, along with their
IP address, firmware version, and created partitions.

#### attach
Attach a partition to a NBD device node on the local machine (i.e. /dev/nbd0).
After attaching the partition, it still needs to be mounted with the standard
"mount" command.

#### resolve
Display the IP address associated with a given partition ID.

Acknowledgements
==============

sc101-nbd was created by Iain Wade in 2007, his original code is available on
Google Code:

http://code.google.com/p/sc101-nbd/

Claudio Jolowicz made some fixes and modernizations and uploaded his fork to
GitHub in 2011.

License
==============

This program is free software; you can redistribute it and/or modify it under
the terms of the GNU General Public License version 2 as published by the Free
Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.

For details, see the file "COPYING" in the source directory.
