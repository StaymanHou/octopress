---
layout: post
title: "Practical Linux - Part 06 - File System | 文件系统"
date: 2014-10-15 02:05:44 +0000
comments: true
categories: [Linux]
keywords: "linux, file system"
---
{% youtube KgzayvsMaHc %}
<!-- more -->
- Oct 9 - File System
  - User/Group/Other
    - `users`
    - `groups`
    - `ls -al`
    - *root
    - /etc/passwd & /etc/group & /etc/shadow
  - File property
    - `ls -al`
    - i-node
    - permission - type user-rwx group -rwx other -rwx
      - set uid, set guid, set bit
      - /tmp, /usr/bin/passwd
    - size `-h`
    - time
    - . hidden file
  - Modify
    - `chown`
    - `chgrp`
    - `chmod`
  - File Type
    - - regular file
    - d directory
    - l link
    - b/c device
    - s sockets
    - p pipe
  - Extension
    - *.sh *.tar *.html *.php
  - System Directories
    - root /
      - /bin
      - /boot
      - /dev
      - /etc
      - /home
      - /lib
      - /media
      - /mnt
      - /opt
      - /root
      - /sbin
      - /tmp
      - /proc
    - /usr - shareable, static
    - /var - vary - cache, log, lock, run file & mysql db
  - directory tree | absolute & relative path
    - . & ..
  - Mount
    - `df`
    - /etc/fstab & /etc/mtab
  - Arhcive
    - Tar
      - `tar zcvfp`
      - `tar zxqf`
    - Dump
      - `dump`
      - backup level
        - full | incremental | differentiate backup
  - Commands
    - `cd`
    - `pwd`
    - `mkdir`
    - `echo $PATH`
    - `ls`
    - `cp`
    - `mv`
    - `rm`
    - `cat` `tac` `more` `less` `head` `tail`
    - `touch`
    - `ln`
      - hard link
      - soft link / symbolic link
    - `df`
    - `du`
    - `mount` `umount`
  - Practice
  - Assignment
    - log on your amazon vm
    - create a directory 'oct9' under your home
    - under the new directory, create a new file 'changemypermission', and change it's permission to '-rwxr-xr--'
    - under the new directory, create a new file 'changemyownnership', and change it's ownership to 'stayman:root'
    - under the new directory, create a hidden file, pick any filename you like
    - under the new directory, create a soft link / symbolic link 'mypasswdlink', pointing '/etc/passwd'
    - under your home directory, use tar to compress the new directory into a file 'oct9.tar.gz'
    - under your home directory, delete the file 'touchme.txt', which you created in the last assignment