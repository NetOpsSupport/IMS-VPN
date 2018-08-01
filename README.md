# Connecting To IMS VPN
<!-- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet -->
# Table of contents
<!--ts-->
   * [Table of contents](#table-of-contents)
   * [Prerequisites](#prerequisites)
   * [1. VPN Client Installation](#1-vpn-client-installation)
      * [1.1 Organizing Files](#11-organizing-files)   
      * [1.2 Running Installer](#12-running-installer)   
    * [2. Configuring VPN Software](#2-configuring-vpn-software)
      * [2.1 Configuration Setup](#21-configuration-setup)   
      * [2.2 Connecting to VPN](#22-connecting-to-vpn)
    * [3. Troubleshooting](#3-troubleshooting)
      * [3.1 Testing Connection](#31-testing-connection)   
      * [3.2 VPN States](#32-vpn-states)
      * [3.3 Password Error](#33-password-error)
    
<!--te-->

# Prerequisites

* You should have received a file named IMS-VPN.ovpn, if not please request from IT.
* You must also download the client software to your computer [from here](https://github.com/NetOpsSupport/IMS-VPN/releases/download/1/VPN-Installer.exe)

# 1. VPN Client Installation

### 1.1 Organizing Files

#### The files below is everything required to get connected.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/OrgFiles-01.PNG)
***

### 1.2 Running Installer

#### Please run the VPN-Installer.exe file by double clicking on it

#### Click "Next"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-01.PNG)
***

#### Click "I Agree"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-02.PNG)
***

#### Click "Next"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-03.PNG)
***
#### Click "Install"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-04.PNG)
***

#### A second window will open, click "Install" on the second window
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-05.PNG)
***

#### Click "Next"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-06.PNG)
***

#### Click "Finish"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-07.PNG)
***

# 2. Configuring VPN Software

## 2.1 Configuration Setup

#### Copy the file IMS-VPN.ovpn into the folder located at C:\Users\YOUR-USERNAME\OpenVPN\config
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-01.PNG)
***

#### The result should look like the following screen shot
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-02.PNG)
***

## 2.2 Connecting to VPN

#### Double click on the OpenVPN GUI icon on the desktop
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-03.PNG)
***

#### Go into the drop down menu on the lower right side of the monitor and right click the OpenVPN GUI icon
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-04.PNG)
***

#### Click "Connect"
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-05.PNG)
***

#### Please enter your username and password
#### Username: domain-user@ims.local
#### Password: Your Domain Password
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-06.PNG)
***

#### Now you are connected
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-07.PNG)
***

# 3. Troubleshooting

## 3.1 Testing Connection

#### In order to test the VPN connection we will try to connect to a computer.

#### Open CMD by going into the start menu and searching for "cmd". Click on the icon when it shows up.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-01.png)

#### Type the following command, if your results look the same as the screenshot the connection is working.
* Command: ping 10.2.1.2

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-02.png)

## 3.2 VPN States

The bottom right drop down menu contains an icon which changes color, depending on the state of the VPN connection.

### Connected State (Green)

* Connected state means that the VPN is connected and working.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-03.png)

### Connecting State (Yellow)

* Connecting state means that a connection to the VPN is attempting to be made.
* This happens every time you connect to the VPN in the beginning of a session.
* This can also occur if your computer has lost internet temporarily.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-04.png)

### Disconnected State (Grey)

* Disconnected state means that the VPN is not active.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-05.png)

## 3.3 Password Error

If your password does not work the VPN will give the following error.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-06.png)

Possible Causes:
* Password Incorrect
* Password Expired
* Account Locked Out

