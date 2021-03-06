# Linux, Apache, MySQL, PHP (LAMP) tasks automation scripts

If you are a "Lazy LAMP" developer who wants to run few script to get things done with no pain, then this repository is for you. This is a collection of few scripts (that I'll keep adding to) that automates few installation commands and tasks for your LAMP environment.

These script assumes few things up:

1. You have root access to the server / machine you are running the scripts on (You will be asked for the root password when needed)
2. You are running these scripts on a Debian Linux distribution (Eg. Ubuntu) 


### Install:

1. Check a clone of this repo: `git clone https://github.com/aymanrb/lazy-lamp.git`
2. Run `echo "alias lazy-lamp=\"sudo bash $PWD/lazy-lamp/lazy-lamp.sh\"" | tee -a ~/.bashrc` (To create an easy access alias of the main script, if you are using ZSH instead of bash you should replace the file with `~/.zshrc` instead of ~/.bashrc)
3. Run `lazy-lamp` or `bash /path/to/lazy-lamp/lazy-lamp.sh` and select your desired script from the index list to run.

### Usage:
Run `lazy-lamp` and select the script you wish to run from the list of available scripts.

# Lazy Lamp Scripts Overview:

## [L]inux
### L1. Install Lamp Server:

If you don't have the LAMP server components installed yet and is lazy to manually install each of the components running this script will only prompt you to enter the root MySQL password you wish to use and will do the rest for for you. It'll also install Phpmyadmin for your convenience.


### L2. Install Webmin Script:

If you are familiar with Webmin (http://www.webmin.com) and would like to have it installed for easier management of your server you can run the following script

### L3. Install Linux Handy Tools:

A script that automates the installation of Vim, Curl, Composer and GIT.

### L4. Change DNS Server:

A script that helps in changing the machine's DNS server to a list of Free ones. (Google, OpenDNS, DnsWatch, etc ...)

### L5. Install oh-my-zsh shell:

A script that helps in installing oh-my-zsh shell (http://www.ohmyz.sh/)



## [A]pache
### A1. New Site Creation:

Automates the process of adding new sites by creating virtual hosts in your apache2 server configurations, activates it and adds the new site's domain to the hosts file of your system.

### A2. Install and Enable Basic Modules

A script that automates the process of installing the basic apache2 modules

### A3. Clear Pagespeed Cache

Automates the process of flushing up the cache directories of the Google PageSpeed apache module.

## [M]ySQL
### M1. Full MySQL Database Backup:

Automates the dumping of the whole MySQL database in one since command and stores the dumped files on a local directory

### M2. Create a New Database:

Creates a new empty MySQL database

### M3. Create a New User:

Creates a new MySQL user and grants this user global 'ALL PRIVILEGES'

## [P]HP
### P1. Install Useful PHP5 Modules:

Installs PHP modules like Curl and Imap
