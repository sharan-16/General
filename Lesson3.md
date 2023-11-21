# Vivado Installation and Licensing

Vivado is one of the most widely used acedemic tools for hardware and hardware-related development projects. Contributing factors are its standard IP component library and support for a wide variety of boards which is both customisable and constanatly updated by the Xilinx Community. The licencing is generally free and should support most of the boards with some case-by-case limitaions.

In this tutorial our aim is to setup the Vivado environment for RFSoC projects and the corresponding licences. Here we set out to install the latest version of the Vivado for Linux systems. Addtional links for the Windows systems and its configurations are added below. 

## DOWNLOAD

**Login to your Xilinx account or create one using the NYU email. A free account is nneded to download the software**

* Open the [Xilinx Vivado Download](https://www.xilinx.com/support/download.html) page. Select the version of choice, depending on any specific needs, we went with the latest one.

<p align="center">
<img src="pic1.png" alt="Alt Text" width="700" height="500">
</p>

Now you could either choose to download the installer and then let it handle all the file dowloads and installation or download the tar.zip file unpack it and then install it. We had some isssues with the former approach so we chose the later one. 
* Select the required pacakage and it will lead you to a form, fill you details there and click on download.It will download the Xilinx_Unified_2020.2_1118_1232.tar.gz file.

<p align="center">
<img src="pic2.png" alt="Alt Text" width="400" height="500">
</p>

* Navigate to downloads folder on the Linux system and extract the files from the Xilinx_Unified_2020.2_1118_1232.tar.gz archive: 
```
tar -xvf Xilinx_Unified_2020.2_1118_1232.tar.gz
```

Run the installer: 
```
sudo ./xsetup
```
## INSTALLER OPTIONS
* Enter your Xilinx account information, and select Download and Install Now.
* On the Select Product to Install screen, choose Vivado ML Enterprise edition as the stabdard edition doesnt support the RFSoCs.
* On the customization screen, uncheck anything if required, except make sure you have the RFSoC files installed as shown in the pic.

* Install Cable Drivers
```
cd /tools/Xilinx/Vivado/2020.2/data/xicom/cable_drivers/lin64/install_script/install_drivers
sudo ./install_drivers
```

* On the next screen, agree to all boxes.
* On the next screen, choose an installation location with enough space.
* On the next screen, click Install and wait a while.

## Opening the Vivado 
Once the software isinstalled it can be accessed with normal user prevelages as follows:

**Note:** Once the
  
## License generation and updating

The license file for the Vivado should be automatically added. If the licence expires for you want to add some other licences, it can be either using the Vivado License manger interface or the Linux terminal.

**Vivado Licence Manager**
For making any changes to system 
