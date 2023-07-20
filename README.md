# Ubuntu22.04-setup

0. Create an Ubuntu live usb 
    - Create it from Ubuntu: use the startup disk creator tool provided by Ubuntu
    - Create it from Mac: https://ubuntu.com/tutorials/create-a-usb-stick-on-macos  
    - Sometimes after reinstallation and restart, the grub2 may get wrong.  If this happens, follow the following instruction.
    
      **You need to ensure (hd0,msdos1)/boot/grub exists** before running the following commands; sometimes grub could be in other places, e.g., (hd0,msdos5)/boot/grub
      ```
      grub> ls (hd0,msdos1)/
      grub> set boot=(hd0,msdos1)
      grub> set prefix=(hd0,msdos1)/boot/grub
      grub> insmod normal
      grub> normal
      ```
      Sometimes may need to change BIOS boot loader sequence.

0. Setup Network
0. Install Google Chrome
0. Install openssh-server and enable ssh connection
	```
	sudo apt install openssh-server
 	/etc/init.d/ssh restart
	```
0. Install and setup screen
0. Install Lambda stack
    - (Don't do this for the desktop machine at my office...the screen goes black after installation and rebooting)
    - https://lambdalabs.com/lambda-stack-deep-learning-software
0. Sync with Google Drive via Insync
0. Install KeepassX
   ```
   sudo apt install keepass2
   ```
0. Install git
   ```
   sudo apt install git
   ```
0. Install and setup vim
   ```
   sudo apt install vim
   ```
0. Install build-essential
   ```
   sudo apt install build-essential
   ```
0. Install Python3 and alias Python to Python3
   - Python3 is likely installed by default.  Check it before installation.
0. Install and setup pyenv
0. Install PyTorch and Tensorflow in pyenv and verify GPU utilization
0. Install and setup git and GitHub
0. Install 嘸蝦米
0. Use Software updater to update packages
0. Setup printer
0. Enable remote desktop
