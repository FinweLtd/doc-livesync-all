# Using LiveSYNC on Oculus Go

![Cover](img/oculus_go.jpg)

## The Device

#### What is it?

[**Oculus Go**](https://www.oculus.com/go/) is an affordable standalone VR headset from [Oculus](https://www.oculus.com), a company owned by [Facebook](https://www.facebook.com).

It has many similarities to [**GearVR**](https://www.samsung.com/global/galaxy/gear-vr/), a product made by [Samsung](https://www.samsung.com). In fact, GearVR uses technology and software from Oculus and is marketed under *Powered by Oculus* term.

The main difference is that Oculus Go is a new standalone device, whereas GearVR consists of an older style combination of a VR frame and a compatible Samsung phone.

In both cases applications are installed from [Oculus Store](https://www.oculus.com/experiences/go/) and same app builds can work on both products. Also the user experience, visual quality and interaction mechanism are almost the same.

Both products are 3DOF devices (three degrees of freedom), ie. you can look around in VR by turning your head, but you cannot walk in VR by physically taking steps. There are no need for a computer and no wires. You can simply take the headset out of your bag, put it on your face and start using it. Bundled hand remote is used as a pointer when selecting objects from screen.

#### Should I get an Oculus Go or a GearVR?

If you already own a [compatible](https://www.samsung.com/global/galaxy/gear-vr/) Samsung phone, purchasing only the VR frame is an affordable choice (about $110). GearVR headset is a lightweight addition to your bag if you travel a lot and carry a large-screen phone anyway.

However, in most cases Oculus Go is a better choice. Since it is a standalone device it has a battery of its own and you can dedicate the device for its sole purpose: VR. You will also save a fortune if you need a large number of headsets.

To learn more about their differences, read comparison articles:

* [Android Central: Oculus Go vs Samsung Gear VR](https://www.androidcentral.com/oculus-go-vs-samsung-gear-vr)

* [How-To Geek: Gear VR vs Oculus Go: Which One is Better?](https://www.howtogeek.com/352453/gear-vr-vs-oculus-go-which-one-is-better/)

* [ThreeSixtyCameras.com: Gear VR vs Oculus Go: Which is the better VR experience?](http://www.threesixtycameras.com/gear-vr-vs-oculus-go-which-is-the-better-vr-experience/)

#### How do I get one?

You can purchase an Oculus Go directly from [Oculus](https://www.oculus.com/go/), from various online stores such as [Amazon](https://www.amazon.com/s/ref=nb_sb_noss_2?url=search-alias%3Daps&field-keywords=oculus+go), or from local computer and electronics stores.

A 32 GB model costs $199 (€219) and a 64 GB model $249 (€269).

## Initial setup

### Oculus app

It might be a bit surprising that when you unpack the Oculus Go headset and begin the initial setup procedure, you must install *an application to your phone*:

> To set up and connect your Oculus Go, you'll need to download the Oculus app on your supported mobile phone. With the Oculus app, you can set up your headset, browse VR games and apps and customize your device settings. *(Oculus Go website)*

This accompanying app is **mandatory** during the initial setup of the headset. After that you will need it very rarely, if ever. If you plan to purchase multiple headsets, they can be all set up and configured from a single phone. Download the Oculus Go app from here:

<https://oculus.com/app>

Alternatively, you can use these direct links for [Android](https://play.google.com/store/apps/details?id=com.oculus.twilight) and [iOS](https://itunes.apple.com/us/app/oculus-vr/id1366478176).

!!! note
    This is NOT the same app that you use with a GearVR headset. Both apps have the same name *Oculus*. You can differentiate them from the icon: GearVR app icon has text GearVR, Oculus Go app icon does not have any text.

![Oculus app](img/screenshot_oculus_1.png)

*Oculus Go accompanying app on Android phone.*

### Pairing & setup

1. Download the Oculus app using the links above, then launch the installed app

2. If you don't have an Oculus account yet, sign up first and then log in

3. Once logged in, navigate to *Settings* and select *Pair New Headset*

4. Select *Oculus Go* from *Choose a Headset* menu, and press *Start Now*

5. Turn on your Oculus Go device and press *Continue*

6. Plug your Oculus Go into a power source and press *Continue*

7. After search completes found headsets are listed. If multiple devices were found nearby, choose the one that matches the serial number in your headset (its below the barcode under the strap), and press *Continue*

8. Select a Wifi access point that will be used for connecting the headset to the network, and press *Continue*

9. Put a battery into the controller and choose with which hand you want to use your controller, and press *Continue*

10. Select language to use in VR, and press *Continue*

11. Add a payment method (a credit card or a PayPal account) or press *Skip*

12. Go through safety etc. information, press *Continue* to proceed

When ready, you will see a dialog saying *Preparing your Oculus Go...*. Once it’s finished, pairing and setup has completed.

For more information, see the questions and answers [here](https://support.oculus.com/183135912238400/).

![Oculus app Settings](img/screenshot_oculus_2.png)

*Once the pairing and setup is complete, your headset(s) will appear in *Settings* tab.*

### First time use

Go to your Oculus Go device. Put the headset on your face. There is *an infrared proximity sensor* inside the headset (between the lenses). The headset will wake up automatically and you will hear a greeting sound.

Grab the hand controller, point straight ahead (to the direction you are looking at), and *press and hold* the Oculus button (ring symbol) on the hand controller.

![Oculus Go calibration](img/screenshot_oculus_go_1.png)

*Whenever the device wakes up from sleep you must calibrate the hand remote.*

!!! note
    Every time the headset wakes up from sleep it will present *a calibration dialog*. Calibration is necessary, because the headset and the hand remote are two independent devices that are both only aware of *rotation around their own center point*. The devices do not know what actual direction they are pointing at (for example, North, South-East, etc.) Hence, they need to be calibrated by making them point to the same direction, and then pressing a button to signal this. Unfortunately, this needs to be repeated every time the headset wakes up, because sensors are turned off to save power during sleep and they will lose the tracking.

After calibration and first time use tutorial you will enter *Oculus Home*. Here you can install new apps, start installed apps, configure the headset, and use services offered by Oculus.

![Oculus Home](img/screenshot_oculus_go_2.png)

*The Oculus Home.*

!!! tip
    We recommend that you spend some time to play around with the device. Get familiar with the hand remote and Oculus Home. Try a couple of pre-installed apps. Ask your boss a permission to take it home for the weekend and watch a couple of movies from Netflix or Youtube VR.

### Installing LiveSYNC

Once you feel familiar with Oculus Go, it is time to install the LiveSYNC app. The installation can be triggered either via the accompanying Oculus app on your phone (outside VR) or via Oculus Home (inside VR).

!!! info
    LiveSYNC has not officially launched on Oculus platform yet. However, you can start using it already by installing it from our beta channel. Follow the steps below.

1. Check your Oculus username and email: start the Oculus accompanying app on your phone, navigate to *Settings*, and find the username and email (see the image below):

    ![Username and email](img/screenshot_oculus_go_3.png)

2. Installing software from Oculus beta channel requires *an invite*. [Contact us](../support/support.md) and tell that you want to join LiveSYNC beta channel for Oculus Go. **We need the email address from Step 1 to be able to add you.** This cannot be just one of your email addresses; it has to be the one that is connected with your Oculus account.

3. Once you receive an invite email from Oculus to that email address, accept the invite by clicking a confirmation link in the email. Notice that we must send each invite manually, so it can take a while before the email arrives.

    ![Invite email](img/screenshot_invite_email.png)

4. You have multiple options how to install the application:
    1. Using the accompanying Oculus app on your phone: tap the magnifier class icon to open search, type *livesync* and select *LiveSYNC Oculus Go*, then click *Install on ...* button.

    ![Install via phone, search](img/livesync_install_via_phone.png)

    2. You can also select *Library* tab from the bottom bar and see if *LiveSYNC Oculus Go* already appears in the apps list. Select it from the list and then click *Install on ...* button.

    ![Install via phone, library](img/livesync_install_via_phone_2.png)

    3. Using the Oculus Go device, select *Search* from the bottom bar, type *livesync*, select *LiveSYNC Oculus Go*, then click *Get*.

    ![Install via headset, search](img/livesync_install_via_headset.jpg)

    4. You can also select *Library* tab from the bottom bar and then *Not Installed* page from the left side menu to see if *LiveSYNC Oculus Go* already appears in the apps list. Select it from the list and then click *Get*.

    ![Install via headset, library](img/livesync_install_via_headset_2.jpg)

5. When the installation has completed, you will see *LiveSYNC Oculus Go* listed in the headset when you select *Library* tab from the bottom bar and then *Apps* page from the left side menu.

6. Start *LiveSYNC Oculus Go* by selecting it from the apps grid.

    ![LiveSYNC splash](img/livesync_splash.png)

## Preparing for a presentation

Presenting with the LiveSYNC tool works as follows:

* The presenter controls the presentation with a separate control device (typically an iOS or an Android tablet). The presenter will reserve *a communication channel* for the presentation.

* Each member of the audience uses a personal viewer device (iOS/Android phone or tablet, or GearVR/Oculus Go headset). The viewer devices will *join the communication channel*, whose number the presenter will share.

A channel number consists of four digits from the area 1000-9999.

### Channel configuration

!!! note
    Here we assume that you have already set up a presentation channel in Director Mode on your director device (tablet). As an example, we will use channel number *5034*.

Next, we will configure a new presentation channel (in Audience Mode):

1. On your Oculus Go device, start LiveSYNC app and select '+' from the *Home* screen.

    ![LiveSYNC Home](img/livesync_home_empty.png)

2. Type in the channel number using the virtual numeric keypad, and click *OK*.

    ![LiveSYNC Channel Editor](img/livesync_channel_input.png)

3. On your control device (tablet), start LiveSYNC app and select the channel from the *Home* screen. Mosaic view will appear, showing only *My device* item (tablet's own view).

    ![LiveSYNC Mosaic](img/livesync_mosaic_empty.png)

4. On your Oculus Go device, select the channel from the *Home* screen.

    !!! note
        If this is the first time you join a channel from this device (or if you have removed file access permission), a permission dialog appears. Select *Allow* to give file access permission, else LiveSYNC app cannot access your own presentation files.

    ![LiveSYNC Permissions](img/livesync_permissions.png)

    Next, *the Lobby* appears. Audience members will wait here for a connection to the control device. This is a 360-degree environment with a 2D screen panel where notifications to the user are presented.

    ![LiveSYNC Lobby](img/livesync_lobby_entry.png)

5. The headset connects with the control device automatically, as soon as it is available / within reach. User does not have to do anything.

    !!! note
        Usually this takes only a few seconds. However, with Bluetooth technology and multiple devices it can take up to tens of seconds. The devices must share the same radio frequencies, which makes connection times longer.

      ![LiveSYNC Lobby](img/livesync_lobby_opening.png)

6. Once the connection is established, the view from the Oculus Go headset appears on the control device's screen: the Mosaic view now contains a new item:

    ![LiveSYNC Mosaic](img/livesync_mosaic_one_device.png)

    On the headset, a notification tells that the device is ready for presentation:

    ![LiveSYNC Lobby](img/livesync_lobby_ready.png)

### Testing the setup

!!! note
    Here we assume that you still have an ongoing connection that was opened in the previous section.

1. To test presenting via the control device, switch to *Player* tab from the bottom bar and drag an item from the *Content* tab to the *Presentation area* at the center of the screen:

    ![LiveSYNC Player](img/livesync_player_content_drop.png)

2. On the headset, the playback command will be received, requested media item loaded, and rendered on screen.

    ![LiveSYNC Player](img/livesync_player_demo_photo.png)

3. The headset will notify the contorl device of success. The control device shows live monitoring view from the headset in the *Devices* tab (and also in *Mosaic* if you return there).

    ![LiveSYNC Player](img/livesync_player_observing.png)


4. Remember to copy your media files on all devices, as instructed
during the setup procedure. If you skipped it during the setup, please
do it now.
4. Make sure that Bluetooth is enabled on all devices. There is no need
to pair the devices.
5. From LiveSYNC app's Home screen, select to Control (director) or Join
(audience) your presentation channel.
6. You should see the views from your audience devices quickly appearing
to the Mosaic view on your iPad.
7. To begin your presentation, change to Player view on your iPad and
simply drag photos/videos/hotspots to the presentation area on the
center of the screen.

The basic presentation features are covered in the LiveSYNC demo video:
https://vimeo.com/207785581

### Copying content files

1. Connect the included USB 2.0 cable to your computer and Oculus Go headset.
2. Put on your headset and select Accept to confirm you want to allow your computer to access files on the headset.
    - On Windows, Oculus Go will automatically appear as a drive on your computer.
    - On Mac, you'll need to install Android File Transfer to successfully transfer files between your Oculus go and computer.
    - On Chromebook/Chrome OS, you'll need to use the Files app to access your Oculus Go headset.
3. Open Android Transfer app from your computer -> Select Movies -> LiveSYNC -> Click and drag files and folders to LiveSYNC Folder.

Are you not able to find LiveSYNC folder under Movies? LiveSYNC folder is auto generated when the app in being installed. However, to be able to create that folder LiveSYNC, needs a permission from user to access file system (read/write).

So the first thing to check is that you are given read/write permission by tapping three dots next to LiveSYNC Oculus Go -> Permissions.


Both switches should be enabled, location is required by Bluetooth connectivity, and Storage for file access.


Copy the same contents (images, videos) to director iPad

1. Connect the included USB 2.0 cable to your computer and iPad.
2. Select device from itunes on your computer
3. Select Apps/File Sharing
4. Select LiveSYNC
5. Click and drag files and folders to LiveSYNC Documents.
6. Open LiveSYNC on iPad -> Select channel number -> Player -> and pull to refresh contents on the left side (where demo contents are located)

Have a look at our video tutorial (https://vimeo.com/222670351) to see how files are copied. After adding video, image, and .png hotspot files to LiveSYNC pull-to-refresh and update contents of LiveSYNC.

### Automation

TODO

Settings.ini

## Viewing a presentation

TODO

## Tips & tricks

TODO


