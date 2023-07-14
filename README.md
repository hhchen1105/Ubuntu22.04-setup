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
0. Install and setup screen
0. Install Lambda stack
	- https://lambdalabs.com/
0. Sync with Google Drive via insync
0. Install KeepassX
0. Install git
0. Install and setup vim
0. Install build-essential
0. Install Python3 and alias Python to Python3
0. Install pyenv
0. Install PyTorch and Tensorflow in pyenv and verify GPU utilization
0. Setup Google Account
0. Install and setup git and github
0. Install 嘸蝦米
0. Use Software updater to update packages
0. Setup printer
0. Enable remote desktop using vino
