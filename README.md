Linux Fundamentals And System Administration<img width="817" height="610" alt="image" src="https://github.com/user-attachments/assets/8491fc18-fd89-4318-9c17-14820e4600e6" />

Linux Fundamentals
Linux and its popularity: Linux is an open-source, Unix-like operating system built around the Linux kernel. It is widely used because it is free, highly secure, exceptionally stable, open-source, and scalable from tiny smart devices to massive cloud servers.
Kernel vs. Distribution: The kernel is the core component of the operating system that directly manages the computer's hardware and memory. A Linux distribution (distro) is a complete operating system package that bundles the Linux kernel with system utilities, package managers, desktop environments, and software applications.
Popular Distributions:
Ubuntu: Used heavily for personal desktop computing and cloud servers due to its user-friendliness and massive community support.
Red Hat Enterprise Linux (RHEL): Used primarily for enterprise and corporate environments because of its stability and paid commercial support.
Kali Linux: Used exclusively for digital forensics, penetration testing, and ethical hacking.
 Linux Filesystem
Root Directory (/): The absolute top-level directory in the Linux filesystem hierarchy. Every other file, directory, and mounted drive branches out from this single root.
/home vs. /root:
/home stores the personal files, documents, and configurations of regular users (e.g., /home/john).
/root is the exclusive, private home directory for the root (administrator) user.
System Configurations: The /etc directory stores system configuration files.
Log Files: The /var/log directory stores most log files.
Navigation and File Management
Display current directory: Use pwd (Print Working Directory).
Change directories: Use cd.
List directory contents: Use ls.
Create a new directory: Use mkdir.
Create an empty file: Use touch.
Copy, move, and delete:
cp copies files.
mv moves or renames files.
rm deletes files.
 Searching
find vs. grep: find searches for files and directories based on names, sizes, or dates. grep searches for specific text lines or patterns inside those files.
Search for files: Use find.
Search inside files: Use grep.
Wildcards: Wildcards (like * or ?) act as placeholders for unknown characters, allowing you to match multiple files at once (e.g., *.txt matches all text files).
 Basic Commands
echo: Prints text or variables to the terminal screen or redirects them into files.
history: Displays a list of previously executed commands in your current session.
Pipe operator (|): Takes the output of one command and passes it as the input to the next command (e.g., ls | grep "notes").
> vs. >>:
> overwrites the contents of a target file with the new data.
>> appends the new data to the end of the target file without erasing what is already there.
Manual pages: Use man <command> (e.g., man ls).

Users and Groups
Regular User vs. Root User: A regular user has restricted privileges and can only modify their own files. The root user is the all-powerful superuser with unrestricted access to modify any file, configuration, or system process.
Group: A collection of users bundled together to easily apply identical access permissions to multiple people at once.
sudo: Superuser Do. It lets permitted regular users execute commands with root privileges.
Current user information: Use id or whoami.
Permissions
r, w, and x:
r stands for read (view file content / list directory).
w stands for write (modify file content / add or delete files in a directory).
x stands for execute (run a file as a program / enter a directory).
File vs. Group Ownership: File ownership designates the specific single user who owns and controls the file. Group ownership assigns a specific user group to the file, defining access levels for everyone in that group.
Change permissions: Use chmod.
Change ownership: Use chown.
Important System Files
/etc/passwd: Stores basic user account details, including usernames, User IDs (UID), Group IDs (GID), home directory paths, and default shells.
/etc/shadow: Heavily protected because it stores the securely encrypted account passwords and password expiration data.
/var/log: Centralizes system, kernel, security, and application logs for troubleshooting and auditing.
System hostname file: The /etc/hostname file stores the hostname.
Installation Basics
Partition: A physically or logically isolated section of a hard drive treated by the OS as an independent storage unit.
Filesystem: The underlying structure and rules used by an operating system to organize, store, name, and retrieve files on a storage drive.
Swap Partition: Virtual memory space on a hard drive used as an overflow area when the system runs out of physical RAM.
ext4 popularity: It is the default filesystem for most Linux distros because it is highly reliable, fast, handles massive file sizes, and includes journaling to prevent data corruption during sudden crashes.


