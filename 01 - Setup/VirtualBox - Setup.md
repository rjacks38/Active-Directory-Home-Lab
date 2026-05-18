
Goal:
Create a Windows Server VM for Active Directory

VM Specs
Name: DC 
RAM: 2048 MB
CPUs: 1

Notes
Using Windows Server 2022 Server Eval ISO 
Using Windows 11 ISO

## After finishing Setup Of Win and Creating PW

1. Click File Explorer --> This PC --> Guest Additions --> Run amd64, and install. *can make VM run smoother.*

2. Click "I want to boot manually"
3. Then shut VM down completely

## Labeling the two Networks

1. Go to network 
2. Click "change adapter settings"
3. Label the network that is connected to home internet to "_Internet_"
4. Label the other "X_Internal_X"

## Rename PC

1. Right Click Windows Icon --> System --> Rename This PC
2. Rename PC to "DC"
3. Click Next and Restart 

## Configure "Internal" Network Settings

1. Go to Network Settings 
2. Right click on "Internal", click Properties
3. Click "IPv4"
4. Click use the following IP address:

IP address: 172.16.0.1
Subnet mask: 255.255.255.0

Preferred DNS Server: 127.0.0.1

