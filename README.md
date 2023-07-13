# URdata-DepthmapX
Fast installation of DepthmapX(https://github.com/SpaceGroupUCL/depthmapX/blob/master/docs/about.md) in Classroom with 20 Linux Computers.

cat /etc/os-release

![alt text](https://github.com/zvonkoilich/URdata-DepthmapX/blob/main/os-release.jpg?raw=true)



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
