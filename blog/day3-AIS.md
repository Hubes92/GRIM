# Blog - AIS set reciever set-up
Today I got the AIS reciever for the USV, and went through the process of getting it working on a Ubuntu PC, turns out it is really easy with some pretty awesome open-source software called openCPN. So lets Get into it.

## Hardware

<p align="center">
  <img width="599" height="647" src="https://github.com/Hubes92/GRIM/blob/master/images/Screenshot%20from%202018-08-22%2021-27-54.png>
</p>

## Software 


### Setting up AIS reciever on Linux 
  sudo apt-get install software-properties-common
  sudo add-apt-repository ppa:opencpn/opencpn
  sudo apt-get update
  sudo apt-get install opencpn
  sudo apt-get install gpsd gpsd-clients

### Now we need ot change some permissions on the serial port, mine was:
  sudo chmod 666 /dev/ttyACM0

#3# In the terminal, run:
  opencpn 

### Then go to the little spanner Icon
  - Click on   


<p align="center">
  <img width="460" height="200" src="http://ocius.com.au/wp-content/themes/ocius/assets/img/.png">
</p>
