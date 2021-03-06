# NetHunter-Rootless
Install Kali NetHunter on any stock &amp; Unrooted Android device without voiding the warranty.

<h1> How to Install Nethunter with KeX (rootless) </h1> 

__Install Kali NetHunter on any stock, unrooted Android device without voiding the warranty.__

**Installation**

1 ) 
Install the NetHunter-Store app from store.nethunter.com

From the NetHunter Store, install Termux, NetHunter-KeX client, and Hacker’s keyboard Note: The button “install” may not change to “installed” in the store client after installation - just ignore it. Starting termux for the first time may seem stuck while displaying “installing” on some devices - just hit enter.

2 ) 
Open Termux & Type 
```termux-setup-storage

  pkg install wget

  wget -O install-nethunter-termux https://offs.ec/2MceZWr

  chmod +x install-nethunter-termux

 ./install-nethunter-termux
 ```
__Commands__
```
nethunter - `start Kali NetHunter command line interface`
nethunter kex passwd - `configure the KeX password (only needed before 1st use)`
nethunter kex & - `start Kali NetHunter Desktop Experience user sessions`
nethunter kex stop - `stop Kali NetHunter Desktop Experience`
nethunter <command> - `run in NetHunter environment`
nethunter -r - `start Kali NetHunter cli as root`
nethunter -r kex passwd - `configure the KeX password for root`
nethunter -r kex &	     - `start Kali NetHunter Desktop Experience as root`
nethunter -r kex stop	   - `stop Kali NetHunter Desktop Experience root sessions`
nethunter -r kex kill	   - `Kill all KeX sessions`
nethunter -r <command>	 - `run <command> in NetHunter environment as root`
```

*Note: The command nethunter can be abbreviated to nh. Tip: If you run kex in the background (&) without having set a password, bring it back to the foreground first when prompted to enter the password, i.e. via fg <job id> - you can later send it to the background again via Ctrl + z and bg <job id>
To use KeX, start the KeX client, enter your password and click connect Tip: For a better viewing experience, enter a custom resolution under “Advanced Settings” in the KeX Client*

__Personal Opinion__
I wouldn't use any Andriod device for any real/and or actual PenTesting/Training -- This guide is made just for testing /Having fun with NetHunter.

*Guide* - `https://www.kali.org/docs/nethunter/nethunter-rootless/`

*APP Link* https://store.nethunter.com/
