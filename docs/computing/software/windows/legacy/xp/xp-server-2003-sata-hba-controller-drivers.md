# SATA/HBA controller drivers
Slipstreaming AHCI SATA/HBA controller drivers into XP/Server 2003 installation media using
nLite is already very well-documented, so I'm not gonna go over that again. But what drivers
to slipstream?

Intel AHCI/RAID controller:

* [Generic textmode drivers version 11.2.0.1006 modded and signed by Fernando](https://winraid.level1techs.com/t/25310),
worked on my Gigabyte B75M-D3H motherboard (Intel B75 chipset)

LSI SAS 2308/9207-8i/9217-8i HBA:

* [Dell driver for Precision **610 workstations](https://www.dell.com/support/home/en-us/drivers/driversdetails?driverid=ccgm0),
worked on my Inspur YPCB-00227-1P2 (rebranded LSI SAS 9207-8i) HBA