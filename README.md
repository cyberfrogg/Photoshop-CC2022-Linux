# Photoshop-CC2022-Linux

## Important

**Please note that the GUI version might not work on your distribution. it worked with some older packager and has broken since. if you used the GUI and it hasn't worked, please try to use the CLI installer wieh a sh file in the RELEASE section. (avoid cloning as master branche can have experimental changes)**

**DISCLAIMER :**
**Please use this software only if you have an active Photoshop subscription. I'm not responsable of any use without subscription.**

This git repo contains an installer for photoshop CC 2022 on linux with wine.

Note that Photoshop CC 2022 isn't as stable as the CC2021 version on linux. If you need a production environement, concidere using PS2021 instead

If you use something from my repo in your project please credit me

| Version  | Rating |
| ------------- | ------------- |
| [CC 2021](https://github.com/MiMillieuh/Photoshop-CC2022-Linux/releases/tag/2.1.1)  | Works almost like on Windows  |
| [CC 2022](https://github.com/MiMillieuh/Photoshop-CC2022-Linux/releases/tag/2.1.1)  | Not ready for production... Basic functions works, No GPU acceleration  |

![Screenshot from 2022-05-17 00-02-27](https://user-images.githubusercontent.com/52078885/168690419-274020b0-c993-4b86-a58f-f0f07237aa4f.png)

*File download is about 2GB*

## Requirements
- wine >=6.1 (Avoid 6.20 to 6.22 **DON'T USE STAGING**) 

(Wine 8.0+ are causing an issue with the windows version see workaround [here](https://github.com/MiMillieuh/Photoshop-CC2022-Linux/issues/94#issuecomment-1426776219))
- zenity
- appmenu-gtk-module
- tar
- xz
- wget
- curl
- All R/W rights on your home folder and the installer folder
- Vulkan capable GPU or APU


## Usage : 

**CLI :**

`sh photoshop2022install.sh /path/to/your/install/folder`

**Camera Raw**
You can install Camera Raw this way :

`curl -L "https://download.adobe.com/pub/adobe/photoshop/cameraraw/win/12.x/CameraRaw_12_2_1.exe" > CameraRaw_12_2_1.exe`
`WINEPREFIX=/Path/To/Your/Photoshop/Install/Adobe-Photoshop wine CameraRaw_12_2_1.exe`

To use camera raw you need to change a settings
Edit -> preferences -> Camera raw... -> performance -> Use graphic processor : Off

If camera raw is sometimes grayed out, just go to : Edit -> preferences -> Tools, and uncheck show Tooltips.



**GUI :**

**THIS METHODE IS DEPRECATED PLEASE USE CLI**

Open photoshop installer :

![Screenshot from 2022-05-17 00-14-15](https://user-images.githubusercontent.com/52078885/168692144-a1819955-c541-4248-bca2-ef4ed248e4bf.png)

Click on install and chose the install folder (You must have acces to it):

![Screenshot from 2022-05-17 00-14-56](https://user-images.githubusercontent.com/52078885/168692184-62e2c937-fa4b-43e8-ab8a-449015b42994.png)

Wait for the install (It can take a long time depending on your internet and computer speed) :

![Screenshot from 2022-05-17 00-17-28](https://user-images.githubusercontent.com/52078885/168692197-c861e67a-01e0-436d-8169-6d23a0aa4edb.png)

Once it's done you can close the window :

![Screenshot from 2022-05-17 00-20-39](https://user-images.githubusercontent.com/52078885/168692210-7093c10d-310d-45f4-98fb-0d8eb25609f5.png)

Then you can launch Photoshop :

![Screenshot from 2022-05-17 00-21-04](https://user-images.githubusercontent.com/52078885/168692218-dd1dd912-83a8-4746-aafa-da7f0a9673c3.png)

**Uninstalling :**

To uninstall remove the photoshop desktop file in *~/.local/share/applications/* then your installation folder


## Special thanks to
- The WineHQ team : For making wine
- Gictorbit : For initial inspiration
- HansKristian-Work : For making VKD3D-Proton
- Adobe : For making Photoshop (also please release an official version for linux...)




## Donate

This isn't necessary but it helps paying the hosting server



BTC : 1LDKrdTKGHtGRjDSL2ULxGGzX4onL5YUsp

ETH : 0x57bf06a94ead7b18beb237e9aec9ae3ef06fe29a

BUSD : 0x57bf06a94ead7b18beb237e9aec9ae3ef06fe29a
