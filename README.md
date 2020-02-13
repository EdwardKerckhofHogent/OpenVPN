# OpenVPN

### Step 1
#### Upgrade Ubuntu server to latest packages
  -  sudo apt-get update
  -  sudo apt-get upgrade
  -  reboot
  
### Step 2
#### Install OpenVPN
  -  sudo apt install openvpn
  
### Step 3
#### Install the OpenVPN configuration script
  -  wget [Raw Script](https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh)
  -  chmod +x openvpn-install.sh (make script runnable)
  -  sudo AUTO_INSTALL=y ./openvpn-install.sh (run script)
  
### Step 4
#### Download client.ovpn to client
  -  scp root@SERVER_IP:path_to_client.ovpn out_path (ex: scp root@127.0.0.1:client.ovpn /home/user/Desktop/)
