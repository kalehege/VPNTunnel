||Google||

 sudo -s

sudo adduser "username"

usermod -aG sudo "username"

exit

||End Google||

||Setup Vpn||

su "username" (Google Only)

sudo -s (Google Only)

cd ..

cd home

mkdir vpn

cd vpn

wget https://github.com/kalehege/VPNTunnel/blob/main/ubi18.sh

chmod +x ubi18.sh

./ubi18.sh

reboot (VPs server reboot)

sudo -s

menu (and create new user)

http://IPVPS:10000 (root login)

