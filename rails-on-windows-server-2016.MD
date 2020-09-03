## Background

The intention of this document is to describe how to successfully run a Ruby on Rails app, built specifically for and entirely on an Ubuntu distribution, in production mode on a Windows Server 2016 environment.

####Prerequisites:

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