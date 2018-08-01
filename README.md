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

* You should have received a file named "IMS VPN.ovpn", if not please request from IT.
* You must also download the client software to your computer [from here](https://github.com/NetOpsSupport/IMS-VPN/releases/download/1/VPN-Installer.exe)

# 1. VPN Client Installation

### 1.1 Organizing Files

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/OrgFiles-01.PNG)

### 1.2 Running Installer


![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-01.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-02.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-03.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-04.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-05.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-06.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-07.PNG)

# 2. Configuring VPN Software

## 2.1 Configuration Setup


![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-01.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-02.PNG)


## 2.2 Connecting to VPN

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-03.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-04.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-05.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-06.PNG)

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-07.PNG)

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

