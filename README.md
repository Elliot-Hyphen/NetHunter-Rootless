# NetHunter-Rootless
Install Kali NetHunter on any stock &amp; Unrooted Android device without voiding the warranty.

<h1> How to Install Nethunter with KeX (rootless) </h1> 

__Install Kali NetHunter on any stock, unrooted Android device without voiding the warranty.__

**Prerequisite:**

Android Device (Stock unmodified device, no root or custom recovery required)



**Installation:**

# 1 
Install the NetHunter-Store app from store.nethunter.com

From the NetHunter Store, install Termux, NetHunter-KeX client, and Hacker’s keyboard Note: The button “install” may not change to “installed” in the store client after installation - just ignore it. Starting termux for the first time may seem stuck while displaying “installing” on some devices - just hit enter.

# 2  
Open Termux & Type 
```
termux-setup-storage

pkg install wget

wget -O install-nethunter-termux https://offs.ec/2MceZWr

chmod +x install-nethunter-termux

./install-nethunter-termux
 ```
__Commands__
```
nethunter                 | start Kali NetHunter command line interface
nethunter kex passwd      | configure the KeX password (only needed before 1st use)
nethunter kex &           | start Kali NetHunter Desktop Experience user sessions
nethunter kex stop        | stop Kali NetHunter Desktop Experience
nethunter <command>       | run in NetHunter environment
nethunter -r              | start Kali NetHunter cli as root
nethunter -r kex passwd   | configure the KeX password for root
nethunter -r kex &        | start Kali NetHunter Desktop Experience as root
nethunter -r kex stop     | stop Kali NetHunter Desktop Experience root sessions
nethunter -r kex kill     | Kill all KeX sessions
nethunter -r <command>    | run <command> in NetHunter environment as root
```

*Note: The command nethunter can be abbreviated to nh. Tip: If you run kex in the background (&) without having set a password, bring it back to the foreground first when prompted to enter the password, i.e. via fg <job id> - you can later send it to the background again via Ctrl + z and bg <job id>
To use KeX, start the KeX client, enter your password and click connect Tip: For a better viewing experience, enter a custom resolution under “Advanced Settings” in the KeX Client*

__Personal Opinion__
I wouldn't use any Andriod device for any real/and or actual PenTesting/Training -- This guide is made just for testing /Having fun with NetHunter.

*Guide* - `https://www.kali.org/docs/nethunter/nethunter-rootless/`

*APP Link* `https://store.nethunter.com/`

**TIPS:**
# Run sudo apt update && sudo apt full-upgrade -y first thing after installation to update Kali. If you have plenty of storage space available you might want to run sudo apt install -y kali-linux-default as well.

# All of the penetration testing tools should work but some might have restrictions, e.g. metasploit works but doesn’t have database support. If you discover any tools that don’t work, please post it in our forums.

# Some utilities like “top” won’t run on unrooted phones. 

# Non-root users still have root access in the chroot. That’s a proot thing. Just be aware of that.

# Galaxy phone’s may prevent non-root users from using sudo. Just use “su -c” instead.

# Perform regular backups of your rootfs by stopping all nethunter sessions and typing the following in a termux session: tar -cJf kali-arm64.tar.xz kali-arm64 && mv kali-arm64.tar.xz storage/downloads That will put the backup in your Android download folder. Note: on older devices, change “arm64” to “armhf”

# Please join us in our forums to exchange tips and ideas and be part of a community that strives to make NetHunter even better. 
