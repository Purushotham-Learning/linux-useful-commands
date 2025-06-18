# Here’s a curated list of essential commands to investigate your Linux system, organized by category for clarity:

**System & Hardware Info**
uname -a          # Display kernel version & OS info
lscpu             # Show CPU architecture and specs
lsblk             # List block devices (disks, partitions)
lspci             # Show PCI devices (e.g., network, storage)
lsusb             # Show USB-connected devices
dmidecode -t memory # Show detailed RAM information
dmesg             # Display kernel and device initialization logs

**CPU, Memory & Performance**
top               # Real-time processes and resource usage
htop              # Interactive, enhanced version of top
vmstat            # Report CPU, memory, and I/O statistics
free -h           # Show memory and swap usage in human-readable format
iostat            # Report CPU and device I/O performance (requires sysstat)

**Disks & Filesystems**
df -h             # Disk space usage on all mounted filesystems
du -sh <path>     # Summarize disk usage for a directory
fsck              # Check and optionally repair filesystem (unmount first)
blkid             # Show block device attributes (UUID, type)
fdisk -l          # List partition tables on all disks
mount -a          # Mount everything defined in /etc/fstab
findmnt           # List all mounted filesystems in tree format

**Processes & Open Resources**
ps aux            # List all running processes
lsof              # List open files and sockets (e.g., to unmount busy volumes)
netstat -plntu    # Show network listening ports and associated processes
ss                # Modern socket statistics (alternative to netstat)

**Networking & Connections**
ping <host>       # Check reachability and packet loss
traceroute <host> # Trace network route to a host
mtr <host>        # Interactive traceroute + ping statistics
dig <domain>      # Query DNS records
nslookup <domain> # DNS lookup utility
arp -a            # Show ARP table entries
iftop / nethogs   # Monitor live network bandwidth usage by connection

**Diagnostic & Debugging**
strace -p <pid>   # Trace system calls of a running process
journalctl -xe    # View recent and detailed systemd logs
tail -f /var/log/syslog # Follow system logs in real-time

**General System Info**
uptime            # Show current uptime and load averages
w / who / users   # Show who’s logged in and what they’re doing
whoami            # Print current effective username
hostname          # Show or set system hostname
date              # Show current date and time
cal               # Display a calendar for the current month/year
compgen -c        # List all available shell commands

