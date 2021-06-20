# Usual linux commands

## General information

Sources:

* http://www.die.net/
* http://www.lanana.org/docs/device-list/devices-2.6+.txt
* http://www.tldp.org/LDP/sag/html/index.html
* https://www.kernel.org/doc/Documentation/
* http://refspecs.linuxfoundation.org/fhs.shtml
* http://refspecs.linuxfoundation.org/lsb.shtml

| Manual                     |     |
| -------------------------- | --- |
| `capabilities` (7)         | overview of Linux capabilities |
| `terminfo` (5)             | terminal capability data base |
| `cpuset` (7)               | confine processes to processor and memory node subsets |
| `mq_overview` (7)          | overview of POSIX message queues |
| `udev` (7)                 | Dynamic device management |

## System administration

### Low level (hardware, dev|ces, boot, kernel, etc.)

| Boot and systemd related   |     |
| -------------------------- | --- |
| `efibootmgr` (8)           | manipulate the EFI Boot Manager |
| `grub-mkconfig` (8)        | generate a GRUB configuration file |
| `systemctl` (1)            | Control the systemd system and service manager |
| `journalctl` (1)           | Query the systemd journal |

| Kernel related             |     |
| -------------------------- | --- |
| `lsinitramfs` (8)          | list content of an initramfs image |
| `dmesg` (1)                | print or control the kernel ring buffer |
| `depmod` (8)               | Generate modules.dep and map files. |
| `modprobe` (8)             | Add and remove modules from the Linux Kernel |
| `lsmod` (8)                | Show the status of modules in the Linux Kernel |
| `modinfo` (8)              | Show information about a Linux Kernel module |
| `sysctl` (2)               | read/write system parameters |
| `update-binfmts` (8)       | maintain registry of executable binary formats |

| Disk utils                 |     |
| -------------------------- | --- |
| `hdparm` (8)               | get/set SATA/IDE device parameters |
| `sdparm` (8)               | access SCSI modes pages; read VPD pages; send simple SCSI commands. |
| `smartctl` (8)             | Control and Monitor Utility for SMART Disks |

| Devices utils              |     |
| -------------------------- | --- |
| `blkid` (8)                | locate/print block device attributes |
| `blockdev` (8)             | call block device ioctls from the command line |
| `badblocks` (8)            | search a device for bad blocks |
| `ddrescue` (1)             | data recovery tool |
| `losetup` (8)              | set up and control loop devices |
| `dmsetup` (8)              | low level logical volume management |
| `mdadm` (8)                | manage MD devices aka Linux Software RAID |
| `cryptsetup` (8)           | manage plain dm-crypt and LUKS encrypted volumes |
| `lvm` (8)                  | LVM2 tools |
| `udisksctl` (8)            | The udisks command line tool |
| `udevadm` (8)              | udev management tool |

| Partitions and fs utils    |     |
| -------------------------- | --- |
| `cfdisk` (8)               | display or manipulate disk partition table |
| `cgdisk` (8)               | Curses-based GUID partition table (GPT) manipulator |
| `parted` (8)               | GNU Parted - a partition manipulation program |
| `fdisk` (8)                | manipulate disk partition table |
| `gdisk` (8)                | Interactive GUID partition table (GPT) manipulator |
| `gparted` (8)              | Gnome partition editor for manipulating disk partitions. |
| `sfdisk` (8)               | partition table manipulator for Linux |
| `mkswap` (8)               | set up a Linux swap area |
| `mkfs.*` (8)               | build a Linux filesystem |
| `fsck.*` (8)               | check and repair a Linux filesystem |
| `debugfs` (8)              | ext2/ext3/ext4 file system debugger |
| `dumpe2fs` (8)             | dump ext2/ext3/ext4 filesystem information |
| `fstrim` (8)               | discard unused blocks on a mounted filesystem |
| `mount` (8)                | mount a filesystem |
| `umount` (2)               | unmount filesystem |
| `findmnt` (8)              | find a filesystem |
| `swapon` (2)               | start/stop swapping to file/device |
| `swapoff` (2)              | start/stop swapping to file/device |
| `sync` (1)                 | flush file system buffers |

| System context - hardware  |     |
| -------------------------- | --- |
| `lscpu` (1)                | display information on CPU architecture |
| `lsblk` (8)                | list block devices |
| `lsdev` (8)                | display information about installed hardware |
| `lshw` (1)                 | list hardware |
| `lspci` (8)                | list all PCI devices |
| `lsusb` (8)                | list USB devices |
| `dmidecode` (8)            | DMI table decoder |
| `nproc` (1)                | print the number of processing units available |
| `hwclock` (8)              | read or set the hardware clock (RTC) |

| System context - software  |     |
| -------------------------- | --- |
| `date` (1)                 | print or set the system date and time |
| `timedatectl` (1)          | Control the system time and date |
| `arch` (1)                 | print machine hardware name (same as uname -m) |
| `uname` (1)                | print system information |
| `uptime` (1)               | Tell how long the system has been running. |
| `hostname` (1)             | show or set the system's host name |
| `hostnamectl` (1)          | Control the system hostname |
| `hostid` (1)               | print the numeric identifier for the current host |
| `locale` (1)               | get locale-specific information |
| `localectl` (1)            | Control the system locale and keyboard layout settings |
| `localedef` (1)            | compile locale definition files |
| `ldconfig` (8)             | configure dynamic linker run-time bindings |
| `lsb_release` (1)          | print distribution-specific information |
| `getconf` (1)              | Query system configuration variables |
| `getent` (1)               | get entries from Name Service Switch libraries |

| Network/sockets utils      |     |
| -------------------------- | --- |
| `ethtool` (8)              | query or control network driver and hardware settings |
| `mmcli` (8)                | Control and monitor the ModemManager |
| `ip` (8)                   | show / manipulate routing, devices, policy routing and tunnels |
| `iw` (8)                   | show / manipulate wireless devices and their configuration |
| `ss` (8)                   | another utility to investigate sockets |
| `tcpdump` (1)              | dump traffic on a network |
| `ping` (8)                 | send ICMP ECHO_REQUEST to network hosts |
| `traceroute` (1)           | print the route packets trace to network host |
| `dig` (1)                  | DNS lookup utility |
| `nc` (1)                   | TCP/IP swiss army knife |
| `telnet` (1)               | User interface to TELNET |
| `nmap` (1)                 | Network exploration tool and security / port scanner |
| `iptables` (8)             | administration tool for IPv4/IPv6 packet filtering and NAT |

| Disk usage                 |     |
| -------------------------- | --- |
| `df` (1)                   | report file system disk space usage |
| `du` (1)                   | estimate file space usage |
| `ncdu` (1)                 | NCurses Disk Usage |
| `stat` (1)                 | display file or file system status |
| `gdmap` (1)                | Graphical Disk Map |
| `truncate` (1)             | shrink or extend the size of a file to the specified size |

| Monitoring/perf utils      |     |
| -------------------------- | --- |
| `atop` (1)                 | AT Computing's System & Process Monitor |
| `htop` (1)                 | interactive process viewer |
| `top` (1)                  | display Linux processes |
| `acpi` (1)                 | Shows battery status and other ACPI information |
| `acpid` (8)                | Advanced Configuration and Power Interface event daemon |
| `sar` (1)                  | Collect, report, or save system activity information. |
| `sensors` (1)              | print sensors information |
| `perf` (1)                 | performance analysis tools for Linux |
| `sysbench` (1)             | A modular, cross-platform and multi-threaded benchmark tool. |
| `stress-ng` (1)            | a tool to load and stress a computer system |

| Monitoring/perf (cpu/load) |     |
| -------------------------- | --- |
| `mpstat` (1)               | Report processors related statistics. |
| `tload` (1)                | graphic representation of system load average |
| `i7z` (1)                  | A better i7 (and now i3, i5) reporting tool for Linux. |

| Monitoring/perf (io)       |     |
| -------------------------- | --- |
| `iotop` (8)                | simple top-like I/O monitor |
| `iostat` (1)               | Report Central Processing Unit (CPU) statistics and input/output statistics for devices and partitions. |
| `cifsiostat` (1)           | Report CIFS statistics. |
| `nfsiostat` (8)            | Emulate iostat for NFS mount points using /proc/self/mountstats |

| Monitoring/perf (network)  |     |
| -------------------------- | --- |
| `iftop` (8)                | display bandwidth usage on an interface by host |
| `iptraf` (8)               | Interactive Colorful IP LAN Monitor |
| `iperf3` (1)               | perform network throughput tests |

| Monitoring/perf (ps)       |     |
| -------------------------- | --- |
| `ps` (1)                   | report a snapshot of the current processes. |
| `pstree` (1)               | display a tree of processes |
| `pidstat` (1)              | Report statistics for Linux tasks. |
| `lsof` (8)                 | list open files |
| `fuser` (1)                | identify processes using files or sockets |

| Monitoring/perf (memory)   |     |
| -------------------------- | --- |
| `vmstat` (8)               | Report virtual memory statistics |
| `free` (1)                 | Display amount of free and used memory in the system |

### High level (files, proc e|ses, users, etc.)

| File attributes            |     |
| -------------------------- | --- |
| `chown` (1)                | change file owner and group |
| `chgrp` (1)                | change group ownership |
| `chmod` (1)                | change file mode bits |
| `touch` (1)                | change file timestamps |
| `setcap` (8)               | set file capabilities |
| `getfacl` (1)              | get file access control lists |
| `setfacl` (1)              | set file access control lists |
| `lsattr` (1)               | list file attributes on a Linux second extended file system |
| `chattr` (1)               | change file attributes on a Linux file system |

| Process control            |     |
| -------------------------- | --- |
| `pidof` (8)                | find the process ID of a running program. |
| `pgrep` (1)                | look  up  or signal processes based on name and other attributes |
| `pkill` (1)                | look up or signal processes based on name and other attributes |
| `kill` (1)                 | send a signal to a process |
| `killall` (8)              | kill processes by name |
| `pmap` (1)                 | report memory map of a process |
| `taskset` (1)              | retrieve or set a process's CPU affinity |
| `strace` (1)               | trace system calls and signals |

| Debian package mngt        |     |
| -------------------------- | --- |
| `apt-get` (8)              | APT package handling utility - command-line interface |
| `apt-cache` (8)            | APT package handling utility -- cache manipulator |
| `apt-key` (8)              | APT key management utility |
| `dpkg` (1)                 | package manager for Debian |
| `dpkg-reconfigure` (8)     | reconfigure an already installed package |

| User info/manip            |     |
| -------------------------- | --- |
| `id` (1)                   | print real and effective user and group IDs |
| `logname` (1)              | print user's login name |
| `whoami` (1)               | print effective userid |
| `groups` (1)               | display current group names |
| `who` (1)                  | show who is logged on |
| `w` (1)                    | Show who is logged on and what they are doing. |
| `users` (1)                | print the user names of users currently logged in to the current host |
| `last` (1)                 | show a listing of last logged in users |
| `lastb` (1)                | show a listing of last logged in users |
| `lastlog` (8)              | reports the most recent login of all users or of a given user |
| `useradd` (8)              | create a new user or update default new user information |
| `userdel` (8)              | delete a user account and related files |
| `usermod` (8)              | modify a user account |
| `groupadd` (8)             | create a new group |
| `groupdel` (8)             | delete a group |
| `groupmod` (8)             | modify a group definition on the system |
| `passwd` (1)               | change user password |
| `chfn` (1)                 | change real user name and information |
| `chage` (1)                | change user password expiry information |
| `su` (1)                   | change user ID or become superuser |
| `sudo` (8)                 | execute a command as another user |
| `pwck` (8)                 | verify integrity of password files |
| `grpck` (8)                | verify integrity of group files |

## User misc

### File manipulation

| Output of entire files     |     |
| -------------------------- | --- |
| `cat` (1)                  | concatenate files and print on the standard output |
| `strings` (1)              | print the strings of printable characters in files. |
| `nl` (1)                   | number lines of files |
| `tac` (1)                  | concatenate and print files in reverse |
| `rev` (1)                  | reverse lines characterwise |
| `od` (1)                   | dump files in octal and other formats |
| `base64` (1)               | base64 encode/decode data and print to standard output |
| `xxd` (1)                  | make a hexdump or do the reverse. |
| `hexdump` (1)              | ASCII, decimal, hexadecimal, octal dump |
| `iconv` (1)                | Convert encoding of given files from one encoding to another |
| `uconv` (1)                | convert data from one encoding to another |
| `uuencode` (1)             | encode a file into email friendly text |

| Formatting file contents   |     |
| -------------------------- | --- |
| `fmt` (1)                  | simple optimal text formatter |
| `pr` (1)                   | convert text files for printing |
| `fold` (1)                 | wrap each input line to fit in specified width |

| Output of parts of files   |     |
| -------------------------- | --- |
| `head` (1)                 | output the first part of files |
| `tail` (1)                 | output the last part of files |
| `split` (1)                | split a file into pieces |
| `csplit` (1)               | split a file into sections determined by context lines |

| Operating on characters    |     |
| -------------------------- | --- |
| `tr` (1)                   | translate or delete characters |
| `expand` (1)               | convert tabs to spaces |
| `unexpand` (1)             | convert spaces to tabs |

| Operating on fields        |     |
| -------------------------- | --- |
| `cut` (1)                  | remove sections from each line of files |
| `paste` (1)                | merge lines of files |
| `join` (1)                 | join lines of two files on a common field |
| `colrm` (1)                | remove columns from a file |
| `column` (1)               | columnate lists |

| Operating on sorted files  |     |
| -------------------------- | --- |
| `sort` (1)                 | sort lines of text files |
| `shuf` (1)                 | generate random permutations |
| `uniq` (1)                 | report or omit repeated lines |
| `comm` (1)                 | compare two sorted files line by line |
| `ptx` (1)                  | produce a permuted index of file contents |
| `tsort` (1)                | perform topological sort |

| Summarizing/cmpring files  |     |
| -------------------------- | --- |
| `wc` (1)                   | print newline, word, and byte counts for each file |
| `sum` (1)                  | checksum and count the blocks in a file |
| `cksum` (1)                | checksum and count the bytes in a file |
| `b2sum` (1)                | compute and check BLAKE2 message digest |
| `md5sum` (1)               | compute and check MD5 message digest |
| `sha(1|256|512)sum` (1)    | compute and check SHA message digest |
| `cmp` (1)                  | compare two files byte by byte |
| `diff` (1)                 | compare files line by line |
| `sdiff` (1)                | side-by-side merge of file differences |
| `patch` (1)                | apply a diff file to an original |

| File compression           |     |
| -------------------------- | --- |
| `atool` (1)                | A script for managing file archives of various types |
| `aunpack` (1)              | A script for managing file archives of various types |
| `apack` (1)                | A script for managing file archives of various types |
| `als` (1)                  | A script for managing file archives of various types |
| `acat` (1)                 | A script for managing file archives of various types |
| `adiff` (1)                | A script for managing file archives of various types |
| `arepack` (1)              | A script for managing file archives of various types |
| `cpio` (1)                 | copy files to and from archives |
| `gunzip` (1)               | compress or expand files |
| `gzip` (1)                 | compress or expand files |
| `zforce` (1)               | force a '.gz' extension on all gzip files |
| `shar` (1)                 | create a shell archive |

| File name manipulation     |     |
| -------------------------- | --- |
| `basename` (1)             | strip directory and suffix from filenames |
| `dirname` (1)              | strip last component from file name |
| `pathchk` (1)              | check whether file names are valid or portable |
| `mktemp` (1)               | create a temporary file or directory |
| `realpath` (1)             | print the resolved path |
| `rename` (1)               | renames multiple files |

### Shell

| Common utils               |     |
| -------------------------- | --- |
| `ls` (1)                   | list directory contents |
| `dircolors` (1)            | color setup for ls |
| `cp` (1)                   | copy files and directories |
| `mv` (1)                   | move (rename) files |
| `rm` (1)                   | remove files or directories |
| `shred` (1)                | overwrite a file to hide its contents, and optionally delete it |
| `tee` (1)                  | read from standard input and write to standard output and files |
| `dd` (1)                   | convert and copy a file |
| `flock` (1)                | manage locks from shell scripts |
| `help` (built-in)          | show bash built-ins |

| Special file types         |     |
| -------------------------- | --- |
| `ln` (1)                   | make links between files |
| `mkdir` (1)                | make directories |
| `mkfifo` (1)               | make FIFOs (named pipes) |
| `mknod` (1)                | make block or character special files |
| `readlink` (1)             | print resolved symbolic links or canonical file names |
| `rmdir` (1)                | remove empty directories |

| Printing text              |     |
| -------------------------- | --- |
| `echo` (1)                 | display a line of text |
| `printf` (1)               | format and print data |
| `yes` (1)                  | output a string repeatedly until killed |

| Conditions                 |     |
| -------------------------- | --- |
| `false` (1)                | do nothing, unsuccessfully |
| `true` (1)                 | do nothing, successfully |
| `test` (1)                 | check file types and compare values |
| `expr` (1)                 | evaluate expressions |

| Numeric operations         |     |
| -------------------------- | --- |
| `seq` (1)                  | print a sequence of numbers |
| `factor` (1)               | factor numbers |
| `numfmt` (1)               | Convert numbers from/to human-readable strings |
| `bc` (1)                   | An arbitrary precision calculator language |

| Working context/env        |     |
| -------------------------- | --- |
| `cd` (1)                   | change the working directory |
| `pwd` (1)                  | print name of current/working directory |
| `printenv` (1)             | print all or part of environment |
| `envsubst` (1)             | substitutes environment variables in shell format strings |
| `tty` (1)                  | print the file name of the terminal connected to standard input |
| `ischroot` (1)             | detect if running in a chroot |
| `ipcs` (1)                 | provide information on ipc facilities |
| `ipck` (1)                 | create various ipc resources |
| `ipcrm` (1)                | remove a message queue, semaphore set or shared memory id |

| Modify command invocation  |     |
| -------------------------- | --- |
| `chroot` (8)               | run command or interactive shell with special root directory |
| `fakeroot` (1)             | run a command in an environment faking root privileges for file manipulation |
| `env` (1)                  | run a program in a modified environment |
| `nice` (1)                 | run a program with modified scheduling priority |
| `chrt` (1)                 | manipulate real-time attributes of a process |
| `nohup` (1)                | run a command immune to hangups, with output to a non-tty |
| `stdbuf` (1)               | Run COMMAND, with modified buffering operations for its standard streams. |
| `timeout` (1)              | run a command with a time limit |
| `time` (1)                 | run programs and summarize system resource usage |

| Delay, reschedule, repeat  |     |
| -------------------------- | --- |
| `at` (1)                   | queue, examine or delete jobs for later execution |
| `batch` (1)                | queue, examine or delete jobs for later execution |
| `crontab` (1)              | maintains crontab files for individual users |
| `sleep` (1)                | delay for a specified amount of time |
| `watch` (1)                | execute a program periodically, showing output fullscreen |

| Misc                       |     |
| -------------------------- | --- |
| `grep` (1)                 | print lines matching a pattern |
| `look` (1)                 | display lines beginning with a given string |
| `locate` (1)               | find files by name |
| `updatedb` (1)             | update a database for mlocate |
| `find` (1)                 | search for files in a directory hierarchy |
| `xargs` (1)                | build and execute command lines from standard input |
| `cal` (1)                  | display a calendar |
| `file` (1)                 | determine file type |
| `mimetype` (1)             | Determine file type |
| `namei` (1)                | follow a pathname until a terminal point is found |
| `logger` (1)               | enter messages into the system log |
| `openssl` (1)              | OpenSSL command line tool |
| `pv` (1)                   | monitor the progress of data through a pipe |
| `uuidgen` (1)              | create a new UUID value |
| `wall` (1)                 | write a message to all users |

### Topics

| Compilation                |     |
| -------------------------- | --- |
| `ar` (1)                   | create, modify, and extract from archives |
| `cmake` (1)                | CMake Command-Line Reference |
| `gcc` (1)                  | GNU project C and C++ compiler |
| `ld` (1)                   | The GNU linker |
| `ldd` (1)                  | print shared library dependencies |
| `make` (1)                 | GNU make utility to maintain groups of programs |
| `nm` (1)                   | list symbols from object files |
| `objcopy` (1)              | copy and translate object files |
| `objdump` (1)              | display information from object files. |
| `od` (1)                   | dump files in octal and other formats |
| `size` (1)                 | list section sizes and total size. |
| `strip` (1)                | Discard symbols from object files. |
| `addr2line` (1)            | convert addresses into file names and line numbers. |

| Terminal utils             |     |
| -------------------------- | --- |
| `tset` (1)                 | terminal initialization |
| `reset` (1)                | terminal initialization |
| `tput` (1)                 | initialize a terminal or query terminfo database |
| `tic` (1)                  | the terminfo entry-description compiler |
| `infocmp` (1)              | compare or print out terminfo descriptions |
| `loadkeys` (1)             | load keyboard translation tables |
| `showkey` (1)              | examine the codes sent by the keyboard |
| `dumpkeys` (1)             | dump keyboard translation tables |
| `getkeycodes` (8)          | print kernel scancode-to-keycode mapping table |
| `script` (1)               | make typescript of terminal session |
| `stty` (1)                 | change and print terminal line settings |

| Login/shell utils          |     |
| -------------------------- | --- |
| `agetty` (8)               | alternative Linux getty |
| `chsh` (1)                 | change login shell |
| `clear` (1)                | clear the terminal screen |
| `screen` (1)               | screen manager with VT100/ANSI terminal emulation |
| `tmux` (1)                 | terminal multiplexer |
| `login` (1)                | begin session on the system |
| `openvt` (1)               | start a program on a new virtual terminal (VT) |
| `ssh` (1)                  | OpenSSH SSH client (remote login program) |
| `ssh-add` (1)              | adds private key identities to the authentication agent |
| `ssh-agent` (1)            | authentication agent |
| `ssh-keygen` (1)           | authentication key generation, management and conversion |
| `ssh-keyscan` (1)          | gather ssh public keys |

| Url manip (transfer, bck)  |     |
| -------------------------- | --- |
| `scp` (1)                  | secure copy (remote file copy program) |
| `borg` (1)                 | deduplicating and encrypting backup tool |
| `rsync` (1)                | a fast, versatile, remote (and local) file-copying tool |
| `sftp` (1)                 | secure file transfer program |
| `curl` (1)                 | transfer a URL |
| `wget` (1)                 | The non-interactive network downloader |

| File viewers/editors       |     |
| -------------------------- | --- |
| `more` (1)                 | file perusal filter for crt viewing |
| `less` (1)                 | file perusal filter for crt viewing |
| `sed` (1)                  | stream editor for filtering and transforming text |
| `awk` (1)                  | pattern scanning and text processing language |
| `vim` (1)                  | Vi IMproved, a programmers text editor |
| `vimdiff` (1)              | edit two, three or four versions of a file with Vim and show differences |

| Executables' information   |     |
| -------------------------- | --- |
| `apropos` (1)              | search the manual page names and descriptions |
| `man` (1)                  | an interface to the on-line reference manuals |
| `manpath` (1)              | determine search path for manual pages |
| `which` (1)                | locate a command |
| `whatis` (1)               | display manual page descriptions |
| `whereis` (1)              | locate the binary, source, and manual page files for a command |

### Desktop

| X-related                  |     |
| -------------------------- | --- |
| `arandr` (1)               | visual front end for XRandR 1.2 |
| `xrandr` (1)               | primitive command line interface to RandR extension |
| `setxkbmap`                | set the keyboard using the X Keyboard Extension |
| `xev` (1)                  | print contents of X events |
| `xmodmap` (1)              | utility for modifying keymaps and pointer button mappings in X |
| `xbacklight` (1)           | adjust backlight brightness using RandR extension |
| `xdotool` (1)              | command-line X11 automation tool |
| `xprop` (1)                | property displayer for X |
| `xdg-mime` (1)             | command line tool for querying information about file type handling |
| `xdg-open` (1)             | opens a file or URL in the user's preferred application |
| `xlsfonts` (1)             | server font list displayer for X |
| `xrdb` (1)                 | X server resource database utility |
| `xset` (1)                 | user preference utility for X |
| `xwd` (1)                  | dump an image of an X window |
| `xwdtopnm` (1)             | convert a X11 or X10 window dump file into a portable anymap |
| `import` (1)               | saves any visible window on an X server and outputs it as an image file |

| Audio/video/graphics utils |     |
| -------------------------- | --- |
| `pacmd` (1)                | Reconfigure a PulseAudio sound server during runtime |
| `pactl` (1)                | Control a running PulseAudio sound server |
| `sox` (1)                  | Sound eXchange, the Swiss Army knife of audio manipulation |
| `mediainfo` (1)            | command line utility to display information about audio/video files |
| `abcde` (1)                | Grab an entire CD and compress it |
| `cdparanoia` (1)           | an audio CD reading utility which includes extra data verification features |
| `flac` (1)                 | Free Lossless Audio Codec |
| `metaflac` (1)             | program to list, add, remove, or edit metadata in one or more FLAC files. |
| `id3v2` (1)                | Adds/Modifies/Removes/Views id3v2 tags, converts/lists id3v1 tags |
| `avconv` (1)               | avconv video converter |
| `ffmpeg` (1)               | ffmpeg video converter |
| `mplayer` (1)              | movie player |
| `mencoder` (1)             | movie encoder |
| `vlc` (1)                  | the VLC media player |
| `feh` (1)                  | image viewer and cataloguer |
| `convert` (1)              | convert between image formats as well as resize an image, blur, crop, etc. |
| `mogrify` (1)              | resize an image, blur, crop, etc. |

| Office utils               |     |
| -------------------------- | --- |
| `pdftk` (1)                | A handy tool for manipulating PDF |
| `evince` (1)               | GNOME document viewer |
| `libreoffice` (1)          | LibreOffice office suite |
| `gap` (1)                  | Groups, Algorithms and Programming |

| Fonts                      |     |
| -------------------------- | --- |
| `fc-cat` (1)               | read font information cache files |
| `fc-cache` (1)             | build font information cache files |
| `fc-list` (1)              | list available fonts |
| `fc-match` (1)             | match available fonts |
| `fc-pattern` (1)           | parse and show pattern |
| `fc-query` (1)             | query font files |
| `fc-scan` (1)              | scan font files or directories |
| `gucharmap` (1)            | Unicode character picker and font browser |
| `mkfontscale` (1)          | create an index of scalable font files for X |
| `mkfontdir` (1)            | create an index of X font files in a directory |
| `unicode` (1)              | command line unicode database query tool |

## Pseudo file system

| Path                                  |     |
| ------------------------------------- | --- |
| /proc/sys/kernel/random/entropy_avail |     |
| /proc/sys/fs/binfmt_misc              | Kernel Support for miscellaneous Binary Formats |
