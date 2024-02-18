# Raspberry Pi + Ansible + Docker

I want to learn how to manage my raspberry pi's with ansible.

This is in preparation of my raspberry pi cluster project.

## Initial Outcomes

As a prereq to managing a cluster of Pis, I want to learn how to manage one Pi to run docker containers.

Use ansible to setup the Pi.

How do I deploy containers to the Pi tho? Can ansible do that?

## Starting point

So what is ansible, and how can I manage one Pi with it?

I'm on mac os, and my Raspberry Pi 4 B is running headless rasp os.

How do I get started with ansible?

### Side notes

Turn off / remove bluetooth

`sudo vim /boot/firmware/config.txt`

add this line `dtoverlay=disable-bt`

then run these lines

```sh
sudo systemctl disable hciuart.service
sudo systemctl disable bluetooth.service
sudo apt purge bluez
sudo apt autoremove
sudo reboot
```
