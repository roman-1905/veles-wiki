Name:               Veles Core Masternode Guide
Image:              https://veles.network/images/mn/veles-mnguide-thumb.png
GuideType:          Masternode Operator's Guide
OS:                 Linux
Generation:			1st
Requirements:       500 VLS, VPS/server, local wallet, SSH client
Difficulty:         Easy
EstimatedTime:      5 minutes

# Linux masternode guide 

This is a step-by step tutorial on how to set-up Veles Masternode on a Linux Server , taking advantage of [Veles Masternode Installer](https://github.com/Velescore/veles-masternode-install) script.

If you require further assistance contact the support team @ [Discord](https://discord.gg/P528fGg)

## Supported Linux distributions
* **Ubuntu**
* **Debian**
* **Linux Mint**
* **Gentoo**
* **Sabayon**
* **Fedora**
* **RHEL**
* **CentOS**

## Requirements
1) **500 VLS**  
2) **VPS running Linux (one of mentioned in start of guide)**  
3) **A local wallet**  
4) **An SSH client such as [PuTTY](https://the.earth.li/~sgtatham/putty/0.72/w64/putty-64bit-0.72-installer.msi) or [BitVise](https://dl.bitvise.com/BvSshClient-Inst.exe)**  
***

## Contents
* **Section A**: Downloading and installing BitVise
* **Section B**: Connecting to the VPS and installing the MN script via BitVise
* **Section C**: Preparing the local wallet
* **Section D**: Connecting & Starting the masternode
***

### Section A: Downloading and installing BitVise

***Step 1***  

* Download BitVise [here](https://dl.bitvise.com/BvSshClient-Inst.exe)  

***

### Section B: Connecting to the VPS & Installing the MN script via Bitvise


***Step 1***  

* Open the bitvise application and fill in the **"Hostname"** box with the **IP of your VPS**

![Example-PuttyInstaller](/images/guides/mn1.png)  

***

***Step 2***  

* Copy the **root password** from your VPS

![Example-RootPass](/images/guides/mn2.png)

***

***Step 3***

* Type **"root"** as the login/username

![Example-Root](/images/guides/mn3.png)  

***

***Step 4***  

* Paste the password into the Bitvise terminal by right clicking (it will not show the password so just press enter)

![Example-RootPassEnter](/images/guides/mn4.png)

***

***Step 5***  

* Once you have clicked open it will open a security alert (**click yes**)   

***

***Step 6***  

* **Paste the code below** into the Bitvise terminal then press enter and wait:  
`source <(curl -s https://raw.githubusercontent.com/velescore/veles-installer/master/masternode.sh)`

![Example-RootPassEnter](/images/guides/mn5.png)  

***

***Step 7***  

* Enter your veles **Masternode Private Key** or leave it blank to generate a new Masternode Private Key for you

![Example-RootPassEnter](/images/guides/mn6.png)

***

### Section C: Preparing the Local wallet

***Step 1***  

* Download and install the Veles wallet [here](https://veles.network/download.html)

***

***Step 2***  

* Generate new address through debug console with command:   
`getnewaddress "MN1" "legacy"`  

* Send exactly **500 VLS** to the address you generated on your local wallet

![Example-console](/images/guides/mn7.png)  

***

***Step 3***  

* Go to the console within the wallet and type the command below and press enter:  
`masternode outputs`  

![Example-outputs](/images/guides/mn8.png)  

***

***Step 4***  

* Copy the **transaction ID and output index**

***

### Section D: Connecting & Starting the masternode 

***Step 1***  

* Go to the **"tools"** tab within the wallet and click open **"masternode configuration file"**  

***

***Step 2***  

* Fill in the form. 
* For `Alias` type something like "MN01" **don't use spaces**
* The `Address` is the **IP of your server** (this will be in the Bitvise terminal that you still have open).
* The `PrivKey` is your **masternode private** key (This is also in the Bitvise terminal that you have open).
* The `TxHash` is the **transaction ID/long key** that you copied to the text file.
* The `Output Index` is the **0 or 1** that you copied to your text file.

![Example-create](/images/guides/mn9.png)

* Click **"File Save"**  

***

***Step 3***  

* Close out of the wallet and reopen Wallet
* Click on the Masternodes tab **"My masternodes"**
* Check if your Masternode collateral transaction have **16 confirmations**
* Click start alias in the **masternodes tab**

![Example-create](/images/guides/mn10.png)

***

***Step 4***  

* Connect your VPS and **change your user from root to veles** by this command:    
`su veles` 

* Check the **status of your masternode** within the VPS by using the command below:  
`veles-cli masternode status`  
  
* Veles user commands :   
`veles-cli masternode status` #To check your MN status  
`veles-cli getblockchaininfo` #To get general info such as Veles version and current block numnber  
`veles-cli mnsync status` #To check if your MN is synced.  

* Root user commands :  
`systemctl status veles.service` #To check if Veles service is running  
`systemctl start veles.service` #To start Veles service  
`systemctl stop veles.service` #To stop Veles service  
`systemctl is-enabled veles.service` #To check if Veles service is enabled on boot  

***

If you do, congratulations! You have now setup a Veles d-VPN . If you do not, please contact support on [Discord](https://discord.gg/P528fGg) and they will assist you.  
