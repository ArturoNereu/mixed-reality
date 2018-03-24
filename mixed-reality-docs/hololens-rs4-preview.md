---
title: HoloLens RS4 Preview
description: Learn more about the RS4 preview build for HoloLens, including how to install the preview, a description of the new features included, and how to provide feedback and get support.
author: mattzmsft
ms.author: mazeller
ms.date: 03/23/2018
keywords: HoloLens, preview, insider, os, rs4, new features
---

# HoloLens RS4 Preview

>[!IMPORTANT]
>By downloading *or* using the HoloLens RS4 preview builds, you are acknowledging and agreeing to the **HoloLens RS4 Preview – EULA (End User License Agreement)**, included in the preview program package.

In this article, you'll learn more about the HoloLens RS4 Preview, a preview of the Windows Holographic OS updates coming to the Windows 10 Spring Creators Update (also known as RS4). Any HoloLens owner who is interested in trying the preview is invited to give it a try, however, please remember that this is a preview build (not final software) and all the warnings that come along with that. If that doesn't worry you, follow the instructions below to install the HoloLens RS4 Preview and read about the new features it includes.

## Downloading the HoloLens RS4 Preview package

You can download the setup package from the [https://aka.ms/hololenspreviewdownload](https://aka.ms/hololenspreviewdownload).

## What's in the package?

| File | Description |
|------|------|
| rs4_release_svc_analog.retail.10.0.17110.1001.FFU | The HoloLens RS4 Preview image that you will flash to your device using the Windows Device Recovery Tool. |
| HoloLens RS4 Preview – EULA | HoloLens RS4 Preview - Evaluation Use Terms (End User License Agreement) |

## Installing the preview

1. On a retail HoloLens device (Windows Holographic 10.0.14393), opt-in to Insider Preview builds to prepare your device for the RS4 Preview:
   * Launch the **Settings** app -> **Update & Security** -> **Get Insider Preview builds** -> **Get started**.
   * Select Restart to restart the device to prepare to install Preview builds and wait until your device is once again booted.

>[!NOTE]
>If you need assistance getting your device back to a known state, refer to the [Reset & Recovery instructions](reset-or-recover-your-hololens.md).

2. Install an updated version of the **Windows Device Recovery Tool (WDRT)** from [https://aka.ms/wdrt](https://aka.ms/wdrt).

>[!NOTE]
>This preview requires WDRT version 3.14.07501 (or newer)

3. Flash the OS Preview Build using the Windows Device Recovery Tool:
   a. Launch Windows Device Recovery Tool from your Start menu or Desktop shortcut.
   
   ![WDRT shortcut](images/WDRT314-RS4Preview-1.png)
   
   b. Plug in your HoloLens device, and then select **Microsoft HoloLens** to continue.
   
   ![Device selection](images/WDRT314-RS4Preview-2.png)
   
   c. Select **Manual package selection** to select a custom OS image to use, then navigate to the .FFU file provided as part of the [Preview package](#downloading-the-hololens-rs4-preview-package).
   
   ![Manual package selection](images/WDRT314-RS4Preview-3.png)
   
   d. Confirm that the correct package is listed, and then select **Install software** to begin the OS installation.
   
   ![Install software](images/WDRT314-RS4Preview-4.png)
   
   e. **WARNING:** this process will erase all the content on your HoloLens device; confirm by selecting **Continue**.
   
   ![Warning](images/WDRT314-RS4Preview-5.png)
   
   f. The installation process will take a few minutes, during which a progress bar will be displayed on-screen.
   
   ![Installation progress](images/WDRT314-RS4Preview-6.png)
   
   g. Once installation is complete, your device will reboot; select **Finish** to complete the process.
   
   ![Finish](images/WDRT314-RS4Preview-7.png)
   
   h. You can confirm the new OS version on your device by selecting your device again in the tool, and verifying on the **Device info** page.
   
   ![Device info](images/WDRT314-RS4Preview-8.png)

4. Go through the HoloLens on-device OOBE setup flow. Sign-in with your personal or work account to experience all the features of this Preview.

## New features in this preview

### For all users

<table>
  <tr>
    <th>Feature</th><th>Details</th><th>Instructions</th>
  </tr>
  <tr>
    <td>Auto-placement of 2D and 3D content on launch</td><td>A 2D app launcher or 2D UWP app auto-places in the world at an optimal size and distance when launched instead of requiring the user to place it. If an <a href="app-views.md">immersive app</a> uses a 2D app launcher instead of a <a href="3d-app-launcher-design-guidance.md">3D app launcher</a>, the immersive app will auto-launch from the 2D app launcher same as in RS1.<br><br>A 3D app launcher from the Start menu also auto-places in the world. Instead of auto-launching the app, users can then click on the launcher to launch the immersive app. 3D content opened from the Holograms app and from Edge also auto-places in the world.</td><td>When opening an app from the Start menu, you will no longer be asked to place it in the world.<br><br>If the 2D app/<a href="3d-app-launcher-design-guidance.md">3D app launcher</a> placement is not optimal, you can easily move them using new fluid app manipulations described below. You can also re-position the 2D app launcher/3D content by saying "Move this" and then using gaze to re-position the content.</td>
  </tr>
  <tr>
    <td>Fluid app manipulation</td><td>Move, resize, and rotate 2D and 3D content without having to enter "Adjust" mode.</td><td>To move a 2D UWP app or 2D app launcher, simply gaze at its app bar and then use the tap + hold + drag gesture. You can move 3D content by gazing anywhere on the object and then using tap + hold + drag.<br><br>To resize 2D content, gaze at its corner. The gaze cursor will turn into a resize cursor, and then you can tap + hold + drag to resize. You can also make 2D content taller or wider by looking at its edges and dragging.<br><br>To resize 3D content, lift up both your hands into gesture frame, fingers up in the ready position. You'll see the cursor turn into a state with 2 little hands. Do the tap and hold gesture with both your hands. Moving your hands closer or farther apart you will change the size of the object. Moving your hands forward and backward relative to each other will rotate the object. You can also resize/rotate 2D content this way.</td>
  </tr>
  <tr>
    <td>2D app horizontal resize with reflow</td><td>Make a 2D UWP app wider in aspect ratio to see more app content. For example, making the Mail app wide enough to show the Preview Pane.</td><td>Simply gaze at the left or right edge of the 2D UWP app to see the resize cursor, then use the tap + hold + drag gesture to resize.</td>
  </tr>
  <tr>
    <td>Expanded voice command support</td><td>You can do more simply using your voice.</td><td>Try these voice commands:<li>"Go to Start" - Brings up the Start menu or exits an [immersive app](app-views.md).</li><li>"Move this" - Allows you to move an object.</li></td>
  </tr>
  <tr>
    <td>Updated Holograms and Photos apps</td><td>Updated Holograms app with new holograms. Updated Photos app.</td><td>You will notice an updated look to the Holograms and Photos apps. The Holograms app includes several new Holograms and a label maker for easier creation of text.</td>
  </tr>
  <tr>
    <td>Improved mixed reality capture</td><td>Hardware shortcut start and end MRC video.</td><td>Hold Volume Up + Down for 3 seconds to start recording MRC video. Tap both again or use the bloom gesture to end.</td>
  </tr>
  <tr>
    <td>Improved audio immersion</td><td>You can now hear HoloLens better in noisy environments, and experience more lifelike sound from applications as their sound will be obscured by real walls detected by the device.</td><td>HoloLens finds your space automatically, and no longer requires you to manage or select spaces. If you have problems with holograms around you, you can go to <b>Settings > System > Holograms > Remove nearby holograms</b>. If needed, you can also select <b>Remove all holograms</b>.</td>
  </tr>
</table>

### For developers

<table>
  <tr>
    <th>Feature</th><th>Details</th><th>Instructions</th>
  </tr>
  <tr>
    <td>Spatial mapping improvements</td><td>A 2D app launcher or 2D UWP app auto-places in the world at an optimal size and distance when launched instead of requiring the user to place it. If an <a href="app-views.md">immersive app</a> uses a 2D app launcher instead of a <a href="3d-app-launcher-design-guidance.md">3D app launcher</a>, the immersive app will auto-launch from the 2D app launcher same as in RS1.<br><br>A 3D app launcher from the Start menu also auto-places in the world. Instead of auto-launching the app, users can then click on the launcher to launch the immersive app. 3D content opened from the Holograms app and from Edge also auto-places in the world.</td><td>When opening an app from the Start menu, you will no longer be asked to place it in the world.<br><br>If the 2D app/<a href="3d-app-launcher-design-guidance.md">3D app launcher</a> placement is not optimal, you can easily move them using new fluid app manipulations described below. You can also re-position the 2D app launcher/3D content by saying "Move this" and then using gaze to re-position the content.</td>
  </tr>
  <tr>
    <td>Automatic selection of focus point based on depth buffer</td><td>Move, resize, and rotate 2D and 3D content without having to enter "Adjust" mode.</td><td>To move a 2D UWP app or 2D app launcher, simply gaze at its app bar and then use the tap + hold + drag gesture. You can move 3D content by gazing anywhere on the object and then using tap + hold + drag.<br><br>To resize 2D content, gaze at its corner. The gaze cursor will turn into a resize cursor, and then you can tap + hold + drag to resize. You can also make 2D content taller or wider by looking at its edges and dragging.<br><br>To resize 3D content, lift up both your hands into gesture frame, fingers up in the ready position. You'll see the cursor turn into a state with 2 little hands. Do the tap and hold gesture with both your hands. Moving your hands closer or farther apart you will change the size of the object. Moving your hands forward and backward relative to each other will rotate the object. You can also resize/rotate 2D content this way.</td>
  </tr>
  <tr>
    <td>Holographic reprojection modes</td><td>Make a 2D UWP app wider in aspect ratio to see more app content. For example, making the Mail app wide enough to show the Preview Pane.</td><td>Simply gaze at the left or right edge of the 2D UWP app to see the resize cursor, then use the tap + hold + drag gesture to resize.</td>
  </tr>
  <tr>
    <td>App tailoring APIs</td><td>Windows APIs know more about where your app is running, such as whether the device’s display is transparent (HoloLens) or opaque (immersive headset) and whether a UWP app’s 2D view is showing up in the holographic shell.</td><td>Unity had previously manually exposed <a href="https://docs.unity3d.com/ScriptReference/XR.WSA.HolographicSettings.IsDisplayOpaque.html">HolographicSettings.IsDisplayOpaque</a> in a way that worked even before this build.<br><br>For DirectX apps, you can now access existing APIs like <a href="https://docs.microsoft.com/en-us/uwp/api/windows.graphics.holographic.holographicdisplay.isopaque">HolographicDisplay.GetDefault().IsOpaque</a>, <a href="https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.preview.holographic.holographicapplicationpreview.iscurrentviewpresentedonholographicdisplay">HolographicApplicationPreview</a>, and <a href="https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.preview.holographic.holographicapplicationpreview.iscurrentviewpresentedonholographicdisplay">IsCurrentViewPresentedOnHolographicDisplay</a> on HoloLens as well.
</td>
  </tr>
  <tr>
    <td>Research mode</td><td><b>needs content</b></td><td><b>needs content</b></td>
  </tr>
</table>

### For commercial customers

### For IT pros


## Known issues in this preview

You can find the latest set of known issues with workarounds at [https://aka.ms/hololenspreviewrelnote](https://aka.ms/hololenspreviewrelnote).

## Note for developers

You are welcome to try developing your applications using this build of HoloLens. Continue using the Windows Mixed Reality developer documentation to guide your development, as these apply to this latest build of HoloLens as well. You can use the same builds of [Unity and Visual Studio](install-the-tools.md) that you're already using for HoloLens development.

Reference the [new features list above](#new-features-in-this-preview) for capabilities specific to the HoloLens RS4 Preview.

## Provide feedback and report issues

Please use the [Feedback Hub app on HoloLens](give-us-feedback.md#feedback-for-hololens) to provide feedback and report issues. Using Feedback Hub ensures that all necessary diagnostics information is included to help our engineers quickly debug and resolve the problem.

>[!IMPORTANT]
>Be sure to accept the prompt that asks whether you’d like Feedback Hub to access your Documents folder (select **Yes** when prompted).

## Questions and support

You can ask questions and engage with our support team in a new section of the [HoloLens developer forums](https://aka.ms/hololenspreviewhelp).