# RaspberryPi

This details projects using my RaspBerry Pi 4

## Gitlab

To install gitlab on the raspberry, I used the official instructions at 
https://about.gitlab.com/install/

but with one addition: 
I had to override the locale settings, as I got an error message. 
Do 
export LC_ALL=C
before the installation, and it worked for me. 
I used the setting
sudo EXTERNAL_URL="http://192.168.0.XXX" apt-get install gitlab-ce
where XXX is the ip adress of my pi.
