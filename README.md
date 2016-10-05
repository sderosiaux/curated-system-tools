A list of tools to help debugging issues or simply check what's going on in the system.

## Classic

> Linux is assumed. On OSX, options can be way different.

- `top cw` : something's taking up all the cpu or mem ?
- `htop` : a colorful top, easy to play with
- `ps fauxww` : list of all processes with command line + hierarchy
- `free -h` : memory and swap

## System resources

List of tools used to look after system performances (mem, cpu, disks, network, processes, files..) :

- [sysdig](http://www.sysdig.org/) : a console ui to monitor (live and snapshots) several aspects of the system
- [iostat](http://linuxcommand.org/man_pages/iostat1.html) : i/o accesses `iostat -m -x -d 2`
- [vmstat](http://linuxcommand.org/man_pages/vmstat8.html) : mem/swap/cpu `vmstat 1`
- [ifstat](https://linux.die.net/man/1/ifstat) : like iostat, vmstat, but for network interfaces
- [netstat](https://linux.die.net/man/8/netstat) : details about all the network connections of the system
- [dstat](http://dag.wiee.rs/home-made/dstat/) :  *stat all-in-one
- [sar](http://linuxcommand.org/man_pages/sar1.html) : monitor network, devices `sar -n DEV 2`
- [iotop](http://guichaz.free.fr/iotop/) : top, with i/o !
- [iperf](https://iperf.fr/) : test maximum bandwidth (tcp/udp) `iperf -c server -f m -d`

## System devices

- [hdparm](https://linux.die.net/man/8/hdparm) : check drives settings `hdparm -t /dev/sda8`
- [ethtool](http://linuxcommand.org/man_pages/ethtool8.html) : check the ethernet cards settings (speed, duplex etc. if you have a doubt) `ethtool eth0`

## Java specifics

- [jstat](http://docs.oracle.com/javase/8/docs/technotes/guides/troubleshoot/tooldescr017.html) : like iostat, vmstat, for java processes `jstat -gc -t -h30 [vmid] 1s : monitor Java GC`
- [jvisualvm](https://visualvm.github.io/) : packaged with java, ultra useful
- [jmc](https://docs.oracle.com/javacomponents/jmc-5-5/jmc-user-guide/jmc.htm) : Java Mission Control. A better jvisualvm


## System tuning

`/proc/sys/vm/vfs_cache_pressure`
`/proc/sys/vm/swappiness`

## Misc info

`cat /proc/cpuinfo` : list of cpus of the system with details (type, MHz, cache size..)

