## TryHackMe Desktop Application
![ScreenShot](https://i.imgur.com/QXLXiZp.png)

## Requirements

- Ubuntu & Debian based (+ MacOS)
```
sudo apt install nodejs
sudo apt install npm
```
- Arch linux
```
sudo pacman -S nodejs
sudo pacman -S npm
```
- Fedora linux
```
sudo dnf install nodejs
sudo dnf install npm
```

## Automatic Installation 
Run multi-install.sh like so:
`sh multi-install.sh`

## Manual Installation
Run the following commands in the exact same order
```
mkdir tryhackme && cd tryhackme

wget https://i.imgur.com/HiIWSQq.png -O icon.png

nativefier -p linux -a x64 -i icon.png --disable-context-menu --disable-dev-tools --single-instance --internal-urls ".*" https://tryhackme.com/

mv TryHackMeLearnCybersecurity-linux-x64 TryHackMe && cd TryHackMe && mv TryHackMeLearnCybersecurity TryHackMe 

chmod 777 TryHackMe

./TryHackMe
```

## Extra
It is recommended to add the application to **/opt** folder for ease of usage.
```
sudo mv TryHackMe/ /opt/

cp /icon.png /opt/TryHackme

sudo chmod 777 -R /opt/TryHackMe/
```
