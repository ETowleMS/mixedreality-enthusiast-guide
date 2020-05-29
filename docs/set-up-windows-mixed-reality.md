---
title: Set up Windows Mixed Reality
description: How to set up your Windows Mixed Reality motion controllers, speech, and audio, and define your room boundary for a safe play space.
ms.topic: article
keywords: Windows Mixed Reality, Mixed Reality, Virtual Reality, VR, MR, get started, setup, motion controller, controller, speech, audio, seated, standing, boundary, graphics drivers, Microsoft Edge, chromium
---


# Set up Windows Mixed Reality

## Prequisites (Graphics Drivers)
Windows Mixed Reality requires a WDDM 2.2 or later graphics driver in order to complete Mixed Reality setup. If your PC does not already have a compatible graphics driver, please try these sources:
1. Check for the latest critical driver updates using Windows Update (**Start -> Windows Settings -> Update and Security -> Check for Updates**)
2. Check for the latest optional driver updates using Device Manager (Right-click **Start -> Device Manager** -> expand **Display Adapters** -> right-click on the graphics card, choose **Update Driver -> Search automatically for updated driver software**)
3. The website for the manufacturer (OEM) of your PC
4. The website for the manufacturer of the graphics card in your PC (e.g., AMD, Intel, NVIDIA)

### Graphics Driver Troubleshooting 
If Windows Mixed Reality setup says your graphics card doesn’t meet the requirements and you think it does, make sure your headset is plugged into the correct card.

This flow chart below helps further explain the best steps to acquire a WDDM 2.2 or later graphics driver.

![Troubleshooting Flow Chart for Graphics Drivers](images/graphics-driver.jpg)


## Set up your motion controllers
The first step is to set up your Motion Controllers. If you plan to use an Xbox gamepad or keyboard and mouse you can skip this step. 

**Note**: Windows Mixed Reality motion controllers require Bluetooth 4.0. If your PC does not have built-in Bluetooth, you will need to plug in a USB Bluetooth adapter that supports Bluetooth 4.0 to enable your motion controllers.

![Motion controllers](images/1050px-controllers.png)

### Get familiar with your motion controllers

![Get familiar with your motion controllers](images/1050px-controllers2.png)

### Pair your motion controllers with your PC

Power on controllers by pressing the Windows button for 2 seconds until LEDs light up.

Remove the battery cover from your controllers and find the small pairing button at the edge of the controller. Per the instructions in Mixed Reality Portal, hold this button down to pair with your PC

![Motion controller pairing](images/1050px-controllers3.png)

### Pairing successful

Once your controllers are paired successfully, you will see two green checkmarks for the left and right controllers

![Motion controller pairing successful](images/1050px-controllersconnected.png)

You may see a message in the bottom right hand corner of your screen as the firmware on your controllers get updated. While this is happening, you can advance to the next step in the tutorial, but please don't turn off your controllers.

Once controller firmware update is complete it will restart and re-connect to host PC. LEDs will be solid on and bright.

### Common issues
* Verify you have one and only one Bluetooth radio active on your PC. If you have more than one Bluetooth radio, you’ll need to disable the other radios in Device Manager.
* Place your Bluetooth dongle in a port that has a clear line of sight to your controllers, and far from plugged in USB 3.0 devices. USB 3.0 is known to have RF interference with Bluetooth (read [this paper](https://www.intel.com/content/dam/www/public/us/en/documents/white-papers/usb3-frequency-interference-paper.pdf) from Intel for more details). USB 2.0 ports may work better for your Bluetooth dongle.
* Make sure your Bluetooth dongle is not plugged into a USB port adjacent to your HMD's USB cable. The HMD's cable has been known to cause interference with Bluetooth dongles as well. Plug the dongle into the front USB port on your PC for best results.
* For notebook ensure WiFi is connected to 5GHz band for best experience (click wireless network icon bottom right tray, select properties for the network you are connected). Notebooks that are designed to share a 2.4GHz antenna for Bluetooth and WiFi connectivity are most likely to see data congestion in the form of slow network speeds or poor tracking performance for motion controllers
* Your motion controllers will receive new software updates from Microsoft on a regular basis. The controllers will show an alternating pattern of flashing lights when they receive these new software updates. This is normal. You will want to wait until the controllers complete the software upgrade, indicated by a vibration and the replacement of the alternating flash pattern with a constant light emitted from the controllers, in order to use the controllers
* You may be told to "Put on the headset and use the thumbstick to teleport" before the controllers finish the update process. The controllers will not be visible or usable until the update is completed. Most updates occur within 2mins, but it's possible the occasional update is as long as ~10mins. Please wait for the update to complete to proceed to the next step

## Set up your room boundary

The next step is to choose a room scale or desk scale experience:

**Option 1: Set me up for all experiences (also known as room scale)** will allow you to walk around the room and is the most immersive mixed reality experience. We recommend you at clear at least 5 foot x 7 foot (1.5 meters x 2 meters) of space for mixed reality.

**Option 2: Set me up for seated and standing (also known as desk scale)** experience will work at your desk. It's a good option if you don't have a lot of room in your space. It also means that you will be using your headset without a boundary. You'll need to stay in one place, as you'll have no boundary to help you avoid physical obstacles. Also, some apps and games may be designed to be used with a boundary, so they might not work as intended.

![Choose a setup](images/1050px-chooseasetup.png)

### If you choose "Set me up for all experiences"

Soon, your room will become a virtual world where you can walk around and interact! Stand up and clear some space in your room for running mixed reality (e.g. clear some floor space and move your chair to the side of the room). We recommend you at clear at least 5 foot x 7 foot (1.5 meters x 2 meters) of space for mixed reality.

![Make sure your space is clear](images/1050px-createaboundary.png)

Make sure your space is clear.

![Center your headset](images/1050px-createaboundary-2.png)

Center your headset.

![Trace your boundary](images/1050px-createaboundary-3.png)

Trace your boundary.

![Stay pointed towards PC](images/1050px-createaboundary-4.png)

Keep your headset pointed toward your PC.

![Here's your boundary](images/1050px-createaboundary-5.png)

Here's your boundary.

### If you choose "Set me up for seated and standing"

There are no additional steps required if you choose this option.

## What is the maximum size of the boundary?
The currently supported maximum boundary size in Windows Mixed Reality is 18x18ft (5.7x5.7m) or 13ft (4m) radius from the center.  The boundary size is dependent on the anchor point and how far from the anchor point you can move before you risk the stability of the boundary.  Windows Mixed Reality is built on a stage abstraction in the platform, the stage being the space you move around in, and that stage depends on a single anchor (which nearly every app also assumes – it’s how Vive and Oculus work too, as they only have a single coordinate system).  The reason that this is important is that with inside-out tracking, as you move further away from an anchor point the headset tracking is reliable at keeping the boundary stable.  Where the boundary is intended to help avoid physical obstacles, it becomes more and more of a problem the further out from the center you go.  Two factors went into the decision on maximum boundary size; the maximum distance at which Windows Mixed Reality headsets could provide the best room scale experience with a boundary and the length of the headset cable, which for most Windows Mixed Reality headsets is 10ft (3m). 

## Set up speech

You can enable Cortana commands inside of mixed reality. This allows you to use speech commands inside of mixed reality to teleport, open apps, and do other things. You'll learn more about this in the [Learn Mixed Reality](learn-mixed-reality.md) chapter.

![Mixed reality is better with speech](images/1050px-betterwithspeech.png)

## Set up your audio headset

Unless you purchased a Samsung HMD Odyssey (which has integrated AKG headphones and an integrated dual microphone array), you will need to get an audio headset (that has both microphone and headphones) and plug that into your headset's 3.5mm audio jack. The 3.5mm audio jack for your headset will - depending on the headset model - be located either on the underside of the headset visor or at the end of a short audio cable coming out of the headset visor.

## Adjusting your headset's display settings

Windows Mixed Reality automatically chooses display settings that balance quality and performance, based on your PC's hardware configuration. To adjust these settings, go to **Settings > Mixed Reality > Headset display**.

### Visuals

This setting controls the visual quality of your Mixed reality home. The default is "Automatic".

### Resolution

Your headset's native resolution is shown here.

If you connect a headset with higher resolution displays (for example, headsets with 4320x2160 displays) to your PC, you'll see a setting to adjust the Mixed reality display resolution.

* This setting provides the option for the Windows Mixed Reality composition stack to render natively (for example, at 4320x2160), or to have the composition stack render at a lower resolution and upscale (for example, render at 2880x1440 and upscale to 4320x2160.
* The default setting is to render natively (for example, the **4320 x 2160 (best quality)** option) to provide the best visual quality possible from your headset.
* If your PC does not meet the minimum graphics hardware requirements for your headset with higher resolution displays, and/or if you're seeing graphics performance issues, you could try using selecting the **Automatic upscaling (best performance)** option.

This setting is available on Windows 10, version 1903, or newer.

### Calibration

This setting is to adjust the IPD calibration for headsets with software IPD support.

### Experience options

This advanced setting overrides the default headset display refresh rate experience.

* **Automatic (default)**: Automatically select the 60Hz or 90Hz experience based on your PC's hardware configuration.
* **60Hz**
* **90Hz**

Certain Windows Mixed Reality features, including Mixed Reality Portal preview and a larger headset display FOV, are only available with the 90Hz experience.

### Input switching

This setting controls the behavior of Windows Mixed Reality in response to your headset's presence sensor:

* **Automatically switch using headset presence sensor** (default): Windows will automatically direct input (keyboard, mouse...) to Windows Mixed Reality whenever you're wearing your headset. You can override this at anytime with Win + Y.
* **Manually switch using Windows logo key + Y**: Windows will not use the headset presence sensor to detect when you're wearing your headset. You'll need to use Win + Y to switch your input between your PC desktop and Windows Mixed Reality.

This setting is available on Windows 10, version 1903, or newer.

## Installing Microsoft Edge (Optional)

To use the new Chromium-based Microsoft Edge in Windows Mixed Reality home, **upgrade to Windows 10 Version 1903 or later for native support of Win32 applications (like the new Microsoft Edge)** in Windows Mixed Reality home. Check Windows Update or [manually install the latest version of Windows 10](https://www.microsoft.com/software-download/windows10).

>[!IMPORTANT]
>The new Microsoft Edge launches with support for WebXR, the new standard for creating immersive web experiences for VR headsets. When you install the new Microsoft Edge, you will no longer be able to play WebVR experiences in Microsoft Edge. 

### Issues with the new Microsoft Edge in Windows Mixed Reality

**Known issues resolved by the 2020-01 Cumulative update for Windows 10 Version 1903 (or later)**
- Launching any Win32 app, including the new Microsoft Edge, causes the headset display to briefly freeze.
- The Microsoft Edge tile disappears from the Windows Mixed Reality Start menu (you can find it in the “Classic apps” folder).
- Windows from the previous Microsoft Edge are still placed around the mixed reality home, but cannot be used. Attempting to activate those windows launches Edge inside of the Desktop app.
- Selecting a hyperlink in the mixed reality home launches a web browser on the desktop instead of the mixed reality home.
- The WebVR Showcase app is present in the mixed reality home, despite WebVR no longer being supported.
- General improvements to keyboard launch and visuals.

**Additional known issues**
-	Websites open in Windows Mixed Reality will be lost when Mixed Reality Portal closes, though the Microsoft Edge windows will remain where they were placed in the mixed reality home.
-	Audio from Microsoft Edge windows is not spatialized.
-	**Fixed in 360 Viewer extension version 2.3.8**: Opening a 360 video from YouTube in Windows Mixed Reality may result in the video being distorted in the headset. Restarting Edge should invisibly update the 360 Viewer extension to resolve this issue. You can confirm which version of the extension you have by entering `edge://system/` in the address bar and selecting the **Expand** button next to "extensions."
-	During Windows Mixed Reality sessions, virtual monitors will appear as generic physical monitors in Settings > System > Display.

## Launching mixed reality after the first time

Entering mixed reality a second time is as easy as putting the headset back on while its connected to your PC. You can also launch the Mixed Reality Portal app manually by opening it from the Start menu. Input and audio will route automatically to the headset when you put it on, or you can trigger this manually by pressing **Windows + Y** on your keyboard. 

## See also

* [Troubleshooting installation and setup](troubleshooting-windows-mixed-reality.md#installation-and-setup)
* [Learn Mixed Reality](learn-mixed-reality.md)
* [How motion controllers work](motion-controllers.md)
* [How inside-out tracking works](tracking-system.md)
