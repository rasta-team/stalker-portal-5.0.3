# Stalker Portal 5.0.3 install on Ubuntu 20.04 LTS / 18.04 LTS

Stalker Portal auto install script on Ubuntu 20.04 LTS / 18.04 LTS

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?hosted_button_id=4H8VAGMLW5RMA)  You can make one-time donations via PayPal.

##### Runs on
[![Ubuntu](https://user-images.githubusercontent.com/12951085/139538206-833d8d33-0d1b-4d51-8ec8-86e5cf14f82e.png)](https://www.ubuntu.com)

This script work only on Clean Ubuntu 20.04 LTS / 18.04 LTS

Stalker auto install script
  * Version of Stalker 5.0.3

## Installation
```bash
apt-get install git
git clone https://github.com/rasta-team/stalker-portal-5.0.3.git
cd stalker-portal-5.0.3/
```

Open stalker_portal_5.0.3.sh with your favorite text editor and change on line 11
```bash
mysql_root_password="test123456"
```
This is the root password for MySQL that will be set during the installation, you can change it with yours if you wish.


And on line 10 change
```bash
TIME_ZONE="Asia/Kuala_Lumpur"
```
This is the time zone that will be set during the installation, you can change it with yours if you wish

The installation itself is as follows:
```bash
chmod +x stalker_portal_5.0.3.sh
./stalker_portal_5.0.3.sh
```
Accordingly, during the installation, when executing the last command, phing will ask you for the root password for MySQL, enter the password you set on line 11



You can access your stalker portal at: http://ipadres/stalker_portal The username and password to login to the portal are your default
```
Login: admin
pass: 1
```

Remove all test channels from the database through the terminal
```bash
mysql -u root -p stalker_db
truncate ch_links;
truncate itv;
```

## Video

[![Click to Watch](https://img.youtube.com/vi/kTqCdGys1OU/hq720.jpg)](https://www.youtube.com/watch?v=kTqCdGys1OU "Click to Watch")


[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?hosted_button_id=4H8VAGMLW5RMA)  You can make one-time donations via PayPal.
