# ELM_BringUP_PSDDR

This Repository is used to Test ZYNQ-DDR interface for the ELM board.

# Getting Started:-

``` git clone --recursive git@github.com:bkushal26/ELM_BringUP_PSDDR.git```.

## Git Repo Structure:

This repo consists of 2 branches-

Main- Corresponds to Latest test version (using Vivado2020.1 and Vitis)
viv191- Old already tested project on vivado2019.1 and SDK, keeping it as a reference.

***Note- This project is under development so repo and readme is incomplete, need to modify the instructions for Vivado-2020.1 version***

### manual

contains steps on how to execute the steps in doc and pdf format.

### myproj
Working Vivado project saved in this folder

### tcl
this folder contains tcl file which needs to be sourced when starting from scratch

## Create a new project from scratch:

1. check the current working directory has 'tcl' folder.
2. Launch Vivado (2019.1)
3. In Vivado Tcl Console run :```source tcl/psddr.tcl```

## Use existing Project:-

1. ```cd myproj```
2. Launch Vivado
3. Lunch XSDK from Vivado: ```File``` -> ```Launch SDK``` (accept defaults, click OK).
4. Follow the Run configuration settings given in manual

## useful commands

1.To check the usb port status- ``` dmesg | grep ttyUSB``` (for madorsky-d2 ,its USB2)

2. To launch serial terminal- ```screen /dev/ttyUSB2 115200```

