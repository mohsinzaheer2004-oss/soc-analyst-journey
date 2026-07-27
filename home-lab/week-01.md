# Week 1 — Home Lab Setup + Linux Basics

## Day 1 
- Set up VMware and installed a Linux VM for hands-on practice
- Practiced core Linux commands: navigating the filesystem (`cd`, `ls`, `pwd`),
  viewing/editing files (`cat`, `nano`), checking permissions (`ls -l`, `chmod`),
  and basic process management (`ps`, `top`)

## Day 2
- Studied the Linux file system hierarchy: `/`, `/home`, `/etc`, `/var`,
  `/bin`, `/usr`, `/tmp` — what each directory is for and why the structure
  matters for navigating a system quickly
- Learned how to use built-in help commands: `man <command>`,
  `<command> --help`, and `whatis <command>` to look up usage without
  needing to search online

## Day 3 
- Learned `sudo` — running commands with admin/root privileges
- Learned `apt` — installing, updating, and removing software packages on
  Debian/Ubuntu-based systems
- Learned `dpkg` — the lower-level tool `apt` is built on, used for
  installing/inspecting individual `.deb` package files
- Learned `git` — basic version control commands for tracking changes and
  pushing to repositories (the same tool behind this GitHub repo)
- Learned `pip` — installing and managing Python packages, which will be
  useful later for security scripts and automation

## Day 4 
- Learned how to manage running processes in Linux:
  - `kill` — stop a specific process using its process ID (PID)
  - `killall` — stop all processes matching a given name
  - `stop` / `Ctrl+Z` — pause (suspend) a running process
  - `start` / `fg` — resume a paused process, bringing it back to the
    foreground
  - `reset` — restore the terminal to its default state when the display
    gets messed up (e.g. after `cat`-ing a binary file)
- Practiced identifying process IDs with `ps` before targeting them with
  `kill`, instead of guessing
  
## Day 5 
- Learned text searching/processing commands:
  - `grep` — search for specific text patterns inside files (critical for
    log analysis later)
  - `find` — locate files/directories by name, type, or other attributes
  - `head` / `tail` — view the first/last lines of a file (useful for
    checking recent log entries without opening the whole file)
  - `wc` — count lines, words, and characters in a file
- Learned redirection and pipes:
  - `>` — send command output to a file (overwrite)
  - `>>` — append command output to a file
  - `|` — chain commands together, e.g. `cat file.txt | grep error` to
    filter output from one command through another
- Learned users & groups basics:
  - `useradd` — create a new user
  - `usermod` — modify an existing user's settings
  - `groups` — check which groups a user belongs to
  - `/etc/passwd` — the file listing all system users and their basic info

## Day 6 
- Learned disk/storage commands:
  - `df -h` — check disk space usage in human-readable format
  - `du -sh` — check the size of a specific file/folder
  - `mount` — view or attach storage devices/partitions to the filesystem
- Learned basic networking commands:
  - `ping` — test connectivity to another host
  - `ifconfig` / `ip a` — view network interfaces and IP addresses
  - `netstat` / `ss` — view active network connections and listening ports
  - `curl` — make requests to URLs/APIs directly from the terminal
- Learned where Linux logs live:
  - `/var/log/` — the main directory for system logs
  - `auth.log` — authentication/login events
  - `syslog` — general system activity log
- Learned `systemctl` — starting, stopping, and checking the status of
  services running on the system

## Notes / takeaways
This closes out the core Linux fundamentals — filesystem navigation, file
system hierarchy, help commands, package management, git, process control,
text processing, pipes/redirection, users & groups, disk/storage, basic
networking commands, and log locations. Enough of a foundation to move
into networking concepts next.

## Next up
Phase 1: Networking — OSI Model, TCP/IP, DNS, DHCP, HTTP/HTTPS, subnetting,
firewalls/VPNs/proxies
