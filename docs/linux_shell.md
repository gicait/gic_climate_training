## What is Linux?

Just like Windows, iOS, and Mac OS, Linux is an operating system. In fact, one of the most popular platforms on the planet, Android, is powered by the Linux operating system. 

An operating system is software that manages all of the hardware resources associated with your desktop or laptop. To put it simply, the operating system manages the communication between your software and your hardware. Without the operating system (OS), the software wouldn’t function.



## Linux: Pros and Cons
| Pros                              | Cons                                          |
|-----------------------------------|-----------------------------------------------|
| Free and open-source              | Far too many different distributions          |
| Portable to any hardware platform | Not user friendly and confusing for beginners |
| Made to keep on running           | Is an open-source product trustworthy?        |
| Secure and versatile              |                                               |
| Scalable                          |                                               |
---
## Interaction with Linux
### The Shell
- Program that **interprets commands** and sends them to the OS
- Provides:
  - Built-in commands
  - Programming control structures
  - Environment vaiables
- Linux supports multiple shells such as **bash** ("**B**ourne-**a**gain **Sh**ell"), **csh** ("**C** **Sh**ell"), **tcsh** ("**T**ENEX **C** **Sh**ell"), and etc.

<div align=center>
<img width=\textwidth src="./_media/linux_shell.png"/>
<figcaption>An example of a Linux command window. Here it shows that the machine is running Ubuntu 20.4 OS, with a BASH shell.</figcaption>
</div>

---

### The "prompt"
<div align=center>
<img width=\textwidth src="./_media/linux_prompt.png"/>
</div>

---
### Command Basics
<div align=center>
<img width=\textwidth src="./_media/linux_command_basics.png"/>
</div>

---

### Commands: Hands-On
Once you have opened a Linux Command window, here are some commands you can try.
```console
username@system_name:~$ whoami  #my login
username@system_name:~$ hostname  #name of this computer
username@system_name:~$ echo "Hello, world!"  #print characters to screeen
username@system_name:~$ echo $HOME  #print environment variable
username@system_name:~$ echo my login is $(whoami)  #preplace $(xx) with program output
username@system_name:~$ date  #print currnt time/date
username@system_name:~$ cal #print this month-s calendar
username@system_name:~$ peekabop  #bad command/does not exist

```
<div align=center>
<img width=\textwidth src="./_media/linux_command_handson.png"/>
<figcaption>An example of outputs from the commands above.</figcaption>
</div>

---

## Navigating Linux's File System
- Directories (i.e. folders) are collections of files and other directories.
- Every directory has a parent except for the root directory.
- Many directories have subdirectories.
- Essential navigation commands:
  - **pwd** &emsp;  print current directory
  - **ls**  &emsp;  list files (filename)
  - **ll**  &emsp;  list files (details)
  - **cd**  &emsp;  change directory
  - **cp** &emsp; copy a file
  - **mv** &emsp; move or rename a file
  - **rm** &emsp; remove a file
  - **mkdir** &emsp; make a new directory(folder)
  - **df** &emsp; report on the system's disk space usage
  - **du** &emsp; report on the disk usage
 

| **Directory** | **Description** |
|---|---|
| **/ (root filesystem)** | The root filesystem is the top-level directory of the filesystem. It must contain all of the files required to boot the Linux system before other filesystems are mounted. It must include all of the required executables and libraries required to boot the remaining filesystems. After the system is booted, all other filesystems are mounted on standard, well-defined mount points as subdirectories of the root filesystem. |
| **/bin** | The /bin directory contains user executable files. |
| **/boot** | Contains the static bootloader and kernel executable and configuration files required to boot a Linux computer. |
| **/dev** | This directory contains the device files for every hardware device attached to the system. These are not device drivers, rather they are files that represent each device on the computer and facilitate access to those devices. |
| **/etc** | Contains the local system configuration files for the host computer. |
| **/home** | Home directory storage for user files. Each user has a subdirectory in /home. |
| **/lib** | Contains shared library files that are required to boot the system. |
| **/media** | A place to mount external removable media devices such as USB thumb drives that may be connected to the host. |
| **/mnt** | A temporary mountpoint for regular filesystems (as in not removable media) that can be used while the administrator is repairing or working on a filesystem. |
| **/opt** | Optional files such as vendor supplied application programs should be located here. |
| **/root** | This is not the root (/) filesystem. It is the home directory for the root user. |
| **/sbin** | System binary files. These are executables used for system administration. |
| **/tmp** | Temporary directory. Used by the operating system and many programs to store temporary files. Users may also store files here temporarily. Note that files stored here may be deleted at any time without prior notice. |
| **/usr** | These are shareable, read-only files, including executable binaries and libraries, man files, and other types of documentation. |
| **/var** | Variable data files are stored here. This can include things like log files, MySQL, and other database files, web server data files, email inboxes, and much more. |

<p>
  <div class="lightgallery" align=center>
    <a href="https://i.pinimg.com/originals/cd/e0/e9/cde0e9e9b0ea37f08710eba34a6773cf.png" data-sub-html="">
      <img alt="" src="https://i.pinimg.com/originals/cd/e0/e9/cde0e9e9b0ea37f08710eba34a6773cf.png" />
    </a>
    <figcaption>Linux's File System</figcaption>
  </div>
</p>