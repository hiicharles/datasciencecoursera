Install R-base and RStudio on Ubuntu 
====================================

***
Install R
---------


        ## Switch to root
        user> sudo su
        
        ## Add GPG Key 
        root> apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9

        ## Add Repository
        root> vim /etc/apt/sources.list.d/rcran.list
        deb http://cran.rstudio.com/bin/linux/ubuntu trusty/
        
        ## Update, Upgrade and Install
        root> apt-get update
        root> apt-get upgrade
        root> apt-get install r-base r-base-dev

        ## Run R
        root> R

      
***
Setup RStudio
-------------
      
        ## Install wget
        root> apt-get install wget
        
        ## Change Directory and Download
        root> cd /opt
        root> wget http://download1.rstudio.org/rstudio-0.98.1049-amd64-debian.tar.gz
        
        ## Extract file
        root> tar -zxvf rstudio-0.98.1049-amd64-debian.tar.gz
        
        ## Run RStudio
        root> cd rstudio-0.98.1049/bin
        root> ./rstudio
        
### Note:
The download URL might changed when new version released.  Please refer to <http://www.rstudio.com/products/rstudio/download/> .