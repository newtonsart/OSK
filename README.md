# OSK
Windows password changer.

Please don't use this for illegal purposes.

## Usage
1. Download **[ParrotOS](https://parrotlinux.org/download-security.php)** Security Edition.
2. Flash ParrotOS onto a USB. You can use **[BalenaEtcher](https://www.balena.io/etcher/)**.
3. Boot live from parrot (IMPORTANT): select Forensics Mode to avoid traces...
4. Mount the windows partition ([How to mount a windows partition](https://www.tecmint.com/mount-windows-partition-in-ubuntu/))
5. Open a terminal and write:
```
git clone https://github.com/newtonsart/win-password-recovery
cd win-password-recovery
sudo python3 OSK.py
```
6. Wait until the program is finished, shutdown the computer and boot Windows.
7. In the login screen run On Screen Keyboard. It will appear a Terminal with administrator permissions.
8. In the terminal run the following code to change the password:
```
net user {USERNAME} {NEW_PASSWORD}
```
 ## How it works???
 It basically changes the program of the On Screen Keyboard to a Terminal with administrator permissions, that way, you'll be able to change the password of any user once you run the On Screen Keyboard in the login screen.
 
 ## Built with
* [Python 3](https://www.python.org/downloads/) - The language used.
* Python modules used: os.
