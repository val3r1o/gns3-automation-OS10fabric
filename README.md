# gns3-automation-OS10fabric

From clean Ubuntu desktop 20.04 to GNS3 running OS10 basic project

sudo apt update</br>
sudo apt install git<br>
git clone https://github.com/val3r1o/gns3-automation-OS10fabric.git <br>
cd gns3-automation-OS10fabric <br>
sudo chmod 755 install.sh <br>

#run the script</br>
./install.sh

now, run GNS3 and import the project under /gns3-automation-OS10fabric/single-leaf</br>

Seems a reboot is needed.

Have fun.

# NOTES:
set DNS to reach public internet </br>
DNS set to resolve repo </br>
# 1
When prompted whether non-root users should be allowed to use wireshark and ubridge, select ‘Yes’ both times</br>
Run GNS3 from Shell or GUI </br>
First run:  next->next->next (no changes) i.e., localhost -> TCP:3080 & /usr/bin/gns3server
# 2
Import (not open) the project wait GNS3 to import </br>
Double check if the interfaces are correctly connected also on the OOB switch </br>
Run the nodes!! 
# 3
if not able to consol on OS10: edit->preferences-> console application -> edit: KDE/KONSOLE <- this package is already installed by the script.
OS10 usr/psw is standard admin/admin</br>
Setup the mgmt interface to the preferred oob IP for your network. example config provided </br>
