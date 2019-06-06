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

## June 26, 2019: QGIS Map Composer (or was it Spatial SQL?)  
 Presenter: **Linc**  
 Prerequisites: TBD  
 
## July 31 or August 7, 2019: Feeding, Watering, and Caring for GIS Servers  
 Presenter: **Mark**  
 Prerequisites: TBD
  
## September 4, 2019: Topic TBD  
 Presenter: **Chris**  
 Prerequisites: TBD  
 
## October 2, 2019: Big Data to go along with FOSS  
Census data, commodity flows, and other publicly available data.  
  Presenter: **Rick**  
  Prerequisites: TBD  
