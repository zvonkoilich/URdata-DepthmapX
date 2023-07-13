# URdata-DepthmapX
Fast installation of DepthmapX in Classroom with 20 Linux Computers

For remote access I installed ssh service on all computers.

sudo apt install openssh-server
sudo systemctl enable ssh
    

For wakeup computers was used wol.service, which is installed, too.
sudo apt install net-tools


For DepthmapX-runtime, was needed library Qt.

sudo apt-get install qtbase5-dev
sudo tar --absolute-names -x -f installZI-p.tar
