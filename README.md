# URdata-DepthmapX
Fast installation of DepthmapX in Classroom with 20 Linux Computers.

cat /etc/os-release 
PRETTY_NAME="Ubuntu 22.04.2 LTS"
NAME="Ubuntu"
VERSION_ID="22.04"
VERSION="22.04.2 LTS (Jammy Jellyfish)"
VERSION_CODENAME=jammy
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=jammy


For remote access I installed ssh service on all computers.

sudo apt install openssh-server

sudo systemctl enable ssh
    

For wakeup computers was used wol.service, which is installed, too.

sudo apt install net-tools

tar xfav wol.tgz 

sudo ./installwoll.sh


For DepthmapX-runtime, was needed library Qt.

sudo apt-get install qtbase5-dev

sudo tar --absolute-names -x -f installZI-p.tar
