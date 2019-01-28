# Quick start: Presentation

## Step 1: Hardware setup

### Devices

In a LiveSYNC-enabled presentation, the person giving the presentation has *a control device* and the audience members each have *a viewer device*. Hence, to give a presentation using the LiveSYNC tool you will need:

* 1 device for controlling the presentation (LiveSYNC tool in *Director Mode*)

* 1-n devices for viewing the presentation (LiveSYNC tool in *Audience Mode*)

#### Director Mode

The Director Mode is currently available for iOS and Android. Thus, you can use either a phone or a tablet for controlling a presentation.

!!! tip
    We highly recommend using a tablet for the Director Mode because of its larger screen.

#### Audience Mode

The Audience Mode is currently available for iOS, Android, GearVR, and Oculus Go. Thus, you can view a presentation either from a phone screen, a tablet screen, or via a phone based or standalone VR headset.

!!! note
    VR mode is available also for iOS and Android phones. A Google Cardboard or a compatible VR headset can be used, but user experience is much superior with a high quality headset and dedicated app version (GearVR, Oculus Go).

#### Networking

Communication between the control device and the viewer devices is *wireless*. You can choose from available options during channel configuration (Step 3). Make sure that the necessary radio technology is enabled on all devices. Depending on your selection this can be for example Bluetooth, Wifi or mobile data.

#### Power

During a presentation the devices will consume a lot of power. Power consumption is related to active radios (communication), photo and video decoding, continuous screen updates, display brightness, and disabled power saving (sleep).

We recommend that you recharge the batteries of all devices before a presentation. If you use VR headsets with hand remotes, check the batteries inside the remotes. If you plan to run a presentation repeatedly, you probably need spare devices that are being recharged while others are in use.

### Big screen

In addition to personal viewing devices you can use a big screen. This can be for example a large TV screen or a projector. We recommend a wired connection between the control device and the big screen. For example, an iPad can be connected using an HDMI cable (via a separately sold adapter).

### Speakers or headphones

Many presentations use sound. You must decide whether you want to use room audio (audience devices muted) or viewer device audio. In the latter case, headphones are recommended.

### Chairs

If your presentation takes more than a few minutes, the audience probably wants to sit. In order to allow comfortable 360-degree photo/video exploration, swivel chairs with enough spacing between them are recommended.

### Step 2: Software install

The same application is used both in the control device (Director Mode) and viewer devices (Audience Mode). The mode will be selected during Step 3.

#### iOS (iPhones & iPads)

On your iOS device, open *App Store*, tap *Search*, and type *livesync*. Then select
*LiveSYNC Presentation Solution* by Finwe Ltd. The app can be installed for FREE.

You can also use this [direct link](https://itunes.apple.com/us/app/livesync-presentation-solution/id1202200449) to find the app.

#### Android (phones and tablets)

On your Android device, open *Play Store*, and type *livesync* to the search field. Then select
*LiveSYNC Presentation Solution* by Finwe Ltd. The app can be installed for FREE.

You can also use this [direct link](https://play.google.com/store/apps/details?id=fi.finwe.livesync.player.android) to find the app.

#### Oculus (GearVR & Oculus Go)

LiveSYNC has not officially launched on these platforms yet. However, you can already start using it. Currently you will need *an invite* to our Beta channel in the Oculus Store. Please use
the contact form in the [support page](../support/support.md) for requesting an invite.

When you get an invite email from Oculus, click the link in the email to accept the invitation.
Then on your GearVR/Oculus Go device, navigate to Oculus Store and type *livesync* to the search field. Select *LiveSYNC Oculus Go*. If you cannot find it, don't forget to check also the *Not installed* tab. The app can be installed for FREE.

### Step 3: Configuration

#### Director Mode

To configure a device for the Director Mode follow these steps:

1. Start the application from the device's application menu

2. Once started, click the big round button with a '+' sign inside it

3. Select device role (Director)

4. Type device name or use the offered default name

5. Select connection type

6. Write down the given channel number

7. Pass the reminder about copying content

Your channel configuration has been created and is visible on the app's *Channels* screen.

#### Audience Mode

To configure a device for the Audience Mode follow these steps:

1. Start the application from the device's application menu

2. Once started, click the big round button with a '+' sign inside it

3. Select device role (Audience)

4. Type device name or use the offered default name

5. Select connection type

6. Type the channel number (the one you wrote down earlier)

7. If you are setting a phone, select normal or VR mode (not asked on tablets)

8. Pass the reminder about copying content

Your channel configuration has been created and is visible on the app's *Channels* screen.

!!! note
    On GearVR/Oculus Go Director Mode is not available and Audience Mode configuration is simpler.

### Step 4: Presentation files

LiveSYNC does not *stream* the content from the control device to audience devices. Only playback commands are sent and received. Thus, each audience device must have its own copy of the files that are used in a presentation. This ensures scalability and good user experience.

Presentation files typically consist of a set of 360-degree photos (.jpg), 360-degree videos (.mp4), and custom hotspots (.png). Also ordinary 2D photos and videos can be used.

!!! note
    To prepare the devices for a presentation you must copy the necessary files to *all devices* in advance.

#### iOS (iPhones & iPads)

Copy the presentation files using Apple's **iTunes** application.

1. Install iTunes application to your PC or Mac computer

2. Start iTunes application

3. Connect your iOS device to your computer using a *Lightning to USB* cable

4. Once the device is detected in iTunes, click the phone/tablet icon

5. Click *File Sharing* from left side menu

6. Select *LiveSYNC* from the apps list

7. Drag'n drop files and folders to the app's file area

#### Android (phones & tablets)

Copy the presentation files using Windows Explorer (PC) or Android File Transfer application.

1. Connect your Android device to your computer using a *USB* cable

2. Once the device is detected it will appear in Explorer / Android File Transfer

3. Find /Movies/LiveSYNC folder (auto generated during first run)

4. Drag'n drop files and folders under /Movies/LiveSYNC

#### Oculus (GearVR & Oculus Go)

Copy the presentation files using Windows Explorer (PC) or Android File Transfer application.

1. Connect your Android device to your computer using a *USB* cable

2. Once the device is detected it will appear in Explorer / Android File Transfer

3. Find /Movies/LiveSYNC folder (auto generated during first run)

4. Drag'n drop files and folders under /Movies/LiveSYNC

## Step 5: Starting a presentation

Follow these steps to start a presentation on the device configured to Director Mode:

1. Start the application from the device's application menu

2. Once started, click the big round button with a channel number you have configured earlier

3. The application switches into the Director Mode and starts from the *Mosaic* tab

4. Wait here until audience devices have joined (their views will appear on your screen)

!!! note
    In case some viewer devices arrive late (during a presentation) they can still join the presentation.

## Step 6: Joining a presentation

Follow these steps to join a presentation on a device configured to Audience Mode:

1. Start the application from the device's application menu

2. Once started, click the big round button with a channel number you have configured earlier

3. The application switches into the Audience Mode and starts from the *Lobby*

4. Wait here until connection to the control device has been established

5. Once connected, you are ready and the presentation begins when the presenter decides to do so

## Step 7: Giving a presentation

When viewer devices have connected, select *Player* tab from the bottom bar.

To start the presentation, drag an item from the *Content* tab and drop it to the *Presentation area* at the center of the screen.

The status of each viewer device appears in the *Devices* tab.

If you want to draw the attention of the audience to something, drag an item from the *Tags* tab and drop it to a position where you want it to appear over the content being presented.

To change content, drag another item from the *Content* tab and drop it to the *Presentation area*.

Once your presentation is over, tap the *Home* button in the top left corner to exit presentation. Connections to viewer devices will be disconnected and they will return to the Lobby.

!!! note
    If you haven't purchased a license, watermarks will be shown when you are presenting your own content files. This concerns both the control and the viewer devices. Only the control device requires a license. Watermarks will not appear on viewer devices when they are connected to a control device that has a valid license.

## What's next

You have barely scratched the surface of what you can do with the LiveSYNC tool. Learn more by reading some of the [tutorials](../tutorials/tutorials.md) or dive into the [User Guide](../user_guide/user_guide.md).
