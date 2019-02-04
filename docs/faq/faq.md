# Frequently Asked Questions (FAQ)

![Cover](img/StockSnap_SWRREC0K3A_edited.jpg)

This is a collection of frequently asked questions, answered by our experts. If you cannot find
an answer to your question, please contact us via the form on the 
[support page](../support/support.md).

**TIP: Try the search feature in the top right corner!**

## Hardware

### What iOS devices are supported?

LiveSYNC can be installed on iPhones and iPads, but currently not on AppleTV. The app requires
iOS 8.0 or later.

While LiveSYNC works fairly well also on iOS devices that are several years old, some feature 
limitations exist:

- Bluetooth chipset may limit simultaneous connections (Director device) to 4 or 2 instead of 8.
Please test with your device before purchasing a license (watermark will appear).

- Video playback on your iOS device may be limited to FullHD quality instead of 4K. Notice that 
you can still use 4K video with your VR headsets if you convert the video to FullHD for your iPad.

### I need to buy an iPad to be used as the director device. Which model do you recommend?

In general, a new standard size (9.7") iPad is a good value for money. You can also choose Pro
version, but it is not necessary unless you want a larger size model (11" or 12.9").

### What Android devices are supported?

LiveSYNC can be installed on Android phones and tablets, but currently not on AndroidTV. The app
requires Android 5.0 (API level 21) or later.

While LiveSYNC works fairly well also on Android devices that are several years old, some feature 
limitations exist:

- Director mode with Bluetooth communication may not work on some old devices that have been
upgraded to Android 5.0, due to Bluetooth chipset that does not support all required features.

- Bluetooth chipset may limit simultaneous connections (Director device) to 4 or 2 instead of 8.
Please test with your device before purchasing a license (watermark will appear).

- Video playback on your Android device may be limited to FullHD quality instead of 4K. Notice that 
you can still use 4K video with your VR headsets if you convert the video to FullHD for your tablet.

### I need to buy an Android tablet to be used as the director device. Which model do you recommend?

Just to name one, we've had good experience with Samsung Galaxy Tab S2 or newer. However, there are
plenty of options.

## Installing

### Can I install LiveSYNC on my iPhone or iPad?

Yes. On your iOS device, open *App Store*, tap *Search*, and type 'livesync'. Then select
'LiveSYNC Presentation Solution' by Finwe Ltd. The app can be installed for FREE.

You can also use this [direct link](https://itunes.apple.com/us/app/livesync-presentation-solution/id1202200449) to find the app.

### Can I install LiveSYNC on my Android phone or tablet?

Yes. On your Android device, open *Play Store*, and type 'livesync' to the search field. Then select
'LiveSYNC Presentation Solution' by Finwe Ltd. The app can be installed for FREE.

You can also use this [direct link](https://play.google.com/store/apps/details?id=fi.finwe.livesync.player.android) to find the app.

### Can I install LiveSYNC on my Windows phone or tablet?

No. Windows is currently not supported.

### Can I install LiveSYNC on my Windows/Mac/Linux computer?

No. Desktop computer operating systems are currently not supported. 

### Can I install LiveSYNC on my GearVR/Oculus Go headset?

Yes, but currently you will need an invite to our Beta channel in the Oculus Store. Please use
the contact form in the [support page](../support/support.md) for requesting an invite.

When you get an invite email from Oculus, click the link in the email to accept the invitation. 
Then on your GearVR/Oculus device, navigate to Oculus Store and type 'livesync' to the search field. 
Select 'LiveSYNC Oculus Go'. If you cannot find it, don't forget to check also the 'Not installed' 
tab. The app can be installed for FREE.

### Can I install LiveSYNC on my Oculus Rift/HTC Vive headset?

No. LiveSYNC is currently available for standalone VR headsets, not for devices that depend on a
desktop/laptop computer.

### I have a Cardboard (or compatible) VR headset. Can I use that with LiveSYNC?

Yes. Both iOS and Android versions have built-in support for VR mode on phones (disabled in tablets).
During channel configuration select 'VR' for viewing mode, or during playback long tap the screen to
toggle between normal and VR mode.

*If you have a GearVR headset, please use our separate Oculus Go version from Oculus Store instead
(invite only). The rendering quality and head tracking are far superior!*

## Beta versions

### Can I test new features before they are released by installing a beta version?

Yes. Please follow the instructions below:

- Android: We have an open beta channel in Google Play. Anyone can join simply by opting-in 
[here](https://play.google.com/apps/testing/fi.finwe.livesync.player.android) and then installing
the beta version by following instructions on that page.

- iOS: We have a closed beta channel in Apple TestFlight. If you wish to participate, please use
the contact form in the [support page](../support/support.md) for requesting an invite.

- GearVR/Oculus Go: We have a closed beta channel in Oculus Store. If you wish to participate, please
 use the contact form in the [support page](../support/support.md) for requesting an invite. 
 **Notice: We need your Oculus username/email for sending the invite.**

### Can I install BOTH the beta version and the store version into the same device?

No. All the stores allow having only one version installed at a time. In general this will be the
newest version ie. the one with the highest version number.

## Configuration

### Can I create multiple channel configurations, and swap between them during my presentation?

Yes, sort of. Each channel has a channel number, and only those audience devices that are listening
on the same channel that you are on will respond to your commands. You can control device group
1 first on channel 1234, and then move on to control device group 2 on channel 5678, for instance.

However, when you leave a presentation to switch to another one, the audience devices that you
were previously controlling will lose the connection and return to the lobby. Hence, you cannot have
more than one presentation ongoing *simultaneously* with only one controller device.

## Content

### What file formats are supported?

In general, LiveSYNC recognizes .mp4 video files, .jpg image files, and .m3u8 HLS streams. For 
custom hotspot images please use 32-bit .png with alpha. 

Notice that for video content the support depends on used hardware (HW decoder), .mp4 is just a 
container. A good rule of thumb is: if it plays with your device's own media player, it likely 
works with LiveSYNC, too.

### Where should I put my content files so that LiveSYNC can pick them up?

- On iOS devices, use iTunes application to copy your media files under LiveSYNC app.

- On Android/GearVR/Oculus Go devices, use file manager to copy your media files under
/Movies/LiveSYNC folder (this should be generated automatically upon first start)

### Can I use an SD card on my Android device for storing content files?

Yes. You need to manually create /Movies/LiveSYNC folder on your SD card and copy the files there.
LiveSYNC will treat this folder on SD card similar to /Movies/LiveSYNC folder in internal storage,
except that if same filename appears in both then internal memory takes precedence.

### Can I use folders to organize my content files?

Yes, but only one level: \LiveSYNC\Summer is OK but \LiveSYNC\Summer\June is not.
Of course you can have as many subfolders directly under LiveSYNC root folder, for example 
\LiveSYNC\January, \LiveSYNC\February, etc.

- On iOS devices, create the folders on your PC/Mac and then *drag* the folder to iTunes. Notice
that it is not possible to view the contents of already copied folder via iTunes - unless you drag
the folder back from iTunes, for example, to your desktop.

- On Android devices, you can use the same method OR create the folders directly to your device
  and then copy there individual files. You can also view the contents of the folders via file manager.

