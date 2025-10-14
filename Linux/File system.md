#### **/**
Root of the entire filesystem. Everything lives under it.

#### **/bin**
Essential user binaries (e.g. ls, cp, mv, bash). Needed even in recovery mode.

#### **/sbin**
System binaries. Admin commands like reboot, shutdown, mount.

#### **/etc**
System configuration files. Editable text files. Includes network config, user accounts, system services.

#### **/dev**
Device files — everything is a file in Linux. Includes hard drives, USB, terminals.

#### **/proc**
Virtual filesystem for kernel and process info. Dynamic. Use cat /proc/cpuinfo, cat /proc/meminfo.

#### **/sys**
Like /proc, but for hardware. Interfaces with devices, drivers, and kernel modules.

#### **/var**
Variable data: logs, mail, spool files, caches. Includes /var/log, /var/tmp.

#### **/tmp**
Temporary files. Auto-cleared on reboot. World-writable.

#### **/usr**
User-level programs and data. Includes:

- /usr/bin: most user commands
    
- /usr/lib: libraries
    
- /usr/share: icons, docs, etc.
    

#### **/home**
User home directories. Your personal files live in /home/yourname.

#### **/root**
Home directory for the root user. Separate from normal /home.

#### **/media**

####  **and** 

#### **/mnt**
Mount points for removable drives, network shares.