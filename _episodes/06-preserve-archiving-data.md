---
title: "Data archiving"
teaching: 30
exercises: 30
questions:
- "What is data archiving?"
- "What is SURFsara Data Archive?"
- "What is Tape Archive?"
- "How can I connect and upload data to SURF Data Archive?"
objectives:
- "Find out what to do with non-research data and where to back up data."
- "Be able to use the commadnConnect to SURF data archive."
- "Transfer data between your machine and the archive."
keypoints:
- "SURF data archive is to be used for larger files or a tar collection of smaller files and not for day to day access."

---

# Table of contents

<!-- MarkdownTOC autolink="True" -->

- [1. Introduction](#1-introduction)
	- [1.1 Backup and archiving](#11-backup-and-archiving)
	- [1.2 Long-term data preservation becomes more crucial](#12-long-term-data-preservation-becomes-more-crucial)
- [2. Tape Archive](#2-tape-archive)
- [2. The SURFsara Data Archive](#2-the-surfsara-data-archive)
- [3. How to archive data with SURF data archive](#3-how-to-archive-data-with-surf-data-archive)
	- [Tools To Connect](#tools-to-connect)
			- [_GUI_](#gui)
			- [_Windows_](#windows)
			- [_MacOS/Linux_](#macoslinux)
	- [Connecting](#connecting)
		- [Using a GUI](#using-a-gui)
		- [Using command line/ssh client](#using-command-linessh-client)
	- [Transferring data](#transferring-data)
		- [Using a GUI](#using-a-gui-1)
		- [Using command line](#using-command-line)
- [References](#references)

<!-- /MarkdownTOC -->

<img src="../img/data_lifecycle.png" width="600px">    

# 1. Introduction

## 1.1 Backup and archiving

This alone means that storing data on various hard drives scattered around the university or at home is not great practice. Hard drives are prone to physical destruction if they fall or being lost or stolen for instance.    

__Data archiving__ should indeed not be be confused with __data backup__:
- __Data backup:__ a data backup makes sure that research data which are regularly accessed can be quickly recovered if something happens (fire, theft). Moreover, a data backup can be _instantaneously_ accessed because the data is on a electrically powered drive and because a disk drive moves rapidly to read the data stored on the hard disk.  
- __Data archiving:__: Data archiving on the other hand serves to preserve data you do not access regularly and ensures long-term preservation. 

## 1.2 Long-term data preservation becomes more crucial

Due to the increasing volume of data being generated in research (e.g. DNA sequencing or imaging), it has become more complex to store large and heterogeneous volumes of data easily. 
Yet, the possibility to re-use research data rather than automatically regenerate new data also becomes important as techniques to aggregate numerous datasets become more commonplace. One such example is Machine Learning that requires large amount of well-curated and labeled data in order to generate meaningful results. 

In addition, research funding agencies or Universities increasingly require that research data are stored for 3 to 10+ years as can be seen from several national research agencies: 
- [Dutch Research Council (NWO)](https://www.nwo.nl/en/research-data-management) (Dutch Research Council).
- [British Biotechnology and Biological Sciences Research Council (BBRSC)](https://researchdata.ox.ac.uk/funder-requirements/bbsrc/)
- [US National Institute of Health](https://grants.nih.gov/grants/policy/data_sharing/data_sharing_guidance.html)
- etc.

# 2. Tape Archive

When it comes to data archiving, storing on hard drives can become quite expensive rapidly. One of the reasons is that hard drives need to be electrically powered in order to be readable by the disk driver. Current estimate are 120€ per terabyte per year (source: SURFsara, 2019).

Data volumes have significanly 
Short-term versus long-term storage

Need staging  slower access to data

hard disk drive versus tape drive

|    <center> Hard disk drive </center>                  | <center> Magnetic tape drive </center>                 |
|-----------------------------------------------------   |--------------------------------------------------------|
| <img src="../img/06-hard-drive.jpg" width="200px"/>    | <img src="../img/06-magnetic-tape.jpg" width="200px"/> |
| Short-term storage                                     | Long-term storage (no electricity required)            | 
| Maximum storage capacity per unit = 100TB (SSD, 2018)  | Maximum storage capacity of 45TB (2018,LTO9)           | 
| Instantaneous data access                              | Sequential access: data needs to be staged on disk first| 


# 2. The SURFsara Data Archive

[SURF](https://www.surf.nl/en) is defined as:
> "a cooperative association of Dutch educational and research institutions in which its members join forces. The members are the owners of SURF."
Source: [SURF website](https://www.surf.nl/en/about-surf/the-surf-cooperative)
The SURF organisation runs a [data archive service](https://www.surf.nl/en/secure-long-term-storage-with-data-archive)


Data stored on the archive is stored in two physical locations. This is much more secure, and can be accessed from any machine with an internet connection plus login credentials.  



For example, the SURFsara data archive is located at two locations: one in Almere and one in Amsterdam within the Amsterdam Data Center which is a 72m-tall building with 13 floors (see below). 

<figure class="figure">
  <img src="../img/06-amsterdam-data-tower.png" alt="Amsterdam Data Tower" width="600px">
  <figcaption><center>The Amsterdam Data Tower</center> </figcaption>
</figure>
<br>

Access to the data center is being checked through ID and fingerprints at the entrance. 

<img src="../img/SURF_Security.jpg" width="300px" height="400px">

<figure class="figure">
  <img src="../img/SURF_Security.jpg" alt="Security at the entrance of the Amsterdam Data Tower" width="600px">
  <figcaption><center>Identity check to enter the servers within the Amsterdam Data Tower</center> </figcaption>
</figure>

SURFsara 

    
    
<img src="../img/SURF_tape.jpg" width="400px" height="400px">    


# 3. How to archive data with SURF data archive 

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


### Using a GUI



When using the GUI for file transfer between servers be sure to open two separate windows with separate connections. This is the easiest method of data transfer, but also the slowest as there is no way to stage your data before making the transfer.


### Using command line









# References

- [Tape Drive](https://en.wikipedia.org/wiki/Tape_drive)
- [Utrecht University guide to data preservation](https://www.uu.nl/en/research/research-data-management/guides/storing-and-preserving-data)

{% include links.md %}
