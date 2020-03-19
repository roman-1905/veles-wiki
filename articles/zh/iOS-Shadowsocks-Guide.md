Name:           Veles iOS Shadowsocks Guide
Image:          https://www.veles.network/images/download/mac-wallet.png
Date:           Feb 12 2020,
Version: 		1.01
Syntax:         Markdown
Authors:        @AltcoinBaggins @mdfkbtc

# iOS Shadowsocks Guide 
This will guide you through the process of installing and using Shadowsocks on the iOS platform.  

If you require further assistance contact the support team @ [Discord](https://discord.gg/P528fGg)

## Requirements
1) **Install Shadowsocks Client**  
2) **Download Veles Shadowsocks config**  

## Contents
* **Section A**: Download and Install Shadowsocks
* **Section B**: Configure Shadowsocks
* **Section C**: Connect to Veles d-VPN with Shadowsocks
* **Section D**: Test Shadowsocks Connection
***

### Section A: Download and Install Shadowsocks

***Step 1***  

* From the App Store, search for and install **Sockswitch**.

***

### Section B: Configure Shadowsocks 

***Step 1***  

* After installing Sockswitch, **download [Veles Shadowsocks config file](https://explorer.veles.network/dapi/getShadowsocksConfig)**.  
[https://explorer.veles.network/dapi/getShadowsocksConfig](https://explorer.veles.network/dapi/getShadowsocksConfig)

***

***Step 2***  

* **Start the Sockswitch app** and tap the **+** to add the profile and press **Manual Input**.

***

***Step 3***  

* Then fill **"Hostname"** with **IP of Masternode** located in Shadowsocks Config.

***

***Step 4***  

* **"Remote Port"** replace with Veles Remote Port **21344**

***

***Step 5***  

* Change **"Encryption Method"** to **aes-256-cfb**

***

***Step 6***  

* Fullfill the **"Password"** with password located in Shadowsocks Config.  

!!! caution "Experimental Warning"
	In testing phase is default password - **`password`**  

***

### Section C: Connect to Veles d-VPN with Shadowsocks 

***Step 1***  

* **Start the connection by sliding the Connect button to the On position**.  

!!! tip "User Tip"
	**Disconnect** by sliding the same button to **Off**.  

***

### Section D: Test Shadowsocks Connection

***Step 1***  

* Once everything is installed, a simple check confirms everything is working properly. Without having a Shadowsocks connection enabled, open a browser and go to [DNSLeakTest](https://www.dnsleaktest.com/).
The site will return the IP address assigned by your internet service provider and as you appear to the rest of the world. To check your DNS settings through the same website, click on Extended Test and it will tell you which DNS servers you are using.
Now connect to your Shadowsocks client and refresh the browser. The completely different IP address of your Shadowsocks  server should now appear. That is now how you appear to the world. Again, [DNSLeakTest's](https://www.dnsleaktest.com/) **Extended Test** will check your DNS settings and confirm you are now using the DNS resolvers pushed by Veles dVPN.

***

If you do, congratulations! You have now setup a Veles d-VPN . If you do not, please contact support on [Discord](https://discord.gg/P528fGg) and they will assist you.  
