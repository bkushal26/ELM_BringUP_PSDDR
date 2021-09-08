# ELM_BringUP_PSDDR

This Repository is used to Test ZYNQ-DDR interface for the ELM board.

# Getting Started:-

``` git clone --recursive git@github.com:bkushal26/ELM_BringUP_PSDDR.git```.

## Git Repo Structure:

This repo consists of 2 branches-

Main- Corresponds to Latest test version (using Vivado2020.1 and Vitis)
viv191- Old already tested project on vivado2019.1 and SDK, keeping it as a reference.

***Note- This project is under development so repo and readme is incomplete, need to modify the instructions for Vivado-2020.1 version***

### Wiki Page for Test Instructions 
The instructions to conduct DDR Tests can be found in [Wiki](https://github.com/bkushal26/ELM_BringUP_PSDDR/wiki) page. The project has been tested for 2 vivado versions. Vivado 2019.1 and 2020. Respective instructions can be found in the Wiki link.

### myproj
Working Vivado project saved in this folder kept as backup. Detail instructions can be found in [Wiki](https://github.com/bkushal26/ELM_BringUP_PSDDR/wiki) page.

### tcl
This folder contains tcl file which needs to be sourced when starting from scratch. 


## useful commands

1.To check the usb port status- ``` dmesg | grep ttyUSB``` (for madorsky-d2 ,its USB2)

2. To launch serial terminal- ```screen /dev/ttyUSB2 115200```

