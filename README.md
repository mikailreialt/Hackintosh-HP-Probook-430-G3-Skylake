Resources for HP Probook 430 G3 to run macOS
============================================

 ## This project is still in maintenance, feel free to create an issue incase you face any difficulty! ##

- Bootloader version: Opencore 0.9.3
- macOS version: macOS Ventura 13.4.1
![Oops, you are not supposed to see this!](https://lookimg.com/images/2023/07/05/QGUgVE.png)

#### WI-FI
- Intel WIFI Cards can be made to work using [Airporttlwm](https://github.com/OpenIntelWireless/itlwm). More Details about this [Here](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/Wireless.html).


#### Working Normally
- iGPU acceleration (Intel HD 520)
- Sleep
- Battery Percentage
- Display Brightness
- USB ports
- Internal Camera
- Audio with mute button (Both internal speakers and Microphone) (CX20724)
- Native Power Management/(Also with cpufriend)
- SMBus Controller
- CPU Temperature Monitoring
- Fan Speed Monitoring
- VGA (*suprisingly*)
- Three Finger Gestures
- Boot Chime
- iMessage
- Facetime

#### Isn't work
- Built-In Realtek Wifi+Bluetooth (*unsupported*)

#### Specs

| Component      | Brand                                                            |
|----------------|------------------------------------------------------------------|
| **CPU**        | `Intel Core i5-6200U ` 
| **iGPU**       | `Intel HD Graphics 520 `                                         |
| **Audio**      | `Conexant 20724 - Layout ID 3`                                      |
| **Ethernet**   | `Realtek RTL8111/8168`                                           |
| **OS**         | `Ventura 13.4.1`

#### Making the Three Finger Gestures Work

- Open System Preferences->Keyboard->Shortcuts
![Oops!There was supposed to be an image here](https://i.imgur.com/pv0wnyy.png)
- Double-tap on shortcut you want it to perform.
- Do the Three Finger Gesture to set it.
- Voila! You're Done!

#### Not tested
- HDMI output (both audio and video)
- RTS522A PCI Express Card Reader
- (*Ideally both should work, If some is willing to test, create an issue*)

#### To Do
- ~~Add pci devices in system information~~  *done*
- ~~macOS Powerchime~~*done*
- ~~Real Time Clock Loss (RTC)~~ *done*
- ~~Battery Cycle count~~ *Fixed by updating to the Latest Bios*
- ~~Fan Speed Monitoring~~ *done*
- Let me know more 

#### Benchmarks
- Geekbench 5 (Not Up to Date!) [Multi-core and Single core](https://browser.geekbench.com/v5/cpu/8013906)

#### Important
- In the config.plist, section `PlatformInfo > Generic`, the following fields are currently edited with CHANGEME. Please generate your own serial. (Reccommended SMBIOS : MacBookPro14,1 for macOS Monterey and below, MacBookPro15,1 for Ventura and above) 

- This repo can be helpful for other HP Probook/Elitebook series notebooks (May Vary)
 
### Bios Configuration


#### Enable

- Fast Boot
- Runtime Power Management
- Extended Idle Power States
- Deep Sleep
- Power Control
- Turbo Boost
- Virtualization Technology (VTx)
- Hyperthreading
- Multi Processor

 #### Disable
 
- Legacy boot
- Wake when lid is opened
- Wake on USB


#### Having Problems?
Create an issue and I'll try to help as many as I can

#### Credits
- [Apple](https://apple.com) for [macOS](https://www.apple.com/macos/ventura/)
- [Acidanthera](https://github.com/Acidanthera) for [OpenCorepkg](https://github.com/acidanthera/OpenCorePkg) and necessary kexts
- [Krazy-Killa](https://github.com/Krazy-Killa) for the Three finger gestures
- [dortania](https://github.com/dortania) for its detailed guides
- [Corpnewt](https://github.com/CorpNewt) for [USBMap](https://github.com/corpnewt/USBMap)
- [Human79](https://github.com/Human79) for [Building This!](https://github.com/Human79/macOS-HP-Probook-430-G3-Resources)
