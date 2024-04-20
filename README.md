# How to install Ubuntu Server to Raspberry Pi
## Abstract
This is a memorandum on installing Ubuntu Server to Raspberry Pi.  
## Targets
- Ubuntu Server 22.04.4 LTS
- Raspberry pi 3 model B
- 64GB SD Memory Card
- Windows 11 home
## Download and Install Raspberry Pi Imager
1. Click the link below to access the Raspberry Pi official site.  
	[Raspberry Pi OS](https://www.raspberrypi.com/software/)
2. Go to the section titled *"Install Raspberry Pi OS using Raspberry Pi Imager"*.
3. Click *"Download for Windows"* to download the '.exe' file below.  
	*imager_1.8.5.exe*  
4. Execute the downloaded file.
5. Click *"YES"* button on the UAC dialog.
6. The *Raspberry Pi Imager Installer* will start.
7. Click *"Install"* button at *"Welcome to Raspverry Pi Imager Setup"*.
8. Click *"Finish"* button at *"Completing Raspberry Pi Imager Setup"*.
## Download Raspberry Pi Server Image
1. Click the link below and access Ubuntu official site.  
	[Install Ubuntu on a Raspberry Pi](https://ubuntu.com/download/raspberry-pi)  
2. Go to the section titled *"Ubuntu 22.04.4 LTS"*
3. Click *"Download Ubuntu Server 22.04.4 LTS"* to download the '.xz' file below.  
	*ubuntu-22.04.4-preinstalled-server-arm64+raspi.img.xz*  
4. Unzip the download file to the '.img' file below.
	*ubuntu-22.04.4-preinstalled-server-arm64+raspi.img*  
## Write Raspberry Pi Server Image to SD Memory card
1. Set the SD Memory card to your Windows machine.
2. Start *Raspberry Pi Imager* from Windows start menu.
3. Choose these items.
	- Choose *"Raspberry Pi 3"* from the device lists.
	- Choose *"Use custom"* from the OS lists. And open the unzipped '.img' file below.  
		*ubuntu-22.04.4-preinstalled-server-arm64+raspi.img*
	- Choose *"Generic STORAGE DEVICE USB Device - 63.9GB"* from the storage lists.
4. Click *"Next"* button.
5. Click *"Edit the settings"* button on the *"Use OF customizetion?"* dialog.
6. Edit your custom setteings.
	- General
		- Host name
		- User name and password
		- Wi-Fi settings
			- SSID
			- Password
			- Country
		- Locale Settings
			- Time zone
			- Keyboard layout
	- Service
		- Check *"Enable SSH"*
			- Use passworad authentication
			- Use only public encryption authentication
	- Option
		- Sound on finish
		- Remove the media on finish
		- Enable Telemetry
7. Click *"Yes"* button on the *"Use of customization?"* dialog.
8. Notice enough and click *"Yes"* on the *"Alert"* dialog.
9. Wait writing and verifing.
10. Click *"Continue"* button on *"Writing is over normally"* dialog after finish install and verify.
11. Remove the SD Memory card from your Windows machine.
12. Exit *Raspberry Pi Imager* by click the window close button.
## Boot Ubuntu Server on Raspberry pi
1. Set the SD Memory card to your Raspberry Pi module.
2. Connect LAN cable when not use Wi-Fi.
3. Turn on your Raspberry Pi module.
4. Have fun!

## References  
- [Ubuntu日和【第35回】3,000円未満の「Raspberry Pi Zero 2 W」でUbuntuを遊ぼう](https://pc.watch.impress.co.jp/docs/column/ubuntu/1531425.html)
- [Raspberry Pi Imagerのバージョンアップと詳細設定](https://raspida.com/rpi-imager181)
- [【Raspberry Pi】公開鍵認証でSSH接続する方法(ラズパイのセキュリティ設定)](https://elirlab.com/publickey-ssh/)
