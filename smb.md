# SMB

## What is smb

SMB - Server Message Block Protocol - is a client-server communication protocol used for sharing access to files, printers, serial ports and other resources on a network.<br><br><br>

![](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-13%20233219.png)

Here in the picture we see that **smb** is running on ports 139 and 445.<br>
Samba, an open source server that supports the SMB protocol, was released for Unix systems.<br><br><br>


# Enumeration

Enumeration is the process of gathering information on a target in order to find potential attack vectors and aid in exploitation.<br>
Enumeration can be used to gather usernames, passwords, network information, hostnames, application data, services, or any other information that may be valuable to an attacker.

The syntax of Enum4Linux is nice and simple: "enum4linux [options] ip"

 ![enum4linux TAG picture](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-13%20234504.png)<br><br>

For the example, we have used the enum4linux -S [ip] command in this image.
![enum4linux -S [ip] picture](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-13%20235524.png)<br><br><br>


# SMBClient
Because we're trying to access an SMB share, we need a client to access resources on servers. We will be using SMBClient because it's part of the default samba suite.<br><br>

Syntax: smbclient //[IP]/[SHARE] -U [USERNAME] -p [PORT]
                                                                                                                                                     
![smbclient picture](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-14%20001751.png)

As shown in the picture, you can type the help command to see what commands you can use.
