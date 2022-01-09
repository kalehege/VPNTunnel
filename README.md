
# Setup SSL SSH VPN Server

its Ezzzzz


## Google User only Installation

# Setup VPC Network
You have to get a static IP address for the instance. In the main menu, select “external IP address” under “VPC network”. Change the IP type to “Static”. The Static IP address is not change during restart the server.

Now, you have to set a firewall rule to allows VPN server ports. In the VM instances page, click “setup firewall rule” at the bottom of the page. Then, click “crate firewall rule” button at the top of the page. Enter a name for the rule and change the target to “all instance in the network”. If you want you can choose a specific target. Enter this source IP range to allow all ranges of IP addresses.

IP  Range: 0.0.0.0/0

Under protocols and ports, select allow all to open all port of the VPS. After all, click “create” button at the bottom. Now, VPS setup is over. Let’s see how to create a VPN server.

Click “SSH” button of the VM instance to get terminal window. To get root access, enter the command.
```bash
sudo -s
```
You have to add a user to the server. 

```bash
sudo adduser username
```
Now, give root access to new user using this command. Replace username that you entered.
```bash
usermod -aG sudo username
```
Use exit command to log out in root user.

```bash
exit
```
Log in to the new user, entering the password.

```bash
su username
```
Use this command to get root access and enter the user password.
```bash
 sudo -s
```
change root password

```bash
sudo passwd
```
## Package Installation

Go to home path and create directory  

```bash
 sudo -s
```
Go to home path and create directory 
```bash
 cd  ..
 cd home
 mkdir vpn
 cd vpn
```

Now, we finished the adding a new user and gave the root access. Download the VPN server script using this command.
```bash
 wget https://github.com/kalehege/VPNTunnel/raw/main/ubi18.sh
```
Use this line for make sure the script is executable.
```bash
 chmod +x ubi18.sh
```
Now execute the script using this command. This takes some time to get ready your server. Please be peasant.
```bash
 ./ubi18.sh
```
### Installation Complete
##  Webmin Admin Access

You can access your VPN server using Webmin IP address that was given by the server information. login in using administrator user we initially created.
```bash
 http://IPVPS:10000

```
## Go to dashboard and click update and install. and wait for end session

## Add a New VPN User
Before adding a user, reboot the VPN server using this command. It may cause to disconnection of the terminal window for a few moments. Try to connect it again.

You can type “menu” to get all VPN server commands.
```bash
 menu
```
Use new user command and add the asking credentials. You have to enter user name, password and expiration time of the account. Then, copy the all details of the user.

Now, all set at the server side. Let’s see how to configure client side.

# Connect to HTTP Injector


## Authors

- [@kalehege](https://github.com/kalehege)


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


## Feedback

If you have any feedback, please reach out to us at fake@fake.com

