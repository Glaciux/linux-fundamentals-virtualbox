# linux-fundamentals-virtualbox
Virtualbox with Ubuntu is used to practice a few Linux commands

### Setup Virtualbox
-- download virtualbox from the official website and install
-- download Ubuntu image from the official website and install
-- run the Ubuntu image on virtualbox and create an Ubuntu VM
![VirtualboxUbuntu](https://github.com/user-attachments/assets/1a9f72ab-294f-4844-b164-cb7eda8a7631)

### Ubuntu Configuration
![Ubuntu_properties](https://github.com/user-attachments/assets/42a4fbbb-7f3c-4292-aff3-8df6ed016f79)

### Folder creation
Use mkdir -p projects/devops
-- this creates two folders(directories) - projects as the parent directory and devops as a sub-directory in the projects folder
![Folders](https://github.com/user-attachments/assets/2f2ab467-c10e-4ff7-9673-5882d3f5e066)

### File Ownership and Permissions
-- create a file in the projects directory
touch file
-- assign execute permission to the owner of the file and read permissions to the group and other users
In essence, only the owner of the file can run/execute the file. Groups and other users can only view the file
chmod 744 file1
ls -l file1
ls -la
-- create user Kodecamp and chnage file ownership
sudo adduser kodecamp
sudo choown kodecamp file1
![File creation   permission](https://github.com/user-attachments/assets/dcbd7c59-7231-4a1a-b316-24db53ebd47b)
![User creation](https://github.com/user-attachments/assets/9a7fe1d3-e161-46fb-90d3-97ae2aa1a2d6)

### Install and configure a package
-- install curl 
sudo apt install curl
-- uninstall curl
sudo apt remove curl -y
![curl app installation](https://github.com/user-attachments/assets/8d052b06-f004-4726-b777-776eebad9573)
-- get the version
curl --version
![version](https://github.com/user-attachments/assets/cbdf06f8-d278-4cfd-8e9c-6acf9b1076c7)

### Networking
-- check network connectivity
ping google.com 
ping facebook.com
-- check listening ports
netstat -tulpn
ss -tulpn
![ping](https://github.com/user-attachments/assets/333a8c3b-1eca-4a6a-bc11-38da3639297d)
![Portss](https://github.com/user-attachments/assets/af1b1a58-e463-4321-893a-77ebd861e7ff)
