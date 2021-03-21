# Intall Alpine in VirtualBox

## Install virtualbox

```sh
sudo apt update -y
sudo apt install -y virtualbox
```

## Download Alpine virt

```sh
# download iso
wget "https://dl-cdn.alpinelinux.org/alpine/v$(wget -qO - https://alpinelinux.org/downloads | grep -Piom 1 'alpine\s+version.*\d+\.\d+\.\d+' | grep -Po '\d+\.\d+')/releases/x86_64/alpine-virt-$(wget -qO - https://alpinelinux.org/downloads | grep -Piom 1 'alpine\s+version.*\d+\.\d+\.\d+' | grep -Po '\d+\.\d+\.\d+')-x86_64.iso"
# download sha256 sum
wget "https://dl-cdn.alpinelinux.org/alpine/v$(wget -qO - https://alpinelinux.org/downloads | grep -Piom 1 'alpine\s+version.*\d+\.\d+\.\d+' | grep -Po '\d+\.\d+')/releases/x86_64/alpine-virt-$(wget -qO - https://alpinelinux.org/downloads | grep -Piom 1 'alpine\s+version.*\d+\.\d+\.\d+' | grep -Po '\d+\.\d+\.\d+')-x86_64.iso.sha256"
# check sum
sha256sum -c alpine-virt-*-x86_64.iso.sha256
```

## Install Alpine on VirtualBox

Install the OS

[![Install alpine in virtualbox](http://img.youtube.com/vi/KbouH7hnSOk/0.jpg)](http://www.youtube.com/watch?v=KbouH7hnSOk "Install alpine in virtualbox")

Remove iso image and configure ssh

[![alpine configure root ssh](http://img.youtube.com/vi/Cj4PFQw8BsE/0.jpg)](http://www.youtube.com/watch?v=Cj4PFQw8BsE "alpine configure root ssh")
