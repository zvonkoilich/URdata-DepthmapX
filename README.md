# URdata-DepthmapX
Fast installation of DepthmapX(https://github.com/SpaceGroupUCL/depthmapX/blob/master/docs/about.md) in Classroom with 20 Linux Computers (https://github.com/zvonkoilich/URdata-DepthmapX/blob/main/ClassRoom-Installation). 
Working under pressure.

cat /etc/os-release

![alt text](https://github.com/zvonkoilich/URdata-DepthmapX/blob/main/os-release.jpg?raw=true)



For remote access I installed ssh service on all computers.

sudo apt install openssh-server

sudo systemctl enable ssh
    


For wakeup computers was used wol.service, which is installed, too.

sudo apt install net-tools

tar xfav wol.tgz 

sudo ./installwoll.sh


Tar archive (installZI-p.tar) content:

![alt text](https://github.com/zvonkoilich/URdata-DepthmapX/blob/main/depthmapX2023-tar.jpg?raw=true)

For DepthmapX-runtime, was needed library Qt.

sudo apt-get install qtbase5-dev

sudo tar --absolute-names -x -f installZI-p.tar

How to add applications icon to taskbar?

dconf write /org/gnome/shell/favorite-apps "['firefox_firefox.desktop', 'org.gnome.Nautilus.desktop', 'libreoffice-writer.desktop', 'snap-store_ubuntu-software.desktop', 'code_code.desktop', 'vlc_vlc.desktop', 'org.gnome.Terminal.desktop', 'depthmapX.desktop']"

