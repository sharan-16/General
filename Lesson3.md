# Vivado Installation and Licensing

Vivado is one of the most widely used acedemic tools for hardware and hardware-related development projects. Contributing factors are its standard IP component library and support for a wide variety of boards
which is both customisable and constanatly updated by the Xilinx Community. The licencing is generally free and should support most of the boards with some case-by-case limitaions.

In this tutorial our aim is to setup the Vivado environment for RFSoC projects and the corresponding licences. Here we set out to install the latest version of the Vivado for Linux systems. Addtional links for the Windows systems 
and its configurations are added below. 

## Download and Install

**Login to your Xilinx account or create one using the NYU email.**
Open the [Xilinx Vivado Download](https://www.xilinx.com/support/download.html) page. Select the version of choice, depending on any specific needs, we went with the latest one.
![](pic1.png)
![Alt Text](pic1.png){:width="300px" height="200px" style="border: 1px solid #000;"}


-- Here we are trying to install Vivado for Linux and this can either be done using an installer and dowloading the tar/zip file and installing them locally. We will be goining with the later. 
-- Click on the link, fill out the form and download it.
![](pic2.png)


The RFSoC 2x2 board is an SDR board that can be used to emulate a radio system. The 2x2 has high speed RF ADCs (2 no.s) to sample RF signals directly without the need of any mixer circuitry, which is then sent to the ZYNQ Ultrascale+ chip on the board; it also has 2 RF DACs to transmit data out from the board. The ZYNQ Ultrascale+ chip contains 2 processing components, that is, a set of ARM core processors (Processing System) and an FPGA (Programmable Logic) along with some memory elements such as DRAMs. The ARM core processors act as the host and the FPGA acts as the target. Using a framework called PYNQ we can communicate with the processing system through a browser where the browser acts as the terminal to send commands as well as a UI front end to display received data.
