# Install Ubuntu Mate
https://ubuntu-mate.org/

## Download requirements for bootable flash drive
- Secure a flash drive that has at least 2GB storage capacity
- Download unetbootin in https://unetbootin.github.io/
- Downloads ubuntu mate in https://ubuntu-mate.org/

## Make the flash drive bootable
- Launch unetbootin
- Select the ubuntu mate image
- Select the flash drive for the installation
- Click create button to begin installation

## Change the BIOS for the flash drive
- Access the BIOS to prioritize the flash drive to boot
- Change the approriate settings like secure boot or EUFI
- Save the new BIOS settings

## Try and install ubuntu mate
- After booting select try without installing option
- Try and test machine features if it is functioning correctly like brightness buttons, etc
- If ubuntu mate satisfies your requirements, click the install icon located in the desktop
- Wait for the installation to finish and reboot the computer

## Update and upgrade
sudo apt-get update && apt-get upgrade

## Install virtualbox
- Open the terminal and copy and paste the command below and press enter

'''
sudo sh -c "echo 'deb http://download.virtualbox.org/virtualbox/debian '$(lsb_release -cs)' contrib non-free' > /etc/apt/sources.list.d/virtualbox.list" && wget -q http://download.virtualbox.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add - && sudo apt-get update && sudo apt-get install virtualbox-5.0
'''

- Wait for the process to finish
- Install xp virtual machine
- Install guest additions
- Install Virtualbox extension pack

## Install GNS3

'''
sudo add-apt-repository ppa:gns3/ppa
sudo apt-get update
sudo apt-get install gns3-gui

# IOU support
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install gns3-iou
'''

## Install MP3 plugins

'''
sudo apt-get install ubuntu-restricted-extras
'''

## Contributing
Please click the link below to follow contribution instructions.
https://github.com/cemax/ubuntu-mate-bootstrap
