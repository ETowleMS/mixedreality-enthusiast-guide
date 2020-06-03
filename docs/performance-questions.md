---
title: Performance questions
description: Advanced Windows Mixed Reality troubleshooting that goes beyond our standard consumer support documentation.
ms.topic: article
keywords: Windows Mixed Reality, Mixed Reality, Virtual Reality, VR, MR, Troubleshoot, Errors, Help, Support, Performance
---

# Performance questions

## How can I tell if the Windows Mixed Reality headset is rendering at 60Hz or 90Hz framerate?

If you have a discrete GPU with HDMI 2.0 ports and a CPU with four or more physical cores, you should be getting 90 Hz. To confirm, check the **Device Portal > Performance** tab. 

Note: If your GPU only has a HDMI 1.4 output, you can use a DisplayPort to [HDMI 2.0 adapter](https://holodocswiki.com/wiki/Recommended_adapters_for_Windows_Mixed_Reality_Capable_PCs) as a workaround. 

Note: The **Headset display > visual quality settings** only affect the rendering of the Windows Mixed Reality Home experience.

## My PC is running slowly

The system may be slow for many reasons and in most cases this only last a few seconds. If you experience this problem over long periods of time:
1. Close all unused application on the desktop.
2. Ensure that your laptop is plugged into a power source.
3. Make sure that the PC is not warming up.
4. Lower the visual quality in your Windows Mixed Reality Home.
5. Ensure that you have the latest graphics drivers for your PC (see the graphics drivers section).

## My PC is warming up as I run the Mixed Reality experiences. How do I keep it cool?

1. Check that the battery is charged and power source is plugged in.
2. Make sure that the fans that blow air into or out of the PC are not blocked.
3. Use the PC in a relatively cool environment.
4. Make sure there are no heat sources (for example, the sun or heat vents) pointed at the PC.

## My visuals are choppy, load slowly, or don't look good.
* Make sure your headset is plugged into the correct graphics card on your PC. Some PCs have both integrated and discrete graphics cards. The discrete card will generally provide the best performance. [Learn more about PC hardware](https://support.microsoft.com/en-us/help/4039260/windows-10-mixed-reality-pc-hardware-guidelines).
* Close unused applications on your desktop.
* Make sure your headset fits snugly (move it lower and higher or left and right to adjust).
* Adjust your headset's visual settings in **Settings > Mixed reality > Headset display**. When "Visual quality" is set to "Automatic", the mixed reality experience for your PC will be chosen automatically. For more visual detail, set "Visual quality" to "High". If your visuals are choppy, select a lower setting.
* Adjust the headset calibration knob to make sure that the lenses are set to the correct distance between your pupils (IPD). If you don't know your IPD, an optometrist should be able to measure it for you, or use a website designed to measure IPD. If the headset doesn't have a calibration knob, select **Settings > Mixed reality > Headset display** and adjust the "Calibration control".
