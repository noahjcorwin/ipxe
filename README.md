# Requirements
sudo apt update \
sudo apt install nginx tftpd-hpa isc-dhcp-server nfs-kernel-server


# Create Directories
sudo mkdir /distros \
sudo mkdir /tftpboot \
sudo mkdir /isos \
sudo mkdir /mnt/isos

# Download ISO and unpack
sudo wget -O ubuntu-20.04.3-desktop-amd64.iso https://releases.ubuntu.com/20.04.3/ubuntu-20.04.3-desktop-amd64.iso \
sudo mount -o loop /isos/ubuntu-20.04.3-desktop-amd64.iso /mnt/iso \
sudo mkdir /distros/ud2004 \
sudo cp -r /mnt/iso/. /distros/ud2004