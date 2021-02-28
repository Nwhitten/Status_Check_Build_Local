
## Installation

### Automatic

`wget -O - https://raw.githubusercontent.com/nwhitten/Status_Check_Build/master/install.sh | sudo bash`


### Additional Requirements
need to run:
`(crontab -l; echo "*/10 * * * * python3 /usr/local/bin/status_check/inky_update.py";) | crontab -`
to install cron job to refresh pihole stats on inky-phat every 10 mins

you will also need to install the following:

Inky Phat library `sudo curl https://get.pimoroni.com/inky | bash`

Unicorn Phat library `sudo curl -sS https://get.pimoroni.com/unicornhat | bash`

button shim library `sudo curl https://get.pimoroni.com/buttonshim | bash`

PiHole-api `sudo python3 -m pip install --no-cache-dir PiHole-api`

zero tier `sudo curl -s https://install.zerotier.com | sudo bash` (extra setup required)

Net Talk `sudo apt install netatalk -y` (extra setup required)
