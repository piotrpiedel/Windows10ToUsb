# Windows10ToUsb
Windows10ToUsb is a BATCH script that installs Windows 10 on an external disk/drive.  

I took inspiration from https://github.com/riklus/win10install-onusb/

## How to use it

### Things to prepare:

- Installation medium: The USB or DISK where to put the Windows 10 `.iso` installation files. Meaning do the bootable windows 10 usb stick.
- Target drive: The USB disk/drive where you would like to install Windows 10.
- `wininstall.bat`: The script that installs Windows 10 on the Target drive.

### Usefull commands:
1. list disk - lists all disks
2. list volume - lists all partitions

### What to do:

1. **First of all:** Download Windows 10 `.iso` from Microsoft.
2. Copy all data inside the `.iso` to your Installation medium.
3. Copy `wininstal2.0.bat` file *from this repo* to the Installation medium.
4. Shutdown the computer.
5. **Boot the pc from the installation medium.**
6. Proceed to install Windows 10 as usual but stop after accepting the Windows License Conditions.
7. Press `shift+f10` to open up a cmd window.
8. Launch the script: `C:\wininstall.bat` and follow the instructions on the screen.


**Done.**

### Things to pay attention to

Be sure to select the right *Target drive*.  
Be sure to Accept Windows License Conditions before launching the script.  
Be sure to enter the *Target drive* size correctly, if unsure subtract a few MB from the number before entering it.  

## FAQ

### Who is it for?

For those who want a Windows 10 to go, or have very low internal hardisk space.

### What does this script do?

This script will install Windows 10 on the *Target drive*:  
It will ERASE all data from the *Target drive* then it will proceed to partition it, like the official Windows 10 installer would do.  
Then it will install Windows 10 on the *Target drive*.  
And at the end, it will shutdown the pc.

### Once the installation began, can I leave the pc alone for the night?

Yes. The script it's made that once the installation ends it will automatically shutdown the pc.
### Does it work for Windows 11?

I don't know. Sorry :/

