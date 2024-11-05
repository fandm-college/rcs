---
layout: page
title: Overview 
permalink: /overview/
description: Accessing compute resources
---

`
If you aren't familiar with command-line style of interaction and/or
with the Linux operating system, we recommend looking through our Linux tutorial 
beginning with the [Introduction to the command-line](404.md)
`

Access to compute resources can be broken into 3 categories
1. Web access, VPN not required
    - [ArcGIS](404.md)
    - [MATLAB](404.md)
    - [Globus](https://auth.globus.org)
 Exact details for logging in to these web-based resources varies
 and it is highly recommended you visit the ???

2. Web access with VPN if off-campus(i.e., not connected to eduroam)
    - [Jupyter](404.md)
    - [WebWork](https://math.fandm.edu)
    - [R/Posit](https://math-r.fandm.edu)
    - [Research cluster through OpenOnDemand](https://rcs-scsn.fandm.edu)
    
3. Command-line with VPN if off-campus(i.e., not connected to eduroam)
    - Research cluster
    - Other computer servers

To access compute resources in the third category you will need
two programs: 

**SSH** - connect to compute resource to run programs<\br>
**SCP** - copy data/files bertween your local computer and the compute resource

### Mac OS X
Mac OS X comes with SSH and SCP installed.  These programs can be run in the terminal, found
in the Utilities folder.  The Utilities folder can be opened using the keyboard shortcut
`Shift+Command+U`

### Windows
For SSH, we recommend installing **PuTTY** which can be found in the Microsoft Store 
(maintained by Simon Tatham).

For SCP, we recommend using **WinSCP**, found [here](https://winscp.net/eng/download.php)