---
title: "Data Archiving"
teaching: 30
exercises: 30
questions:
- "What can I learn by following this data management tutorial?"
- "What are the tools that I will be using?"
objectives:
- "Find out what to do with non-research data and where to back up data."
- "Connect to SURF data archive."
- "Transfer data between your machine and the archive."
keypoints:
- "SURF data archive is to be used for larger files or a tar collection of smaller files and not for day to day access."

---

## Table of Contents
1. [Overview](#overview)
2. [What you will learn](#what-you-will-learn)
3. [Tools To Connect](#tools-to-connect)
4. [Connecting](#connecting)
5. [Transferring Data](#transferring-data)

<img src="../img/data_lifecycle.png" width="400px" height="400px">    


## Overview

Storing data on various hard drives scattered around the university/at home is not great practice. 

Data stored on the archive is stored in two physical locations. This is much more secure, and can be accessed from any machine with an internet connection plus login credentials.  

<img src="../img/SURF_Security.jpg" width="300px" height="400px">

## What you will learn

**Where to store data to be archived**

- What is a tape archiving system?
- How can I store my data on tape?
    
    
<img src="../img/SURF_tape.jpg" width="400px" height="400px">    




## Tools To Connect

The tools used for uploading/accessing/transferring are common for both data processing and managing archive data. 


Some differ depending on operating systems.

#### _GUI_

Files can be transferred across the data processing/archiving systems using a GUI filemanager like [Cyberduck](https://cyberduck.io/) or [filezilla](https://filezilla-project.org/).



#### _Windows_
  - _SSH client_ [Mobaxterm](https://mobaxterm.mobatek.net/download.html) is recommended if you don't already have a preferred method.
  - To use a windows 10 machine as if it were linux: _Windows subsystem for linux (WSL)_ - details on setting this up can be found [here](https://www.windowscentral.com/install-windows-subsystem-linux-windows-10). _THIS IS NOT A NECESSARY STEP_. The above can be used instead.




#### _MacOS/Linux_
  - _Terminal_ is built in for both Mac and Linux machines. Can be used as an ssh client.



## Connecting 

### Using a GUI
Cyberduck is the recommended GUI for file transfer with the Data Archive. See the [Cyberduck website](https://cyberduck.io/) for more information. Or for some [tips from SURF](https://userinfo.surfsara.nl/systems/shared/archiving-high-performance).


<img src="../img/Cyberduck_Connect.png" width="600px" height="400px">


### Using command line/ssh client

If using an ssh client on windows then you can input the required details to connect similarly to the GUI option.

<img src="../img/Mobaxterm_Connect.png" width="700px" height="450px">




Otherwise open up preferred method for ssh connection and type the following:


~~~
ssh USER@archive.surfsara.nl
~~~
{: .language-shell}


Then input your password when prompted.


## Transferring data

When transferring data; remember that the tape system is not instant and your files will get stored distributed across their system. For this reason if you want to store lots of small files the these need to be collected together into a tar archive beforehand.

#### How to create a tar archive


_Windows_

No built in tarballing in windows. [7-zip](https://www.7-zip.org/) is currently recommended to add this functionality. A tutorial on how to use it can be found [here](https://dailydoseoftech.com/how-to-open-and-create-tar-files-on-windows/)



_Mac/Linux/WSL_
Using terminal: 

tar -x



### Using a GUI



When using the GUI for file transfer between servers be sure to open two separate windows with separate connections. This is the easiest method of data transfer, but also the slowest as there is no way to stage your data before making the transfer.


### Using command line









## References




### Teaching materials
This lesson was originally formatted according to the [Carpentries Foundation](https://carpentries.org/) lesson template and following their recommendations on how to teach researchers good practices in programming and data analysis.   

{% include links.md %}
