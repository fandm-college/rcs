---
layout: page
title: Overview for acccessing compute resources
permalink: /overview/
description: Accessing compute resources
---

```note
If you aren't familiar with such means of interaction and/or aren't familiar 
with the Linux operating system, we recommend looking through our Linux tutorial 
beginning with the [Introduction to the command line](404.md)
```

Access to compute resources can be broken into 3 categories
1. Web access, VPN not required
    - ArcGIS
    - MATLAB
    - Globus
2. Web access with VPN if off-campus(i.e., not connected to eduroam)
    - Jupyter
    - WebWork
    - R/Posit
    - Research cluster through OpenOnDemand
3. Command-line with VPN if off-campus(i.e., not connected to eduroam)
    - Research cluster
    - Other computer servers

To access compute resources in the third category you will need
two programs: 

SSH - connect to compute resource to run programs

SCP - copy data/files bertween your local computer and the compute resource

### Mac OS X
Mac OS X comes with SSH and SCP installed.  These programs can be run in the terminal, found
in the Utilities folder.  The Utilities folder can be opened using the keyboard shortcut
`Shift+Command+U`

### Windows
For SSH, we recommend installing PuTTY which can be found in the Microsoft Store 
(maintained by Simon Tatham).

For SCP, we recommend using WinSCP, found [here](https://winscp.net/eng/download.php)