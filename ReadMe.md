## Background

The intention of this document is to describe how to successfully run a Ruby on Rails app, built specifically for and entirely on an Ubuntu distribution, in production mode on a Windows Server 2016 environment.

#### Prerequisites:

1. A Windows Server 2016 VM (Currently running on Amazon lightsail)
2. Internet connection -- Access to github to clone repo
3. Server Manager > Disable IE Enhanced security mode
4. Git - well, to clone repo
5. What is the default site on host?


### How to

1. On your Windows Server machine, download and install https://www.microsoft.com/web/downloads/platform.aspx
2. Run Web Platform Installer and click on "Options"
3. Add Helicon Zoo Custom Feed http://www.helicontech.com/zoo/feed.xml
4. From the "Zoo" tab, go to "Packages" and install the Ruby hosting package
5. Install the Ruby template from the "templates" section
6. 







Source: http://www.helicontech.com/zoo/install.html


### Method 2, with docker on Windows Server 2016

Apparently windows server 2016 supports containerization, but setting it up is proving a challenge!
In any case, havent really had any rails deployments on docker before, might be a good learning experience, but meh!

1. On Winows PowerShell `Install-WindowsFeature containers`
2. Restart - Scheduled OS Reconfiguration
3. 


Notes:
Running into unable to get package x, search criteria?
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12

### Method 3, Virtual Machine on Windows 
-- Needs CPU to support some special virtualization technologies etc
Lets see how this goes -- Can't use the cloud VMs though

Ref: https://www.nakivo.com/blog/creating-configuring-vms-in-windows-server-2016-hyper-v/