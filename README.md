
# Setup Free VPN Server

its Ezzzzz


## Google User only Installation

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
## Package Installation

Go to home path and create directory

```bash
 sudo -s
```
Now, we finished the adding a new user and gave the root access. Download the VPN server script using this command.
```bash
 wget https://github.com/kalehege/VPNTunnel/blob/main/ubi18.sh
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

## Add a New VPN User
Before adding a user, reboot the VPN server using this command. It may cause to disconnection of the terminal window for a few moments. Try to connect it again.

```bash
 reboot
```
You can type “menu” to get all VPN server commands.
```bash
 menu
```
Use new user command and add the asking credentials. You have to enter user name, password and expiration time of the account. Then, copy the all details of the user.

Now, all set at the server side. Let’s see how to configure client side.

# Connect to HTTP Injector
## Authors

- [@katherinepeterson](https://github.com/kalehege)


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


## Feedback

If you have any feedback, please reach out to us at fake@fake.com

