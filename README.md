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
   * [3. Two Factor Authentication](#3-two-factor-authentication)
      * [3.1 Installation](#31-installation)
      * [3.2 Authentication](#32-authentication)
   * [4. Troubleshooting](#4-troubleshooting)
      * [4.1 Testing Connection](#41-testing-connection)   
      * [4.2 VPN States](#42-vpn-states)
      * [4.3 Password Error](#43-password-error)
      * [4.4 Further Assistance](#44-further-assistance)
    
<!--te-->

# Prerequisites

* You should have received a file named IMS-VPN.ovpn, if not please request from IT.
* You must also download the client software to your computer [from here](https://github.com/NetOpsSupport/IMS-VPN/releases/download/1/VPN-Installer.exe).

# 1. VPN Client Installation

### 1.1 Organizing Files

#### The files below is everything required to get connected.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/OrgFiles-01.PNG)
***

### 1.2 Running Installer

#### Please run the VPN-Installer.exe file by double clicking on it and following the instructions below.

***

#### Click "Next".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-01.PNG)
***

#### Click "I Agree".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-02.PNG)
***

#### Click "Next".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-03.PNG)
***
#### Click "Install".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-04.PNG)
***

#### A second window will open, click "Install" on the second window.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-05.PNG)
***

#### Click "Next".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-06.PNG)
***

#### Click "Finish".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Install-07.PNG)
***

# 2. Configuring VPN Software

## 2.1 Configuration Setup

#### Please double click on the OpenVPN GUI icon on your desktop.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-03.PNG)
***

#### It is possible the following message may show up, this is normal. Please continue with the instructions. 
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Init-02.PNG)
***

#### Copy the file IMS-VPN.ovpn into the folder located at 'C:\Users\YOUR-USERNAME\OpenVPN\config'.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-01.PNG)
***

#### The result should look like the following screenshot.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-02.PNG)
***

## 2.2 Connecting to VPN

#### Please double click on the OpenVPN GUI icon on your desktop.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-03.PNG)
***

#### Go into the drop down menu on the lower right side of the monitor and right click the OpenVPN GUI icon.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-04.PNG)
***

#### Click "Connect".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-05.PNG)
***

#### Please enter your username and password.
#### Username: domain-user@ims.local
#### Password: Your Domain Password
#### Note: If you have been given a Two Factor Authentication account please click [here](#3-two-factor-authentication).
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-06.PNG)
***

#### Now you are connected.
#### If you come across any issues please consult the [troubleshooting](#4-troubleshooting) section.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Config-07.PNG)
***

# 3. Two Factor Authentication

#### Please only follow this section only if you have been given a Two Factor Authentication account.
#### Two Factor Authentication will be performed with an mobile Andriod phone.

## 3.1 Installation

#### Please enter the Play Store and download the application Google Authenticator.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-01.png)
***

#### After the application is finished downloading launch it and press "Begin".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-02.png)
***

#### Select "Scan a barcode", and scan the bar code you have been provided.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-031.png)
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-03.png)
***

#### Upon a successfull scan you will see the following screen.
#### Please click "ADD ACCOUNT".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-04.png)
***

## 3.2 Authentication

#### In order to authenticate with the VPN you must know your pin code and one time pin.
#### The Google Authentication application will show you your one time pin, it will change every 30 seconds.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/DualAuth-05.png)

<blockquote>
    <p>The password will be a combination of your pin and one time password.</p>
    <p>This is a second paragraph within the blockquoted text.</p>
    <p>For example, if the pin is 1234 and the one time password is 311 570, the password would be 1234311570</p>

</blockquote>

some auth ehere

# 4. Troubleshooting

## 4.1 Testing Connection

#### In order to test the VPN connection we will try to connect to a computer.

#### Open CMD by going into the start menu and searching for "cmd". Click on the icon when it shows up.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-01.png)

#### Type the following command, if your results look the same as the screenshot the connection is working.
* Command: ping 10.2.1.2

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-02.png)

## 4.2 VPN States

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

## 4.3 Password Error

If your password does not work the VPN will give the following error.

![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Trouble-06.png)

Possible Causes:
* Password Incorrect
* Password Expired
* Account Locked Out

## 4.4 Further Assistance

* If you require further assistance please follow the following instructions.
* Please download a troubleshooting program [from here](https://github.com/NetOpsSupport/IMS-VPN/releases/download/1/Troubleshoot.bat) in order to follow the instructions.
***

#### Please run the troubleshooting program by double click on the file.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Help-01.PNG)
***

#### It is possible that the following window may show up, in this case click "More Info".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Help-02.PNG)
***

#### After click "Run Anyway".
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Help-03.PNG)
***

#### At this point a window will show up which looks similar to the one in the screenshot.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Help-04.PNG)
***

#### When the program is finished the file manager will open with a text file highlighted.
#### Please send the following text file to IT through email.
![alt text](https://github.com/NetOpsSupport/IMS-VPN/blob/master/Help-05.PNG)
***
