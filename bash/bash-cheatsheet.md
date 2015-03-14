Bash Cheatsheet
===============

Symbolic Links
--------------

Make a symbolic link

    ln -s /path/to/file /path/to/symlink

Calendar
--------

Display the current month

    cal

Display the whole year

    cal 2015

ssh
---

To login to remote server

    ssh username@remotehostname

To make an ssh key

    ssh-keygen

To send an ssh key

    ssh-copy-key username@remotehostname

scp
---

#### Useful refernce: [man](http://dell9.ma.utexas.edu/cgi-bin/man-cgi?00+00), [scp syntax](http://www.hypexr.org/linux_scp_help.php)

Copy the file "foobar.txt" from a remote host to the local host

    scp your_username@remotehost.edu:foobar.txt /some/local/directory

Copy the file "foobar.txt" from the local host to a remote host

    scp foobar.txt your_username@remotehost.edu:/some/remote/directory

Copy the directory "foo" from the local host to a remote host's directory "bar"

    scp -r foo your_username@remotehost.edu:/some/remote/directory/bar

Copy the file "foobar.txt" from the local host to a remote host using port 2264

    scp -P 2264 foobar.txt your_username@remotehost.edu:/some/remote/directory

Using globs with scp and zsh
    scp your_username@remotehost.edu:\*.txt /some/local/directory
