# **Hackintosh Opencore Guide**

# 

# **Getting Started...**



###### OpenCore is a modern and powerful bootloader used to run macOS on non-Apple computers, commonly known as Hackintosh systems. It focuses on stability, security, and accuracy, making the system behave as close as possible to a real Mac.

###### 

###### Before starting with OpenCore, it’s important to understand your computer’s hardware. Things like the CPU, GPU, motherboard, and Wi-Fi card must be compatible with macOS. Without proper hardware support, macOS may not boot or work correctly.

###### 

###### The next step is preparing the required files. OpenCore uses an EFI folder that contains essential components such as drivers, ACPI files, and the main configuration file called config.plist. This file controls how macOS communicates with your hardware, so careful setup is very important.

###### 

###### Once the EFI folder is ready, it is placed on a USB installer or directly on the system’s EFI partition. After booting through OpenCore, macOS installation can begin just like on a real Mac.

###### 

###### Although OpenCore can seem difficult at first, following official documentation and guides step by step makes the process much easier. With patience and attention to detail, OpenCore provides a reliable way to experience macOS on compatible hardware.







# **Program/ Files used...** (Direct Download Link)



https://apps.microsoft.com/detail/9pnrbtzxmb4z?hl=en-US\&gl=US

https://github.com/lzhoang2801/OpCore-Simplify/archive/refs/heads/main.zip

https://github.com/USBToolBox/tool/releases/download/0.2/Windows.exe

https://github.com/USBToolBox/kext/releases/download/1.2.0/USBToolBox-1.2.0-RELEASE.zip

https://github.com/ic005k/OCAuxiliaryTools/releases/download/20250001/OCAT-Win64.zip

https://github.com/pbatard/rufus/releases/download/v4.11/rufus-4.11.exe

https://github.com/acidanthera/OpenCorePkg/releases/download/1.0.5/OpenCore-1.0.5-RELEASE.zip



# **Install progress...**



\*\*Install all files that will be uses further

1st extracted the OpCore-Simplify and launch an app inside, follow the step inside to create an EFI folder!

2nd Download the USB toolbox tool and you will get a kext file

3rd Download the USB toolbox kext and put both kext into EFI>OC>Kext

4th Open the OCAT app in its folder then press Ctrl+O to open the config.plist file

5th Click Kext in the sidebar then click the "+" button to add the 2 new kexts

6th Read the next progress, ur close :D



# **Making the installer...**



Open CMD 

Type in:

cd ~/Downloads/OpenCore-1.0.5-RELEASE/Utilities/macrecovery/ (Or where you download the "OpenCore-1.0.5-RELEASE" file)



## **Commands to download the installer:**





###### **Mojave (10.14)**

###### **python3 ./macrecovery.py -b Mac-7BA5B2DFE22DDD8C -m 00000000000KXPG00 download**

###### 

###### **Catalina 10.15**

###### **python3 ./macrecovery.py -b Mac-CFF7D910A743CAAF -m 00000000000PHCD00 download**



###### **Big Sur 11**

###### **python3 ./macrecovery.py -b Mac-2BD1B31983FE1663 -m 00000000000000000 download**

###### 

###### **Monterey 12**

###### **python3 ./macrecovery.py -b Mac-E43C1C25D4880AD6 -m 00000000000000000 download**

###### 

###### **Ventura 13**

###### **python3 ./macrecovery.py -b Mac-B4831CEBD52A0C4C -m 00000000000000000 download**

###### 

###### **Sonoma 14**

###### **python3 ./macrecovery.py -b Mac-827FAC58A8FDFA22 -m 00000000000000000 download**

###### 

###### **Sequoia 15**

###### **python3 ./macrecovery.py -b Mac-7BA5B2D9E42DDD94 -m 00000000000000000 download**

###### 

###### **Tahoe 26**

###### **python3 ./macrecovery.py -b Mac-CFF7D910A743CAAF -m 00000000000000000 -os latest download**





# **Putting everything together!!!**



##### **SO after you got all the files working format a USB flash drive as FAT 32 then put both 'com.apple.recovery.boot' and 'EFI' in there.** 

##### **After the flash drive is working boot into BIOS and set 'Secure Boot' and 'Fast Boot' off then boot using the flash drive now install macOS then your done!!**

