# Vector_Clock
Code in Python to Synchronize the computer clock using the Lamport method.

People use physical time to order events. For example, we say that an event at 8:15 AM occurs before an event at 8:16 AM. In distributed systems, physical clocks are not always precise, so we can't rely on physical time to order events. Instead, we can use logical clocks to create a partial or total ordering of events. This article explores the concept of and an implementation of the logical clocks invented by Leslie Lamport in his seminal paper Time, Clocks, and the Ordering of Events in a Distributed System.


![animacao](https://user-images.githubusercontent.com/32453979/47199699-d9c90e00-d340-11e8-94b7-6b609d44561e.gif)

# What are the Possible Applications?
Its purpose is the synchronization of logical clocks of computers connected to the same network.

# Methodology
* OS: Ubuntu 18.10 cosmic
* Kernel: x86_64 Linux 4.18.0-10-generic
* CPU: Intel Core i7 Q 740 @ 8x 1.734GHz
* GPU: GeForce GT 425M
* RAM: 7956MiB

# Prerequisites
* Pyhton2.7
* Idle-Python2.7
* Python-Dateutil
* Python-Netifaces
* Python-Ipaddr
* Python-WXgtk2.8

# What do you need to use the software?
* You will need a GNU/Linux Ubuntu 18.04.1 cosmic /  KERNEL x86_64 Linux 4.18.0-10-generic or Debian 9.5 Stretch / KERNEL x86_64 Linux 4.9.0-8-amd64. 
* Internet connection for download.
* OBS: Software does not work on 32 bits systems

Probably the software will also work on any other Debian-based distribution, but it has only been tested on the systems listed above.

These are the necessary packages and modules
The version may not necessarily be the same, but these versions have been tested and confirmed the operation

* 1. PYTHON IDLE
Package: idle-python2.7
Version: 2.7.12-1ubuntu0~16.04.3

* 2. PIP
Package: python-pip
Version: 8.1.1-2ubuntu0.4 

* 3. DATEUTIL
Package: python-dateutil
Version: 2.4.2-1

* 4. NETIFACES
Package: python-netifaces
Version: 0.10.4-0.1build2

* 5. IPADDR
Package: python-ipaddr
Version: 2.1.11-2

* 6. LIBPNG
Package: libpng12-0
Version: 1.2.54-1ubuntu1.1

* 7. LIBTIFF
 Package: libtiff4
 Version: 3.9.6-11+deb7u11

* 8. LIBWXBASE
Package: libwxbase2.8-0
Version: 2.8.12.1-12

* 9. LIBWXGTK
Package: libwxgtk2.8-0
Version: 2.8.12.1-12

* 10. XWPYTHON
Package: python-wxgtk2.8
Version: 2.8.12.1-12

***********************************************************************************************
# How to install

Give permission to file INSTALL.sh
`$sudo chmod +x INSTALL.sh`

Obs: For the above command to work the terminal must be open where the file is located

Run the file
`$sudo ./INSTALL.sh`

***********************************************************************************************
* You can do an installation automatically by running the file 'INSTALL.sh'. But if you want to install manually just follow the steps below

1 . INSTALL PYTHON IDLE
Package: idle-python2.7
Version: 2.7.12-1ubuntu0~16.04.3
`$sudo apt install idle-python2.7`

2 . INSTALE PIP
Package: python-pip
Version: 8.1.1-2ubuntu0.4 
`$sudo apt install python-pip`

3 . INSTALL DATEUTIL (PIP)
Package: python-dateutil
Version: 2.4.2-1
`$sudo pip install python-dateutil`

4 . INSTALL NETIFACES (PIP)
Package: python-netifaces
Version: 0.10.4-0.1build2
`$sudo pip install netifaces`

5 . INSTALL IPADDR
Package: python-ipaddr
Version: 2.1.11-2
$sudo apt install python-ipaddr`

6 . DOWNLOAD LIBPNG
Package: libpng12-0
Version: 1.2.54-1ubuntu1.1
`$sudo wget http://ftp.us.debian.org/debian/pool/main/libp/libpng/libpng12-0_1.2.49-1+deb7u2_amd64.deb`
6 . 1 .INSTALL LIBPNG
`$sudo dpkg -i libpng12-0_1.2.49-1+deb7u2_amd64.deb`

7 . DOWNLOAD LIBTIFF
Package: libtiff4
Version: 3.9.6-11+deb7u11
`$sudo wget http://security.debian.org/debian-security/pool/updates/main/t/tiff3/libtiff4_3.9.6-11+deb7u11_amd64.deb`
7 . 1INSTALL LIBTIFF
`$sudo dpkg -i libtiff4_3.9.6-11+deb7u11_amd64.deb`

8 . DOWNLOAD LIBWXBASE
Package: libwxbase2.8-0
Version: 2.8.12.1-12
`$sudo wget http://ftp.us.debian.org/debian/pool/main/w/wxwidgets2.8/libwxbase2.8-0_2.8.12.1-12_amd64.deb`
8 . 1 . INSTALL LIBWXBASE
`$sudo dpkg -i libwxbase2.8-0_2.8.12.1-12_amd64.deb`

9 . DOWNLOAD LIBWXGTK
Package: libwxgtk2.8-0
Version: 2.8.12.1-12
`$sudo wget http://ftp.us.debian.org/debian/pool/main/w/wxwidgets2.8/libwxgtk2.8-0_2.8.12.1-12_amd64.deb`
9 . 1 . INSTALL LIBWXGTK
`$sudo dpkg -i libwxgtk2.8-0_2.8.12.1-12_amd64.deb`

10 . DOWLOAD XWPYTHON
Package: python-wxgtk2.8
Version: 2.8.12.1-12
`$sudo wget http://ftp.us.debian.org/debian/pool/main/w/wxwidgets2.8/python-wxgtk2.8_2.8.12.1-12_amd64.deb`
10 . 1 . INSTALL ALL DEPENDENCIES MISSING
`$sudo apt-get install -f`
10 . 2 . INSTALL XWPYTHON
`$sudo dpkg -i python-wxgtk2.8_2.8.12.1-12_amd64.deb`

***********************************************************************************************
# Possibles erros

* If any module for unknown reasons has not been installed

Any module error that you may have to re-view the "HOW TO USE" session and manually install each module in sequence according to the tutorial. Follow steps 1 through 10.2.

In the Debian system you may have a user error
If you get the error "./INSTALL.sh: sudo: not found". By default sudo is not installed, but you can install it. First enable su-mode:
`$su`
`#apt install sudo -y`

After that you would need to play around with users and permissions. Give sudo rigth to you own user.
`#usermod -aG sudo yoursername`
Edit the file 'sudoers'
`#nano /etc/sudoers`

#User privilege specification
root ALL=(ALL:ALL) ALL
yoursername ALL=(ALL:ALL) ALL 
#The top line was the one we added. 
#Replace 'yoursername' with the name of your user who wants to have root permission
`#exit`
***********************************************************************************************

# How to use

*  IMPORTANT: For the hours to change you must have root permission or be the root user.

Open 'idle-python', it must have root permission
`$sudo idle-python2.7`
or
`#idle python2.7`

Click on 'File ==> Open ==> ds_logic_clocks_mc.py'

The source code will appear on your screen

Click on 'run ==> run module'
or
Press 'F5'
***********************************************************************************************
# Why the development?
It was developed by Professor Diogenes on the campus of UNEMAT BBG - MT in order to ... and being under my responsibility the documentation and implementation of the project in GitHub

# Is this the only system of sync?
I do not know

# Is this system 100% complete?
Yes, it can be used in full according to the proposal.


