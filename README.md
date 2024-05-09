# Log in with root user in Ubunto

sudo -s 

sudo ufw allow 3389
sudo apt-get install tightvncserver
sudo apt-get install xrdp

sudo systemctl enable --now xrdp

nano /etc/xrdp/startwm.sh

# Before "if test ..." line, put these texts:
unset DBUS_SESSION_BUS_ADDRESS
unset XDG_RUNTIME_DIR
. $HOME/.profile


# Ctrl+X: to exit and save
# Reboot command

# if cannot connect, continue:
sudo apt-get -y install xserver-xorg-input-all

sudo apt-get install xorgxrdp

sudo apt-get install xserver-xorg-core

# if full blue screen and no reponse:
sudo apt-get install xorgxrdp-hwe-18.04
