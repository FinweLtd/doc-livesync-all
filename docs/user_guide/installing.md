# 2. Installing

## Versions

The LiveSYNC app is available as different *versions*. Read this section first to understand which version is best for you and what hardware you need for using it.

### Platforms

The LiveSYNC app can be installed and run on multiple *platforms*. Currently, the supported platforms include **iOS**, **Android**, and **Oculus**. Each platform has its own version of the app. They are compatible with each other, but not exactly the same.

The app works on multiple *device types*. Currently, the supported device types include **phones**, **tablets**, and **VR headsets**. All of these are great for viewing content. A tablet is recommended for creating, editing, and presenting content.

There are combinations of platforms and device types that are not supported. For example, you cannot install LiveSYNC on AppleTV, Android smart watch / smart TV, or Oculus Rift headset.

Some device types allow viewing content in **VR mode** via a passive or an active VR headset. The availability of VR mode varies. Tablets are not physically compatible with VR headsets, hence the VR mode is not available there. On phones the VR mode is *selectable*. You can view content via the touchscreen, but you can also put the phone inside a passive VR headset like Google Cardboard. On devices that were made for VR, such as GearVR and Oculus Go, the VR mode is always active.

The table below summarizes the supported device types and the availability of the VR mode on each platform.

Platform | Device Type | VR Mode
---------|-------------|--------
iOS | iPhone and iPad | Selectable on iPhone, N/A on iPad
Android | Phones and tablets | Selectable on phones, N/A on tablets
Oculus | VR headset | Always on

!!! example
    Tina works in the manufacturing industry. Clients often come to visit the factory. They are taken to a tour in groups of five. For safety reasons, some parts of the factory are closed from visitors. To demonstrate the whole process, Tina wants to show 360-degree video clips from the closed areas. Hence, she chooses to buy an iPad and 5 Oculus Go headsets. In the beginning of the tour, she shares the headsets to the visitors and keeps the iPad herself. During the tour around the factory, they often stop in front of a closed area to watch a video clip via the headsets.

!!! example
    Mark is a teacher in the elementary school. They have a rack of 20 Android tablets, which any of the teachers can reserve for their class. Mark wants to use 360-degree video clips around the World in his geography lessons. In the beginning of the class, he shares 19 tablets to his students and uses one of them for controlling his presentation.

!!! example
    Kate is participating a voluntary project. They are documenting an old building that used to be a boarding school. Now it is about to get demolished. To preserve precious memories, they have shot a 360-degree image of each of the rooms of the building and are planning to present them in a class reunion. The team has only a small budget, hence they have ordered 30 pieces of Google Cardboards. During the reunion, they will circulate among the former students and copy the photos to everyone's mobiles. Kate uses her own phone for controlling the presentation.

### Store vs. Beta

The LiveSYNC app is installed to a device via the platform's own app store. On iOS it is **Apple iTunes AppStore**, on Android it is **Google Play Store**, and on Oculus it is **Oculus Store**. The app version that is publicly available for everyone is called *the store version*. This is the recommended version for most users.

LiveSYNC is continuously being developed further. New features are added and previous ones improved. Feedback from ordinary users is essential. Thus, new features are made first available via beta channels. Users who wish to try out new things and provide feedback can choose to install *the beta version* instead.

Installing the beta version is only slightly different than installing the store version. Instructions are given separately for both later in this chapter.

!!! note
    The store version and the beta version cannot exist simultaneously on a single device. For each device, you can install either but not both at the same time. Of course, it is possible to reinstall the app to get a different version.

!!! note
    On some platforms, the maximum number of beta testers is limited by the platform. Hence, we may not be able to accept all requests to become a beta tester. When the beta tester status is given for a specific need such as testing a particular new feature, we may later need to remove the user from the beta channel (switch to the public store version).

!!! example
    Jerome has a business where he sells 360-degree videos and VR headsets to retirement homes. They are used for relaxation and entertainment. Most popular are videos where old style working methods are documented. Each of Jerome's setups consists of an Android tablet and an Oculus Go headset. The nurse helps in placing the headset comfortably to the senior's face, and selects from the tablet a video he wishes to see. Jerome uses the store version on kits that have been delivered, and the beta version on his own devices - just to stay up-to-date on what's coming.

!!! example
    Anthony has purchased a set of 360 Video Start kits for his construction company. They are building in several cities and Anthony wants to keep himself up-to-date without spending his days traveling between the sites. Twice per week his site managers take a set of 360-degree photos and annotate the progress and next tasks. They email a PDF report to Anthony straight from LiveSYNC. They use the beta version because it has some new annotation features they wish to test.

### Roles

When you are presenting content with LiveSYNC, each device acts either as *the viewing device* of an audience member or as *the control device* of the presenter. You can read more about this [here](introduction.md#key-concepts).

The device's role (*audience* or *director*) can be selected in the setup phase. When you create a channel configuration, one of the choices you make is the role that the device assumes. Since the role is configurable, the same app version is used for both the audience and the director roles.

However, the director role is not available in all versions of the app. For example, app versions made for VR headsets support only the audience role. In addition, the store version and the beta version may differ at times.

The table below summarizes the current situation: which roles are available in which version.

Platform | Store version | Beta version
---------|---------------|-------------
iOS | Audience & Director | Audience & Director
Android | Audience | Audience & Director
Oculus | N/A | Audience

!!! note
    In a presentation, you can freely mix all kinds of devices. For example, an iOS tablet can control a mix of iOS phones & tablets, Android phones & tablets, GearVR headsets, and Oculus Go headsets. Some of the phones can be in VR mode and some not.

!!! example
    Joan's marketing team is participating in a trade show. Their company is launching a new product. Joan's team is using a 360-degree video to showcase it at their booth. They are controlling six Oculus Go headsets with LiveSYNC. To reduce waiting time, they run two groups of three headsets in parallel. The groups are controlled with two iPads. Hence, the iPads act in the director role, and the headsets act in the audience role. Joan configures two channels, so that the groups can work in parallel without disturbing each other.

### Version Number

New features and fixes are implemented and tested frequently. Then, a new software build is pushed to the release channels and release notes are published.

Each build has a version number. To learn what has changed, take note of the version number from your app installation, and compare it to the release notes document.

If you want to check which version (build) you have installed on a particular device, start the LiveSYNC app and notice the version number from the splash screen.

![LiveSYNC splash](img/install_version_number.jpg)

On iOS and Android versions, you can find the version number and other build details also when you start the LiveSYNC app, navigate to *Settings*, then *About*, and scroll down the page near the end until you find *Version* section.

![LiveSYNC splash](img/install_version_details.jpg)

These details are also pre-filled to support request emails when you send a request directly from the LiveSYNC app. The support email link appears just below version details.

## System Requirements

Your hardware must meet the minimum technical specifications outlined below to run and use the LiveSYNC app. If you plan to purchase new hardware, consider our recommendations.

### iOS

Feature | Minimum requirement | Recommendation
---------|--------------------|---------------
Form factor | iPhone or iPad[^1] | iPad for the director mode, either for the audience mode
Model | iPhone 6[^2] or iPad Air[^3] | iPad 5th/6th gen. or any iPad Pro
Operating system | iOS 8.0 or later | iOS 11.0 or later
Accessories | - | AV adapter[^4]

!!! tip
    All iPad Pro models are much more expensive than the standard iPad. When using the LiveSYNC app, they are usually not worth the extra cost. Unless, you prefer to have a larger screen.

    You cannot extend the storage size. LiveSYNC does not support memory sticks on iOS, not even those sold as iOS compatible (they only work with the manufacturer's own app). Hence, we recommend that you invest in a model with large storage capacity.

    In most cases Wifi-only model is enough. Mobile LTE network can be useful if you plan to control other devices via GlobalSYNC and do not rely on Wifi availability.

[^1]: iPhone and iPad are supported. iPod Touch and Apple TV are iOS devices but not supported. Apple Watch and Apple MacBook use different operating systems and are not supported.
[^2]: iPhone 6/6+/6s/6s+/7/7+/8/8+/X/XR/XS/XS Max are supported. iPhone 2007/3G/3GS/4/4s/5/5c/5s/SE are not supported. See [iPhone models](https://support.apple.com/en-us/HT201296) for reference.
[^3]: iPad Air/Air 2/5th gen./6th gen./Pro (all) are supported. iPad 2010/2/3rd gen./4th gen./mini/mini 2/mini 3/mini 4 are not supported. See [iPhone models](https://support.apple.com/en-us/HT201471) for reference.
[^4]: You can use the AV adapter for sharing your iPad's screen to a big screen via an HDMI cable. See [product info](https://www.apple.com/shop/product/MD826AM/A/lightning-digital-av-adapter) for reference.

### Android

Feature | Minimum requirement | Recommendation
---------|--------------------|---------------
Form factor | Phone or Tablet [^5] | Tablet for the director mode, either for the audience mode
Model | n/a[^6] | Samsung Galaxy Tab S2/S3/S4 are known to work well
Operating system | Android 5.0 (API 21) or later | Android 6.0 (API 23) or later
Accessories | - | Micro SD card, Micro USB memory stick [^7]

[^5]: Android phones and tablets are supported. Android TV, Android Auto and Android Wear devices are not supported. Chromebook uses a different operating system and is not supported.
[^6]: There are thousands of supported models. It is not possible to list them all here.
[^7]: If your device has a micro SD card slot, you can expand storage size (LiveSYNC supports SD card for media files). Micro USB to USB memory stick (with OTG feature) is handy for copying media files from PC/Mac to tablet.

!!! tip
    There is a huge selection of devices to choose from. Many low-end Android devices have poor display resolution, no support for 4K video playback, and no gyro sensor. Check at least these features before purchasing a new Android tablet. We recommend ~10 inch screen size for the director mode.

    You can extend the storage size if your device has an SD card slot. LiveSYNC supports SD card for media files.

    In most cases Wifi-only model is enough. Mobile LTE network can be useful if you plan to control other devices via GlobalSYNC and do not rely on Wifi availability.

!!! warning
    LiveSYNC's director mode is more advanced on iOS than Android. If you plan to purchase a new director's device, we currently recommend iOS over Android. If you prefer to use Android, please check that the Android version of the app contains features that are relevant to you. It will take time before Android version catches iOS version in features.

### Oculus

Feature | Minimum requirement | Recommendation
---------|--------------------|---------------
Form factor | GearVR or Oculus Go[^8] | Oculus Go[^9]
Model | Galaxy S7/S7 Edge[^10] | Galaxy S8 & GearVR SM-324 (or newer), or Oculus Go
Operating system | Android 7.0 (API 24) or later | Android 7.0 (API 24) or later
Accessories | - | Micro SD card, Micro USB memory stick [^11]

[^8]: Oculus Quest will likely be supported later. Oculus Rift and HTC Vive are not supported.
[^9]: GearVR is also OK, but we prefer Oculus Go as it is a standalone low-cost device.
[^10]: GearVR compatible phones older than Galaxy S7 tend to overheat quickly.
[^11]: If your device has a micro SD card slot, you can expand storage size (LiveSYNC supports SD card for media files). Micro USB to USB memory stick (with OTG feature) is handy for copying media files from PC/Mac to tablet.

!!! note
    You can try installing and using the LiveSYNC app also on models that are not officially supported. If the app is not visible in the store with a particular device, then that device is not supported (even unofficially). If you use an unsupported device, performance may suffer and some features may not be available.

## Installing the Store Version

The store version is the official release version of the LiveSYNC app. It is available via each platform's own app store. This is the recommended version for most users.

### iOS

!!! tip
    If you are familiar with installing apps on iOS, you can use this direct link:
    
    <https://itunes.apple.com/us/app/livesync-presentation-solution/id1202200449?mt=8>

**Option A: Watch a video installation guide**

<iframe src="https://player.vimeo.com/video/221436477" width="640" height="480" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

*Video not working? Click [here](https://vimeo.com/221436477) to open it in Vimeo.*

**Option B: Follow the steps described below**

1. Go to your iOS device and turn it on. When it starts, unlock it and enter the home screen. Look for *App Store* icon and tap it.

    ![iOS Install](img/install_ios_step_1.jpg)

2. From the bottom bar, select *Search* tab.

    ![iOS Install](img/install_ios_step_2.jpg)

3. Type *livesync* to the search box.

    ![iOS Install](img/install_ios_step_3.jpg)

4. Tap *Search* button.

    ![iOS Install](img/install_ios_step_4.jpg)

5. Select *LiveSYNC Presentation Solution* from the search results.

    ![iOS Install](img/install_ios_step_5.jpg)

6. Select *Install* button (cloud symbol with an arrow). Wait a moment.

    ![iOS Install](img/install_ios_step_6.jpg)
 
7. Once downloading and installation has completed, select *Open*.

    ![iOS Install](img/install_ios_step_7.jpg)

8. The app starts. It is now listed in your device's application menu. The next time you can start it from there.

    ![iOS Install](img/install_ios_step_8.jpg)

### Android

!!! tip
    If you are familiar with installing apps on Android, you can use this direct link:
    
    <https://play.google.com/store/apps/details?id=fi.finwe.livesync.player.android&hl=en>

**Option A: Watch a video installation guide**

<iframe src="https://player.vimeo.com/video/221453486" width="640" height="480" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

*Video not working? Click [here](https://vimeo.com/221453486) to open it in Vimeo.*

**Option B: Follow the steps described below**

1. Go to your Android device and turn it on. When it starts, unlock it and enter the home screen. Look for *Play Store* icon and tap it.

    ![Android Install](img/install_android_step_1.jpg)

2. Type *livesync* to the search box and tap *Enter*. (On some software keyboards it appears as the search button, which you can recognize from a magnifier icon.)

    ![Android Install](img/install_android_step_2.jpg)

3. Select *LiveSYNC Presentation Solution* from the search results.

    ![Android Install](img/install_android_step_3.jpg)

4. Select *Install*. Wait a moment.

    ![Android Install](img/install_android_step_4.jpg)
 
5. Once downloading and installation has completed, select *Open*.

    ![Android Install](img/install_android_step_5.jpg)

6. The app starts. It is now listed in your device's application menu. The next time you can start it from there.

    ![Android Install](img/install_android_step_6.jpg)

### Oculus

!!! info
    LiveSYNC has not officially launched on Oculus platform yet. However, you can start using it already by installing it from our [beta channel](installing.md#oculus_2).

## Installing the Beta Version

The beta version is the official test version of the LiveSYNC app. It is available via each platform's own beta distribution method. Beta version is recommended for users who are eager to try out new features and provide feedback for developers.

!!! warning
    We test all releases internally before pushing them to beta channels, but be aware that beta versions are more likely to contain bugs. Feature and user interface changes occur frequently based on user feedback - what you see on a beta release may not end up to store release. Releases are published more often via beta channels. Also, documentation for new features may not be available at the time of release.

### iOS

Request access to beta version [here](../support/support.md). Mention that you want to be added to LiveSYNC iOS beta channel, and provide your email account.

If you are accepted as a beta tester, you will need to install the beta version via TestFlight app. This is Apple's distribution method for beta versions.

### Android

!!! note
    There is no need to request access to beta version on Android. It is open for everyone.

Follow the instructions below to install *the beta version* of the LiveSYNC app on your Android device.

1. Go to your Android device and turn it on. When it starts, unlock it and enter the home screen. Start the web browser (*Chrome* or *Internet*) and open this link:

    <https://play.google.com/apps/testing/fi.finwe.livesync.player.android>
  
2. Once the following page appears, click the button that says *BECOME A TESTER*.
    
    ![Android Install](img/install_android_beta_step_1.jpg)
  
3. You are now a beta tester. Read the instructions on the page. If you haven't installed the app yet, click the link that has been emphasized in the screen capture. Then follow normal Android install instructions from [here](installing.md#android_1), continuing from Step 4 onwards.

    ![Android Install](img/install_android_beta_step_2.jpg)

!!! note
    If you want to switch back to the store version, simply uninstall the beta version and install the app again from the store. You are still part of the beta program and can switch back to the beta version at any time.

    If you want to leave the beta program completely, repeat steps 1 and 2. Then click button that says *LEAVE THE PROGRAM*. You are not a beta tester anymore.

### Oculus

!!! tip
    Read our [full step-by-step tutorial](../tutorials/oculus_go_device.md) about Oculus Go headset and learn how to use it with LiveSYNC.

Follow the instructions below to install *the beta version* of the LiveSYNC app on your Oculus Go headset or GearVR compatible phone. The instructions are written for Oculus Go. When something differs for GearVR, it is mentioned.

Notice that the installation can be triggered either via the accompanying Oculus app on your phone (outside VR) or via Oculus Home (inside VR). We will cover both methods.

1. Installing software from Oculus beta channel requires *an invite*. First check your Oculus username and email: start the Oculus app on your phone, navigate to *Settings* (GearVR: *More*), and find the username and email. See the image below for reference:

    ![Username and email](img/install_oculus_email.png)

2.  [Contact us](../support/support.md) and tell that you want to join LiveSYNC beta channel for Oculus. **We need the email address from Step 1 to be able to add you**. This cannot be just one of your email addresses; it has to be the one that is connected with your Oculus account.

3. Once you receive an invite email from Oculus to that email address, accept the invite by clicking a confirmation link in the email. Notice that we must send each invite manually, so it can take a while before the email arrives.

    ![Invite email](../tutorials/img/screenshot_invite_email.png)

4. After accepting the invite you have multiple options how to install the application:

    1. Using the Oculus app on your phone: tap the magnifier class icon to open search, type *livesync* and select *LiveSYNC Oculus Go*, then click *Install on ...* button.
    ![Install via phone, search](../tutorials/img/livesync_install_via_phone.png)
    2. You can also select *Library* tab from the bottom bar and see if *LiveSYNC Oculus Go* already appears in the apps list (GearVR: check *Not Installed* tab). Select it from the list and then click *Install on ...* button.
    ![Install via phone, library](../tutorials/img/livesync_install_via_phone_2.png)
    3. Using the Oculus Go / GearVR headset, select *Search* from the bottom bar, type *livesync*, select *LiveSYNC Oculus Go*, then click *Get*.
    ![Install via headset, search](../tutorials/img/livesync_install_via_headset.jpg)
    4. You can also select *Library* tab from the bottom bar and then *Not Installed* page from the left side menu to see if *LiveSYNC Oculus Go* already appears in the apps list. Select it from the list and then click *Get*.
    ![Install via headset, library](../tutorials/img/livesync_install_via_headset_2.jpg)
5. When the installation has completed you will find *LiveSYNC Oculus Go* listed in the apps grid: Select *Library* tab from the bottom bar, and then *Apps* page from the left side menu (GearVR phone: *My Apps* tab from the top menu).

6. Start *LiveSYNC Oculus Go* by selecting it from the apps grid. (On GearVR, you can start the app from the Oculus app on your phone, or you can first enter VR and then start it from the Oculus Home.)

    ![LiveSYNC splash](../tutorials/img/livesync_splash.png)

## License

**LiveSYNC is a commercial product. You can install if from the stores free of charge and try it out. Continuing using the product requires purchasing a license**.

### Licensing model

A license needs to be purchased only for the device that is being used for creating, editing, or presenting content (the director role).

The devices that are used *only* for viewing do not need a license (the audience role).

A license is valid for a limited period of time. Typically a subscription is purchased for 12 months at a time.

The cost of the license depends on the selected features and subscription length.

### Watermarks

When you are using the product without a license, watermarks are overlaid over your own content. The watermarks disappear on all connected devices when the controlling device (the one running in the director role) has a valid license.

For your convenience, the trial period is currently not limited. This does not mean that actively using the product without a license is allowed. After a reasonable trial period, you must purchase a licence to continue using the product.

### Buying

You can get a license directly via the app: purchase a subscription using an in-app payment. It is also possible to get a license from a local distributor or directly from Finwe (the makers of LiveSYNC).

If you received the LiveSYNC app pre-installed in a kit, the software is probably already licensed. If in doubt, please check from your seller.

### Store vs. Beta

On iOS, the string that uniquely identifies an app installation is different between the store and the beta version. This is a platform feature. It means that the same license file cannot work on both installations.

**We recommend that you activate the license when the store version is installed**. If you wish to use the beta version for a while, we can provide a temporary license that will work with the beta version.

### Locked Features

Some features can be locked from use.

For example, a feature may be reserved for a customer who has funded developing the feature (for a limited period of time).

In another example, a customer may request that a certain feature is disabled for security reasons (such as insecure sharing via email).

To avoid confusion, locked features are usually hidden from the app.

### Enterprise Features

![Enterprise feature](../img/enterprise_feature.png)

Enterprise features are not included in the standard license that you can purchase from the app stores. They are always enabled with a license file.

### 360 Video Starter Kit

The kit contains a tablet where the LiveSYNC app is pre-installed. The bundled license only needs to be activated. Follow the instructions that are included in the kit.
