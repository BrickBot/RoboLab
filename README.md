RoboLab
=======
There are two distinct releases of RoboLab
* A standalone release that was made available through LEGO and popular for educational LEGO robotics
* An add-in release for LabVIEW

RoboLab (standalone)
-------
[RoboLab](http://legoengineering.com/platform/robolab/) is a visual programming language built in LabVIEW that was developed by the Tufts CEEO.  Offering support for both the RCX and the NXT, it was the dominant programming language for educational LEGO robotics prior to the release of the NXT Software (NXT-G), and it providedg inspiration for not only the NXT Software but also the LabVIEW for LEGO MINDSTORMS releases that followed.

This standalone version of RoboLab does _not_ support the USB IR Tower.  The last official version was 2.9.4c, and for users with the version 2.9 installation, there is also a [patch avaiable](http://legoengineering.com/robolab-2-9-4c-patch/).

<!--
#### Archived Releases
* [RoboLab 2.5](https://archive.org/details/ROBOLAB2.5) 
* [RoboLab 2.9](https://archive.org/details/robolab-29)
* [BrickLink Description and Images](https://www.bricklink.com/v2/catalog/catalogitem.page?G=2000069)
-->

RoboLab for LabVIEW
-------------------
RoboLab for LabVIEW is an add-on for LabVIEW that enables you to run the classic and much loved RoboLab within an installation of LabVIEW.  As such, this is not a standalone product, so an edition of LabVIEW (either LabVIEW itself or a more specialized edition such as LabVIEW for LEGO MindStorms [LVLM] or LabVIEW for Education [LV4E]) is required.

### Overview
LabVIEW for LEGO® MINDSTORMS® is optimized for classroom use with instructional videos, tutorials and teaching resources created exclusively for high school students and teachers using LEGO MINDSTORMS Education and TETRIX by Pitsco. It introduces students to advanced concepts such as autonomous robotics and scientific measurements using real-world examples and replacing obscure syntax with an intuitive graphical interface. Because of this, the software is ideal for teachers seeking to engage students with technology in a fun, hands-on way.
* [LEGO Engineering Overview: RoboLab for LabVIEW](http://legoengineering.com/robolab-for-labview/)
* [National Instruments: LabVIEW for LEGO MindStorms](https://web.archive.org/web/20200222200939/http://www.ni.com/download/labview-for-lego-mindstorms-2012-sp1/3877/en/)

### Preparation
In odrer to complete these steps, the creation of a free account on National Instrument’s website will be required.  This can be completed during the first download step.

__NOTE__: _The combined size of these downloads is just over 8¼ GB_.

* For users **_with_** an existing installation of a LabVIEW version between 7.1 and 2016 (different LabVIEW versions may be installed side by side)
  1. Browse to the [LabVIEW Toolkit page for LEGO MindStorms](https://decibel.ni.com/content/docs/DOC-15615)  ([alternate link](https://forums.ni.com/t5/NI-Labs-Toolkits/NI-LabVIEW-for-LEGO-MINDSTORMS-LabVIEW-Module-for-LEGO/ta-p/3516439))
  2. Scroll down to the section entitled “LabVIEW Toolkit for LEGO MindStorms”
  3. Select the toolkit appropriate for your version of LabVIEW
     + NOTE: This toolkit is [unavailable for LabVIEW 2017 or newer](https://knowledge.ni.com/KnowledgeArticleDetails?id=kA00Z000000P80ySAC&l=en-US)

* For users **_without_** an existing installation of LabVIEW
  1. Download [LabVIEW for Education version 2014 SP1](https://www.ni.com/en/support/downloads/software-products/download.labview-for-education.html)
     + [Release Notes](https://www.ni.com/en/support/documentation/release-notes/product.labview-for-education.html#version-2014-sp1)
  2. Download [LEGO MindStorms Module for LabVIEW version 2014 SP1 Patch](https://www.ni.com/en/support/downloads/software-products/download.lego-mindstorms-module-for-labview.html#351217)
  3. Download [LEGO MindStorms Module for LabVIEW version 2014 SP1](https://download.ni.com/support/softlib/labview/labview_toolkits/NXT%20Module/2014%20SP1/windows/2014%20SP1%20Eng.zip)
  4. Download RoboLab for LabVIEW files from Lego Engineering (c.f. [overview page](http://legoengineering.com/robolab-for-labview/)):
     1. [LEGO Engineering’s RoboLabPC](https://web.archive.org/web/20210926164643/http://legoengineering.com/wp-content/uploads/2013/04/RoboLabPC.zip)
        - NOTE: The link above to download via archive.org must be used, as the version of this file that now downloads from LegoEngineering.com is corrupt and will not open.
     2. [LEGO Engineering’s RoboLab Installer](http://legoengineering.com/wp-content/uploads/2013/04/ROBOLAB_installer.vi_.zip)
  5. Download [NI-VISA version 14.0.1 Full edition](https://www.ni.com/en/support/downloads/drivers/download.ni-visa.html#306025)
     + [Release Notes](https://www.ni.com/en/support/documentation/release-notes/product.ni-visa.html#version-14-0-1)

### Installation
Installation instructions are based on the [RoboLab for LabVIEW](http://legoengineering.com/robolab-for-labview/) and [RCX USB Tower Support](http://legoengineering.com/rcx-usb-tower-support/) guides from LEGO Engineering.
1. Install LabVIEW for Education version 2014 SP1 (_if no existing, compatible LabVIEW install_)
2. Install LEGO MindStorms Module for LabVIEW version 2014 SP1 (_or your compatible LabVIEW version_)
3. Install LEGO MindStorms Module for LabVIEW version 2014 SP1 Patch (_if applicable for your LabVIEW version_)
4. Install RoboLab for LabViEW
   1. Unzip __ONLY__ the RoboLab installer RL_installer.vi_.zip to extract the file RL_installer.vi
   2. Ensure that both the installer and the add-on zip file are in the same folder (the installer will unzip the zip file)
   3. Open the installer in LabVIEW
   4. Work through the installation steps
      - Should start running automatically
      - Might take a while as it must recompile everything
   5. Close all windows and exit LabVIEW
5. Install NI-VISA
6. Setup the USB IR Tower for use on a 64-bit OS (if applicable)
   1. Plug in the LEGO USB IR Tower
   2. Launch the NI-VISA Driver Wizard (typically found under Start > VISA > NI-VISA Driver Wizard)
   3. Under “Hardware Bus” in the window that opens, select “USB”
   4. Select the “LEGO USB Tower” from the “USB - Device Selection” dialog window
   5. Give the INF files a name (default is fine)
   6. Select to allow the wizard to “Install the generated files on this computer”
   7. Click “Finish”
   8. Close all windows and exit LabVIEW

To run RoboLab, go to the Tools menu and select Robolab 2.9.4d


### Resources
* LEGO Engineering
  + [RoboLab Quick Guide](http://legoengineering.com/robolab-quick-guide/)
  + [Downloads for RoboLab](http://legoengineering.com/category/support/downloads/)
  + [RCX Content, including LabVIEW support, Challenge Ideas, and Learning Information](http://legoengineering.com/platform/rcx/)
* [Forum for LabVIEW for LEGO MindStorms and LabVIEW for Education](https://forums.ni.com/t5/LabVIEW-for-LEGO-MINDSTORMS-and/bd-p/460)
