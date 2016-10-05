# system-performances-tools

## Classic

> A linux is assumed. On OSX, options can be way different.

- `top cw` : something's taking up all the cpu or mem ?
- `htop` : a colorful top, easy to play with
- `ps fauxww` : list of all processes with command line + hierarchy

## System resources

List of tools used to look after system performances (mem, cpu, disks, network, processes, files..) :

- [sysdig](http://www.sysdig.org/) : a console ui to monitor (live and snapshots) several aspects of the system
- [iostat](http://linuxcommand.org/man_pages/iostat1.html) : i/o accesses
- [vmstat](http://linuxcommand.org/man_pages/vmstat8.html) : mem/swap/cpu
- [ifstat](https://linux.die.net/man/1/ifstat) : like iostat, vmstat, but for network interfaces
- [netstat](https://linux.die.net/man/8/netstat) : details about all the network connections of the system
- [dstat](http://dag.wiee.rs/home-made/dstat/) :  *stat all-in-one
- [sar](http://linuxcommand.org/man_pages/sar1.html) : monitor network, devices
- [iotop](http://guichaz.free.fr/iotop/) : top, with i/o !
- [iperf](https://iperf.fr/) : test maximum bandwidth (tcp/udp)


## Java specifics

- [jstat](http://docs.oracle.com/javase/8/docs/technotes/guides/troubleshoot/tooldescr017.html) : like iostat, vmstat, for java processes. eg: `jstat -gc -t -h30 [vmid] 1s : monitor Java GC`
- [jvisualvm](https://visualvm.github.io/) : packaged with java, ultra useful
- [jmc](https://docs.oracle.com/javacomponents/jmc-5-5/jmc-user-guide/jmc.htm) : Java Mission Control. A better jvisualvm

