# SMB

## What is smb

SMB - Server Message Block Protocol - is a client-server communication protocol used for sharing access to files, printers, serial ports and other resources on a network.<br><br><br>

![](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-13%20233219.png)

Here in the picture we see that **smb** runs on TCP 139 (NetBIOS) and 445 (Direct SMB).<br>
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

As shown in the picture, you can type the help command to see what commands you can use.<br><br><br>

**For educational use only. Do not use on systmes you do not own or have permission to test.**<br><br><br>


If you want practical exercises, follow this [link](https://tryhackme.com/room/networkservices)<br><br><br>

# Ftp
## What is ftp?

File Transfer Protocol (FTP) is, as the name suggests , a protocol used to allow remote transfer of files over a network. It uses a client-server model to do this, and- as we'll come on to later- relays commands and data in a very efficient way.<br><br>


![picture of ftp](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-15%20205914.png)

As you can see in the picture, ftp is running on port 21.<br><br>

It can be used with the **ftp [ip]** command

![](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-15%20210614.png)<br><br><br>


# Telnet
## What is telnet

Telnet is an application protocol which allows you, with the use of a telnet client, to connect to and execute commands on a remote machine that's hosting a telnet server.

The telnet client will establish a connection with the server. The client will then become a virtual terminal - allowing you to interact with the remote host.<br><br>

![telnet port](https://github.com/Andreas512514/Network-Services/blob/main/Screenshot%202025-10-15%20231106.png)

As you can see in the picture here, telnet is on port 23.s
