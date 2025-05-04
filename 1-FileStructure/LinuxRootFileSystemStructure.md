## Linux Root File System Structure

- `/` - The root directory . Everything starts from here.
- `/bin`  - Essential binaries (executables), like ls, cp, mv. Needed for basic system operation.
- `/boot` - Files needed to boot the system, including the Linux kernel and GRUB bootloader files.
- `/dev` - Contains device files for hardware devices, e.g., /dev/sda for a disk.
- `/etc` - System-wide configuration files. E.g., /etc/passwd, /etc/fstab.
- `/home` - User Home Directories.
- `/lib` - Libraries needed by binaries in /bin and /sbin. Like DLLs on Windows.
- `/media` - Mount point for external devices (USB, CD-ROM, etc.) automatically mounted.
- `/mnt` - 	Temporarily mounted filesystems. Often used for manual mounting.
- `/opt` - Optional application software packages. Third-party software might go here.
- `/proc`- Virtual filesystem providing process and system info (like CPU, memory).
- `/run` - Stores runtime data since the last boot (like PID files).
- `/sbin` - System binaries for superuser (like ifconfig, reboot). Not meant for regular users.
- `/srv` - Service data (like web or FTP servers' data). Rarely used directly.
- `/sys` - Interface to the kernel. Like /proc, used for system management.
- `/tmp` - Temporary files. Often cleared on reboot.
- `/usr` - User-installed software and libraries. Subdirectories include:
* /usr/bin: Non-essential user binaries
* /usr/lib: Libraries for /usr/bin
* /usr/include: Header files for C programming
* /usr/share: Architecture-independent data
 | /var | Variable data like logs (/var/log), mail, and spool files. |