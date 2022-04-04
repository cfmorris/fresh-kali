# fresh-kali
Procedures for setting up a kali box after its inevitably destroyed. Update this list next time with the information needed to automate as much as possible with .sh scripts.  Create a git repo for THM and cryptohacks stuff for redundancy.

# You did it again?
1. sudo apt update
2. sudo apt full-upgrade
3. sudo reboot now

fix graphics output:

1. sudo apt install nvidia-detect nvidia-drivers nvidia-cuda-toolkit
2. sudo reboot now
3. nvidia-smi
4. lspci | grep -i vga

Dev Environment:
1. VS code (wgettable?)
2. Discord (wgettable?)
3. sudo apt install ruby sqlite3 node yarn
4. sudo gem install rails
5. postgresql should be good, but but get the local dev DB running (document this).
6. sudo apt install git heroku htop

CyberSec Stuff:
1. sudo apt install gobuster
2. sudo wget -c https://github.com/danielmiessler/SecLists/archive/master.zip -O /usr/share/wordlists/seclists.zip
3. cd /usr/share/wordlists
4. sudo unzip seclists.zip
5. sudo gzip -d rockyou*
6. openvpn stuff
7. update burp
8. set up foxy proxy, Burp CA Certificates
9. download standalone jython for burp

#Tips for not bricking kali:
- installing R seems to have weird and inexplicable consequences.  Figure out how to use a virtual environment.
- sudo apt uninstall python3 is a silly command to enter.  Fix broken dependency paths another way.
