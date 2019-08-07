# Tallahassee FOSS Meetups

Tallahassee's homegrown FOSS meetup group. Located in the *terra incognita* somewhere between the GIS lab and a group therapy session.  
  
# Guidelines for presenters and audience  
  
The first half of each meeting is volunteer-led instruction. The second half is a freeform experimentation/mutual assistance/bullshitting session.  

**Presenters:**
  + Target is 45-60 minute length.  
  + Focus is 'how to do X using FOSS'  
  + Any prerequisites - software and data - should be sent to Seth at least 7 days prior to your scheduled presentation.  
  + Do your best to keep any example data relatively small in size.  
  + **Do NOT** use proprietary or private data in your presentation.  
  + Slides and handouts should be platform agnostic and exported to HTML or PDF. HTML is strongly preferred.  
  + Unless you want to opt out, please bring digital copies of your materials with you so Seth can post to github.  
  + Don't stop your presentation to troubleshoot a single person's technical issue - take care of it in the second hour.  
  + Failure is OK!  
  
**Audience:**  
  + Bring your laptop  
  + Have any prerequisites downloaded and installed when you arrive  
  + If you hit a technical snag and can't resolve it youself, wait until the second half to ask for assistance  
    
# Scheduled Meetings  

Generally speaking, we meet the first Wednesday evening of every month, unless otherwise noted.  

## April 3, 2019: Introduction to FOSS GIS  

Presenter: **Seth**  
Prerequisites: None  

## May 1, 2019: Using Virtual Machines and Linux  
Presenter: **Seth**   
Using linux virtual machines to play with FOSS in a sane and safe manner.
  + Installing Ubuntu as a guest OS  
  + Using the Bash terminal  
  + Installing and configuring QGIS and PostGIS  
  + Loading sample data into PostGIS  
  + VM Snapshots and Backups  
  
My tutorial will use VirtualBox and Linux Mint, but you are welcome to use Hyper-V and any \*buntu variant with a desktop that you want to use. It all does the same thing with a slightly different look and feel and we will be using the terminal for most everything anyway. People that would like to take this knowledge back to their job will probably want to use Hyper-V, as this is the virtualization software most orgs use at the systems level.  

### **Prerequisites:**  
   + A laptop with 8gb of RAM, 2+ cores, and 30-50 Gb of free disk space.  
   + **Pre-installed Software:**
     + Both:
       + [Oracle VirtualBox 6.0.6](https://www.virtualbox.org/wiki/Downloads) 
       + [Oracle VM VirtualBox Extension Pack](https://download.virtualbox.org/virtualbox/6.0.6/Oracle_VM_VirtualBox_Extension_Pack-6.0.6.vbox-extpack)  
      
Download the VirtualBox installer that is appropriate for your system and install VirtualBox. Download the extension pack file - clicking on it should run it with VirtualBox and install the extension pack automatically. 
 
   + **Data:**  
     + One of:  
        + [Linux Mint 19.1 "Tessa" ISO Image](https://linuxmint.com/edition.php?id=261)  
        + [Ubuntu 18.04.2 LTS "Bionic Beaver" ISO Image](http://releases.ubuntu.com/18.04/)  
        + Any other .iso file containing the installer for any [\*buntu variant (Kubuntu, Xubuntu, etc.)](https://www.psychocats.net/ubuntu/whichbuntu) that **is based on Ubuntu 18.04.2 "Bionic Beaver"**
     + [Florida County Boundaries](https://download.fgdl.org/pub/state/county_sep15.zip) or similar shapefile data. 
     + (Optional) [OSGeo osgeolive-vm.vmdk file](https://live.osgeo.org/en/download.html)  

If you have Windows 10 installed [you can opt to use Hyper-V instead of VirtualBox](https://www.nextofwindows.com/how-to-enable-configure-and-use-hyper-v-on-windows-10). You shouldn't have problems but I won't be able to troubleshoot anything that comes up until the second hour.  

## June 5, 2019: QGIS Tools, Toolboxes, Utilities, and Plugins  
Presenter: **Phil**

This tutorial aims to cover the basic functions provided by QGIS for working with:
  + Coordinate systems
  + Raster data
    + Raster calculator, DEMs, Raster to Vector Conversion
  + Vector data
    + Append, Union, Intersect, Buffer, Clip

We'll cover all of these topics by working through a site selection exercise.

You can find the slides to the presentation [here](https://docs.google.com/presentation/d/1VrU04zedVM4MTOhmbHMPutT7sl_-WF1VpqABXryX8os/edit?usp=sharing).

### **Prerequisites:**
  + A laptop with QGIS already installed (either 2.18+ or 3.4+).
  + **Data:**
    + Zipped GIS data available [here](/20190605_QGIS_SiteSelection/FOSS_Data.zip) (~15MB).

## June 26, 2019: PostGIS & Spatial SQL
 Presenter: **Linc**  
 Prerequisites:  
  + A laptop with 1 GHz processor or better, at least 1 GB RAM, and at least 5 GB of available disk space (for this session, not sufficient for production uses).  
  + Required Software:  
    + PostgreSQL 10 (this demo uses 10.8)  
    + PostGIS 2 (this demo uses 2.4)  
    + QGIS (any currently supported version should work)  

Installing PostgreSQL and PostGIS:

  + The simplest approach is the EnterpriseDB install package at:
    + https://www.enterprisedb.com/downloads/postgres-postgresql-downloads  
    + This includes Stack Builder that installs PostGIS (and other packages)  
  + Installation notes (differences from the instructions linked below)  
    + In the Stack Builder dialog, select “PostGIS 2.4 Bundle for PostgreSQL 10”  
    + In the Choose Components dialog, also select “Create spatial database”  
    + Accept the defaults as you navigate the installation  
    + Remember your password!

Installation instructions (courtesy of Boston GIS and PSU GEOG 868) are at  
  + http://www.bostongis.com/PrinterFriendly.aspx?content_name=postgis_tut01  
  + https://www.e-education.psu.edu/spatialdb/open_software_download_instructions
   
 
## July 31 or August 7, 2019: Feeding, Watering, and Caring for GIS Servers  
 Presenter: **Mark**  
 Prerequisites:  
 
    + A Ubuntu installation (Linux Mint, Kubuntu etc) on a laptop (most of us have already done this in prior meetups).  This can be a virtual machine.  Version 18.04 LTS.  This installation needs to have the ability to connect to the internet as that’s how you’ll communicate with your server.    
    + For the second half of the discussion, if you want to try standing up a server, you’ll need an account (with credit card) with a cloud server provider.  I use Digital Ocean, but Amazon or Azure will also work.  The example I go through will use Digital Ocean.  Whatever cloud provider you choose, they need to have Ubuntu 18.04 server deployments.  You can run a decent experimental server at Digital Ocean for about 6 cents an hour (8 GB RAM, 160 GB HD, 4 Processors). There are other models that are significantly cheaper, others that are more.  If you don’t want to set up a server, you’ll still learn some of the inner-workings of Ubuntu and you can install and configure some of the examples on your non-server Ubuntu laptop if you want.  
    + Here’s the URL for Digital Ocean if you want to check them out: https://www.digitalocean.com/  
  
## September 4, 2019: Topic TBD  
 Presenter: **Chris**  
 Prerequisites: TBD  
 
## October 2, 2019: Big Data to go along with FOSS  
Census data, commodity flows, and other publicly available data.  
  Presenter: **Rick**  
  Prerequisites: TBD  
