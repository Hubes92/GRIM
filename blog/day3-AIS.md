# Blog - AIS set reciever set-up
Today I got the AIS reciever for the USV, and went through the process of getting it working on a Ubuntu PC, turns out it is really easy with some pretty awesome open-source software called openCPN. So lets Get into it.

## Hardware

Pretty much all you need is a Ubuntu or linux computer an AIS reciever (I have a GME AIR Reciever AISR120) with a USB interface and an antenna. Attach it all up as shown below.

<p align="center">
  <img width="599" height="647" src="https://github.com/Hubes92/GRIM/blob/master/images/hardware.png">
</p>
 
 A little green light should show up. Make sure the antenna is connected before you turn it on, can wreck it otherwise. 

## Software 
After the hardware is conencted, follow these steps in teh terminal

### Setting up the dependencies and software 
  sudo apt-get install software-properties-common
  sudo add-apt-repository ppa:opencpn/opencpn
  sudo apt-get update
  sudo apt-get install opencpn
  sudo apt-get install gpsd gpsd-clients

### Now we need ot change some permissions on the serial port, mine was:
  sudo chmod 666 /dev/ttyACM0

### In the terminal, run:
  -opencpn 
  -go to settings
  - go to connections
  - click add connection
  - select serial
  - enter the devices (mine was ttyACM0)
  - click add
  - should see boats start to appear! 
  - done!
