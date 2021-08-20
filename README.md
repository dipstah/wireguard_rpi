Setup RPI 4 , wireguard 

headless boot after burning im to SD card

enable SSH create file in SDcard boot partition
touch ssh

Enable Wifi create wpa_supplicant.conf in SDcard boot partitio
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=US

network={
   ssid="SSID"
   psk="PASSWORD"
}

boot PI
Update PI 
sudo apt-get update && sudo apt-get upgrade -y

Change Hostname
Change Password
reboot

**raspi-coonfig 
update local settings (timezone, keyboard, etc...)

sudo apt-get install wireguard



