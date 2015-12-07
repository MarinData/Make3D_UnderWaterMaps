How to make UnderWaterMaps using OpenDroneMap

It uses the open source software from OpenDroneMap
- https://github.com/OpenDroneMap/OpenDroneMap

## Instructions

### AWS
Make an account on amazon if you dont have ubuntu, or of you dont have enough cpu power for the calculations
- http://aws.amazon.com/

Launch a ec2 instance (and choose to create a "ubuntu" machine)

Choose a c type instance ( this cost some $ but it calculates faster)

Then you have to ssh into the ubuntu machine, EXemple bellow:   
- chmod 400 /Users/larsbrusletto/Documents/MASTER/odm_key.pem
- ssh -i /Users/larsbrusletto/Documents/MASTER/odm_key.pem ubuntu@54.77.92.209

### Install git and other programs to run OpenDroneMap
- sudo apt-get -y install git
- sudo apt-get update
- git clone https://github.com/OpenDroneMap/OpenDroneMap
- cd OpenDroneMap;
- ./install.sh

### OpenDroneMap
Then follow this instructions:
- https://github.com/OpenDroneMap/OpenDroneMap/wiki/2.-Running-OpenDroneMap


### Using FileZila
To get the folders from your remote ubunto machine on AWS
Download FileZila - https://filezilla-project.org/download.php
then: 
- https://www.youtube.com/watch?v=e9BDvg42-JI&index=45&list=PLR3c0t83cVzS4MJwSeLSr46slVCcDfc52

Send over your image files by draging your files into the right hans side folders under Ubuntu

Then run OpenDroneMap on your dataset.

When the 3d maps are created. Drag them over to your desktop using FilZila. 

### Warning
Warning. Remember to terminate the AWS ec2 instance as it cost money. 
When you terminate the server. All the data will be lost. 
